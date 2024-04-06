# Comparing `tmp/sbmlnetwork-0.0.17-py3-none-any.whl.zip` & `tmp/sbmlnetwork-0.0.18-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4354 bytes, number of entries: 7
+Zip file size: 3238 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      104 b- defN 24-Apr-06 17:42 sbmlnetwork/__init__.py
--rw-r--r--  2.0 unx     5298 b- defN 24-Apr-06 17:49 sbmlnetwork/sbmlnetwork.py
--rw-r--r--  2.0 unx     1084 b- defN 24-Apr-06 17:56 sbmlnetwork-0.0.17.dist-info/LICENSE
--rw-r--r--  2.0 unx     1282 b- defN 24-Apr-06 17:56 sbmlnetwork-0.0.17.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 17:56 sbmlnetwork-0.0.17.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-06 17:56 sbmlnetwork-0.0.17.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      573 b- defN 24-Apr-06 17:56 sbmlnetwork-0.0.17.dist-info/RECORD
-7 files, 8445 bytes uncompressed, 3334 bytes compressed:  60.5%
+-rw-r--r--  2.0 unx      998 b- defN 24-Apr-06 18:27 sbmlnetwork/sbmlnetwork.py
+-rw-r--r--  2.0 unx     1084 b- defN 24-Apr-06 18:31 sbmlnetwork-0.0.18.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1282 b- defN 24-Apr-06 18:31 sbmlnetwork-0.0.18.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 18:31 sbmlnetwork-0.0.18.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-06 18:31 sbmlnetwork-0.0.18.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      572 b- defN 24-Apr-06 18:31 sbmlnetwork-0.0.18.dist-info/RECORD
+7 files, 4144 bytes uncompressed, 2218 bytes compressed:  46.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sbmlnetwork/__init__.py
 Comment: 
 
 Filename: sbmlnetwork/sbmlnetwork.py
 Comment: 
 
-Filename: sbmlnetwork-0.0.17.dist-info/LICENSE
+Filename: sbmlnetwork-0.0.18.dist-info/LICENSE
 Comment: 
 
-Filename: sbmlnetwork-0.0.17.dist-info/METADATA
+Filename: sbmlnetwork-0.0.18.dist-info/METADATA
 Comment: 
 
-Filename: sbmlnetwork-0.0.17.dist-info/WHEEL
+Filename: sbmlnetwork-0.0.18.dist-info/WHEEL
 Comment: 
 
-Filename: sbmlnetwork-0.0.17.dist-info/top_level.txt
+Filename: sbmlnetwork-0.0.18.dist-info/top_level.txt
 Comment: 
 
-Filename: sbmlnetwork-0.0.17.dist-info/RECORD
+Filename: sbmlnetwork-0.0.18.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbmlnetwork/sbmlnetwork.py

