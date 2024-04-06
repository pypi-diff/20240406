# Comparing `tmp/lungmask-0.2.19.tar.gz` & `tmp/lungmask-0.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lungmask-0.2.19.tar", last modified: Sat Jan  6 08:23:17 2024, max compression
+gzip compressed data, was "lungmask-0.2.20.tar", last modified: Sat Apr  6 09:51:01 2024, max compression
```

## Comparing `lungmask-0.2.19.tar` & `lungmask-0.2.20.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 08:23:17.180444 lungmask-0.2.19/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-06 08:23:08.000000 lungmask-0.2.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-01-06 08:23:17.180444 lungmask-0.2.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-01-06 08:23:08.000000 lungmask-0.2.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 08:23:17.176444 lungmask-0.2.19/lungmask/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-06 08:23:08.000000 lungmask-0.2.19/lungmask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-01-06 08:23:08.000000 lungmask-0.2.19/lungmask/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-06 08:23:08.000000 lungmask-0.2.19/lungmask/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-01-06 08:23:08.000000 lungmask-0.2.19/lungmask/mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-01-06 08:23:08.000000 lungmask-0.2.19/lungmask/resunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14202 2024-01-06 08:23:08.000000 lungmask-0.2.19/lungmask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 08:23:17.180444 lungmask-0.2.19/lungmask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-01-06 08:23:17.000000 lungmask-0.2.19/lungmask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-01-06 08:23:17.000000 lungmask-0.2.19/lungmask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 08:23:17.000000 lungmask-0.2.19/lungmask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-06 08:23:17.000000 lungmask-0.2.19/lungmask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-06 08:23:17.000000 lungmask-0.2.19/lungmask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-06 08:23:17.000000 lungmask-0.2.19/lungmask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-01-06 08:23:08.000000 lungmask-0.2.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 08:23:17.180444 lungmask-0.2.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-01-06 08:23:08.000000 lungmask-0.2.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 08:23:17.180444 lungmask-0.2.19/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-06 08:23:08.000000 lungmask-0.2.19/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-01-06 08:23:08.000000 lungmask-0.2.19/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-01-06 08:23:08.000000 lungmask-0.2.19/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:51:01.712046 lungmask-0.2.20/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 09:50:56.000000 lungmask-0.2.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-06 09:51:01.712046 lungmask-0.2.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-06 09:50:56.000000 lungmask-0.2.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:51:01.712046 lungmask-0.2.20/lungmask/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-06 09:50:56.000000 lungmask-0.2.20/lungmask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-06 09:50:56.000000 lungmask-0.2.20/lungmask/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-06 09:50:56.000000 lungmask-0.2.20/lungmask/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-04-06 09:50:56.000000 lungmask-0.2.20/lungmask/mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-06 09:50:56.000000 lungmask-0.2.20/lungmask/resunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-04-06 09:50:56.000000 lungmask-0.2.20/lungmask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:51:01.712046 lungmask-0.2.20/lungmask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-06 09:51:01.000000 lungmask-0.2.20/lungmask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-06 09:51:01.000000 lungmask-0.2.20/lungmask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 09:51:01.000000 lungmask-0.2.20/lungmask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 09:51:01.000000 lungmask-0.2.20/lungmask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 09:51:01.000000 lungmask-0.2.20/lungmask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 09:51:01.000000 lungmask-0.2.20/lungmask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-06 09:50:56.000000 lungmask-0.2.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 09:51:01.712046 lungmask-0.2.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-06 09:50:56.000000 lungmask-0.2.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:51:01.712046 lungmask-0.2.20/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-06 09:50:56.000000 lungmask-0.2.20/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-06 09:50:56.000000 lungmask-0.2.20/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-06 09:50:56.000000 lungmask-0.2.20/tests/test_utils.py
```

### Comparing `lungmask-0.2.19/LICENSE` & `lungmask-0.2.20/LICENSE`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.19/PKG-INFO` & `lungmask-0.2.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lungmask
-Version: 0.2.19
+Version: 0.2.20
 Summary: Package for automated lung segmentation in CT
 Home-page: https://github.com/JoHof/lungmask
 Author: Johannes Hofmanninger
-Author-email: johannes.hofmanninger@gmail.com
+Author-email: j.hofmanninger@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydicom
 Requires-Dist: numpy
@@ -127,8 +127,9 @@
 ```
 lungmask INPUT OUTPUT --modelname R231CovidWeb
 ```
 The regular U-net(R231) model works very well for COVID-19 CT scans. However, collections of slices and case reports from the web are often cropped, annotated or encoded in regular image formats so that the original hounsfield unit (HU) values can only be estimated. The training data of the U-net(R231CovidWeb) model was augmented with COVID-19 slices that were mapped back from regular imaging formats to HU. The data was collected and prepared by MedSeg (http://medicalsegmentation.com/covid19/). While the regular U-net(R231) showed very good results for these images there may be cases for which this model will yield slighty improved segmentations. Note that you have to map images back to HU when using images from the web. This [blog post](https://medium.com/@hbjenssen/covid-19-radiology-data-collection-and-preparation-for-artificial-intelligence-4ecece97bb5b) describes how you can do that. Alternatively you can set the ```--noHU``` tag.
 ![alt text](figures/example_covid.jpg "COVID examples")
 
 ## jpg, png and non HU images
+**This feature is only available in versions between 0.2.5 and 0.2.14**
 As of version 0.2.5 these images are supported. Use the ```--noHU``` tag if you process images that are not encoded in HU. Keep in mind that the models were trained on proper CT scans encoded in HU. The results on cropped, annotated, very high and very low intensity shifted images may not be very reliable. When using the ```--noHU``` tag only single slices can be processed.
```

