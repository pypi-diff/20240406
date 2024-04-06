# Comparing `tmp/broken_source-0.1.1-py3-none-any.whl.zip` & `tmp/broken_source-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 642272 bytes, number of entries: 108
+Zip file size: 642221 bytes, number of entries: 108
 -rw-r--r--  2.0 unx    61393 b- defN 20-Feb-02 00:00 Broken/Base.py
 -rw-r--r--  2.0 unx     8139 b- defN 20-Feb-02 00:00 Broken/Dotmap.py
 -rw-r--r--  2.0 unx     6363 b- defN 20-Feb-02 00:00 Broken/Logging.py
 -rw-r--r--  2.0 unx    14924 b- defN 20-Feb-02 00:00 Broken/Project.py
 -rw-r--r--  2.0 unx     2221 b- defN 20-Feb-02 00:00 Broken/Spinner.py
 -rw-r--r--  2.0 unx     1395 b- defN 20-Feb-02 00:00 Broken/Types.py
 -rw-r--r--  2.0 unx     3666 b- defN 20-Feb-02 00:00 Broken/__init__.py
@@ -54,15 +54,15 @@
 -rw-r--r--  2.0 unx     3321 b- defN 20-Feb-02 00:00 ShaderFlow/Module.py
 -rw-r--r--  2.0 unx     3878 b- defN 20-Feb-02 00:00 ShaderFlow/Notes.py
 -rw-r--r--  2.0 unx    37584 b- defN 20-Feb-02 00:00 ShaderFlow/Scene.py
 -rw-r--r--  2.0 unx    11684 b- defN 20-Feb-02 00:00 ShaderFlow/Shader.py
 -rw-r--r--  2.0 unx    12979 b- defN 20-Feb-02 00:00 ShaderFlow/Texture.py
 -rw-r--r--  2.0 unx     4219 b- defN 20-Feb-02 00:00 ShaderFlow/Variable.py
 -rw-r--r--  2.0 unx      437 b- defN 20-Feb-02 00:00 ShaderFlow/__init__.py
--rw-r--r--  2.0 unx     3915 b- defN 20-Feb-02 00:00 ShaderFlow/__main__.py
+-rw-r--r--  2.0 unx     3699 b- defN 20-Feb-02 00:00 ShaderFlow/__main__.py
 -rw-r--r--  2.0 unx    12133 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Audio.py
 -rw-r--r--  2.0 unx     2806 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Bouncing.py
 -rw-r--r--  2.0 unx    17629 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Camera.py
 -rw-r--r--  2.0 unx     9042 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Dynamics.py
 -rw-r--r--  2.0 unx     2332 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Frametimer.py
 -rw-r--r--  2.0 unx     1494 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Keyboard.py
 -rw-r--r--  2.0 unx     2475 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Noise.py
@@ -99,12 +99,12 @@
 -rw-r--r--  2.0 unx      538 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Shaders/Vertex/Default.glsl
 -rw-r--r--  2.0 unx     1965 b- defN 20-Feb-02 00:00 SpectroNote/SpectroNote.py
 -rw-r--r--  2.0 unx      290 b- defN 20-Feb-02 00:00 SpectroNote/__init__.py
 -rw-r--r--  2.0 unx      342 b- defN 20-Feb-02 00:00 SpectroNote/__main__.py
 -rw-r--r--  2.0 unx    20132 b- defN 20-Feb-02 00:00 SpectroNote/Resources/Images/SpectroNote.png
 -rw-r--r--  2.0 unx     1448 b- defN 20-Feb-02 00:00 SpectroNote/Resources/Images/SpectroNote.svg
 -rw-r--r--  2.0 unx     3088 b- defN 20-Feb-02 00:00 SpectroNote/Resources/Shaders/SpectroNote.frag
-?rw-r--r--  2.0 unx     2980 b- defN 20-Feb-02 00:00 broken_source-0.1.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 broken_source-0.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx      194 b- defN 20-Feb-02 00:00 broken_source-0.1.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     9764 b- defN 20-Feb-02 00:00 broken_source-0.1.1.dist-info/RECORD
-108 files, 1388829 bytes uncompressed, 626666 bytes compressed:  54.9%
+?rw-r--r--  2.0 unx     2934 b- defN 20-Feb-02 00:00 broken_source-0.1.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 broken_source-0.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx      194 b- defN 20-Feb-02 00:00 broken_source-0.1.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     9764 b- defN 20-Feb-02 00:00 broken_source-0.1.2.dist-info/RECORD
+108 files, 1388567 bytes uncompressed, 626615 bytes compressed:  54.9%
```

## zipnote {}

```diff
@@ -306,20 +306,20 @@
 
 Filename: SpectroNote/Resources/Images/SpectroNote.svg
 Comment: 
 
 Filename: SpectroNote/Resources/Shaders/SpectroNote.frag
 Comment: 
 