```diff
@@ -1,117 +1,35 @@
-import libsbmlnetwork as sbmln
-import networkinfotranslator as netranslator
-from PIL import Image
-from IPython.core.display import display
+import libsbmlnetworkeditor
+import networkinfotranslator
+from IPython.display import display
 
-class SBMLNetwork:
 
-    """
-    A wrapper class to use libSBMLNetwork, which is an API to work with the Layout and Render packages of libSBML
+class SBMLNetworkEditor(libsbmlnetworkeditor.LibSBMLNetworkEditor):
 
-    """
-    def __init__(self, sbml):
+    def __init__(self, sbml=""):
+        super().__init__(sbml)
 
+    def draw(self, file_name=""):
         """
-        Initializes the SBMLNetwork class by reading an SBML document from the given file name or the given text string
-
-        :Parameters:
+        Draws the network of the SBML model. Saves the figure to the file_directory if specified, otherwise displays the figure.
 
-            - sbml: an SBML document in the form of either an SBML string or an SBML file (.xml) directory
+        :param file_directory:
+        :param file_name:
+        :param file_format:
         """
-
-        self.sbml_object = None
-        self.load(sbml)
-
-    def load(self, sbml):
-
-        """
-        Reads an SBML document from the given file name or the given text string
-
-        :Parameters:
-
-            - sbml (string): a string that determines either the name or full pathname of the SBML(.xml) file to be read
-                or a string containing a full SBML model.
-
-        :Returns:
-
-            SBMLDocument: a pointer to the SBMLDocument structure created from the SBML content in the given file name or
-                from the SBML content in the given text string
-        """
-
-        self.sbml_object = sbmln.readSBML(sbml)
-        return self.sbml_object
-
-    def export(self, file_name=""):
-        """
-        Writes the given SBML document to either the file_name or a string
-
-        :Parameters:
-
-            - file_name (string, optional): a string (default : "") that determines the name or full pathname of the file where the SBML is to be written
-
-        :Returns:
-
-            either success: true on success and false if the filename could not be opened for writing
-            or text: the SBML text string on success and empty string if one of the underlying parser components fail.
-        """
-
         if file_name:
-            return sbmln.writeSBML(self.sbml_object, file_name)
+            networkinfotranslator.import_sbml_export_figure(self.save(), file_name, self.use_name_as_text_label, self.display_reactions_text_label)
         else:
-            return sbmln.writeSBML(self.sbml_object)
-
-    def autolayout(self, stiffness=10.0, gravity=15.0, use_magnetism=False, use_boundary=False, use_grid=False):
-        """
-        checks if a Layout object, a GlobalRenderInformation object, and LocalRenderInformation object does not exists in the SBMLDocument,
-            then adds them to it, and set all the necessary features for them.
-
-        :Parameters:
-
-            - stiffness (float, optional): a float (default: 10.0) that determines the stiffness value used in the autolayout algorithm (can affect the canvas dimensions).
-            - gravity (float, optional): a float (default: 15.0) that determines the gravity value used in the autolayout algorithm (can affect the how densely nodes are distributed).
-            - use_magnetism (boolean, optional): a boolean (default: False) that determines whether to use magnetism in the autolayout algorithm.
-            - useBoundary (boolean, optional): a boolean (default: False) that determines whether to use boundary restriction in the autolayout algorithm.
-            - use_grid (boolean, optional): a boolean (default: False) that determines whether to use grid restriction in the autolayout algorithm.
+            display(networkinfotranslator.import_sbml_export_pil_image(self.save(), self.use_name_as_text_label, self.display_reactions_text_label))
 
-        :Returns:
 
-            either success: true on success and false if the filename could not be opened for writing
-            or text: the SBML text string on success and empty string if one of the underlying parser components fail.
-        """
-
-        return sbmln.autolayout(self.sbml_object, stiffness, gravity, use_magnetism, use_boundary, use_grid)
-
-    def draw(self, file_directory="", file_name="", file_format="", display_image=True):
-        """
-        create an image of the network using networkinfotranslator package, save it as file to the provided directory (or the current directory), and then load and display it
-
-        :Parameters:
+def load(sbml):
+    """
+    Loads the SBML model.
 
-            - file_directory (string, optional): a string (default: "") that specifies the directory to which the output image will be saved.
-            - file_name (string, optional): a string (default: "") that specifies the name of the output image.
-            - file_format (string, optional): a sting (default: "") that specifies that format of the output image (examples are 'pdf', 'png', 'svg', and 'jpg')
-            - display_image (boolean, optional): a boolean (default: True) that determines whether to display the generated image or not
+    :param sbml: The SBML model.
+    :return: SBMLNetworkEditor
+    """
+    return SBMLNetworkEditor(sbml)
 
-        """
-        if not self._layout_is_specified() or not self._render_is_specified():
-            self.autolayout()
 
-        sbml_graph_info = netranslator.NetworkInfoImportFromSBMLModel()
-        sbml_graph_info.extract_info(self.export())
-        sbml_export = netranslator.NetworkInfoExportToMatPlotLib()
-        sbml_export.extract_graph_info(sbml_graph_info)
-        sbml_export.export(file_directory, file_name, file_format)
-        if display_image and file_format != "pdf":
-            display(Image.open(sbml_export.get_output_name(file_directory, file_name, file_format)))
-
-    def _layout_is_specified(self):
-        if sbmln.getNumLayouts(self.sbml_object):
-            return True
-
-        return False
-
-    def _render_is_specified(self):
-        if sbmln.getNumGlobalRenderInformation(self.sbml_object) or sbmlne.getNumLocalRenderInformation(self.sbml_object):
-            return True
 
-        return False
```

