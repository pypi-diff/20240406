# Comparing `tmp/fplab-0.0.1.3.tar.gz` & `tmp/fplab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fplab-0.0.1.3.tar", last modified: Fri Apr  5 04:03:04 2024, max compression
+gzip compressed data, was "fplab-0.0.2.tar", last modified: Sat Apr  6 16:19:45 2024, max compression
```

## Comparing `fplab-0.0.1.3.tar` & `fplab-0.0.2.tar`

### file list

```diff
@@ -1,46 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.311618 fplab-0.0.1.3/
--rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      523 2024-04-05 04:03:04.311618 fplab-0.0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      807 2024-03-31 02:53:23.000000 fplab-0.0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.234901 fplab-0.0.1.3/fplab/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.3/fplab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.264691 fplab-0.0.1.3/fplab/enhancement/
--rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.1.3/fplab/enhancement/__init__.py
--rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.1.3/fplab/enhancement/frequency.py
--rw-rw-rw-   0        0        0     4454 2024-03-31 13:48:46.000000 fplab-0.0.1.3/fplab/enhancement/spatial.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.264691 fplab-0.0.1.3/fplab/generation/
--rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.1.3/fplab/generation/__init__.py
--rw-rw-rw-   0        0        0       75 2024-04-02 15:55:02.000000 fplab-0.0.1.3/fplab/generation/distortion.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.264691 fplab-0.0.1.3/fplab/intrinsic/
--rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.1.3/fplab/intrinsic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.281979 fplab-0.0.1.3/fplab/intrinsic/frequency/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.3/fplab/intrinsic/frequency/__init__.py
--rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.1.3/fplab/intrinsic/frequency/projection.py
--rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.1.3/fplab/intrinsic/frequency/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.281979 fplab-0.0.1.3/fplab/intrinsic/mask/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.3/fplab/intrinsic/mask/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.281979 fplab-0.0.1.3/fplab/intrinsic/multiple/
--rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.1.3/fplab/intrinsic/multiple/__init__.py
--rw-rw-rw-   0        0        0     7036 2024-03-31 08:36:57.000000 fplab-0.0.1.3/fplab/intrinsic/multiple/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.295990 fplab-0.0.1.3/fplab/intrinsic/orientation/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.3/fplab/intrinsic/orientation/__init__.py
--rw-rw-rw-   0        0        0     7102 2024-03-31 08:46:45.000000 fplab-0.0.1.3/fplab/intrinsic/orientation/gradient.py
--rw-rw-rw-   0        0        0     5254 2024-04-01 02:18:24.000000 fplab-0.0.1.3/fplab/intrinsic/orientation/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.295990 fplab-0.0.1.3/fplab/matching/
--rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.1.3/fplab/matching/__init__.py
--rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.1.3/fplab/matching/matching.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.295990 fplab-0.0.1.3/fplab/minutiae/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.3/fplab/minutiae/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.311618 fplab-0.0.1.3/fplab/tools/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.1.3/fplab/tools/__init__.py
--rw-rw-rw-   0        0        0    13494 2024-03-25 14:10:10.000000 fplab-0.0.1.3/fplab/tools/array.py
--rw-rw-rw-   0        0        0     4651 2024-03-31 08:46:45.000000 fplab-0.0.1.3/fplab/tools/image.py
--rw-rw-rw-   0        0        0    15079 2024-03-31 08:46:45.000000 fplab-0.0.1.3/fplab/tools/nbis.py
--rw-rw-rw-   0        0        0    15550 2024-03-13 03:07:50.000000 fplab-0.0.1.3/fplab/tools/tensor.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:03:04.249055 fplab-0.0.1.3/fplab.egg-info/
--rw-rw-rw-   0        0        0      523 2024-04-05 04:03:04.000000 fplab-0.0.1.3/fplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      869 2024-04-05 04:03:04.000000 fplab-0.0.1.3/fplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 04:03:04.000000 fplab-0.0.1.3/fplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-05 04:03:04.000000 fplab-0.0.1.3/fplab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 04:03:04.311618 fplab-0.0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      801 2024-04-01 02:14:01.000000 fplab-0.0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.236638 fplab-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      521 2024-04-06 16:19:45.236638 fplab-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.175407 fplab-0.0.2/fplab/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2/fplab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.205306 fplab-0.0.2/fplab/enhancement/
+-rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.2/fplab/enhancement/__init__.py
+-rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.2/fplab/enhancement/frequency.py
+-rw-rw-rw-   0        0        0     4454 2024-03-31 13:48:46.000000 fplab-0.0.2/fplab/enhancement/spatial.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.205306 fplab-0.0.2/fplab/generation/
+-rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.2/fplab/generation/__init__.py
+-rw-rw-rw-   0        0        0     6948 2024-04-06 06:07:55.000000 fplab-0.0.2/fplab/generation/tps.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.205306 fplab-0.0.2/fplab/intrinsic/
+-rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.2/fplab/intrinsic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.220944 fplab-0.0.2/fplab/intrinsic/frequency/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2/fplab/intrinsic/frequency/__init__.py
+-rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.2/fplab/intrinsic/frequency/projection.py
+-rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.2/fplab/intrinsic/frequency/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.223622 fplab-0.0.2/fplab/intrinsic/mask/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2/fplab/intrinsic/mask/__init__.py
+-rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.2/fplab/intrinsic/mask/mask.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.224125 fplab-0.0.2/fplab/intrinsic/multiple/
+-rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.2/fplab/intrinsic/multiple/__init__.py
+-rw-rw-rw-   0        0        0     7036 2024-03-31 08:36:57.000000 fplab-0.0.2/fplab/intrinsic/multiple/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.224125 fplab-0.0.2/fplab/intrinsic/orientation/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2/fplab/intrinsic/orientation/__init__.py
+-rw-rw-rw-   0        0        0     6640 2024-04-06 09:18:53.000000 fplab-0.0.2/fplab/intrinsic/orientation/gradient.py
+-rw-rw-rw-   0        0        0     5490 2024-04-06 09:04:39.000000 fplab-0.0.2/fplab/intrinsic/orientation/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.224125 fplab-0.0.2/fplab/intrinsic/skeleton/
+-rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.2/fplab/intrinsic/skeleton/__init__.py
+-rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.2/fplab/intrinsic/skeleton/skeleton.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.236638 fplab-0.0.2/fplab/matching/
+-rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.2/fplab/matching/__init__.py
+-rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.2/fplab/matching/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.236638 fplab-0.0.2/fplab/minutiae/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2/fplab/minutiae/__init__.py
+-rw-rw-rw-   0        0        0     5997 2024-04-05 16:32:39.000000 fplab-0.0.2/fplab/minutiae/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.236638 fplab-0.0.2/fplab/tools/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2/fplab/tools/__init__.py
+-rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.2/fplab/tools/array.py
+-rw-rw-rw-   0        0        0     5367 2024-04-06 14:01:28.000000 fplab-0.0.2/fplab/tools/image.py
+-rw-rw-rw-   0        0        0    15076 2024-04-06 09:13:19.000000 fplab-0.0.2/fplab/tools/nbis.py
+-rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.2/fplab/tools/tensor.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:19:45.192789 fplab-0.0.2/fplab.egg-info/
+-rw-rw-rw-   0        0        0      521 2024-04-06 16:19:45.000000 fplab-0.0.2/fplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      986 2024-04-06 16:19:45.000000 fplab-0.0.2/fplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 16:19:45.000000 fplab-0.0.2/fplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-06 16:19:45.000000 fplab-0.0.2/fplab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 16:19:45.236638 fplab-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      799 2024-04-05 16:53:40.000000 fplab-0.0.2/setup.py
```

### Comparing `fplab-0.0.1.3/LICENSE.txt` & `fplab-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.3/PKG-INFO` & `fplab-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.1.3
+Version: 0.0.2
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.1.3/README.md` & `fplab-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 If you want to use this package, you should install all the required library:
 pytorch==1.13.1, 
 cuda==11.6,
 torchvision==0.14.1, 
 pillow, 
 numpy, 
 opencv, 