-Filename: broken_source-0.1.1.dist-info/METADATA
+Filename: broken_source-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: broken_source-0.1.1.dist-info/WHEEL
+Filename: broken_source-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: broken_source-0.1.1.dist-info/entry_points.txt
+Filename: broken_source-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: broken_source-0.1.1.dist-info/RECORD
+Filename: broken_source-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ShaderFlow/__main__.py

```diff
@@ -53,54 +53,47 @@
             files.update(Path.cwd().glob("*.py"))
 
         # Add the files, exit if no scene was added
         if sum(apply(self.add_scene_file, files)) == 0:
             log.warning("No ShaderFlow Scenes found")
             exit(1)
 
-    docscene = re.compile(r"class\s+(\w+)\s*\(.*?(?:Scene).*\):\s*(?:\"\"\"((?:\n|.)*?)\"\"\")?")
+    docscene = re.compile(r"^class\s+(\w+)\s*\(.*?(?:Scene).*\):\s*(?:\"\"\"((?:\n|.)*?)\"\"\")?", re.MULTILINE)
     """Matches any class that contains "Scene" on the inheritance and its docstring"""
 
     def add_scene_file(self, file: Path) -> bool:
         """Add classes that inherit from Scene from a file to the CLI"""
 
         # Must be a valid path with string content
         if not (file := BrokenPath(file, valid=True)):
             return False
         if not (code := LoaderString(file)):
             return False
 
+        def partial_run(file, name, code):
+            def run_scene(ctx: Context):
+                SHADERFLOW.DIRECTORIES.CURRENT_SCENE = file.parent
+                try:
+                    # Note: Point of trust transfer to the file the user is running
+                    exec(compile(code, file.stem, "exec"), namespace := {})
+                    scene = namespace[name]
+                    instance = scene()
+                    instance.cli(*ctx.args)
+                finally:
+                    instance.destroy()
+            return run_scene
+
         # Match all scenes and their optional docstrings
         for match in ShaderFlowManager.docscene.finditer(code):
             name, docstring = match.groups()
-
-            def partial_run(file, name, code):
-                def run_scene(ctx: Context):
-                    SHADERFLOW.DIRECTORIES.CURRENT_SCENE = file.parent
-                    try:
-                        # Note: Point of trust transfer to the file the user is running
-                        exec(compile(code, file.stem, "exec"), namespace := {})
-                        scene = namespace[name]
-                        instance = scene()
-                        instance.cli(*ctx.args)
-                    finally:
-                        instance.destroy()
-                return run_scene
-
-            if ("pyapp" in str(file)):
-                panel = "🎥 Built-in release ShaderScenes"
-            else:
-                panel = f"🎥 ShaderScenes at [bold]({file})[/bold]"
-
-            # Create the command
             self.broken_typer.command(
                 callable=partial_run(file, name, code),
                 name=name.lower(),
                 help=(docstring or "No description available"),
-                panel=panel,
+                panel=f"🎥 ShaderScenes at [bold]({file})[/bold]",
                 add_help_option=False,
                 context=True,
             )
 
         return True
 
 def main():
```

## Comparing `broken_source-0.1.1.dist-info/METADATA` & `broken_source-0.1.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: broken-source
-Version: 0.1.1
+Version: 0.1.2
 Summary: Broken Source Software Framework
 Project-URL: repository, https://github.com/BrokenSource/BrokenSource
-Project-URL: homepage, https://brokensource.github.io
-Project-URL: documentation, https://brokensource.github.io
-Project-URL: issues, https://brokensource.github.io/contact
+Project-URL: homepage, https://brokensrc.dev
+Project-URL: documentation, https://brokensrc.dev
+Project-URL: issues, https://brokensrc.dev/contact
 Author-email: Tremeschin <29046864+Tremeschin@users.noreply.github.com>
 Requires-Python: >=3.10
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: arrow>=1.3.0
 Requires-Dist: attrs>=23.2.0
 Requires-Dist: audioread>=3.0.1
 Requires-Dist: cachetools>=5.3.3
@@ -50,31 +50,31 @@
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: typer>=0.10.0
 Requires-Dist: validators>=0.24.0
 Requires-Dist: watchdog>=4.0.0
 Description-Content-Type: text/markdown
 
 <div align="center">
-  <a href="https://brokensource.github.io"><img src="https://raw.githubusercontent.com/BrokenSource/BrokenSource/Master/Broken/Resources/Images/Broken.png" width="200"></a>
+  <a href="https://brokensrc.dev"><img src="https://raw.githubusercontent.com/BrokenSource/BrokenSource/Master/Broken/Resources/Images/Broken.png" width="200"></a>
   <h2>Broken Source Software</h2>
   <br>