## Comparing `sbmlnetwork-0.0.17.dist-info/LICENSE` & `sbmlnetwork-0.0.18.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbmlnetwork-0.0.17.dist-info/METADATA` & `sbmlnetwork-0.0.18.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sbmlnetwork
-Version: 0.0.17
+Version: 0.0.18
 Summary: A python api to work with libsbmlnetwork library
 Home-page: https://github.com/adelhpour/SBMLNetwork
 Author: Adel Heydarabadipour
 Author-email: adelhp@uw.edu
 Project-URL: Bug Tracker, https://github.com/adelhpour/SBMLNetwork/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: libsbmlnetwork ==0.0.15
+Requires-Dist: libsbmlnetwork ==0.0.16
 Requires-Dist: networkinfotranslator ==0.0.20
 Requires-Dist: pillow
 Requires-Dist: ipython
 
 # SBMLNetwork
 
 SBMLNetwork is a python package designed to visualize and edit SBML model networks. It uses libsbmlnetwork package, which employs an embedded force-directed autolayout algorithm to create aesthetically pleasing networks and utilizes SBML Layout and Render packages to store and retrieve visualization information of models. With its drawing tool and its comprehensive command-line API, users can generate and modify graphical representations of their SBML models, save the visual information of their model to SBML files or strings, and export rendered figures of their model in PDF, PNG, and JPG formats.
```

## Comparing `sbmlnetwork-0.0.17.dist-info/RECORD` & `sbmlnetwork-0.0.18.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 sbmlnetwork/__init__.py,sha256=yaTYN_SWt9c_LAgnNCSqqq5wBGPEZRujumNvj3choPc,104
-sbmlnetwork/sbmlnetwork.py,sha256=wKTimx1zQ-5IP562E0SiVYf7LiVoJEJUAxttCRsayp8,5298
-sbmlnetwork-0.0.17.dist-info/LICENSE,sha256=gGnkw4gXz_FZnTTWOhvH4kGG_w3jDFAHlIE8ESRa-b4,1084
-sbmlnetwork-0.0.17.dist-info/METADATA,sha256=np7WWPq97Yj6j_I0hJ5qzOJr21MoOrn-F-KLF02Xfkk,1282
-sbmlnetwork-0.0.17.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-sbmlnetwork-0.0.17.dist-info/top_level.txt,sha256=n2VJnirWoFrbr61pdAjVKFaDBYgHB-2l0brB92WpAm8,12
-sbmlnetwork-0.0.17.dist-info/RECORD,,
+sbmlnetwork/sbmlnetwork.py,sha256=4zY3wY5yQFYM-IdAwIddFW00VlCE5TKH7Yy_bgXzBR4,998
+sbmlnetwork-0.0.18.dist-info/LICENSE,sha256=gGnkw4gXz_FZnTTWOhvH4kGG_w3jDFAHlIE8ESRa-b4,1084
+sbmlnetwork-0.0.18.dist-info/METADATA,sha256=-8hBl7e1SFr1iunp_IUPKLV7ozwNUhvmSk9tPS2aznY,1282
+sbmlnetwork-0.0.18.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+sbmlnetwork-0.0.18.dist-info/top_level.txt,sha256=n2VJnirWoFrbr61pdAjVKFaDBYgHB-2l0brB92WpAm8,12
+sbmlnetwork-0.0.18.dist-info/RECORD,,
```

