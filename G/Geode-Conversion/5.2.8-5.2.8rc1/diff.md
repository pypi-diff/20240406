# Comparing `tmp/Geode_Conversion-5.2.8-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Conversion-5.2.8rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1631807 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      171 b- defN 24-Apr-06 06:48 geode_conversion/__init__.py
--rw-rw-rw-  2.0 fat      178 b- defN 24-Apr-06 06:48 geode_conversion/model.py
--rw-rw-rw-  2.0 fat  4043776 b- defN 24-Apr-06 06:49 geode_conversion/bin/Geode-Conversion_model.dll
--rw-rw-rw-  2.0 fat   150528 b- defN 24-Apr-06 06:49 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1990 b- defN 24-Apr-06 06:49 Geode_Conversion-5.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-06 06:49 Geode_Conversion-5.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-06 06:49 Geode_Conversion-5.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      731 b- defN 24-Apr-06 06:49 Geode_Conversion-5.2.8.dist-info/RECORD
-8 files, 4197491 bytes uncompressed, 1630519 bytes compressed:  61.2%
+Zip file size: 1631832 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      171 b- defN 24-Apr-05 10:08 geode_conversion/__init__.py
+-rw-rw-rw-  2.0 fat      178 b- defN 24-Apr-05 10:08 geode_conversion/model.py
+-rw-rw-rw-  2.0 fat  4043776 b- defN 24-Apr-05 10:09 geode_conversion/bin/Geode-Conversion_model.dll
+-rw-rw-rw-  2.0 fat   150528 b- defN 24-Apr-05 10:09 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1993 b- defN 24-Apr-05 10:09 Geode_Conversion-5.2.8rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-05 10:09 Geode_Conversion-5.2.8rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-05 10:09 Geode_Conversion-5.2.8rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      743 b- defN 24-Apr-05 10:09 Geode_Conversion-5.2.8rc1.dist-info/RECORD
+8 files, 4197506 bytes uncompressed, 1630520 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: geode_conversion/bin/Geode-Conversion_model.dll
 Comment: 
 
 Filename: geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Conversion-5.2.8.dist-info/METADATA
+Filename: Geode_Conversion-5.2.8rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Conversion-5.2.8.dist-info/WHEEL
+Filename: Geode_Conversion-5.2.8rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Conversion-5.2.8.dist-info/top_level.txt
+Filename: Geode_Conversion-5.2.8rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Conversion-5.2.8.dist-info/RECORD
+Filename: Geode_Conversion-5.2.8rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_conversion/bin/Geode-Conversion_model.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802e28f4
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr  6 06:49:10 2024
+Time/Date		Fri Apr  5 10:09:06 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000002e7000
 SizeOfInitializedData	00000000000f6800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002e28f4
@@ -397885,15 +397885,15 @@
    18015508e:	test   %rax,%rax
    180155091:	je     0x1801550d1
    180155093:	movq   $0x1,(%rax)
    18015509a:	movb   $0x0,0x8(%rax)
    18015509e:	xor    %eax,%eax
    1801550a0:	mov    %rax,0x10(%rdi)
    1801550a4:	mov    %rbx,0x10(%rdi)
-   1801550a8:	lea    0x22f8e9(%rip),%rax        # 0x180384998
+   1801550a8:	lea    0x22f8c9(%rip),%rax        # 0x180384978
    1801550af:	mov    %rax,0x18(%rdi)
    1801550b3:	mov    %r13,0x40(%rdi)
    1801550b7:	lea    0xf8(%rbp),%rax
    1801550be:	mov    %rax,0x48(%rdi)
    1801550c2:	movsd  %xmm6,0x50(%rdi)
    1801550c7:	mov    %r14d,0x58(%rdi)
    1801550cb:	mov    %r12d,0x5c(%rdi)
