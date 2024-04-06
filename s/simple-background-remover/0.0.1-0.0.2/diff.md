# Comparing `tmp/simple_background_remover-0.0.1.tar.gz` & `tmp/simple_background_remover-0.0.2.tar.gz`

## Comparing `simple_background_remover-0.0.1.tar` & `simple_background_remover-0.0.2.tar`

### file list

```diff
@@ -1,1789 +1,10 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/requirements.txt
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/BdfFontFile.py
--rw-r--r--   0        0        0    16044 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/BlpImagePlugin.py
--rw-r--r--   0        0        0    18170 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/BmpImagePlugin.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/BufrStubImagePlugin.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ContainerIO.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/CurImagePlugin.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/DcxImagePlugin.py
--rw-r--r--   0        0        0    17105 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/DdsImagePlugin.py
--rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/EpsImagePlugin.py
--rw-r--r--   0        0        0    10134 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ExifTags.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/FitsImagePlugin.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/FliImagePlugin.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/FontFile.py
--rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/FpxImagePlugin.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/FtexImagePlugin.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/GbrImagePlugin.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/GdImageFile.py
--rw-r--r--   0        0        0    38300 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/GifImagePlugin.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/GimpGradientFile.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/GimpPaletteFile.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/GribStubImagePlugin.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/Hdf5StubImagePlugin.py
--rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/IcnsImagePlugin.py
--rw-r--r--   0        0        0    11930 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/IcoImagePlugin.py
--rw-r--r--   0        0        0    11275 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImImagePlugin.py
--rw-r--r--   0        0        0   138424 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/Image.py
--rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageChops.py
--rw-r--r--   0        0        0    38188 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageCms.py
--rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageColor.py
--rw-r--r--   0        0        0    37500 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageDraw.py
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageDraw2.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageEnhance.py
--rw-r--r--   0        0        0    25140 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageFile.py
--rw-r--r--   0        0        0    17711 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageFilter.py
--rw-r--r--   0        0        0    62104 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageFont.py
--rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageGrab.py
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageMath.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageMode.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageMorph.py
--rw-r--r--   0        0        0    23113 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageOps.py
--rw-r--r--   0        0        0     8025 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImagePalette.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImagePath.py
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageQt.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageSequence.py
--rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageShow.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageStat.py
--rw-r--r--   0        0        0     8780 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageTk.py
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageTransform.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImageWin.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/ImtImagePlugin.py
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/IptcImagePlugin.py
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/Jpeg2KImagePlugin.py
--rw-r--r--   0        0        0    30446 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/JpegImagePlugin.py
--rw-r--r--   0        0        0    12619 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/JpegPresets.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/McIdasImagePlugin.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/MicImagePlugin.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/MpegImagePlugin.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/MpoImagePlugin.py
--rw-r--r--   0        0        0     5843 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/MspImagePlugin.py
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PSDraw.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PaletteFile.py
--rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PalmImagePlugin.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PcdImagePlugin.py
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PcfFontFile.py
--rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PcxImagePlugin.py
--rw-r--r--   0        0        0     9144 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PdfImagePlugin.py
--rw-r--r--   0        0        0    35481 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PdfParser.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PixarImagePlugin.py
--rw-r--r--   0        0        0    47941 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PngImagePlugin.py
--rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PpmImagePlugin.py
--rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PsdImagePlugin.py
--rw-r--r--   0        0        0    10273 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/PyAccess.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/QoiImagePlugin.py
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/SgiImagePlugin.py
--rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/SpiderImagePlugin.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/SunImagePlugin.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/TarIO.py
--rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/TgaImagePlugin.py
--rw-r--r--   0        0        0    78860 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/TiffImagePlugin.py
--rw-r--r--   0        0        0    17112 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/TiffTags.py
--rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/WalImageFile.py
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/WebPImagePlugin.py
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/WmfImagePlugin.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/XVThumbImagePlugin.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/XbmImagePlugin.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/XpmImagePlugin.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/__main__.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/_binary.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/_deprecate.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/_imagingcms.pyi
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/_imagingft.pyi
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/_tkinter_finder.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/_typing.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/_util.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/_version.py
--rw-r--r--   0        0        0     9985 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/PIL/features.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/build-1.2.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/build-1.2.1.dist-info/LICENSE
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/build-1.2.1.dist-info/METADATA
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/build-1.2.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/build-1.2.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/build-1.2.1.dist-info/WHEEL
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/build-1.2.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/certifi/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/certifi/__main__.py
--rw-r--r--   0        0        0   292541 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/certifi/cacert.pem
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/certifi/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/certifi-2024.2.2.dist-info/INSTALLER
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/certifi-2024.2.2.dist-info/LICENSE
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/certifi-2024.2.2.dist-info/METADATA
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/certifi-2024.2.2.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/certifi-2024.2.2.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/certifi-2024.2.2.dist-info/top_level.txt
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/__init__.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/__main__.py
--rw-r--r--   0        0        0    21723 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/api.py
--rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/cd.py
--rw-r--r--   0        0        0    42476 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/constant.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/legacy.py
--rw-r--r--   0        0        0    20239 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/md.py
--rw-r--r--   0        0        0    11964 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/py.typed
--rw-r--r--   0        0        0    12315 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/utils.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/version.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/cli/__init__.py
--rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer/cli/__main__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer-3.3.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
--rw-r--r--   0        0        0    34233 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer-3.3.2.dist-info/METADATA
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer-3.3.2.dist-info/RECORD
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer-3.3.2.dist-info/WHEEL
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer-3.3.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/charset_normalizer-3.3.2.dist-info/top_level.txt
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama-0.4.6.dist-info/INSTALLER
--rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama-0.4.6.dist-info/METADATA
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama-0.4.6.dist-info/RECORD
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama-0.4.6.dist-info/WHEEL
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0    10293 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/__init__.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/__main__.py
--rw-r--r--   0        0        0    33045 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/core.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/examples.py
--rw-r--r--   0        0        0    40002 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/frontend.py
--rw-r--r--   0        0        0    23958 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/io.py
--rw-r--r--   0        0        0    81006 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/nodes.py
--rw-r--r--   0        0        0    56956 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/statemachine.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/af.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/ar.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/ca.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/cs.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/da.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/de.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/en.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/eo.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/es.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/fa.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/fi.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/fr.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/gl.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/he.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/it.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/ja.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/ko.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/lt.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/lv.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/nl.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/pl.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/pt_br.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/ru.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/sk.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/sv.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/uk.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/zh_cn.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/languages/zh_tw.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/__init__.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/commonmark_wrapper.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/null.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py
--rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/__init__.py
--rw-r--r--   0        0        0    16119 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/roles.py
--rw-r--r--   0        0        0   132550 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/states.py
--rw-r--r--   0        0        0    20912 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/tableparser.py
--rw-r--r--   0        0        0    14652 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/directives/__init__.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py
--rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/directives/body.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/directives/html.py
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/directives/images.py
--rw-r--r--   0        0        0    26302 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/directives/misc.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/directives/parts.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/directives/references.py
--rw-r--r--   0        0        0    23825 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/directives/tables.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/README.txt
--rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt
--rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isobox.txt
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isodia.txt
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isogrk4.txt
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt
--rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isonum.txt
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isopub.txt
--rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/isotech.txt
--rw-r--r--   0        0        0    45428 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt
--rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt
--rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt
--rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/__init__.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/af.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/ar.py
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/ca.py
--rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/cs.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/da.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/de.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/en.py
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/eo.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/es.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/fa.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/fi.py
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/fr.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/gl.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/he.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/it.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/ja.py
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/ko.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/lt.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/lv.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/nl.py
--rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/pl.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/ru.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/sk.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/sv.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/uk.py
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/readers/__init__.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/readers/doctree.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/readers/pep.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/readers/standalone.py
--rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/transforms/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/transforms/components.py
--rw-r--r--   0        0        0    21371 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/transforms/frontmatter.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/transforms/misc.py
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/transforms/parts.py
--rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/transforms/peps.py
--rw-r--r--   0        0        0    36819 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/transforms/references.py
--rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/transforms/universal.py
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/transforms/writer_aux.py
--rw-r--r--   0        0        0    29382 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/__init__.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/code_analyzer.py
--rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/error_reporting.py
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/punctuation_chars.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/roman.py
--rw-r--r--   0        0        0    38972 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/smartquotes.py
--rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/urischemes.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/math/__init__.py
--rw-r--r--   0        0        0    51496 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/math/latex2mathml.py
--rw-r--r--   0        0        0   107993 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/math/math2html.py
--rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py
--rw-r--r--   0        0        0    37497 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/math/tex2unichar.py
--rw-r--r--   0        0        0    18393 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/utils/math/unichar2tex.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/__init__.py
--rw-r--r--   0        0        0    70896 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/_html_base.py
--rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/docutils_xml.py
--rw-r--r--   0        0        0    36654 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/manpage.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/null.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/pseudoxml.py
--rw-r--r--   0        0        0    37675 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/html4css1/__init__.py
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/html4css1/html4css1.css
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/html4css1/template.txt
--rw-r--r--   0        0        0    16718 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py
--rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/html5_polyglot/math.css
--rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/html5_polyglot/minimal.css
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/html5_polyglot/plain.css
--rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/html5_polyglot/responsive.css
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/html5_polyglot/template.txt
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/html5_polyglot/tuftig.css
--rw-r--r--   0        0        0   137132 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/latex2e/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/latex2e/default.tex
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/latex2e/docutils.sty
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/latex2e/titlepage.tex
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/latex2e/titlingpage.tex
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/latex2e/xelatex.tex
--rw-r--r--   0        0        0   132358 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/odf_odt/__init__.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/odf_odt/prepstyles.py
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/odf_odt/styles.odt
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/pep_html/__init__.py
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/pep_html/pep.css
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/pep_html/template.txt
--rw-r--r--   0        0        0    14517 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/__init__.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/README.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/big-black/__base__
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/default/framing.css
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/default/opera.css
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/default/outline.css
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/default/pretty.css
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/default/print.css
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.css
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/default/slides.js
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/__base__
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/small-black/__base__
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
--rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils/writers/xetex/__init__.py
--rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils-0.20.1.dist-info/COPYING.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils-0.20.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils-0.20.1.dist-info/METADATA
--rw-r--r--   0        0        0    28201 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils-0.20.1.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils-0.20.1.dist-info/WHEEL
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils-0.20.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/docutils-0.20.1.dist-info/top_level.txt
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna/__init__.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna/compat.py
--rw-r--r--   0        0        0    12908 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna/core.py
--rw-r--r--   0        0        0    44351 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna/py.typed
--rw-r--r--   0        0        0   206503 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna/uts46data.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna-3.6.dist-info/INSTALLER
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna-3.6.dist-info/LICENSE.md
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna-3.6.dist-info/METADATA
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna-3.6.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/idna-3.6.dist-info/WHEEL
--rw-r--r--   0        0        0    34302 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata/_text.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata/diagnose.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata/compat/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata/compat/py39.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata-7.1.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata-7.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata-7.1.0.dist-info/METADATA
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata-7.1.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata-7.1.0.dist-info/WHEEL
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/importlib_metadata-7.1.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     8927 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco/context.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco/classes/__init__.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco/classes/ancestry.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco/classes/meta.py
--rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco/classes/properties.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco/classes/py.typed
--rw-r--r--   0        0        0    16642 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco/functools/__init__.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco/functools/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco/functools/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.classes-3.4.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.classes-3.4.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.classes-3.4.0.dist-info/METADATA
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.classes-3.4.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.classes-3.4.0.dist-info/WHEEL
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.classes-3.4.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.context-5.1.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.context-5.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.context-5.1.0.dist-info/METADATA
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.context-5.1.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.context-5.1.0.dist-info/WHEEL
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.context-5.1.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.functools-4.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.functools-4.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.functools-4.0.0.dist-info/METADATA
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.functools-4.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.functools-4.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/jaraco.functools-4.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/__main__.py
--rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backend.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backend_complete.bash
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backend_complete.zsh
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/cli.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/completion.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/core.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/credentials.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/devpi_client.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/errors.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/http.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/py.typed
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backends/SecretService.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backends/Windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backends/__init__.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backends/chainer.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backends/fail.py
--rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backends/kwallet.py
--rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backends/libsecret.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backends/null.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backends/macOS/__init__.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/backends/macOS/api.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/compat/__init__.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/compat/properties.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/compat/py312.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/compat/py38.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/testing/__init__.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/testing/backend.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/testing/util.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/util/__init__.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring/util/platform_.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring-25.1.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring-25.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0    20418 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring-25.1.0.dist-info/METADATA
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring-25.1.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring-25.1.0.dist-info/WHEEL
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring-25.1.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/keyring-25.1.0.dist-info/top_level.txt
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/_compat.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/_punycode.py
--rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/main.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/parser_block.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/parser_core.py
--rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/parser_inline.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/port.yaml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/py.typed
--rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/renderer.py
--rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/ruler.py
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/token.py
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/tree.py
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/cli/__init__.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/cli/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/common/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/common/entities.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/common/html_blocks.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/common/html_re.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/common/normalize_url.py
--rw-r--r--   0        0        0    10728 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/common/utils.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/helpers/__init__.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/helpers/parse_link_destination.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/helpers/parse_link_label.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/helpers/parse_link_title.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/presets/__init__.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/presets/commonmark.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/presets/default.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/presets/zero.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/__init__.py
--rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/blockquote.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/code.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/fence.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/heading.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/hr.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/html_block.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/lheading.py
--rw-r--r--   0        0        0     9668 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/list.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/paragraph.py
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/reference.py
--rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/state_block.py
--rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_block/table.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_core/__init__.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_core/block.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_core/inline.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_core/linkify.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_core/normalize.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_core/replacements.py
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_core/smartquotes.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_core/state_core.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_core/text_join.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/__init__.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/autolink.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/backticks.py
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/emphasis.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/entity.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/escape.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/fragments_join.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/html_inline.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/image.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/link.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/linkify.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/newline.py
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/state_inline.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/strikethrough.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it/rules_inline/text.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it_py-3.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE.markdown-it
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it_py-3.0.0.dist-info/METADATA
--rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it_py-3.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it_py-3.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/markdown_it_py-3.0.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/mdurl/__init__.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/mdurl/_decode.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/mdurl/_encode.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/mdurl/_format.py
--rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/mdurl/_parse.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/mdurl/_url.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/mdurl/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/mdurl-0.1.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/mdurl-0.1.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/mdurl-0.1.2.dist-info/METADATA
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/mdurl-0.1.2.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/mdurl-0.1.2.dist-info/WHEEL
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/more_itertools/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/more_itertools/__init__.pyi
--rw-r--r--   0        0        0   143045 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/more_itertools/more.py
--rw-r--r--   0        0        0    21044 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/more_itertools/more.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/more_itertools/py.typed
--rw-r--r--   0        0        0    27548 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/more_itertools/recipes.py
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/more_itertools/recipes.pyi
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/more_itertools-10.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/more_itertools-10.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0    34886 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/more_itertools-10.2.0.dist-info/METADATA
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/more_itertools-10.2.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/more_itertools-10.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/nh3/__init__.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/nh3/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/nh3/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/nh3-0.2.17.dist-info/INSTALLER
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/nh3-0.2.17.dist-info/METADATA
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/nh3-0.2.17.dist-info/RECORD
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/nh3-0.2.17.dist-info/WHEEL
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/_elffile.py
--rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/_manylinux.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/_musllinux.py
--rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/markers.py
--rw-r--r--   0        0        0    33036 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/py.typed
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/requirements.py
--rw-r--r--   0        0        0    39784 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/specifiers.py
--rw-r--r--   0        0        0    18950 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/tags.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/utils.py
--rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging-24.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging-24.0.dist-info/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging-24.0.dist-info/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging-24.0.dist-info/LICENSE.BSD
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging-24.0.dist-info/METADATA
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging-24.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/packaging-24.0.dist-info/WHEEL
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pillow-10.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    56516 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pillow-10.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pillow-10.2.0.dist-info/METADATA
--rw-r--r--   0        0        0    13366 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pillow-10.2.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pillow-10.2.0.dist-info/REQUESTED
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pillow-10.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pillow-10.2.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pillow-10.2.0.dist-info/zip-safe
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/py.typed
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    23634 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    28782 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37843 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    20777 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    35460 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24551 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    21052 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    32292 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    23623 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/py.typed
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/certifi/py.typed
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/py.typed
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51965 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51767 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18315 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
--rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    67530 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23747 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
--rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43958 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/distro/py.typed
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/idna/py.typed
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/platformdirs/py.typed
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyparsing/py.typed
--rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/resolvelib/py.typed
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tenacity/py.typed
--rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/tomli/py.typed
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/truststore/__init__.py
--rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/truststore/_api.py
--rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/truststore/_macos.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/truststore/_openssl.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/truststore/_ssl_constants.py
--rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/truststore/_windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/truststore/py.typed
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip-24.0.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip-24.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip-24.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip-24.0.dist-info/METADATA
--rw-r--r--   0        0        0    78960 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip-24.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip-24.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip-24.0.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip-24.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pip-24.0.dist-info/top_level.txt
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/__init__.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/__init__.pyi
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/bdist.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/bdist.pyi
--rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/commandline.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/commandline.pyi
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/develop.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/develop.pyi
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/distribution.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/distribution.pyi
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/index.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/index.pyi
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/installed.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/installed.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/py.typed
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/sdist.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/sdist.pyi
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/utils.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/utils.pyi
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/wheel.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/wheel.pyi
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/tests/__init__.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/tests/test_bdist.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/tests/test_commandline.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/tests/test_develop.py
--rw-r--r--   0        0        0    19713 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/tests/test_distribution.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/tests/test_index.py
--rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/tests/test_installed.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/tests/test_sdist.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/tests/test_utils.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo/tests/test_wheel.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo-1.10.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo-1.10.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo-1.10.0.dist-info/METADATA
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo-1.10.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo-1.10.0.dist-info/WHEEL
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo-1.10.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pkginfo-1.10.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/__init__.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/__main__.py
--rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/filter.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatter.py
--rw-r--r--   0        0        0    35044 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/modeline.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/scanner.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/sphinxext.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/style.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/util.py
--rw-r--r--   0        0        0    40338 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35640 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/html.py
--rw-r--r--   0        0        0    23116 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/img.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19303 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/other.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12113 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/__init__.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_ada_builtins.py
--rw-r--r--   0        0        0    27287 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_asy_builtins.py
--rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_cl_builtins.py
--rw-r--r--   0        0        0   105182 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_cocoa_builtins.py
--rw-r--r--   0        0        0    18414 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_csound_builtins.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_css_builtins.py
--rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_julia_builtins.py
--rw-r--r--   0        0        0   134510 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_lasso_builtins.py
--rw-r--r--   0        0        0   108094 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_lilypond_builtins.py
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_lua_builtins.py
--rw-r--r--   0        0        0    68026 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    24713 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_mql_builtins.py
--rw-r--r--   0        0        0    25842 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_mysql_builtins.py
--rw-r--r--   0        0        0    49398 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_openedge_builtins.py
--rw-r--r--   0        0        0   107930 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_php_builtins.py
--rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_postgres_builtins.py
--rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_qlik_builtins.py
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_scheme_builtins.py
--rw-r--r--   0        0        0    52413 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_scilab_builtins.py
--rw-r--r--   0        0        0    26781 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py
--rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_stan_builtins.py
--rw-r--r--   0        0        0    27227 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_stata_builtins.py
--rw-r--r--   0        0        0    15460 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_tsql_builtins.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_usd_builtins.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_vbscript_builtins.py
--rw-r--r--   0        0        0    57066 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/_vim_builtins.py
--rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/actionscript.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ada.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/agile.py
--rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/algebra.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ambient.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/amdgpu.py
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ampl.py
--rw-r--r--   0        0        0    30766 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/apdlexer.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/apl.py
--rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/archetype.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/arrow.py
--rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/arturo.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/asc.py
--rw-r--r--   0        0        0    41243 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/asm.py
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/asn1.py
--rw-r--r--   0        0        0    19815 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/automation.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/bare.py
--rw-r--r--   0        0        0    27923 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/basic.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/bdd.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/berry.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/bibtex.py
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/blueprint.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/boa.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/bqn.py
--rw-r--r--   0        0        0    28112 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/business.py
--rw-r--r--   0        0        0    17946 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/c_cpp.py
--rw-r--r--   0        0        0    29206 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/c_like.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/capnproto.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/carbon.py
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/cddl.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/chapel.py
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/clean.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/comal.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/compiled.py
--rw-r--r--   0        0        0    50077 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/configs.py
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/console.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/cplint.py
--rw-r--r--   0        0        0    15757 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/crystal.py
--rw-r--r--   0        0        0    16994 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/csound.py
--rw-r--r--   0        0        0    25322 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/css.py
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/d.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/dalvik.py
--rw-r--r--   0        0        0    27032 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/data.py
--rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/dax.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/devicetree.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/diff.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/dns.py
--rw-r--r--   0        0        0    37623 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/dotnet.py
--rw-r--r--   0        0        0    36786 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/dsls.py
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/dylan.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ecl.py
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/eiffel.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/elm.py
--rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/elpi.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/email.py
--rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/erlang.py
--rw-r--r--   0        0        0    10396 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/esoteric.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ezhil.py
--rw-r--r--   0        0        0    19531 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/factor.py
--rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/fantom.py
--rw-r--r--   0        0        0     9646 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/felix.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/fift.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/floscript.py
--rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/forth.py
--rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/fortran.py
--rw-r--r--   0        0        0    26212 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/foxpro.py
--rw-r--r--   0        0        0    26914 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/freefem.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/func.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/functional.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/futhark.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/gcodelexer.py
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/gdscript.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/go.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/grammar_notation.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/graph.py
--rw-r--r--   0        0        0    39026 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/graphics.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/graphql.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/graphviz.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/gsql.py
--rw-r--r--   0        0        0    32898 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/haskell.py
--rw-r--r--   0        0        0    30976 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/haxe.py
--rw-r--r--   0        0        0    22520 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/hdl.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/hexdump.py
--rw-r--r--   0        0        0    20260 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/html.py
--rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/idl.py
--rw-r--r--   0        0        0    31658 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/igor.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/inferno.py
--rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/installers.py
--rw-r--r--   0        0        0    57119 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/int_fiction.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/iolang.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/j.py
--rw-r--r--   0        0        0    62859 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/javascript.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/jmespath.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/jslt.py
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/jsonnet.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/jsx.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/julia.py
--rw-r--r--   0        0        0    72929 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/jvm.py
--rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/kuin.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/kusto.py
--rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ldap.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/lean.py
--rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/lilypond.py
--rw-r--r--   0        0        0   144398 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/lisp.py
--rw-r--r--   0        0        0    32171 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/macaulay2.py
--rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/make.py
--rw-r--r--   0        0        0    60257 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/markup.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/math.py
--rw-r--r--   0        0        0   132852 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/matlab.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/maxima.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/meson.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/mime.py
--rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/minecraft.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/mips.py
--rw-r--r--   0        0        0    35315 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ml.py
--rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/modeling.py
--rw-r--r--   0        0        0    53073 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/modula2.py
--rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/monte.py
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/mosel.py
--rw-r--r--   0        0        0    63962 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ncl.py
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/nimrod.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/nit.py
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/nix.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/oberon.py
--rw-r--r--   0        0        0    22961 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/objective.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ooc.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/openscad.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/other.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/parasail.py
--rw-r--r--   0        0        0    25904 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/parsers.py
--rw-r--r--   0        0        0    30880 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/pascal.py
--rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/pawn.py
--rw-r--r--   0        0        0    39170 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/perl.py
--rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/phix.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/php.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/pointless.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/pony.py
--rw-r--r--   0        0        0    12677 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/praat.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/procfile.py
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/prolog.py
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/promql.py
--rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/prql.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ptx.py
--rw-r--r--   0        0        0    53400 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/python.py
--rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/q.py
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/qlik.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/qvt.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/r.py
--rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/rdf.py
--rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/rebol.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/resource.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ride.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/rita.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/rnc.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/roboconf.py
--rw-r--r--   0        0        0    18449 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/robotframework.py
--rw-r--r--   0        0        0    22672 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ruby.py
--rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/rust.py
--rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/sas.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/savi.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/scdoc.py
--rw-r--r--   0        0        0    70014 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/scripting.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/sgf.py
--rw-r--r--   0        0        0    36466 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/shell.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/sieve.py
--rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/slash.py
--rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/smalltalk.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/smithy.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/smv.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/snobol.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/solidity.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/sophia.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/special.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/spice.py
--rw-r--r--   0        0        0    42107 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/sql.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/srcinfo.py
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/stata.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/supercollider.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/tal.py
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/tcl.py
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/teal.py
--rw-r--r--   0        0        0    72610 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/templates.py
--rw-r--r--   0        0        0     9719 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/teraterm.py
--rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/testing.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/text.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/textedit.py
--rw-r--r--   0        0        0    15310 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/textfmts.py
--rw-r--r--   0        0        0    16659 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/theorem.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/thingsdb.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/tlb.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/tls.py
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/tnt.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/trafficscript.py
--rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/typoscript.py
--rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/ul4.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/unicon.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/urbi.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/usd.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/varnish.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/verification.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/verifpal.py
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/vip.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/vyper.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/web.py
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/webassembly.py
--rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/webidl.py
--rw-r--r--   0        0        0    40549 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/webmisc.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/wgsl.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/whiley.py
--rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/wowtoc.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/wren.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/x10.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/xorg.py
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/yang.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/yara.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/lexers/zig.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/__init__.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/_mapping.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/abap.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/algol.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/algol_nu.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/arduino.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/autumn.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/borland.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/bw.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/colorful.py
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/default.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/dracula.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/emacs.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/friendly.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/friendly_grayscale.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/fruity.py
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/gh_dark.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/gruvbox.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/igor.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/inkpot.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/lightbulb.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/lilypond.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/lovelace.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/manni.py
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/material.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/monokai.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/murphy.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/native.py
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/nord.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/onedark.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/paraiso_dark.py
--rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/paraiso_light.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/pastie.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/perldoc.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/rainbow_dash.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/rrt.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/sas.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/solarized.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/staroffice.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/stata_dark.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/stata_light.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/tango.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/trac.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/vim.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/vs.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/xcode.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments/styles/zenburn.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments-2.17.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments-2.17.2.dist-info/METADATA
--rw-r--r--   0        0        0    45069 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments-2.17.2.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments-2.17.2.dist-info/WHEEL
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments-2.17.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0    10281 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments-2.17.2.dist-info/licenses/AUTHORS
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/METADATA
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/WHEEL
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/pywin32_ctypes-0.2.2.dist-info/top_level.txt
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer/__init__.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer/__main__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer/clean.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer/markdown.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer/py.typed
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer/rst.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer/txt.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer-43.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer-43.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer-43.0.dist-info/METADATA
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer-43.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer-43.0.dist-info/WHEEL
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/readme_renderer-43.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/_internal_utils.py
--rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/auth.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/certs.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/cookies.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/exceptions.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/hooks.py
--rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/models.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/structures.py
--rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests/utils.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests-2.31.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests-2.31.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests-2.31.0.dist-info/METADATA
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests-2.31.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests-2.31.0.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests-2.31.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/__init__.py
--rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/_compat.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/exceptions.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/sessions.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/streaming_iterator.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/adapters/__init__.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/adapters/appengine.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/adapters/socket_options.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/adapters/source.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/adapters/ssl.py
--rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/adapters/x509.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/auth/__init__.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/auth/guess.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/auth/handler.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/cookies/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/cookies/forgetful.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/downloadutils/__init__.py
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/downloadutils/stream.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/downloadutils/tee.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/multipart/__init__.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/multipart/decoder.py
--rw-r--r--   0        0        0    20769 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/multipart/encoder.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/threaded/__init__.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/threaded/pool.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/threaded/thread.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/utils/__init__.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/utils/deprecated.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/utils/dump.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/utils/formdata.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt/utils/user_agent.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/AUTHORS.rst
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0    14638 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/requests_toolbelt-1.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/__init__.py
--rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/_mixin.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/abnf_regexp.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/api.py
--rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/builder.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/compat.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/exceptions.py
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/iri.py
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/misc.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/normalizers.py
--rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/parseresult.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/uri.py
--rw-r--r--   0        0        0    13676 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986/validators.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986-2.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986-2.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986-2.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986-2.0.0.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986-2.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/__init__.py
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/__main__.py
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_export_format.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_inspect.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_pick.py
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_timer.py
--rw-r--r--   0        0        0    22784 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_win32_console.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_windows.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_windows_renderer.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/_wrap.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/abc.py
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/ansi.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/bar.py
--rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/box.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/cells.py
--rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/columns.py
--rw-r--r--   0        0        0    99101 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/constrain.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/containers.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/control.py
--rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/default_styles.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/diagnose.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/filesize.py
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/highlighter.py
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/json.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/jupyter.py
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/layout.py
--rw-r--r--   0        0        0    14271 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/live.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/live_render.py
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/logging.py
--rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/markdown.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/measure.py
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/pager.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/palette.py
--rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/panel.py
--rw-r--r--   0        0        0    35812 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/pretty.py
--rw-r--r--   0        0        0    59703 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/progress.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/progress_bar.py
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/prompt.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/region.py
--rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/repr.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/rule.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/scope.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/screen.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/spinner.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/style.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/styled.py
--rw-r--r--   0        0        0    35367 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/syntax.py
--rw-r--r--   0        0        0    39644 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/terminal_theme.py
--rw-r--r--   0        0        0    47300 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/themes.py
--rw-r--r--   0        0        0    29529 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/traceback.py
--rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich/tree.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich-13.7.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich-13.7.1.dist-info/LICENSE
--rw-r--r--   0        0        0    18636 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich-13.7.1.dist-info/METADATA
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich-13.7.1.dist-info/RECORD
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/rich-13.7.1.dist-info/WHEEL
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/__main__.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/auth.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/cli.py
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/exceptions.py
--rw-r--r--   0        0        0    11018 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/py.typed
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/repository.py
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/settings.py
--rw-r--r--   0        0        0    10979 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/utils.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/wheel.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/wininst.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/commands/__init__.py
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/commands/check.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/commands/register.py
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine/commands/upload.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine-5.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine-5.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine-5.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine-5.0.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine-5.0.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine-5.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine-5.0.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/twine-5.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/__init__.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/_base_connection.py
--rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/_collections.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/_request_methods.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/_version.py
--rw-r--r--   0        0        0    34704 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/connection.py
--rw-r--r--   0        0        0    43556 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/connectionpool.py
--rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/exceptions.py
--rw-r--r--   0        0        0    10843 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/fields.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/filepost.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/http2.py
--rw-r--r--   0        0        0    22935 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/poolmanager.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/py.typed
--rw-r--r--   0        0        0    43874 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0    19161 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/contrib/socks.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/contrib/emscripten/__init__.py
--rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/contrib/emscripten/connection.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/contrib/emscripten/fetch.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/contrib/emscripten/request.py
--rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/contrib/emscripten/response.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/connection.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/proxy.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/request.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/response.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/retry.py
--rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/timeout.py
--rw-r--r--   0        0        0    15213 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/url.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/util.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3/util/wait.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3-2.2.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3-2.2.1.dist-info/METADATA
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3-2.2.1.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3-2.2.1.dist-info/WHEEL
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/__init__.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/pywintypes.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/version.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/win32api.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/win32cred.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/_winerrors.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/compat.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/cffi/__init__.py
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/cffi/_authentication.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/cffi/_common.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/cffi/_dll.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/cffi/_nl_support.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/cffi/_resource.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/cffi/_system_information.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/cffi/_time.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/cffi/_util.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/ctypes/__init__.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/ctypes/_common.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/ctypes/_dll.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/ctypes/_nl_support.py
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/ctypes/_resource.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/ctypes/_time.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/core/ctypes/_util.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/pywin32/__init__.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/pywin32/pywintypes.py
--rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/pywin32/win32api.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/pywin32/win32cred.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/tests/__init__.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/tests/test_backends.py
--rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/tests/test_win32api.py
--rw-r--r--   0        0        0     7718 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/win32ctypes/tests/test_win32cred.py
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/zipp/__init__.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/zipp/glob.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/zipp/compat/__init__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/zipp/compat/py310.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/zipp-3.18.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/zipp-3.18.1.dist-info/LICENSE
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/zipp-3.18.1.dist-info/METADATA
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/zipp-3.18.1.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/zipp-3.18.1.dist-info/WHEEL
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/Lib/site-packages/zipp-3.18.1.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/src/simple_background_remover/__init__.py
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/src/simple_background_remover/color_helper.py
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/src/simple_background_remover/simple_background_remover.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/LICENSE
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/README.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 simple_background_remover-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 simple_background_remover-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 simple_background_remover-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 simple_background_remover-0.0.2/src/simple_background_remover/__init__.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 simple_background_remover-0.0.2/src/simple_background_remover/color_helper.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 simple_background_remover-0.0.2/src/simple_background_remover/simple_background_remover.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 simple_background_remover-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 simple_background_remover-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 simple_background_remover-0.0.2/README.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 simple_background_remover-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 simple_background_remover-0.0.2/PKG-INFO
```