-  Here lies <b>Broken</b>: The <b>Shared Library</b> and <b>Manager</b>) + <b>Submodules</b> of all my <b>Projects</b>
+  Here lies <b>Broken</b>: The <b>Shared Library</b> and <b>Manager</b> + <b>Submodules</b> of all my <b>Projects</b>
 </div>
 
 <br>
 
 - **🌟 Framework**: A solution for Unification and Consistency
 - **🚀 Automation**: Spend more time **using** the Projects
 
 <br>
 <br>
 
 <div align="center">
   <h2>🍁 Learn More 🍁</h2>
-  <h3>✨ Check out my <a href="https://brokensource.github.io"><b>Awesome Website</b></a> instead of a boring Readme ✨</h3>
+  <h3>✨ Check out my <a href="https://brokensrc.dev"><b>Awesome Website</b></a> instead of a boring Readme ✨</h3>
   <h5>Installation Guides, Usage, Tips, Code Reference and More!</h5>
 </div>
 
 <br>
 <br>
 
 # 📦 About this PyPI Package
```

### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.3 Name: broken-source Version: 0.1.1 Summary: Broken Source
+Metadata-Version: 2.3 Name: broken-source Version: 0.1.2 Summary: Broken Source
 Software Framework Project-URL: repository, https://github.com/BrokenSource/
-BrokenSource Project-URL: homepage, https://brokensource.github.io Project-URL:
-documentation, https://brokensource.github.io Project-URL: issues, https://
-brokensource.github.io/contact Author-email: Tremeschin
+BrokenSource Project-URL: homepage, https://brokensrc.dev Project-URL:
+documentation, https://brokensrc.dev Project-URL: issues, https://
+brokensrc.dev/contact Author-email: Tremeschin
 <29046864+Tremeschin@users.noreply.github.com> Requires-Python: >=3.10
 Requires-Dist: appdirs>=1.4.4 Requires-Dist: arrow>=1.3.0 Requires-Dist:
 attrs>=23.2.0 Requires-Dist: audioread>=3.0.1 Requires-Dist: cachetools>=5.3.3
 Requires-Dist: cattrs>=23.2.3 Requires-Dist: datetime>=5.5 Requires-Dist:
 distro>=1.9.0 Requires-Dist: dotmap>=1.3.30 Requires-Dist: glcontext>=2.5.0
 Requires-Dist: glfw>=2.7.0 Requires-Dist: imgui>=2.0.0 Requires-Dist:
 intervaltree>=3.1.0 Requires-Dist: midi2audio>=0.1.1 Requires-Dist: moderngl-
@@ -23,15 +23,15 @@
 Requires-Dist: thefuzz>=0.22.1 Requires-Dist: toml>=0.10.2 Requires-Dist:
 tqdm>=4.64.1 Requires-Dist: typer>=0.10.0 Requires-Dist: validators>=0.24.0
 Requires-Dist: watchdog>=4.0.0 Description-Content-Type: text/markdown
   _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_B_r_o_k_e_n_S_o_u_r_c_e_/_B_r_o_k_e_n_S_o_u_r_c_e_/_M_a_s_t_e_r_/_B_r_o_k_e_n_/
                          _R_e_s_o_u_r_c_e_s_/_I_m_a_g_e_s_/_B_r_o_k_e_n_._p_n_g_]
                       ********** BBrrookkeenn SSoouurrccee SSooffttwwaarree **********
 
-   Here lies BBrrookkeenn: The SShhaarreedd LLiibbrraarryy and MMaannaaggeerr) + SSuubbmmoodduulleess of all my
+    Here lies BBrrookkeenn: The SShhaarreedd LLiibbrraarryy and MMaannaaggeerr + SSuubbmmoodduulleess of all my
                                    PPrroojjeeccttss
 
 - **ð Framework**: A solution for Unification and Consistency - **ð
 Automation**: Spend more time **using** the Projects
 
                        ********** ?ð??? LLeeaarrnn MMoorree ?ð??? **********
    ******** ?â??¨ CChheecckk oouutt mmyy _AA_ww_ee_ss_oo_mm_ee_ _WW_ee_bb_ss_ii_tt_ee iinnsstteeaadd ooff aa bboorriinngg RReeaaddmmee ?â??¨ ********
```