@@ -397961,15 +397961,15 @@
    1801551b9:	test   %rax,%rax
    1801551bc:	je     0x1801551fc
    1801551be:	movq   $0x1,(%rax)
    1801551c5:	movb   $0x0,0x8(%rax)
    1801551c9:	xor    %eax,%eax
    1801551cb:	mov    %rax,0x10(%rdi)
    1801551cf:	mov    %rbx,0x10(%rdi)
-   1801551d3:	lea    0x22f79e(%rip),%rax        # 0x180384978
+   1801551d3:	lea    0x22f7fe(%rip),%rax        # 0x1803849d8
    1801551da:	mov    %rax,0x18(%rdi)
    1801551de:	mov    %r13,0x40(%rdi)
    1801551e2:	lea    0xf8(%rbp),%rax
    1801551e9:	mov    %rax,0x48(%rdi)
    1801551ed:	movsd  %xmm6,0x50(%rdi)
    1801551f2:	mov    %r15d,0x58(%rdi)
    1801551f6:	mov    %r12d,0x5c(%rdi)
@@ -416519,15 +416519,15 @@
    180164dd9:	test   %rax,%rax
    180164ddc:	je     0x180164e19
    180164dde:	movq   $0x1,(%rax)
    180164de5:	mov    %r15b,0x8(%rax)
    180164de9:	xor    %eax,%eax
    180164deb:	mov    %rax,0x10(%rsi)
    180164def:	mov    %r15,0x10(%rsi)
-   180164df3:	lea    0x21fbde(%rip),%rax        # 0x1803849d8
+   180164df3:	lea    0x21fbbe(%rip),%rax        # 0x1803849b8
    180164dfa:	mov    %rax,0x18(%rsi)
    180164dfe:	mov    (%rbx),%rax
    180164e01:	mov    %rax,0x40(%rsi)
    180164e05:	mov    0x80(%rsp),%rcx
    180164e0d:	mov    (%rcx),%rax
    180164e10:	mov    %rax,0x48(%rsi)
    180164e14:	mov    %r15,(%rcx)
@@ -416701,15 +416701,15 @@
    180165043:	jne    0x180164fb0
    180165049:	jmp    0x1801651b2
    18016504e:	movq   $0x1,0x80(%rbp)
    180165059:	movb   $0x0,0x88(%rbp)
    180165060:	xor    %eax,%eax
    180165062:	mov    %rax,0x90(%rbp)
    180165069:	mov    %rax,0x90(%rbp)
-   180165070:	lea    0x21f941(%rip),%rax        # 0x1803849b8
+   180165070:	lea    0x21f921(%rip),%rax        # 0x180384998
    180165077:	mov    %rax,0x98(%rbp)
    18016507e:	mov    %r13,0xc0(%rbp)
    180165085:	lea    0x30(%rbp),%rax
    180165089:	mov    %rax,0xc8(%rbp)
    180165090:	mov    %r15,0xd0(%rbp)
    180165097:	mov    0x80(%rbp),%rax
    18016509e:	inc    %rax
@@ -1081040,59 +1081040,59 @@
    180384967:	imul   $0x0,0x6e(%rdi),%ebp
    18038496e:	add    %al,(%rax)
    180384970:	movabs 0xe00000000180384c,%al
    180384979:	pop    %rcx
    18038497a:	(bad)
    18038497b:	addb   $0x0,(%rcx)
    18038497e:	add    %al,(%rax)
-   180384980:	and    %bl,0x16(%rdx)
+   180384980:	lock pop %rdx
+   180384982:	(bad)
    180384983:	addb   $0x0,(%rcx)
    180384986:	add    %al,(%rax)
    180384988:	push   %rax
    180384989:	rex.R adc $0x80,%al
    18038498c:	add    %eax,(%rax)
    18038498e:	add    %al,(%rax)
    180384990:	add    %al,-0x80(%rsp,%rdx,1)
    180384994:	add    %eax,(%rax)
    180384996:	add    %al,(%rax)