### Comparing `simple_background_remover-0.0.1/Lib/site-packages/build-1.2.1.dist-info/LICENSE` & `simple_background_remover-0.0.2/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-Copyright © 2019 Filipe Laíns <filipe.lains@gmail.com>
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
+Copyright (c) 2024 oversizedcanoe
 
-The above copyright notice and this permission notice (including the next
-paragraph) shall be included in all copies or substantial portions of the
-Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `simple_background_remover-0.0.1/src/simple_background_remover/color_helper.py` & `simple_background_remover-0.0.2/src/simple_background_remover/color_helper.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-import math
-
-class _ColorHelper:
-    """
-    Contains logic for handling color-related tasks.
-    """
-
-    MAX_COLOR_DIFFERENCE: float = 764.83
-    MIN_WIGGLE_ROOM: float = 0.03
-    TRANSPARENT_COLOR: tuple[int, int, int] = (0,0,0,0)
-
-    def __init__(self, background_color):
-        self.__wiggle_room: float = self.MIN_WIGGLE_ROOM
-        self.background_color: tuple[int, int, int] = background_color
-        self.min_red: int | None = None
-        self.max_red: int | None = None
-        self.min_blue: int | None = None
-        self.max_blue: int | None = None
-        self.min_green: int | None = None
-        self.max_green: int | None = None
-
-    def __mins_and_maxes_not_initialized(self) -> bool:
-        return (self.min_red is None \
-                or self.max_red is None \
-                or self.min_green is None \
-                or self.max_green is None \
-                or self.min_blue is None \
-                or self.max_blue is None)
-
-    def __initialize_mins_and_maxes(self) -> None:
-        self.min_red = self.__get_min_color_value(self.background_color[0])
-        self.max_red = self.__get_max_color_value(self.background_color[0])
-        self.min_green = self.__get_min_color_value(self.background_color[1])
-        self.max_green = self.__get_max_color_value(self.background_color[1])
-        self.min_blue = self.__get_min_color_value(self.background_color[2])
-        self.max_blue = self.__get_max_color_value(self.background_color[2])
-
-    def __get_min_color_value(self, color_value: tuple[int, int, int]) -> float:
-        min_value = round(color_value * (1 - self.__wiggle_room))
-
-        if min_value < 0:
-            min_value = 0
-
-        return min_value
-
-    def __get_max_color_value(self, color_value: tuple[int, int, int]) -> float:
-        max_value = round((color_value * (1 + self.__wiggle_room)) + 1)
-
-        if max_value >= 255:
-            max_value = 256
-
-        return max_value
-    
-    def get_wiggle_room(self) -> float:
-        return self.__wiggle_room
-    
-    def set_wiggle_room(self, wiggle_room_value: float) -> None:
-        self.__wiggle_room = wiggle_room_value
-        self.__initialize_mins_and_maxes()
-
-    def is_close_to_background(self, color_r_value, color_g_value, color_b_value) -> bool:
-        bg_r_value = self.background_color[0]
-        bg_g_value = self.background_color[1]
-        bg_b_value = self.background_color[2]
-
-        if (color_r_value, color_g_value, color_b_value) == (bg_r_value, bg_g_value, bg_b_value):
-            return True
-
-        if self.__mins_and_maxes_not_initialized():
-            self.__initialize_mins_and_maxes()
-
-        red_in_range = color_r_value in range(self.min_red, self.max_red)
-        green_in_range = color_g_value in range(self.min_green, self.max_green)
-        blue_in_range = color_b_value in range(self.min_blue, self.max_blue)
-
-        return red_in_range and green_in_range and blue_in_range
-
-    def get_color_difference(self, average_color: tuple[int, int, int]) -> bool:
-        # Euclidean distance
-        delta_r_squared = (average_color[0] - self.background_color[0]) ** 2
-        delta_g_squared = (average_color[1] - self.background_color[1]) ** 2
-        delta_b_squared = (average_color[2] - self.background_color[2]) ** 2
-        average_r = round((average_color[0] + self.background_color[0]) / 2)
-
-        # redmean -> https://en.wikipedia.org/wiki/Color_difference
-        term_1 = (2 + (average_r / 256)) * delta_r_squared
-        term_2 = 4 * delta_g_squared
-        term_3 = (2 + ((255 - average_r) / 256)) * delta_b_squared
-
-        return math.sqrt(term_1 + term_2 + term_3)
-    
-    def get_ideal_wiggle_room(self, color_difference: float) -> float:
-        # In "redmean" Euclidean distance, the largest value (where the background is white
-        # and all non-background is black) is 764.83.
-        # Take the ratio between calculated color difference and the max possible value (764.83).
-
-        # I find squaring them before dividing gets a more accurate result
+import math
+
+class _ColorHelper:
+    """
+    Contains logic for handling color-related tasks.
+    """
+
+    MAX_COLOR_DIFFERENCE: float = 764.83
+    MIN_WIGGLE_ROOM: float = 0.03
+    TRANSPARENT_COLOR: tuple[int, int, int] = (0,0,0,0)
+
+    def __init__(self, background_color):
+        self.__wiggle_room: float = self.MIN_WIGGLE_ROOM
+        self.background_color: tuple[int, int, int] = background_color
+        self.min_red: int | None = None
+        self.max_red: int | None = None
+        self.min_blue: int | None = None
+        self.max_blue: int | None = None
+        self.min_green: int | None = None
+        self.max_green: int | None = None
+
+    def __mins_and_maxes_not_initialized(self) -> bool:
+        return (self.min_red is None \
+                or self.max_red is None \
+                or self.min_green is None \
+                or self.max_green is None \
+                or self.min_blue is None \
+                or self.max_blue is None)
+
+    def __initialize_mins_and_maxes(self) -> None:
+        self.min_red = self.__get_min_color_value(self.background_color[0])
+        self.max_red = self.__get_max_color_value(self.background_color[0])
+        self.min_green = self.__get_min_color_value(self.background_color[1])
+        self.max_green = self.__get_max_color_value(self.background_color[1])
+        self.min_blue = self.__get_min_color_value(self.background_color[2])
+        self.max_blue = self.__get_max_color_value(self.background_color[2])
+
+    def __get_min_color_value(self, color_value: tuple[int, int, int]) -> float:
+        min_value = round(color_value * (1 - self.__wiggle_room))
+
+        if min_value < 0:
+            min_value = 0
+
+        return min_value
+
+    def __get_max_color_value(self, color_value: tuple[int, int, int]) -> float:
+        max_value = round((color_value * (1 + self.__wiggle_room)) + 1)
+
+        if max_value >= 255:
+            max_value = 256
+
+        return max_value
+    
+    def get_wiggle_room(self) -> float:
+        return self.__wiggle_room
+    
+    def set_wiggle_room(self, wiggle_room_value: float) -> None:
+        self.__wiggle_room = wiggle_room_value
+        self.__initialize_mins_and_maxes()
+
+    def is_close_to_background(self, color_r_value, color_g_value, color_b_value) -> bool:
+        bg_r_value = self.background_color[0]
+        bg_g_value = self.background_color[1]
+        bg_b_value = self.background_color[2]
+
+        if (color_r_value, color_g_value, color_b_value) == (bg_r_value, bg_g_value, bg_b_value):
+            return True
+
+        if self.__mins_and_maxes_not_initialized():
+            self.__initialize_mins_and_maxes()
+
+        red_in_range = color_r_value in range(self.min_red, self.max_red)
+        green_in_range = color_g_value in range(self.min_green, self.max_green)
+        blue_in_range = color_b_value in range(self.min_blue, self.max_blue)
+
+        return red_in_range and green_in_range and blue_in_range
+
+    def get_color_difference(self, average_color: tuple[int, int, int]) -> bool:
+        # Euclidean distance
+        delta_r_squared = (average_color[0] - self.background_color[0]) ** 2
+        delta_g_squared = (average_color[1] - self.background_color[1]) ** 2
+        delta_b_squared = (average_color[2] - self.background_color[2]) ** 2
+        average_r = round((average_color[0] + self.background_color[0]) / 2)
+
+        # redmean -> https://en.wikipedia.org/wiki/Color_difference
+        term_1 = (2 + (average_r / 256)) * delta_r_squared
+        term_2 = 4 * delta_g_squared
+        term_3 = (2 + ((255 - average_r) / 256)) * delta_b_squared
+
+        return math.sqrt(term_1 + term_2 + term_3)
+    
+    def get_ideal_wiggle_room(self, color_difference: float) -> float:
+        # In "redmean" Euclidean distance, the largest value (where the background is white
+        # and all non-background is black) is 764.83.
+        # Take the ratio between calculated color difference and the max possible value (764.83).
+
+        # I find squaring them before dividing gets a more accurate result
         return color_difference ** 2 / self.MAX_COLOR_DIFFERENCE ** 2
```