### Comparing `lungmask-0.2.19/README.md` & `lungmask-0.2.20/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -105,8 +105,9 @@
 ```
 lungmask INPUT OUTPUT --modelname R231CovidWeb
 ```
 The regular U-net(R231) model works very well for COVID-19 CT scans. However, collections of slices and case reports from the web are often cropped, annotated or encoded in regular image formats so that the original hounsfield unit (HU) values can only be estimated. The training data of the U-net(R231CovidWeb) model was augmented with COVID-19 slices that were mapped back from regular imaging formats to HU. The data was collected and prepared by MedSeg (http://medicalsegmentation.com/covid19/). While the regular U-net(R231) showed very good results for these images there may be cases for which this model will yield slighty improved segmentations. Note that you have to map images back to HU when using images from the web. This [blog post](https://medium.com/@hbjenssen/covid-19-radiology-data-collection-and-preparation-for-artificial-intelligence-4ecece97bb5b) describes how you can do that. Alternatively you can set the ```--noHU``` tag.
 ![alt text](figures/example_covid.jpg "COVID examples")
 
 ## jpg, png and non HU images
+**This feature is only available in versions between 0.2.5 and 0.2.14**
 As of version 0.2.5 these images are supported. Use the ```--noHU``` tag if you process images that are not encoded in HU. Keep in mind that the models were trained on proper CT scans encoded in HU. The results on cropped, annotated, very high and very low intensity shifted images may not be very reliable. When using the ```--noHU``` tag only single slices can be processed.
```

### Comparing `lungmask-0.2.19/lungmask/__main__.py` & `lungmask-0.2.20/lungmask/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,46 +29,34 @@
         type=path,
         help="Path to the input image, can be a folder for dicoms",
     )
     parser.add_argument(
         "output", metavar="output", type=str, help="Filepath for output lungmask"
     )
     parser.add_argument(
-        "--modeltype", help="Default: unet", type=str, choices=["unet"], default="unet"
-    )
-    parser.add_argument(
         "--modelname",
         help="spcifies the trained model, Default: R231",
         type=str,
         choices=["R231", "LTRCLobes", "LTRCLobes_R231", "R231CovidWeb"],
         default="R231",
     )
     parser.add_argument(
         "--modelpath", help="spcifies the path to the trained model", default=None
     )
     parser.add_argument(
-        "--classes",
-        help="spcifies the number of output classes of the model",
-    )
-    parser.add_argument(
         "--cpu",
         help="Force using the CPU even when a GPU is available, will override batchsize to 1",
         action="store_true",
     )
     parser.add_argument(
         "--nopostprocess",
         help="Deactivates postprocessing (removal of unconnected components and hole filling)",
         action="store_true",
     )
     parser.add_argument(
-        "--noHU",
-        help="For processing of images that are not encoded in hounsfield units (HU). E.g. png or jpg images from the web. Be aware, results may be substantially worse on these images",
-        action="store_true",
-    )
-    parser.add_argument(
         "--batchsize",
         type=int,
         help="Number of slices processed simultaneously. Lower number requires less memory but may be slower.",
         default=20,
     )
     parser.add_argument(
         "--noprogress",
@@ -77,65 +65,85 @@
     )
     parser.add_argument(
         "--version",
         help="Shows the current version of lungmask",
         action="version",
         version=version,
     )