+opencv-contrib, 
 scipy,
 tqdm, 
 matplotlib
 
 The following is the recommended command.
 
 conda create -n fpLAB python=3.10
@@ -21,12 +22,14 @@
 
 conda install pillow
 
 conda install numpy
 
 pip install opencv
 
+pip install opencv-contrib-python
+
 conda install scipy
 
 conda install tqdm
 
 conda install matplotlib
```

### Comparing `fplab-0.0.1.3/fplab/enhancement/frequency.py` & `fplab-0.0.2/fplab/enhancement/frequency.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.3/fplab/enhancement/spatial.py` & `fplab-0.0.2/fplab/enhancement/spatial.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.3/fplab/intrinsic/frequency/projection.py` & `fplab-0.0.2/fplab/intrinsic/frequency/projection.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.3/fplab/intrinsic/frequency/tools.py` & `fplab-0.0.2/fplab/intrinsic/frequency/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.3/fplab/intrinsic/multiple/transform.py` & `fplab-0.0.2/fplab/intrinsic/multiple/transform.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.3/fplab/intrinsic/orientation/gradient.py` & `fplab-0.0.2/fplab/intrinsic/orientation/gradient.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,24 +34,20 @@
     cost, sint = torch.cos(out), torch.sin(out)
     g = hg**2+wg**2
     g_cos = imt_sum_average(g*cost*cost, wsp, kmd="s")
     g_sin = imt_sum_average(g*sint*sint, wsp, kmd="s")
     g_2cs = imt_sum_average(2*g*sint*cost, wsp, kmd="s")
     sum_g = imt_sum_average(g, wsp, kmd="s")
     cd = (cost*cost*g_cos+sint*sint*g_sin+cost*sint*g_2cs)/(sum_g+1e-8)