### Comparing `simple_background_remover-0.0.1/src/simple_background_remover/simple_background_remover.py` & `simple_background_remover-0.0.2/src/simple_background_remover/simple_background_remover.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-from PIL import Image
-from color_helper import _ColorHelper
-
-def remove_background(input_filename: str, output_filename: str, wiggle_room: float = None, background_color: tuple[int, int, int] = None) -> None:
-    """
-    Removes the background of the provided image and saves it as a PNG.
-    
-    :param input_filename: The path and file name of the input image, including file type.
-    :param output_filename: The desired path and file name of the output image, not including file type. 
-    :param wiggle_room: Optional parameter between 0 and 1, which contains the +/- %
-    range a color can be similar to the background color. If not passed, the wiggle room
-    will be auto-determined.
-    :param background_color: Optional parameter for the RGB color of the background.
-    If not passed, the background will be auto-determined.
-
-    See https://github.com/oversizedcanoe/BackgroundRemover for more detailed info.
-    """
-    image = Image.open(input_filename).convert("RGBA")
-    image_data = image.getdata()
-    new_data = []
-
-    if background_color is None:
-        background_color = __get_determined_background_color(image)
-
-    helper = _ColorHelper(background_color)
-
-    if wiggle_room is None:
-        wiggle_room = __get_ideal_wiggle_room(helper, image_data)
-
-    helper.set_wiggle_room(wiggle_room)
-        
-    for pixel_data in image_data:
-        if helper.is_close_to_background(pixel_data[0], pixel_data[1], pixel_data[2]):
-            new_data.append(helper.TRANSPARENT_COLOR)
-        else:
-            new_data.append(pixel_data)
-
-    image.putdata(new_data)
-    file_name = f'{output_filename}-{round(helper.get_wiggle_room(), 3)}.png'
-    image.save(file_name, "PNG")
-    print(f'Image saved: \'{file_name}\'')
-            
-
-def __get_determined_background_color(image: Image.Image) -> tuple[int, int, int]:
-    """
-    Determines the solid background color of an image by looking at 
-    the top-left 5% of the image and taking the average pixel color.
-    """
-    width, height = image.size
-    
-    # top 5%
-    width_limit = round(width * 0.05)
-    height_limit = round(height * 0.05)
-
-    total_pixels = 0
-    total_red = 0
-    total_green = 0
-    total_blue = 0
-
-    for x in range(0, width_limit):
-        for y in range(0, height_limit):
-            pixel_color = image.getpixel((x,y))
-            total_red += pixel_color[0]
-            total_green += pixel_color[1]
-            total_blue += pixel_color[2]
-            total_pixels += 1
-
-    return (round(total_red/total_pixels), round(total_green/total_pixels), round(total_blue/total_pixels))
-
-def __get_ideal_wiggle_room(helper: _ColorHelper, image_data: list) -> float:
-    """
-    Determine the ideal wiggle room of an image. This is done by determining the contrast between
-    foreground and background colors. A larger contrast means a larger wiggle room can be used. A
-    smaller contrast means foreground pixels are similar to the background, and we need to
-    use a smaller contrast to prevent accidentally transparent-ifying foreground pixels.
-    """
-    
-    total_r = 0
-    total_g = 0
-    total_b = 0
-    foreground_pixels_counted = 0
-
-    # Start with min wiggle room to take a conservative estimate of foreground vs background pixels
-    helper.set_wiggle_room(helper.MIN_WIGGLE_ROOM)
-
-    for pixel_data in image_data:
-        red = pixel_data[0]
-        green = pixel_data[1]
-        blue = pixel_data[2]
-        if helper.is_close_to_background(red, green, blue) == False:
-            total_r += red
-            total_g += green
-            total_b += blue
-            foreground_pixels_counted += 1
-
-    if foreground_pixels_counted == 0:
-        # Only possible if image is 'all background', meaning it will be made entirely transparent.
-        return helper.MIN_WIGGLE_ROOM
-    
-    average_r = round(total_r / foreground_pixels_counted)
-    average_g = round(total_g / foreground_pixels_counted)
-    average_b = round(total_b / foreground_pixels_counted)
-    color_difference = helper.get_color_difference((average_r, average_g, average_b))
-    ideal_wiggle_room = helper.get_ideal_wiggle_room(color_difference)
-
+from PIL import Image
+from color_helper import _ColorHelper
+
+def remove_background(input_filename: str, output_filename: str, wiggle_room: float = None, background_color: tuple[int, int, int] = None) -> None:
+    """
+    Removes the background of the provided image and saves it as a PNG.
+    
+    :param input_filename: The path and file name of the input image, including file type.
+    :param output_filename: The desired path and file name of the output image, not including file type. 
+    :param wiggle_room: Optional parameter between 0 and 1, which contains the +/- %
+    range a color can be similar to the background color. If not passed, the wiggle room
+    will be auto-determined.
+    :param background_color: Optional parameter for the RGB color of the background.
+    If not passed, the background will be auto-determined.
+
+    See https://github.com/oversizedcanoe/BackgroundRemover for more detailed info.
+    """
+    image = Image.open(input_filename).convert("RGBA")
+    image_data = image.getdata()
+    new_data = []
+
+    if background_color is None:
+        background_color = __get_determined_background_color(image)
+
+    helper = _ColorHelper(background_color)
+
+    if wiggle_room is None:
+        wiggle_room = __get_ideal_wiggle_room(helper, image_data)
+
+    helper.set_wiggle_room(wiggle_room)
+        
+    for pixel_data in image_data:
+        if helper.is_close_to_background(pixel_data[0], pixel_data[1], pixel_data[2]):
+            new_data.append(helper.TRANSPARENT_COLOR)
+        else:
+            new_data.append(pixel_data)
+
+    image.putdata(new_data)
+    file_name = f'{output_filename}-{round(helper.get_wiggle_room(), 3)}.png'
+    image.save(file_name, "PNG")
+    print(f'Image saved: \'{file_name}\'')
+            
+
+def __get_determined_background_color(image: Image.Image) -> tuple[int, int, int]:
+    """
+    Determines the solid background color of an image by looking at 
+    the top-left 5% of the image and taking the average pixel color.
+    """
+    width, height = image.size
+    
+    # top 5%
+    width_limit = round(width * 0.05)
+    height_limit = round(height * 0.05)
+
+    total_pixels = 0
+    total_red = 0
+    total_green = 0
+    total_blue = 0
+
+    for x in range(0, width_limit):
+        for y in range(0, height_limit):
+            pixel_color = image.getpixel((x,y))
+            total_red += pixel_color[0]
+            total_green += pixel_color[1]
+            total_blue += pixel_color[2]
+            total_pixels += 1
+
+    return (round(total_red/total_pixels), round(total_green/total_pixels), round(total_blue/total_pixels))
+
+def __get_ideal_wiggle_room(helper: _ColorHelper, image_data: list) -> float:
+    """
+    Determine the ideal wiggle room of an image. This is done by determining the contrast between
+    foreground and background colors. A larger contrast means a larger wiggle room can be used. A
+    smaller contrast means foreground pixels are similar to the background, and we need to
+    use a smaller contrast to prevent accidentally transparent-ifying foreground pixels.
+    """
+    
+    total_r = 0
+    total_g = 0
+    total_b = 0
+    foreground_pixels_counted = 0
+
+    # Start with min wiggle room to take a conservative estimate of foreground vs background pixels
+    helper.set_wiggle_room(helper.MIN_WIGGLE_ROOM)
+
+    for pixel_data in image_data:
+        red = pixel_data[0]
+        green = pixel_data[1]
+        blue = pixel_data[2]
+        if helper.is_close_to_background(red, green, blue) == False:
+            total_r += red
+            total_g += green
+            total_b += blue
+            foreground_pixels_counted += 1
+
+    if foreground_pixels_counted == 0:
+        # Only possible if image is 'all background', meaning it will be made entirely transparent.
+        return helper.MIN_WIGGLE_ROOM
+    
+    average_r = round(total_r / foreground_pixels_counted)
+    average_g = round(total_g / foreground_pixels_counted)
+    average_b = round(total_b / foreground_pixels_counted)
+    color_difference = helper.get_color_difference((average_r, average_g, average_b))
+    ideal_wiggle_room = helper.get_ideal_wiggle_room(color_difference)
+
     return ideal_wiggle_room