-   180384998:	loopne 0x1803849f3
-   18038499a:	(bad)
-   18038499b:	addb   $0x0,(%rcx)
+   180384998:	rolb   $0x80,0x14(%rbx)
+   18038499c:	add    %eax,(%rax)
    18038499e:	add    %al,(%rax)
-   1803849a0:	lock pop %rdx
-   1803849a2:	(bad)
+   1803849a0:	nop
+   1803849a1:	jle    0x1803849b9
    1803849a3:	addb   $0x0,(%rcx)
    1803849a6:	add    %al,(%rax)
    1803849a8:	push   %rax
    1803849a9:	rex.R adc $0x80,%al
    1803849ac:	add    %eax,(%rax)
    1803849ae:	add    %al,(%rax)
    1803849b0:	add    %al,-0x80(%rsp,%rdx,1)
    1803849b4:	add    %eax,(%rax)
    1803849b6:	add    %al,(%rax)
-   1803849b8:	rolb   $0x80,0x14(%rbx)
-   1803849bc:	add    %eax,(%rax)
-   1803849be:	add    %al,(%rax)
-   1803849c0:	nop
-   1803849c1:	jle    0x1803849d9
+   1803849b8:	movabs 0x8000000001801675,%al
+   1803849c1:	jbe    0x1803849d9
    1803849c3:	addb   $0x0,(%rcx)
    1803849c6:	add    %al,(%rax)
-   1803849c8:	push   %rax
-   1803849c9:	rex.R adc $0x80,%al
-   1803849cc:	add    %eax,(%rax)
+   1803849c8:	adc    %dh,0x16(%rsi)
+   1803849cb:	addb   $0x0,(%rcx)
    1803849ce:	add    %al,(%rax)
    1803849d0:	add    %al,-0x80(%rsp,%rdx,1)
    1803849d4:	add    %eax,(%rax)
    1803849d6:	add    %al,(%rax)
-   1803849d8:	movabs 0x8000000001801675,%al
-   1803849e1:	jbe    0x1803849f9
+   1803849d8:	loopne 0x180384a33
+   1803849da:	(bad)
+   1803849db:	addb   $0x0,(%rcx)
+   1803849de:	add    %al,(%rax)
+   1803849e0:	and    %bl,0x16(%rdx)
    1803849e3:	addb   $0x0,(%rcx)
    1803849e6:	add    %al,(%rax)
-   1803849e8:	adc    %dh,0x16(%rsi)
-   1803849eb:	addb   $0x0,(%rcx)
+   1803849e8:	push   %rax
+   1803849e9:	rex.R adc $0x80,%al
+   1803849ec:	add    %eax,(%rax)
    1803849ee:	add    %al,(%rax)
    1803849f0:	add    %al,-0x80(%rsp,%rdx,1)
    1803849f4:	add    %eax,(%rax)
    1803849f6:	add    %al,(%rax)
    1803849f8:	rolb   $0x80,0x14(%rbx)
    1803849fc:	add    %eax,(%rax)
    1803849fe:	add    %al,(%rax)
@@ -1082508,18 +1082508,19 @@
    1803859ba:	(bad)
    1803859bb:	(bad)
    1803859bc:	(bad)
    1803859bd:	(bad)
    1803859be:	(bad)
    1803859bf:	incl   (%rax)
    1803859c1:	add    %al,(%rax)
-   1803859c3:	add    %ah,-0x10(%rsi)
-   1803859c6:	adc    %ah,0x0(%rsi)
-   1803859c9:	add    %al,(%rax)
-   1803859cb:	add    %cl,-0x78000000(%rip)        # 0x1083859d1
+   1803859c3:	add    %al,%dl
+   1803859c5:	int    $0xf
+   1803859c7:	data16 add %al,(%rax)
+   1803859ca:	add    %al,(%rax)
+   1803859cc:	or     $0x88000000,%eax
    1803859d1:	add    (%rax),%eax
    1803859d3:	add    %dh,%ah
    1803859d5:	xchg   %bh,(%rax)
    1803859d7:	add    %dh,%ah
    1803859d9:	jp     0x180385a13
    1803859db:	add    %al,(%rax)
    1803859dd:	add    %al,(%rax)