+    parser.add_argument(
+        "--removemetadata",
+        action="store_true",
+        help="Do not keep study/patient related metadata of the input, if any. Only affects output file formats that can store such information (e.g. DICOM).",
+    )
 
     argsin = sys.argv[1:]
     args = parser.parse_args(argsin)
 
-    if args.classes is not None:
-        logger.warn(
-            "!!! Warning: The `classes` parameter is deprecated and will be removed in the next version !!!"
-        )
-
     batchsize = args.batchsize
     if args.cpu:
         batchsize = 1
 
+    # keeping any Patient / Study info is the default, deactivate in case of arg specified or non-HU data
+    keepmetadata = not args.removemetadata
+
     logger.info("Load model")
 
-    input_image = utils.load_input_image(args.input, disable_tqdm=args.noprogress)
+    input_image = utils.load_input_image(
+        args.input, disable_tqdm=args.noprogress, read_metadata=keepmetadata
+    )
+
     logger.info("Infer lungmask")
     if args.modelname == "LTRCLobes_R231":
         assert (
             args.modelpath is None
         ), "Modelpath can not be specified for LTRCLobes_R231 mode"
         inferer = LMInferer(
             modelname="LTRCLobes",
             force_cpu=args.cpu,
             fillmodel="R231",
             batch_size=batchsize,
             volume_postprocessing=not (args.nopostprocess),
-            noHU=args.noHU,
             tqdm_disable=args.noprogress,
         )
         result = inferer.apply(input_image)
     else:
         inferer = LMInferer(
             modelname=args.modelname,
             modelpath=args.modelpath,
             force_cpu=args.cpu,
             batch_size=batchsize,
             volume_postprocessing=not (args.nopostprocess),
-            noHU=args.noHU,
             tqdm_disable=args.noprogress,
         )
         result = inferer.apply(input_image)
 
-    if args.noHU:
-        file_ending = args.output.split(".")[-1]
-        if file_ending in ["jpg", "jpeg", "png"]:
-            result = (result / (result.max()) * 255).astype(np.uint8)
-        result = result[0]
-
     result_out = sitk.GetImageFromArray(result)
     result_out.CopyInformation(input_image)
+
+    writer = sitk.ImageFileWriter()
+    writer.SetFileName(args.output)
+
+    if keepmetadata:
+        # keep the Study Instance UID
+        writer.SetKeepOriginalImageUID(True)
+
+        DICOM_tags_to_keep = utils.get_DICOM_tags_to_keep()
+
+        # copy the DICOM tags we want to keep
+        for key in input_image.GetMetaDataKeys():
+            if key in DICOM_tags_to_keep:
+                result_out.SetMetaData(key, input_image.GetMetaData(key))
+
+        # set the Series Description tag
+        result_out.SetMetaData("0008|103e", "Created with lungmask")
+
+        # set WL/WW
+        result_out.SetMetaData("0028|1050", "1")  # Window Center
+        result_out.SetMetaData("0028|1051", "2")  # Window Width
+
     logger.info(f"Save result to: {args.output}")
-    sitk.WriteImage(result_out, args.output)
+    writer.Execute(result_out)
 
 
 if __name__ == "__main__":
     print("called as script")
     main()
