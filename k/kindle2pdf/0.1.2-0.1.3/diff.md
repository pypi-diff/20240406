# Comparing `tmp/kindle2pdf-0.1.2.tar.gz` & `tmp/kindle2pdf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kindle2pdf-0.1.2.tar", max compression
+gzip compressed data, was "kindle2pdf-0.1.3.tar", max compression
```

## Comparing `kindle2pdf-0.1.2.tar` & `kindle2pdf-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      718 2024-04-06 15:42:50.462637 kindle2pdf-0.1.2/README.md
--rw-r--r--   0        0        0    12795 2024-04-06 20:54:53.410584 kindle2pdf-0.1.2/kindle2pdf.py
--rw-r--r--   0        0        0      461 2024-04-06 20:55:19.935392 kindle2pdf-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 kindle2pdf-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      718 2024-04-06 15:42:50.462637 kindle2pdf-0.1.3/README.md
+-rw-r--r--   0        0        0    12923 2024-04-06 21:02:24.916341 kindle2pdf-0.1.3/kindle2pdf.py
+-rw-r--r--   0        0        0      461 2024-04-06 21:02:45.112957 kindle2pdf-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 kindle2pdf-0.1.3/PKG-INFO
```

### Comparing `kindle2pdf-0.1.2/README.md` & `kindle2pdf-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kindle2pdf-0.1.2/kindle2pdf.py` & `kindle2pdf-0.1.3/kindle2pdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,26 +35,29 @@
     """
 
     def __init__(
         self,
         asin: str,
         font_size: int = 12,
         page_size: tuple[float, float] = A4,
+        dpi: int = 160,
     ) -> None:
         """
         Initializes the Kindle2PDF object with the specified ASIN and starts a reading session.
 
         Args:
             asin (str): The ASIN of the book to convert.
             font_size (int): The font size to use for rendering the book.
             page_size (tuple[float, float]): The size of the PDF pages.
+            dpi (int): The DPI to use for rendering images.
         """
         self.asin = asin
         self.font_size = font_size
         self.page_size = page_size
+        self.dpi = dpi
         self.session = self.start_reading_session()
 
     def start_reading_session(self) -> dict:
         """
         Starts a new reading session by authenticating with Amazon and retrieving session tokens.
 
         Returns:
@@ -146,17 +149,17 @@
             "version": "3.0",
             "asin": self.asin,
             "contentType": "FullBook",
             "revision": self.session["version"],
             "fontFamily": "Bookerly",
             "fontSize": str(self.font_size),
             "lineHeight": "1.4",
-            "dpi": 72,
-            "height": str(int(self.page_size[1])),
-            "width": str(int(self.page_size[0])),
+            "dpi": str(self.dpi),
+            "height": str(int(self.page_size[1] * self.dpi / 72)),
+            "width": str(int(self.page_size[0] * self.dpi / 72)),
             "marginBottom": "0",
             "marginLeft": "9",
             "marginRight": "9",
             "marginTop": "0",
             "maxNumberColumns": "1",
             "theme": "default",
             "locationMap": "true",
@@ -246,14 +249,16 @@
             pages (dict): A dictionary containing page data.
             fonts (dict): A dictionary containing font data.
             images (dict): A dictionary of decrypted images.
             pdf_canvas (canvas.Canvas): The canvas object to draw the PDF on.
         """
         for page in pages:
             for child in page["children"]:
+                transform = [_ * 72 / self.dpi for _ in child["transform"]]
+
                 if child["type"] == "run":
                     font = None
                     for font in fonts:
                         if font["fontKey"] == child["fontKey"]:
                             break
 
                     glyphs = ""
@@ -263,34 +268,34 @@
                             <path d="{font['glyphs'][str(glyph)].get('path', '')}" 
                                 fill="{child['textColor']}" stroke="{child['textColor']}"/>
                         </g>
                         """
 
                     svg_content = f"""<?xml version="1.0" standalone="no"?>
                     <svg version="1.1" xmlns="http://www.w3.org/2000/svg">
-                        <g transform="matrix({child["transform"][0]}, {child["transform"][1]}, {child["transform"][2]}, {child["transform"][3]}, {child["transform"][4]}, {child["transform"][5]})">
+                        <g transform="matrix({transform[0]}, {transform[1]}, {transform[2]}, {transform[3]}, {transform[4]}, {transform[5]})">
                             {glyphs}
                         </g>
                     </svg>
                     """
 
                     drawing = svg2rlg(io.StringIO(svg_content))
                     renderPDF.draw(drawing, pdf_canvas, 0, self.page_size[1])
 
                 elif child["type"] == "image":
                     with tempfile.NamedTemporaryFile(delete=True, suffix=".jpg") as tmp:
                         tmp.write(images[child["imageReference"]])
                         tmp.flush()
-                        x = child["transform"][4]
+                        x = transform[4]
                         y = self.page_size[1] - (
-                            child["transform"][5]
-                            + child["rect"]["bottom"] * child["transform"][3]
+                            transform[5]
+                            + child["rect"]["bottom"] * transform[3]
                         )
-                        width = child["rect"]["right"] * child["transform"][0]
-                        height = child["rect"]["bottom"] * child["transform"][3]
+                        width = child["rect"]["right"] * transform[0]
+                        height = child["rect"]["bottom"] * transform[3]
                         pdf_canvas.drawImage(
                             image=tmp.name, x=x, y=y, width=width, height=height
                         )
 
             pdf_canvas.showPage()
 
     def render_book(self, output_path: Optional[str]) -> None:
```

### Comparing `kindle2pdf-0.1.2/PKG-INFO` & `kindle2pdf-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kindle2pdf
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Robert Dargavel Smith
 Author-email: teticio@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