```

## Comparing `Geode_Conversion-5.2.8.dist-info/METADATA` & `Geode_Conversion-5.2.8rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geode-Conversion
-Version: 5.2.8
+Version: 5.2.8rc1
 Summary: Conversion module for Geode-solutions OpenGeode modules
 Home-page: https://github.com/Geode-solutions/Geode-Conversion
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.2.8 Summary: Conversion
-module for Geode-solutions OpenGeode modules Home-page: https://github.com/
-Geode-solutions/Geode-Conversion Author: Geode-solutions Author-email:
-contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: opengeode-core ==14.*,>=14.18.1
+Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.2.8rc1 Summary:
+Conversion module for Geode-solutions OpenGeode modules Home-page: https://
+github.com/Geode-solutions/Geode-Conversion Author: Geode-solutions Author-
+email: contact@geode-solutions.com License: Proprietary Platform: UNKNOWN
+Description-Content-Type: text/markdown Requires-Dist: opengeode-core
+==14.*,>=14.18.1
                ************ GGeeooddee--CCoonnvveerrssiioonnbbyy GGeeooddee--ssoolluuttiioonnss ************
                      ******** CCoonnvveerrssiioonn OOppeennGGeeooddee mmoodduullee ********
             [Build Status][Deploy Status][Coverage Status][Version]
               [Windows support][Ubuntu support][Red Hat support]
  [Language][License][Semantic-release]_[_S_l_a_c_k_ _i_n_v_i_t_e_]Copyright (c) 2019 - 2024,
                                 Geode-solutions
```

## Comparing `Geode_Conversion-5.2.8.dist-info/RECORD` & `Geode_Conversion-5.2.8rc1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 geode_conversion/__init__.py,sha256=K2g9LCrqwB6gfE3Ca5Ia_5Q8csgvLJwn6uiVylAsCsA,171
 geode_conversion/model.py,sha256=kPyg0FrL-HSROjMRnY025-loYYW-S1CTSoEcOZXw4mE,178
-geode_conversion/bin/Geode-Conversion_model.dll,sha256=n3rJ2gMTwjfhO8SuJKNT4jVzBpS9znmGkvPt3MwzziQ,4043776
-geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd,sha256=SNKv3WYjxyedQBBMmV9hUa5X92fGybnxnm_J_73W6g4,150528
-Geode_Conversion-5.2.8.dist-info/METADATA,sha256=FMPsiYiANm0y5OVq7bDZgb9fBi0t2VrqATKWDwVPw8E,1990
-Geode_Conversion-5.2.8.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-Geode_Conversion-5.2.8.dist-info/top_level.txt,sha256=PnM_M6Sy8psC1M_rMpCs6FAGjv7uyDWsRvR46jFUpXU,17
-Geode_Conversion-5.2.8.dist-info/RECORD,,
+geode_conversion/bin/Geode-Conversion_model.dll,sha256=i5DNdR_xPch7EDcH5QG0zLTITt18lIwkfiQeN29_kpM,4043776
+geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd,sha256=Pkuo-NSLweWoiDacaUp43gvJp129ZxjBnFDsb_wa7Qw,150528
+Geode_Conversion-5.2.8rc1.dist-info/METADATA,sha256=3zArvIJBDJ8wSa-SbXH2eCyDHYyueWn2AqUicXH5duY,1993
+Geode_Conversion-5.2.8rc1.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
+Geode_Conversion-5.2.8rc1.dist-info/top_level.txt,sha256=PnM_M6Sy8psC1M_rMpCs6FAGjv7uyDWsRvR46jFUpXU,17
+Geode_Conversion-5.2.8rc1.dist-info/RECORD,,
```