-    mk = cd.clone()
-    mk = imt_gaussian(mk, 9)
-    mk = torch.where(mk > 0, torch.ones_like(mk), torch.zeros_like(mk))
     out = type_as(out, im)
     cd = type_as(cd, im)
-    mk = type_as(mk, im)
     del ksp, wsp, imt, hg, wg, vy, vx
     del cost, sint, g, g_cos, g_sin, g_2cs, sum_g
     gc.collect()
-    return out, cd, mk
+    return out, cd
 
 
 def hong1998(im, blk_sz=(16, 16), wd_sz=(3, 3), device=None):
     """使用1998年HongLin使用的方法估计指纹方向场。
     首先使用1990年Rao的方法估计指纹方向场，然后使用高斯滤波平滑方向场
     im是需要处理的指纹图像。
     blk_sz是估计方向场时的图像块大小，可以为整数或2维向量。
@@ -103,23 +99,19 @@
     hwg, hhg, wwg = 2*hg*wg, hg*hg, wg*wg
     hwg = imt_gaussian(hwg, ksp)
     hhg = imt_gaussian(hhg, ksp)
     wwg = imt_gaussian(wwg, ksp)
     out = 0.5*torch.atan2(hwg, hhg-wwg)
     # 计算方向场可信度
     cd = torch.sqrt((hhg-wwg)**2+hwg**2)/(hhg+wwg+1e-8)
-    mk = cd.clone()
-    mk = imt_gaussian(mk, 9)
-    mk = torch.where(mk > 0, torch.ones_like(mk), torch.zeros_like(mk))
     out = type_as(out, im)
     cd = type_as(cd, im)
-    mk = type_as(mk, im)
     del ksp, imt, hg, wg, hwg, hhg, wwg
     gc.collect()
-    return out, cd, mk
+    return out, cd
 
 
 def scholar_x(im, blk_sz, sg_sz=(9, 9), sa_sz=(25, 25), device=None):
     """从网络上找到的方向场估计算法
     基于1990年Rao的方法，多次使用了高斯滤波平滑提取到的特征，使用了2002年Bazen的置信度计算方法
     im是需要处理的指纹图像。
     blk_sz是估计方向场时的图像块大小，可以为整数或2维向量。
@@ -163,15 +155,11 @@
     # 计算方向场可信度
     rho = (hhg+wwg)/rho
     rho = imt_pad_blk(rho, asp)[0]
     rho = imt_gaussian(rho, asp, s=asp, keep_shape=False) + 1e-8
     cd = torch.sqrt(cos2theta**2 + sin2theta**2) / rho
     cd = cd.repeat_interleave(asp[-1], -1).repeat_interleave(asp[-2], -2)
     cd = imt_pad_crop(cd, im_sp)
-    mk = cd.clone()
-    mk = imt_gaussian(mk, 9)
-    mk = torch.where(mk > 0, torch.ones_like(mk), torch.zeros_like(mk))
     cd = type_as(cd, im)
-    mk = type_as(mk, im)
     del ksp, gsp, asp, imt, hg, wg, hwg, hhg, wwg, rho, sin2theta, cos2theta
     gc.collect()