```

### Comparing `lungmask-0.2.19/lungmask/mask.py` & `lungmask-0.2.20/lungmask/mask.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,28 +74,26 @@
         modelname: str = "R231",
         modelpath: Optional[str] = None,
         fillmodel: Optional[str] = None,
         fillmodel_path: Optional[str] = None,
         force_cpu: bool = False,
         batch_size: int = 20,
         volume_postprocessing: bool = True,
-        noHU: bool = False,
         tqdm_disable: bool = False,
     ):
         """LungMaskInference
 
         Args:
             modelname (str, optional): Model to be applied. Defaults to 'R231'.
             modelpath (str, optional): Path to modeleights. `modelname` parameter will be ignored if provided. Defaults to None.
             fillmodel (Optional[str], optional): Fillmodel to be applied. Defaults to None.
             fillmodel_path (Optional[str], optional): Path to weights for fillmodel. `fillmodel` parameter will be ignored if provided. Defaults to None.
             force_cpu (bool, optional): Will not use GPU is `True`. Defaults to False.
             batch_size (int, optional): Batch size. Defaults to 20.
             volume_postprocessing (bool, optional): If `Fales` will not perform postprocessing (connected component analysis). Defaults to True.
-            noHU (bool, optional): If `True` no HU intensities are expected. Not recommended. Defaults to False.
             tqdm_disable (bool, optional): If `True`, will disable progress bar. Defaults to False.
         """
         assert (
             modelname in MODEL_URLS
         ), "Modelname not found. Please choose from: {}".format(MODEL_URLS.keys())
         if fillmodel is not None:
             assert (
@@ -109,15 +107,14 @@
             fillmodel = os.path.basename(fillmodel_path)
 
         self.fillmodel = fillmodel
         self.modelname = modelname
         self.force_cpu = force_cpu
         self.batch_size = batch_size
         self.volume_postprocessing = volume_postprocessing
-        self.noHU = noHU
         self.tqdm_disable = tqdm_disable
 
         self.model = get_model(self.modelname, modelpath)
 
         self.device = torch.device("cpu")
         if not self.force_cpu:
             if torch.cuda.is_available():
@@ -162,28 +159,17 @@
                     image.GetDirection()
                 )
             )
             if curr_orient != "LPS":
                 image = sitk.DICOMOrient(image, "LPS")
             inimg_raw = sitk.GetArrayFromImage(image)
 