```

### Comparing `simple_background_remover-0.0.1/.gitignore` & `simple_background_remover-0.0.2/.gitignore`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
-
-
-# User added
-Scripts
-pyvenv.cfg
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
+
+
+# User added
+Scripts
+pyvenv.cfg
 .vs
```

### Comparing `simple_background_remover-0.0.1/README.md` & `simple_background_remover-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,48 @@
-# simple_background_remover
-This library is meant to be a quick and dirty background remover for simple images with solid(ish) background colors. Basically, a green screen. It does not have any sort of 'foreground detection'; it simply transparent-ifies pixels which are similar to the provided (or determined) background color.
-
-The processed files automatically get saved as PNGs.
-
-#### Usage
-```python
-from simple_background_remover import remove_background
-
-remove_background(input_filename='images/myPhoto.jpg',
-                  output_filename='images/processed/myPhoto', 
-                  wiggle_room=0.15, 
-                  background_color=(0, 0, 0))
-```
-
-#### wiggle_room
-`wiggle_room` is an optional parameter between 0 and 1. It determines how similar a pixels color can be to the background color and still be considered 'background'. For example, a value of 0.2 means that pixels can be +/- 20% similar to the background color and still be considered background pixels, and therefore made transparents. Note: This 20% range is applied to the R, G, and B value of the background color, so it's not perfect. Ideally it would use [redmean/Euclidean distance](https://en.wikipedia.org/wiki/Color_difference) like the auto-generated `wiggle_room` (more on that below) uses.
-
-If wiggle_room is not passed/left as `None`, the wiggle room will be auto-determined by roughly calculating the contrast between the average foreground and background color. The larger the contrast (i.e. foreground black, background white), the higher `wiggle_room` can be. The smaller the constrast (i.e. foreground black, background dark gray), the lower `wiggle_room` must be, otherwise you risk accidentally transparent-ifying foreground pixels.
-
-#### background_color
-`background_color` is an optional parameter for the background color of the image (passed as an RGB color, as `tuple[int, int, int]` -- i.e. (0, 0, 0) for white). If not passed `background_color` will be estimated based on the average color of the top left 5% of the image. Ideally this could be flexible for the caller in the future. 
-
-#### Examples
- - To do: post some images
-
----
-## Todo
-Lots more can be done to improve this repo. 
- - General clean up -- I wrote this pretty quickly and many places could be cleaned up/refactored
- - Validation on user inputs
- - Improvements on the auto determination of background color and wiggle room
-   - Could use the redmean to determine the closeness to background per pixel instead of doing +/- wiggle room -- although may be very slow
+Metadata-Version: 2.3
+Name: simple_background_remover
+Version: 0.0.2
+Summary: A quick and dirty background remover for simple images with solid(ish) background colors.
+Project-URL: Homepage, https://github.com/oversizedcanoe/simple_background_remover 
+Author: oversizedcanoe
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Requires-Dist: pillow>=10.2.0
+Description-Content-Type: text/markdown
+
+# simple_background_remover
+This library is meant to be a quick and dirty background remover for simple images with solid(ish) background colors. Basically, a green screen. It does not have any sort of 'foreground detection'; it simply transparent-ifies pixels which are similar to the provided (or determined) background color.
+
+The processed files automatically get saved as PNGs.
+
+#### Usage
+```python
+from simple_background_remover import remove_background
+
+remove_background(input_filename='images/myPhoto.jpg',
+                  output_filename='images/processed/myPhoto', 
+                  wiggle_room=0.15, 
+                  background_color=(0, 0, 0))
+```
+
+#### wiggle_room
+`wiggle_room` is an optional parameter between 0 and 1. It determines how similar a pixels color can be to the background color and still be considered 'background'. For example, a value of 0.2 means that pixels can be +/- 20% similar to the background color and still be considered background pixels, and therefore made transparents. Note: This 20% range is applied to the R, G, and B value of the background color, so it's not perfect. Ideally it would use [redmean/Euclidean distance](https://en.wikipedia.org/wiki/Color_difference) like the auto-generated `wiggle_room` (more on that below) uses.
+
+If wiggle_room is not passed/left as `None`, the wiggle room will be auto-determined by roughly calculating the contrast between the average foreground and background color. The larger the contrast (i.e. foreground black, background white), the higher `wiggle_room` can be. The smaller the constrast (i.e. foreground black, background dark gray), the lower `wiggle_room` must be, otherwise you risk accidentally transparent-ifying foreground pixels.
+
+#### background_color
+`background_color` is an optional parameter for the background color of the image (passed as an RGB color, as `tuple[int, int, int]` -- i.e. (0, 0, 0) for white). If not passed `background_color` will be estimated based on the average color of the top left 5% of the image. Ideally this could be flexible for the caller in the future. 
+
+#### Examples
+ - To do: post some images
+
+---
+## Todo
+Lots more can be done to improve this repo. 
+ - General clean up -- I wrote this pretty quickly and many places could be cleaned up/refactored
+ - Validation on user inputs
+ - Improvements on the auto determination of background color and wiggle room
+   - Could use the redmean to determine the closeness to background per pixel instead of doing +/- wiggle room -- although may be very slow
    - Allow user to pass in which corner to read background from
```

### Comparing `simple_background_remover-0.0.1/PKG-INFO` & `simple_background_remover-0.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.3
-Name: simple_background_remover
-Version: 0.0.1
-Summary: A quick and dirty background remover for simple images with solid(ish) background colors.
-Project-URL: Homepage, https://github.com/oversizedcanoe/simple_background_remover
-Author: oversizedcanoe
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Requires-Dist: pillow>=10.2.0
-Description-Content-Type: text/markdown
-
 # simple_background_remover
 This library is meant to be a quick and dirty background remover for simple images with solid(ish) background colors. Basically, a green screen. It does not have any sort of 'foreground detection'; it simply transparent-ifies pixels which are similar to the provided (or determined) background color.
 
 The processed files automatically get saved as PNGs.
 
 #### Usage
 ```python
```