-    return out, cd, mk
+    return out, cd
```

### Comparing `fplab-0.0.1.3/fplab/intrinsic/orientation/tools.py` & `fplab-0.0.2/fplab/intrinsic/orientation/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,16 @@
     im为指纹图像，可以为(h, w, 3)或(h, w)的数组，(1, h, w)或(3, h, w)的张量，
     ot为对应的方向场，可以为(h, w)的数组或(1, h, w)的张量，以弧度形式表示角度，
     cd为方向场置信度，可以为(h, w)的数组或(1, h, w)的张量，值为0，1之间的浮点数，控制方向向量的长度，
     当cd缺省时，则取与ot大小相同的全一数组
     blk_sz为展示方向场的块大小，可以为整数或2维向量
     md决定计算块方向的方法，"m"表示使用块所有方向的均值，"c"表示使用块中心处的方向
     color为三元元组，控制绘制线段的RGB值，默认为红色
-    thickness为整数，控制绘制线段的宽度，默认为3
-    tip_length为0，1之间的浮点数，控制箭头相对于线段的长度，默认为0.1
+    thickness为整数，控制绘制线段的宽度，默认为1
+    tip_length为0，1之间的浮点数，控制箭头相对于线段的长度，默认为0.3
     flag控制函数的行为：展示结果图像（"show"）、保存结果图像（"save"）、返回结果图像（"return"）
     "save"命令需要配合save_path使用，若未指定save_path，则该命令将不会起作用"""
     if isinstance(blk_sz, int):
         ksp = blk_sz, blk_sz
     else:
         ksp = blk_sz
     # 方向线段将画到ima上
@@ -105,10 +105,14 @@
         ima_show(out)
     if "save" in flag and save_path:
         ima_save(out, save_path)
     if "return" in flag:
         return type_as(out, im)
 
 
-def compare_orientation_nd(o1, o2, c):
-    """比较两个无向方向场的相似度"""
-    return ((np.cos(2*(o1-o2)))*c).sum()/c.sum()
+def compare_orientation_nd(ot1, ot2, oc):
+    """比较两个无向方向场的相似度
+    ot1, ot2        无向方向场，可以为数组或张量
+    oc              方向场可信度或者mask，可以为数组或张量
+    """
+    ota1, ota2, oca = type_as(ot1, "a"), type_as(ot2, "a"), type_as(oc, "a")
+    return ((np.cos(2*(ota1-ota2)))*oca).sum()/oca.sum()
```

### Comparing `fplab-0.0.1.3/fplab/matching/matching.py` & `fplab-0.0.2/fplab/matching/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.1.3/fplab/tools/array.py` & `fplab-0.0.2/fplab/tools/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 ima_pad_blk         根据块大小填充图像
 ima_conv2d          2维卷积
 ima_sum_average     局部求和、求平均
 ima_gaussian        高斯模糊
 ima_cal_grad        计算梯度
 """
 from PIL import Image
+from pathlib import Path
 import numpy as np
 import gc
 import typing
 import cv2
 
 
 class IMA:
     def __init__(self, ima):
         self.ima = ima
+        self.shape = ima.shape
 
     @ staticmethod
     def read(path):
         """读取图像"""
         return IMA(ima_read(path))
 
     def show(self):
@@ -93,16 +95,20 @@
 
     def cal_grad(self, md="sobel", pad_md="reflect101"):
         """计算梯度"""
         g_h, g_w = ima_cal_grad(self.ima, md=md, pad_md=pad_md)
         return IMA(g_h), IMA(g_w)
 
 
-def ima_read(path):
-    """读取路径为path的图像，输出大小为(h, w)或(h, w, 3)，取值为0，1之间的float32值"""
+def ima_read(im_p):
+    """读取路径为im_p的图像，输出大小为(h, w)或(h, w, 3)，取值为0，1之间的float32值"""
+    if isinstance(im_p, str):
+        path = Path(im_p)
+    else:
+        path = im_p
     im = Image.open(path)
     if im.mode not in ["L", "RGB"]:
         im = im.convert("RGB")
     ima = np.asarray(im, dtype=np.float32) / 255.
     del im
     gc.collect()
     return ima
@@ -120,18 +126,22 @@
     ima = ima.astype(np.uint8)
     im = Image.fromarray(ima, mode=md)
     im.show()
     del ima, im, md
     gc.collect()
 
 
-def ima_save(ima_in, path):
-    """保存数组ima_in所表示的图像到path，
+def ima_save(ima_in, im_p):
+    """保存数组ima_in所表示的图像到im_p，
     ima_in形状为(h, w)或(h, w, 3)，取值为0，1之间的float32值，
-    path为pathlib的Path对象"""
+    im_p为pathlib的Path对象"""
+    if isinstance(im_p, str):
+        path = Path(im_p)
+    else:
+        path = im_p
     ima = np.clip(ima_in, 0., 1.)
     ima = ima.squeeze()
     md = 'L'
     if ima.ndim == 3:
         md = 'RGB'
     ima = ima * 255
     ima = np.round(ima)