## Comparing `broken_source-0.1.1.dist-info/RECORD` & `broken_source-0.1.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 ShaderFlow/Module.py,sha256=uNS-Yrop8j_zLabM0mChjPsb66BDfN9_xSBz4q3dr1Y,3321
 ShaderFlow/Notes.py,sha256=UAaxG2FsYyKQBHTmOhlBE2sJTtHDXIPwbjfcxXczzO4,3878
 ShaderFlow/Scene.py,sha256=oYscRkdtGsIH6I85uRrziJlEUAdJcaI-ultbSYH8awg,37584
 ShaderFlow/Shader.py,sha256=5i7oFUHp-mCchdGY6oJiUFI1FSZXJdP2G5Y_KKKr3L4,11684
 ShaderFlow/Texture.py,sha256=TjvJBRae8rhPyhcm-XnGjmEBCdxTv2mil_pBmkEUFW4,12979
 ShaderFlow/Variable.py,sha256=78H8K1hUKtIfK56u9HiEB6fs3Xr3HS66UR-EjbpC2iA,4219
 ShaderFlow/__init__.py,sha256=Joj_tFA2qYy86nLgRhUKwnV9pwdzcGHa7R-vmLnM4nQ,437
-ShaderFlow/__main__.py,sha256=8KOsuoMcbFkUNhRqIBXmko0hGFpTR0XZm1K0Pmt6fT8,3915
+ShaderFlow/__main__.py,sha256=XHKcI0hdKRlGO9604KWr_EopMfRuABAIxQ4lUlnvNyA,3699
 ShaderFlow/Modules/Audio.py,sha256=fJkdIF-mZVteSymQdanyc7fTcic1NiRUjvVKVwA_Lu4,12133
 ShaderFlow/Modules/Bouncing.py,sha256=HiI3qakzVPTrYIrrLe6RqGCkP1_v1cexyO1BlfAG9wo,2806
 ShaderFlow/Modules/Camera.py,sha256=BmJ2yI-cIIR-i4qTf8VeM0BGLl_TTUYfBEOiqcW0sMI,17629
 ShaderFlow/Modules/Dynamics.py,sha256=TpOZ19SDa1g4h2GOZGDBQr3Wfn9dOOa24VkRWp-e1qw,9042
 ShaderFlow/Modules/Frametimer.py,sha256=9fsVLPoV90v6cXeyv5wszxv9v4_lLSUazCMhCPgIv_w,2332
 ShaderFlow/Modules/Keyboard.py,sha256=uSq0WKVcZA3gNklF9vdtnKa1ZQWH92MA533cXSNvoLU,1494
 ShaderFlow/Modules/Noise.py,sha256=MDUHEA4kS-5iUCHaKgdyDXRnRBqplIBSUVNMuGEYlvY,2475
@@ -98,11 +98,11 @@
 ShaderFlow/Resources/Shaders/Vertex/Default.glsl,sha256=mptLPRKopeWq7ybJL5kV4xT_yL3hMeUAxe2LsJYX4gA,538
 SpectroNote/SpectroNote.py,sha256=ldoN5iXHaxLpxYt-PE9Aa2NtG2P98WIvm1qQDdfgrr8,1965
 SpectroNote/__init__.py,sha256=eTj2Y_jbZgApkTk-d8z2UM1AnofAMRZPnlbd6nc3z1w,290
 SpectroNote/__main__.py,sha256=gT5JAcy6y0HMfOAlnKJUxx_Va1qsOUQuMYL7yfP6gx0,342
 SpectroNote/Resources/Images/SpectroNote.png,sha256=Z7DL7FqIiwG6o6U3inHe1QmipsRkcmnjXNPxM5-xlWs,20132
 SpectroNote/Resources/Images/SpectroNote.svg,sha256=5SlxYmSOAODpXpClTSI2DceG8gbmfKViU1EX2scIbDE,1448
 SpectroNote/Resources/Shaders/SpectroNote.frag,sha256=EO1NrbDp8yZGo6X5ZV0g7NKmGMk68jNL3NX4UnmPYjo,3088
-broken_source-0.1.1.dist-info/METADATA,sha256=JTYA6LwGp7DgdFxu9jGFRU-AAx7CDa_i2vHP34yXaXc,2980
-broken_source-0.1.1.dist-info/WHEEL,sha256=as-1oFTWSeWBgyzh0O_qF439xqBe6AbBgt4MfYe5zwY,87
-broken_source-0.1.1.dist-info/entry_points.txt,sha256=sliTXdLGMPAHvny75SJgCoSIb556KPPyvqTew_2EI98,194
-broken_source-0.1.1.dist-info/RECORD,,
+broken_source-0.1.2.dist-info/METADATA,sha256=XmrovUwwQtRqduxh7VFRoKcBizBHPAsBfSJir5YX18k,2934
+broken_source-0.1.2.dist-info/WHEEL,sha256=as-1oFTWSeWBgyzh0O_qF439xqBe6AbBgt4MfYe5zwY,87
+broken_source-0.1.2.dist-info/entry_points.txt,sha256=sliTXdLGMPAHvny75SJgCoSIb556KPPyvqTew_2EI98,194
+broken_source-0.1.2.dist-info/RECORD,,
```