-        if self.noHU:
-            # support for non HU images. This is just a hack. The models were not trained with this in mind
-            tvolslices = skimage.color.rgb2gray(inimg_raw)
-            tvolslices = skimage.transform.resize(tvolslices, [256, 256])
-            tvolslices = np.asarray([tvolslices * x for x in np.linspace(0.3, 2, 20)])
-            tvolslices[tvolslices > 1] = 1
-            sanity = [
-                (tvolslices[x] > 0.6).sum() > 25000 for x in range(len(tvolslices))
-            ]
-            tvolslices = tvolslices[sanity]
-        else:
-            tvolslices, xnew_box = utils.preprocess(inimg_raw, resolution=[256, 256])
-            tvolslices[tvolslices > 600] = 600
-            tvolslices = np.divide((tvolslices + 1024), 1624)
+        tvolslices, xnew_box = utils.preprocess(inimg_raw, resolution=[256, 256])
+        tvolslices[tvolslices > 600] = 600
+        tvolslices = np.divide((tvolslices + 1024), 1624)
 
         timage_res = np.empty((np.append(0, tvolslices[0].shape)), dtype=np.uint8)
 
         with torch.inference_mode():
             for mbnp in tqdm(
                 chunked(tvolslices, self.batch_size),
                 disable=self.tqdm_disable,
@@ -203,30 +189,21 @@
         # postprocessing includes removal of small connected components, hole filling and mapping of small components to
         # neighbors
         if self.volume_postprocessing:
             outmask = utils.postprocessing(timage_res, disable_tqdm=self.tqdm_disable)
         else:
             outmask = timage_res
 
-        if self.noHU:
-            outmask = skimage.transform.resize(
-                outmask[np.argmax((outmask == 1).sum(axis=(1, 2)))],
-                inimg_raw.shape[:2],
-                order=0,
-                anti_aliasing=False,
-                preserve_range=True,
-            )[None, :, :]
-        else:
-            outmask = np.asarray(
-                [
-                    utils.reshape_mask(outmask[i], xnew_box[i], inimg_raw.shape[1:])
-                    for i in range(outmask.shape[0])
-                ],
-                dtype=np.uint8,
-            )
+        outmask = np.asarray(
+            [
+                utils.reshape_mask(outmask[i], xnew_box[i], inimg_raw.shape[1:])
+                for i in range(outmask.shape[0])
+            ],
+            dtype=np.uint8,
+        )
 
         if not numpy_mode:
             if curr_orient != "LPS":
                 outmask = sitk.GetImageFromArray(outmask)
                 outmask = sitk.DICOMOrient(outmask, curr_orient)
                 outmask = sitk.GetArrayFromImage(outmask)
 
@@ -257,50 +234,46 @@
 
 def apply(
     image: Union[sitk.Image, np.ndarray],
     model=None,
     force_cpu=False,
     batch_size=20,
     volume_postprocessing=True,
-    noHU=False,
     tqdm_disable=False,
 ):
     warnings.warn(
         "The function `apply` will be removed in a future version. Please use the LMInferer class!",
         DeprecationWarning,
     )
     inferer = LMInferer(
         force_cpu=force_cpu,
         batch_size=batch_size,
         volume_postprocessing=volume_postprocessing,
-        noHU=noHU,
         tqdm_disable=tqdm_disable,
     )
     if model is not None:
         inferer.model = model.to(inferer.device)
     return inferer.apply(image)
 
 
 def apply_fused(
     image,
     basemodel="LTRCLobes",
     fillmodel="R231",
     force_cpu=False,
     batch_size=20,
     volume_postprocessing=True,
-    noHU=False,
     tqdm_disable=False,
 ):
     warnings.warn(
         "The function `apply_fused` will be removed in a future version. Please use the LMInferer class!",
         DeprecationWarning,
     )
     inferer = LMInferer(
         modelname=basemodel,
         force_cpu=force_cpu,
         fillmodel=fillmodel,
         batch_size=batch_size,
         volume_postprocessing=volume_postprocessing,
-        noHU=noHU,
         tqdm_disable=tqdm_disable,
     )
     return inferer.apply(image)
```

### Comparing `lungmask-0.2.19/lungmask/resunet.py` & `lungmask-0.2.20/lungmask/resunet.py`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.19/lungmask/utils.py` & `lungmask-0.2.20/lungmask/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,28 @@
 import skimage.morphology
 from scipy import ndimage
 from torch.utils.data import Dataset
 from tqdm import tqdm
 
 from lungmask.logger import logger
 
+DICOM_METADATA_TO_KEEP = (
+    '0008|0020', # StudyDate
+    '0008|0030', # StudyTime
+    '0008|0050', # AccessionNumber
+    '0008|0090', # ReferringPhysicianName
+    '0008|1030', # StudyDescription
+    '0010|0010', # PatientName
+    '0010|0020', # PatientID
+    '0010|0030', # PatientBirthDate
+    '0010|0040', # PatientSex
+    '0018|5100', # Patient Position
+    '0020|000d', # StudyInstanceUID
+    '0020|0010'  # StudyID
+)
 
 def preprocess(
     img: np.ndarray, resolution: list = [192, 192]
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Preprocesses the image by clipping, cropping and resizing. Clipping at -1024 and 600 HU, cropping to the body
 
     Args:
@@ -111,16 +125,17 @@
     res = np.ones(origsize) * 0
     resize = [tbox[2] - tbox[0], tbox[3] - tbox[1]]
     imgres = ndimage.zoom(mask, resize / np.asarray(mask.shape), order=0)
     res[tbox[0] : tbox[2], tbox[1] : tbox[3]] = imgres
     return res
 
 
-def read_dicoms(path, primary=True, original=True, disable_tqdm=False):
+def read_dicoms(path, primary=True, original=True, disable_tqdm=False, read_metadata=False):
     allfnames = []
+    
     for dir, _, fnames in os.walk(path):
         [allfnames.append(os.path.join(dir, fname)) for fname in fnames]
 
     dcm_header_info = []
     unique_set = (
         []
     )  # need this because too often there are duplicates of dicom files with different names
@@ -195,37 +210,56 @@
             [np.asarray(x[2]) for x in dcm_header_info[info_idxs, 3]]
         )
         slicesort_idx = np.argsort(positions)
         vol_files = vol_files[slicesort_idx]
         relevant_series.append(vol_files)
         reader = sitk.ImageSeriesReader()
         reader.SetFileNames(vol_files)
+
+        if read_metadata:
+            reader.SetMetaDataDictionaryArrayUpdate(True)
+            reader.LoadPrivateTagsOn()
+
         vol = reader.Execute()
+
+        if read_metadata:
+            for key in reader.GetMetaDataKeys(0):
+                vol.SetMetaData(key, reader.GetMetaData(0, key))
+
         relevant_volumes.append(vol)
 
     return relevant_volumes
 
 
-def load_input_image(path: str, disable_tqdm=False) -> sitk.Image:
+def load_input_image(path: str, disable_tqdm=False, read_metadata=False) -> sitk.Image:
     """Loads image, if path points to a file, file will be loaded. If path points ot a folder, a DICOM series will be loaded. If multiple series are present, the largest series (higher number of slices) will be loaded.
 
     Args:
         path (str): File or folderpath to be loaded. If folder, DICOM series is expected
         disable_tqdm (bool, optional): Disable tqdm progress bar. Defaults to False.
+        read_metadata (bool, optional): Read the metadata - including DICOM tags - from the input and store in the loaded image
 
     Returns:
         sitk.Image: Loaded image
     """
     if os.path.isfile(path):
         logger.info(f"Read input: {path}")
-        input_image = sitk.ReadImage(path)
+
+        reader = sitk.ImageFileReader()
+        reader.SetFileName(path)
+        input_image = reader.Execute()
+
+        if read_metadata:
+            for key in reader.GetMetaDataKeys():
+                input_image.SetMetaData(key, reader.GetMetaData(key))
+                
     else:
         logger.info(f"Looking for dicoms in {path}")
         dicom_vols = read_dicoms(
-            path, original=False, primary=False, disable_tqdm=disable_tqdm
+            path, original=False, primary=False, disable_tqdm=disable_tqdm, read_metadata=read_metadata
         )
         if len(dicom_vols) < 1:
             sys.exit("No dicoms found!")
         if len(dicom_vols) > 1:
             logger.warning(
                 "There are more than one volume in the path, will take the largest one"
             )
@@ -364,7 +398,18 @@
     """
     mask = skimage.measure.label(mask)
     regions = skimage.measure.regionprops(mask)
     resizes = np.asarray([x.area for x in regions])
     max_region = np.argsort(resizes)[-1] + 1
     mask = mask == max_region
     return mask
+
+def get_DICOM_tags_to_keep():
+    """Returns the DICOM metadata to keep
+
+    Args:
+        none
+
+    Returns:
+        Tuple with the DICOM tags to keep
+    """
+    return DICOM_METADATA_TO_KEEP
```

### Comparing `lungmask-0.2.19/lungmask.egg-info/PKG-INFO` & `lungmask-0.2.20/lungmask.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lungmask
-Version: 0.2.19
+Version: 0.2.20
 Summary: Package for automated lung segmentation in CT
 Home-page: https://github.com/JoHof/lungmask
 Author: Johannes Hofmanninger
-Author-email: johannes.hofmanninger@gmail.com
+Author-email: j.hofmanninger@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydicom
 Requires-Dist: numpy
@@ -127,8 +127,9 @@
 ```
 lungmask INPUT OUTPUT --modelname R231CovidWeb
 ```
 The regular U-net(R231) model works very well for COVID-19 CT scans. However, collections of slices and case reports from the web are often cropped, annotated or encoded in regular image formats so that the original hounsfield unit (HU) values can only be estimated. The training data of the U-net(R231CovidWeb) model was augmented with COVID-19 slices that were mapped back from regular imaging formats to HU. The data was collected and prepared by MedSeg (http://medicalsegmentation.com/covid19/). While the regular U-net(R231) showed very good results for these images there may be cases for which this model will yield slighty improved segmentations. Note that you have to map images back to HU when using images from the web. This [blog post](https://medium.com/@hbjenssen/covid-19-radiology-data-collection-and-preparation-for-artificial-intelligence-4ecece97bb5b) describes how you can do that. Alternatively you can set the ```--noHU``` tag.
 ![alt text](figures/example_covid.jpg "COVID examples")
 
 ## jpg, png and non HU images
+**This feature is only available in versions between 0.2.5 and 0.2.14**
 As of version 0.2.5 these images are supported. Use the ```--noHU``` tag if you process images that are not encoded in HU. Keep in mind that the models were trained on proper CT scans encoded in HU. The results on cropped, annotated, very high and very low intensity shifted images may not be very reliable. When using the ```--noHU``` tag only single slices can be processed.
```

### Comparing `lungmask-0.2.19/setup.py` & `lungmask-0.2.20/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lungmask",
-    version="0.2.19",
+    version="0.2.20",
     author="Johannes Hofmanninger",
-    author_email="johannes.hofmanninger@gmail.com",
+    author_email="j.hofmanninger@gmail.com",
     description="Package for automated lung segmentation in CT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JoHof/lungmask",
     packages=setuptools.find_packages(),
     entry_points={"console_scripts": ["lungmask = lungmask.__main__:main"]},
     install_requires=[
```

### Comparing `lungmask-0.2.19/tests/test_cli.py` & `lungmask-0.2.20/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.19/tests/test_mask.py` & `lungmask-0.2.20/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.19/tests/test_utils.py` & `lungmask-0.2.20/tests/test_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 import numpy as np
 import SimpleITK as sitk
+import pytest
 
 from lungmask.utils import (
     bbox_3D,
     crop_and_resize,
     load_input_image,
     postprocessing,
     preprocess,
@@ -58,17 +59,19 @@
     m = np.zeros((10, 10, 10), dtype=np.uint8)
     m[2:8, 3:7, 4:6] = 1
 
     bb = bbox_3D(m, margin=2)
     assert tuple(bb) == (0, 10, 1, 9, 2, 8)
 
 
-def test_read_dicoms():
-    d = read_dicoms(os.path.join(os.path.dirname(__file__), "testdata"))
+@pytest.mark.parametrize("read_metadata,exp_len_metadata", [(True, 22),(False, 0)])
+def test_read_dicoms(read_metadata, exp_len_metadata):
+    d = read_dicoms(os.path.join(os.path.dirname(__file__), "testdata"), read_metadata=read_metadata)
     assert d[0].GetSize() == (512, 512, 2)
+    assert len(d[0].GetMetaDataKeys()) == exp_len_metadata
 
 
 def test_simple_bodymask():
     img = np.full((10, 10), dtype=np.int16, fill_value=-1000)
     img[2:8, 3:7] = 1
     img[9, 9] = 1
     mask = simple_bodymask(img)
@@ -100,18 +103,20 @@
     msk = np.full((10, 10), dtype=np.uint8, fill_value=1)
     bb = (2, 2, 22, 22)
     cropped_mask = reshape_mask(msk, bb, origsize=(30, 30))
     assert cropped_mask.shape == (30, 30)
     assert np.sum(cropped_mask) == 400
 
 
-def test_load_input_image(tmp_path):
+@pytest.mark.parametrize("read_metadata,exp_len_metadata", [(True, 22),(False, 0)])
+def test_load_input_image(tmp_path, read_metadata, exp_len_metadata):
     # test dicom
-    d = load_input_image(os.path.join(os.path.dirname(__file__), "testdata"))
+    d = load_input_image(os.path.join(os.path.dirname(__file__), "testdata"), read_metadata=read_metadata)
     assert d.GetSize() == (512, 512, 2)
+    assert len(d.GetMetaDataKeys()) == exp_len_metadata
 
     # test nifti
     fp_testnii = str(tmp_path / "test.nii.gz")
     sitk.WriteImage(d, fp_testnii)
     d = load_input_image(fp_testnii)
     assert d.GetSize() == (512, 512, 2)
```