```

### Comparing `fplab-0.0.1.3/fplab/tools/image.py` & `fplab-0.0.2/fplab/tools/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,19 @@
     """
     获得data_folder_path路径下的所有指定格式ext（默认为PIL库支持读取的所有格式）的文件的绝对路径字符串列表
     当top_flag为True时，会对输出字符串排序
     data_folder_path是一个Path对象, data_dirs是一个字符串列表，ext是一个字符串列表，top_flag为布尔值
     """
     if not ext:
         ext = get_support_extensions()
-    for path in data_folder_path.iterdir():
+    if isinstance(data_folder_path, str):
+        data_folder_p = Path(data_folder_path)
+    else:
+        data_folder_p = data_folder_path
+    for path in data_folder_p.iterdir():
         if path.is_dir():
             data_dirs = get_data_dirs(path, data_dirs, ext=ext, top_flag=False)
         elif path.suffix in ext:
             data_dirs.append(str(path.absolute()))
     if top_flag:
         data_dirs = sorted(data_dirs)
     return data_dirs
@@ -89,38 +93,53 @@
         elif isinstance(im, torch.Tensor):
             out = im.clone()
         else:
             raise Exception("Error!")
     return out
 
 
-def change_image(im_pt, sv_pt=None, ext=None, dpi=None, md=None, rm_flag=False):
+def change_image(im_pt, sv_pt=None, ext=None, dpi=None, md=None, rm_flag=False, re_sz=None, rs_md='bicubic'):
     """改变图像的属性
     im_pt, 图像路径
     sv_pt, 图像保存路径，默认为图像所在文件夹的路径
     ext, 指定图像后缀名
     dpi, 指定图像分辨率
     md, 指定图像类型：'RGB' 表示转化为RGB图像, 'L' 表示转化为灰度图像的方法，
-    rm_flag控制是否删除原图像"""
+    rm_flag控制是否删除原图像
+    re_sz, 指定图像大小，可以为整数或2元整数元组
+    rs_md, 改变图像大小方法：'bicubic'、'nearest'、'box'、'bilinear'、'hamming'、'lanczos'"""
+    if isinstance(im_pt, str):
+        im_p = Path(im_pt)
+    else:
+        im_p = im_pt
     if not sv_pt:
-        save_path = im_pt.parent
+        save_path = im_p.parent
     else:
-        save_path = sv_pt
+        if isinstance(sv_pt, str):
+            save_path = Path(sv_pt)
+        else:
+            save_path = sv_pt
     if not ext:
-        save_path = save_path / im_pt.name
+        save_path = save_path / im_p.name
     else:
-        save_path = save_path / (im_pt.stem+ext)
-    im = Image.open(im_pt)
+        save_path = save_path / (im_p.stem+ext)
+    im = Image.open(im_p)
     if md:
         im = im.convert(md)
+    if re_sz:
+        if isinstance(re_sz, int):
+            sz = (re_sz, re_sz)
+        else:
+            sz = re_sz
+        im = im.resize(sz, resample=eval("Image." + rs_md.upper()))
     if dpi:
         if isinstance(dpi, (int, float)):
             im_dpi = dpi, dpi
         else:
             im_dpi = dpi
         im.info['dpi'] = im_dpi
         im.save(save_path, dpi=im_dpi)
     else:
         im.save(save_path)
     if rm_flag:
-        im_pt.unlink()
+        im_p.unlink()
     return save_path
```

### Comparing `fplab-0.0.1.3/fplab/tools/nbis.py` & `fplab-0.0.2/fplab/tools/nbis.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 import numpy as np
 from os import popen, system
 from pathlib import Path
 from fplab.tools.image import change_image, get_data_dirs
 from time import strftime, localtime
 from tqdm import tqdm
-from fplab.matching.matching import analyse_score
+from fplab.matching.tools import analyse_score
 
 
 def nfiq(im_dir, src_dir=r'C:\SRC\NBIS\Main\bin\nfiq.exe', temp_flag=True, temp_dir=None):
     """封装NBIS的NFIQ程序
     im_dir是图像路径
     src_dir是NFIQ源程序路径
     temp_flag控制是否生成缓存文件
```

### Comparing `fplab-0.0.1.3/fplab/tools/tensor.py` & `fplab-0.0.2/fplab/tools/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 imt_pad_blk         根据块大小填充图像
 imt_conv2d          2维卷积
 imt_sum_average     局部求和、求平均
 imt_gaussian        高斯模糊、高斯池化
 imt_cal_grad        计算梯度
 """
 from PIL import Image
+from pathlib import Path
 import numpy as np
 import torch
 import gc
 
 
 class IMT:
     def __init__(self, imt):
         self.imt = imt
+        self.shape = imt.shape
 
     @ staticmethod
     def read(path, device='cpu'):
         """读取图像"""
         return IMT(imt_read(path, device=device))
 
     def show(self):
@@ -84,17 +86,21 @@
 
     def cal_grad(self, md="sobel", pad_md="reflect", pad_v=0, **kwargs):
         """计算梯度"""
         g_h, g_w = imt_cal_grad(self.imt, md=md, pad_md=pad_md, pad_v=pad_v,  **kwargs)
         return IMT(g_h), IMT(g_w)
 
 
-def imt_read(path, device='cpu'):
-    """读取路径为path的图像，设置device为指定值，
+def imt_read(im_p, device='cpu'):
+    """读取路径为im_p的图像，设置device为指定值，
     图像元素类型为0，1之间的float32值，大小为(3,h,w)或(1,h,w)"""
+    if isinstance(im_p, str):
+        path = Path(im_p)
+    else:
+        path = im_p
     im = Image.open(path)
     if im.mode not in ["L", "RGB"]:
         im = im.convert("RGB")
     ima = np.asarray(im, dtype=np.float32) / 255.
     imt = torch.from_numpy(ima)
     imt = imt.to(device)
     if imt.ndim == 3:
@@ -121,18 +127,22 @@
     ima = ima.astype(np.uint8)
     im = Image.fromarray(ima, mode=md)
     im.show()
     del imt, ima, im, md
     gc.collect()
 
 
-def imt_save(imt_in, path):
-    """保存tensor向量imt_in所表示的图像到path，
+def imt_save(imt_in, im_p):
+    """保存tensor向量imt_in所表示的图像到im_p，
     imt_in元素应为0，1之间的值，形状为(3, h, w)或(h, w)，
-    path为pathlib的Path对象"""
+    im_p为pathlib的Path对象"""
+    if isinstance(im_p, str):
+        path = Path(im_p)
+    else:
+        path = im_p
     imt = torch.clip(imt_in, 0., 1.)
     imt = imt.squeeze()
     md = 'L'
     if imt.ndim == 3:
         imt = imt.permute(1, 2, 0)
         md = 'RGB'
     imt = imt.to('cpu')
```

### Comparing `fplab-0.0.1.3/fplab.egg-info/PKG-INFO` & `fplab-0.0.2/fplab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.1.3
+Version: 0.0.2
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.1.3/fplab.egg-info/SOURCES.txt` & `fplab-0.0.2/fplab.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 fplab.egg-info/SOURCES.txt
 fplab.egg-info/dependency_links.txt
 fplab.egg-info/top_level.txt
 fplab/enhancement/__init__.py
 fplab/enhancement/frequency.py
 fplab/enhancement/spatial.py
 fplab/generation/__init__.py
-fplab/generation/distortion.py
+fplab/generation/tps.py
 fplab/intrinsic/__init__.py
 fplab/intrinsic/frequency/__init__.py
 fplab/intrinsic/frequency/projection.py
 fplab/intrinsic/frequency/tools.py
 fplab/intrinsic/mask/__init__.py
+fplab/intrinsic/mask/mask.py
 fplab/intrinsic/multiple/__init__.py
 fplab/intrinsic/multiple/transform.py
 fplab/intrinsic/orientation/__init__.py
 fplab/intrinsic/orientation/gradient.py
 fplab/intrinsic/orientation/tools.py
+fplab/intrinsic/skeleton/__init__.py
+fplab/intrinsic/skeleton/skeleton.py
 fplab/matching/__init__.py
-fplab/matching/matching.py
+fplab/matching/tools.py
 fplab/minutiae/__init__.py
+fplab/minutiae/tools.py
 fplab/tools/__init__.py
 fplab/tools/array.py
 fplab/tools/image.py
 fplab/tools/nbis.py
 fplab/tools/tensor.py
```

### Comparing `fplab-0.0.1.3/setup.py` & `fplab-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1.3'
+VERSION = '0.0.2'
 DESCRIPTION = 'Python3 Package for Fingerprint Processing'
 LONG_DESCRIPTION = ('This is a python3 package for fingerprint processing,'
                     ' which can be used for fingerprint enhancement.')
 
 setup(
     name="fplab",
     version=VERSION,
```

