# Comparing `tmp/guiqwt-4.4.0.tar.gz` & `tmp/guiqwt-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guiqwt-4.4.0.tar", last modified: Thu Jul  6 17:58:21 2023, max compression
+gzip compressed data, was "guiqwt-4.4.1.tar", last modified: Fri Jul 21 16:19:09 2023, max compression
```

## Comparing `guiqwt-4.4.0.tar` & `guiqwt-4.4.1.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.663087 guiqwt-4.4.0/
--rw-rw-rw-   0        0        0    37564 2023-07-06 17:55:17.000000 guiqwt-4.4.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    21603 2019-10-08 16:03:22.000000 guiqwt-4.4.0/Licence_CeCILL_V2-en.txt
--rw-rw-rw-   0        0        0      451 2021-02-06 17:38:23.000000 guiqwt-4.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2640 2023-07-06 17:58:21.663087 guiqwt-4.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2516 2022-08-01 14:49:33.000000 guiqwt-4.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:20.958638 guiqwt-4.4.0/doc/
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:20.958638 guiqwt-4.4.0/doc/_static/
--rw-rw-rw-   0        0        0     7886 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/_static/favicon.ico
--rw-rw-rw-   0        0        0     7119 2021-12-19 10:52:19.000000 guiqwt-4.4.0/doc/conf.py
--rw-rw-rw-   0        0        0      512 2021-12-19 10:39:43.000000 guiqwt-4.4.0/doc/development.rst
--rw-rw-rw-   0        0        0     1942 2023-07-06 13:56:54.000000 guiqwt-4.4.0/doc/disthelpers.rst
--rw-rw-rw-   0        0        0     2648 2023-07-06 17:17:16.000000 guiqwt-4.4.0/doc/examples.rst
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:20.958638 guiqwt-4.4.0/doc/images/
--rw-rw-rw-   0        0        0    32373 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/images/curve_widgets.png
--rw-rw-rw-   0        0        0     3360 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/guiqwt.png
--rw-rw-rw-   0        0        0    49787 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/images/image_widgets.png
--rw-rw-rw-   0        0        0    28528 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/my_plot_manager.png
--rw-rw-rw-   0        0        0   142571 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/panorama.png
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.027667 guiqwt-4.4.0/doc/images/screenshots/
--rw-rw-rw-   0        0        0    33973 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/__init__.png
--rw-rw-rw-   0        0        0    32219 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/computations.png
--rw-rw-rw-   0        0        0   103911 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/contrast.png
--rw-rw-rw-   0        0        0   123005 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/cross_section.png
--rw-rw-rw-   0        0        0   123510 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/cross_section2.png
--rw-rw-rw-   0        0        0    68152 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/images/screenshots/dotarraydemo.png
--rw-rw-rw-   0        0        0    52268 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/fit.png
--rw-rw-rw-   0        0        0    33435 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/get_point.png
--rw-rw-rw-   0        0        0    70160 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/hist2d.png
--rw-rw-rw-   0        0        0   146225 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/image_plot_tools.png
--rw-rw-rw-   0        0        0   114920 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/imagefilter.png
--rw-rw-rw-   0        0        0    73527 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/imagesuperp.png
--rw-rw-rw-   0        0        0   187178 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/imagexy.png
--rw-rw-rw-   0        0        0   100238 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/manager.png
--rw-rw-rw-   0        0        0   123059 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/mandelbrot.png
--rw-rw-rw-   0        0        0    49104 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/pcolor.png
--rw-rw-rw-   0        0        0    80158 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/plot.png
--rw-rw-rw-   0        0        0    66602 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/sift1.png
--rw-rw-rw-   0        0        0   139606 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/sift2.png
--rw-rw-rw-   0        0        0    94356 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/sift3.png
--rw-rw-rw-   0        0        0    47500 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/simple_dialog.png
--rw-rw-rw-   0        0        0    76231 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/simple_window.png
--rw-rw-rw-   0        0        0   391598 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/transform.png
--rw-rw-rw-   0        0        0      824 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/index.rst
--rw-rw-rw-   0        0        0     1503 2023-07-06 13:43:56.000000 guiqwt-4.4.0/doc/installation.rst
--rw-rw-rw-   0        0        0     1360 2021-12-19 10:56:36.000000 guiqwt-4.4.0/doc/migrating_from_v2_to_v3.rst
--rw-rw-rw-   0        0        0     5960 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/overview.rst
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.058937 guiqwt-4.4.0/doc/reference/
--rw-rw-rw-   0        0        0       36 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/annotations.rst
--rw-rw-rw-   0        0        0       33 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/baseplot.rst
--rw-rw-rw-   0        0        0       32 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/builder.rst
--rw-rw-rw-   0        0        0       38 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/cross_section.rst
--rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/curve.rst
--rw-rw-rw-   0        0        0       34 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/histogram.rst
--rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/image.rst
--rw-rw-rw-   0        0        0      345 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/index.rst
--rw-rw-rw-   0        0        0       27 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/io.rst
--rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/label.rst
--rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/panels.rst
--rw-rw-rw-   0        0        0       29 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/plot.rst
--rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/pyplot.rst
--rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/shapes.rst
--rw-rw-rw-   0        0        0       32 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/signals.rst
--rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/styles.rst
--rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/tools.rst
--rw-rw-rw-   0        0        0       36 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/widgets_fit.rst
--rw-rw-rw-   0        0        0       45 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/widgets_resizedialog.rst
--rw-rw-rw-   0        0        0       43 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/widgets_rotatecrop.rst
--rw-rw-rw-   0        0        0      903 2023-06-10 14:03:47.000000 guiqwt-4.4.0/doc/sift.rst
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.121451 guiqwt-4.4.0/guiqwt/
--rw-rw-rw-   0        0        0    26398 2023-06-04 08:30:11.000000 guiqwt-4.4.0/guiqwt/__init__.py
--rw-rw-rw-   0        0        0   421487 2021-12-11 14:47:07.000000 guiqwt-4.4.0/guiqwt/_cm.py
--rw-rw-rw-   0        0        0    24601 2023-07-06 13:47:44.000000 guiqwt-4.4.0/guiqwt/annotations.py
--rw-rw-rw-   0        0        0    34502 2023-07-06 13:55:37.000000 guiqwt-4.4.0/guiqwt/baseplot.py
--rw-rw-rw-   0        0        0    53108 2023-06-04 08:46:35.000000 guiqwt-4.4.0/guiqwt/builder.py
--rw-rw-rw-   0        0        0     3798 2021-03-13 15:31:59.000000 guiqwt-4.4.0/guiqwt/colormap.py
--rw-rw-rw-   0        0        0    33453 2023-05-14 09:35:27.000000 guiqwt-4.4.0/guiqwt/config.py
--rw-rw-rw-   0        0        0    36835 2023-07-06 13:48:38.000000 guiqwt-4.4.0/guiqwt/cross_section.py
--rw-rw-rw-   0        0        0    65731 2023-07-06 13:49:01.000000 guiqwt-4.4.0/guiqwt/curve.py
--rw-rw-rw-   0        0        0     2189 2021-12-19 10:50:52.000000 guiqwt-4.4.0/guiqwt/debug.py
--rw-rw-rw-   0        0        0    25456 2022-08-01 14:49:33.000000 guiqwt-4.4.0/guiqwt/events.py
--rw-rw-rw-   0        0        0     3003 2021-12-11 14:46:59.000000 guiqwt-4.4.0/guiqwt/geometry.py
--rw-rw-rw-   0        0        0    20183 2023-07-06 13:49:23.000000 guiqwt-4.4.0/guiqwt/histogram.py
--rw-rw-rw-   0        0        0   103756 2023-07-06 13:54:21.000000 guiqwt-4.4.0/guiqwt/image.py
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.240439 guiqwt-4.4.0/guiqwt/images/
--rw-rw-rw-   0        0        0      827 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/arrow_down.png
--rw-rw-rw-   0        0        0      828 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/arrow_up.png
--rw-rw-rw-   0        0        0     1095 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/autorefresh.png
--rw-rw-rw-   0        0        0      739 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/axes.png
--rw-rw-rw-   0        0        0      593 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/center.png
--rw-rw-rw-   0        0        0      562 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/contrast.png
--rw-rw-rw-   0        0        0     1227 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/copytoclipboard.png
--rw-rw-rw-   0        0        0      953 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/csapplylut.png
--rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/csautoscale.png
--rw-rw-rw-   0        0        0      594 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/csection.png
--rw-rw-rw-   0        0        0      558 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/csection_a.png
--rw-rw-rw-   0        0        0      959 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/csection_oblique.png
--rw-rw-rw-   0        0        0      408 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/csperimage.png
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.250516 guiqwt-4.4.0/guiqwt/images/curvestyles/
--rw-rw-rw-   0        0        0      369 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/curvestyles/dots.png
--rw-rw-rw-   0        0        0      412 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/curvestyles/lines.png
--rw-rw-rw-   0        0        0      384 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/curvestyles/steps.png
--rw-rw-rw-   0        0        0      435 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/curvestyles/sticks.png
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.260614 guiqwt-4.4.0/guiqwt/images/curvetypes/
--rw-rw-rw-   0        0        0      570 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/curvetypes/xfy.png
--rw-rw-rw-   0        0        0      570 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/curvetypes/yfx.png
--rw-rw-rw-   0        0        0      430 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/eliminate_outliers.png
--rw-rw-rw-   0        0        0      882 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/eraser.png
--rw-rw-rw-   0        0        0     1108 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/export.png
--rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/font.png
--rw-rw-rw-   0        0        0      432 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/full_range.png
--rw-rw-rw-   0        0        0     1112 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/funct.png
--rw-rw-rw-   0        0        0    15224 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/guiqwt.svg
--rw-rw-rw-   0        0        0      399 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/hcursor.png
--rw-rw-rw-   0        0        0      660 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/hflip.png
--rw-rw-rw-   0        0        0     1041 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/imagestats.png
--rw-rw-rw-   0        0        0      684 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/item_list.png
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.299313 guiqwt-4.4.0/guiqwt/images/items/
--rw-rw-rw-   0        0        0      877 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/annotation.png
--rw-rw-rw-   0        0        0      551 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/curve.png
--rw-rw-rw-   0        0        0      419 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/errorbar.png
--rw-rw-rw-   0        0        0      368 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/grid.png
--rw-rw-rw-   0        0        0      387 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/histogram.png
--rw-rw-rw-   0        0        0     1104 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/histogram2d.png
--rw-rw-rw-   0        0        0     1077 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/image.png
--rw-rw-rw-   0        0        0      742 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/label.png
--rw-rw-rw-   0        0        0      564 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/legend.png
--rw-rw-rw-   0        0        0     2267 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/magnifier.png
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.321534 guiqwt-4.4.0/guiqwt/images/markers/
--rw-rw-rw-   0        0        0      337 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/cross.png
--rw-rw-rw-   0        0        0      420 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/diamond.png
--rw-rw-rw-   0        0        0      468 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/ellipse.png
--rw-rw-rw-   0        0        0      484 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/hexagon.png
--rw-rw-rw-   0        0        0      331 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/point.png
--rw-rw-rw-   0        0        0      363 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/square.png
--rw-rw-rw-   0        0        0      357 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/star.png
--rw-rw-rw-   0        0        0      449 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/triangle_d.png
--rw-rw-rw-   0        0        0      445 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/triangle_l.png
--rw-rw-rw-   0        0        0      438 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/triangle_r.png
--rw-rw-rw-   0        0        0      449 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/triangle_u.png
--rw-rw-rw-   0        0        0      349 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/xcross.png
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.331605 guiqwt-4.4.0/guiqwt/images/markerstyles/
--rw-rw-rw-   0        0        0      343 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markerstyles/cross_marker.png
--rw-rw-rw-   0        0        0      331 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markerstyles/horiz_marker.png
--rw-rw-rw-   0        0        0      333 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markerstyles/vert_marker.png
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.339652 guiqwt-4.4.0/guiqwt/images/mask/
--rw-rw-rw-   0        0        0      619 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/mask/mask_circle.png
--rw-rw-rw-   0        0        0      623 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/mask/mask_circle_outside.png
--rw-rw-rw-   0        0        0      445 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/mask/mask_rectangle.png
--rw-rw-rw-   0        0        0      446 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/mask/mask_rectangle_outside.png
--rw-rw-rw-   0        0        0      411 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/mask/mask_tool.png
--rw-rw-rw-   0        0        0      339 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/move.png
--rw-rw-rw-   0        0        0      644 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/on_curve.png
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.369823 guiqwt-4.4.0/guiqwt/images/patterns/
--rw-rw-rw-   0        0        0      325 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/bdiagpattern.png
--rw-rw-rw-   0        0        0      311 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/crosspattern.png
--rw-rw-rw-   0        0        0      303 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense1pattern.png
--rw-rw-rw-   0        0        0      305 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense2pattern.png
--rw-rw-rw-   0        0        0      309 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense3pattern.png
--rw-rw-rw-   0        0        0      300 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense4pattern.png
--rw-rw-rw-   0        0        0      307 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense5pattern.png
--rw-rw-rw-   0        0        0      311 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense6pattern.png
--rw-rw-rw-   0        0        0      308 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense7pattern.png
--rw-rw-rw-   0        0        0      324 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/diagcrosspattern.png
--rw-rw-rw-   0        0        0      330 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/fdiagpattern.png
--rw-rw-rw-   0        0        0      306 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/horpattern.png
--rw-rw-rw-   0        0        0      299 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/nobrush.png
--rw-rw-rw-   0        0        0      296 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/solidpattern.png
--rw-rw-rw-   0        0        0      304 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/verpattern.png
--rw-rw-rw-   0        0        0      442 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/point_selection.png
--rw-rw-rw-   0        0        0      913 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/print.png
--rw-rw-rw-   0        0        0      967 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/refresh.png
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.369823 guiqwt-4.4.0/guiqwt/images/scales/
--rw-rw-rw-   0        0        0      395 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/scales/lin_lin.png
--rw-rw-rw-   0        0        0      402 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/scales/lin_log.png
--rw-rw-rw-   0        0        0      403 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/scales/log_lin.png
--rw-rw-rw-   0        0        0      407 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/scales/log_log.png
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.385458 guiqwt-4.4.0/guiqwt/images/shapes/
--rw-rw-rw-   0        0        0      777 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/circle.png
--rw-rw-rw-   0        0        0      794 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/ellipse_shape.png
--rw-rw-rw-   0        0        0      552 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/freeform.png
--rw-rw-rw-   0        0        0      568 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/gtaxes.png
--rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/marker.png
--rw-rw-rw-   0        0        0      898 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/oblique_rectangle.png
--rw-rw-rw-   0        0        0      366 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/point_shape.png
--rw-rw-rw-   0        0        0      479 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/polyline.png
--rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/rectangle.png
--rw-rw-rw-   0        0        0      467 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/segment.png
--rw-rw-rw-   0        0        0    14258 2019-10-08 16:03:22.000000 guiqwt-4.4.0/guiqwt/images/sift.svg
--rw-rw-rw-   0        0        0     1340 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/snapshot.png
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.401085 guiqwt-4.4.0/guiqwt/images/styles/
--rw-rw-rw-   0        0        0      333 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/styles/dash.png
--rw-rw-rw-   0        0        0      338 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/styles/dashdot.png
--rw-rw-rw-   0        0        0      332 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/styles/dashdotdot.png
--rw-rw-rw-   0        0        0      328 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/styles/dot.png
--rw-rw-rw-   0        0        0      328 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/styles/solid.png
--rw-rw-rw-   0        0        0      401 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/trash.png
--rw-rw-rw-   0        0        0      407 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/vcursor.png
--rw-rw-rw-   0        0        0      658 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/vflip.png
--rw-rw-rw-   0        0        0      375 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/xcursor.png
--rw-rw-rw-   0        0        0      417 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/xrange.png
--rw-rw-rw-   0        0        0     9529 2021-12-11 14:46:59.000000 guiqwt-4.4.0/guiqwt/interfaces.py
--rw-rw-rw-   0        0        0    21868 2023-07-06 13:56:01.000000 guiqwt-4.4.0/guiqwt/io.py
--rw-rw-rw-   0        0        0    20156 2023-07-06 13:50:04.000000 guiqwt-4.4.0/guiqwt/label.py
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.414073 guiqwt-4.4.0/guiqwt/locale/
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:20.927373 guiqwt-4.4.0/guiqwt/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.425824 guiqwt-4.4.0/guiqwt/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    30153 2023-02-20 09:04:37.000000 guiqwt-4.4.0/guiqwt/locale/fr/LC_MESSAGES/guiqwt.mo
--rw-rw-rw-   0        0        0    57708 2022-08-01 14:49:33.000000 guiqwt-4.4.0/guiqwt/locale/fr/LC_MESSAGES/guiqwt.po
--rw-rw-rw-   0        0        0    44618 2023-02-20 09:03:54.000000 guiqwt-4.4.0/guiqwt/locale/guiqwt.pot
--rw-rw-rw-   0        0        0     3242 2023-07-06 13:50:35.000000 guiqwt-4.4.0/guiqwt/panels.py
--rw-rw-rw-   0        0        0    48599 2023-07-06 13:50:47.000000 guiqwt-4.4.0/guiqwt/plot.py
--rw-rw-rw-   0        0        0    19841 2023-02-19 15:02:16.000000 guiqwt-4.4.0/guiqwt/pyplot.py
--rw-rw-rw-   0        0        0     3361 2021-12-19 11:05:20.000000 guiqwt-4.4.0/guiqwt/qtdesigner.py
--rw-rw-rw-   0        0        0     5824 2022-04-08 12:35:06.000000 guiqwt-4.4.0/guiqwt/qthelpers.py
--rw-rw-rw-   0        0        0     1852 2021-12-11 14:47:00.000000 guiqwt-4.4.0/guiqwt/scaler.py
--rw-rw-rw-   0        0        0    54040 2023-07-06 13:50:11.000000 guiqwt-4.4.0/guiqwt/shapes.py
--rw-rw-rw-   0        0        0     4530 2023-05-13 07:53:17.000000 guiqwt-4.4.0/guiqwt/signals.py
--rw-rw-rw-   0        0        0    62787 2022-08-01 14:49:33.000000 guiqwt-4.4.0/guiqwt/styles.py
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.614626 guiqwt-4.4.0/guiqwt/tests/
--rw-rw-rw-   0        0        0      440 2021-12-11 14:47:02.000000 guiqwt-4.4.0/guiqwt/tests/__init__.py
--rw-rw-rw-   0        0        0     4305 2023-06-10 14:04:27.000000 guiqwt-4.4.0/guiqwt/tests/benchmarks.py
--rw-rw-rw-   0        0        0    39666 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/tests/brain.png
--rw-rw-rw-   0        0        0    35354 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/tests/brain_cylinder.png
--rw-rw-rw-   0        0        0     1374 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/computations.py
--rw-rw-rw-   0        0        0     1088 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/contrast.py
--rw-rw-rw-   0        0        0     1164 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/cross_section.py
--rw-rw-rw-   0        0        0     2021 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/cross_section_oblique.py
--rw-rw-rw-   0        0        0     1144 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/cursors.py
--rw-rw-rw-   0        0        0     1742 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/customize_shape_tool.py
--rw-rw-rw-   0        0        0      977 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/dicom_image.py
--rw-rw-rw-   0        0        0     6069 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/dotarraydemo.py
--rw-rw-rw-   0        0        0     2839 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/filtertest1.py
--rw-rw-rw-   0        0        0     3590 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/filtertest2.py
--rw-rw-rw-   0        0        0      807 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/fit.py
--rw-rw-rw-   0        0        0     1153 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/fliprotate.py
--rw-rw-rw-   0        0        0      401 2023-06-10 14:04:31.000000 guiqwt-4.4.0/guiqwt/tests/fontparam.py
--rw-rw-rw-   0        0        0     1514 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/get_point.py
--rw-rw-rw-   0        0        0     1517 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/get_segment.py
--rw-rw-rw-   0        0        0      801 2023-06-10 14:04:35.000000 guiqwt-4.4.0/guiqwt/tests/highprecisionxy.py
--rw-rw-rw-   0        0        0     1208 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/hist2d.py
--rw-rw-rw-   0        0        0     1357 2021-12-11 14:47:02.000000 guiqwt-4.4.0/guiqwt/tests/hist2d_func.py
--rw-rw-rw-   0        0        0      694 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/histogram.py
--rw-rw-rw-   0        0        0     3046 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/image.py
--rw-rw-rw-   0        0        0     1887 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/image_coords.py
--rw-rw-rw-   0        0        0     1416 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/image_masked.py
--rw-rw-rw-   0        0        0     1866 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/image_plot_tools.py
--rw-rw-rw-   0        0        0      954 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/image_rgb.py
--rw-rw-rw-   0        0        0     1635 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/imagefilter.py
--rw-rw-rw-   0        0        0     1605 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/imagesuperp.py
--rw-rw-rw-   0        0        0     1680 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/imagexy.py
--rw-rw-rw-   0        0        0      879 2023-07-06 13:51:49.000000 guiqwt-4.4.0/guiqwt/tests/loadsaveitems_hdf5.py
--rw-rw-rw-   0        0        0     1278 2023-07-06 13:51:55.000000 guiqwt-4.4.0/guiqwt/tests/loadsaveitems_json.py
--rw-rw-rw-   0        0        0     3881 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/loadsaveitems_pickle.py
--rw-rw-rw-   0        0        0     2710 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/loadtest.py
--rw-rw-rw-   0        0        0     2402 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/manager.py
--rw-rw-rw-   0        0        0     2617 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/mandelbrot.py
--rw-rw-rw-   0        0        0   525620 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/tests/mr-brain.dcm
--rw-rw-rw-   0        0        0     2660 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/pcolor.py
--rw-rw-rw-   0        0        0     1802 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/plot.py
--rw-rw-rw-   0        0        0      908 2023-06-10 14:04:39.000000 guiqwt-4.4.0/guiqwt/tests/plot_log.py
--rw-rw-rw-   0        0        0    14151 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/plot_timecurve.py
--rw-rw-rw-   0        0        0      785 2023-06-10 14:04:43.000000 guiqwt-4.4.0/guiqwt/tests/plot_yreverse.py
--rw-rw-rw-   0        0        0      587 2023-06-10 14:04:47.000000 guiqwt-4.4.0/guiqwt/tests/png_test.py
--rw-rw-rw-   0        0        0     2195 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/polygons.py
--rw-rw-rw-   0        0        0     1887 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/pyplot.py
--rw-rw-rw-   0        0        0     1032 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/qtdesigner.py
--rw-rw-rw-   0        0        0      993 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/tests/qtdesigner.ui
--rw-rw-rw-   0        0        0      617 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/resize.py
--rw-rw-rw-   0        0        0     2810 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/rotatecrop.py
--rw-rw-rw-   0        0        0    54603 2023-07-06 13:52:55.000000 guiqwt-4.4.0/guiqwt/tests/sift.py
--rw-rw-rw-   0        0        0     3757 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/simple_dialog.py
--rw-rw-rw-   0        0        0     9236 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/simple_window.py
--rw-rw-rw-   0        0        0     2895 2023-06-10 14:04:54.000000 guiqwt-4.4.0/guiqwt/tests/styles.py
--rw-rw-rw-   0        0        0     4809 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/syncplot.py
--rw-rw-rw-   0        0        0     1280 2023-06-10 14:05:01.000000 guiqwt-4.4.0/guiqwt/tests/test_line.py
--rw-rw-rw-   0        0        0     5352 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/transform.py
--rw-rw-rw-   0        0        0    88336 2023-06-10 14:03:47.000000 guiqwt-4.4.0/guiqwt/tools.py
--rw-rw-rw-   0        0        0      749 2021-12-11 14:47:03.000000 guiqwt-4.4.0/guiqwt/transitional.py
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.632626 guiqwt-4.4.0/guiqwt/widgets/
--rw-rw-rw-   0        0        0      578 2019-10-08 16:03:22.000000 guiqwt-4.4.0/guiqwt/widgets/__init__.py
--rw-rw-rw-   0        0        0     8406 2021-12-11 14:47:03.000000 guiqwt-4.4.0/guiqwt/widgets/base.py
--rw-rw-rw-   0        0        0    24376 2023-06-10 14:03:47.000000 guiqwt-4.4.0/guiqwt/widgets/fit.py
--rw-rw-rw-   0        0        0     5169 2022-08-01 14:49:33.000000 guiqwt-4.4.0/guiqwt/widgets/fliprotate.py
--rw-rw-rw-   0        0        0     5064 2021-12-19 10:53:14.000000 guiqwt-4.4.0/guiqwt/widgets/resizedialog.py
--rw-rw-rw-   0        0        0     4550 2021-12-11 14:47:04.000000 guiqwt-4.4.0/guiqwt/widgets/rotatecrop.py
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.127963 guiqwt-4.4.0/guiqwt.egg-info/
--rw-rw-rw-   0        0        0     2640 2023-07-06 17:58:20.000000 guiqwt-4.4.0/guiqwt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8112 2023-07-06 17:58:20.000000 guiqwt-4.4.0/guiqwt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 17:58:20.000000 guiqwt-4.4.0/guiqwt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-07-06 17:58:20.000000 guiqwt-4.4.0/guiqwt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      111 2023-07-06 17:58:20.000000 guiqwt-4.4.0/guiqwt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 17:58:20.000000 guiqwt-4.4.0/guiqwt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2022-08-01 14:49:33.000000 guiqwt-4.4.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.636625 guiqwt-4.4.0/qtdesigner/
--rw-rw-rw-   0        0        0      446 2019-10-08 16:03:22.000000 guiqwt-4.4.0/qtdesigner/imageplotplugin.py
--rw-rw-rw-   0        0        0      435 2019-10-08 16:03:22.000000 guiqwt-4.4.0/qtdesigner/plotplugin.py
--rw-rw-rw-   0        0        0       42 2023-07-06 17:58:21.663087 guiqwt-4.4.0/setup.cfg
--rw-rw-rw-   0        0        0     9569 2023-07-06 13:46:26.000000 guiqwt-4.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.642637 guiqwt-4.4.0/sift/
--rw-rw-rw-   0        0        0     1136 2023-07-06 13:57:01.000000 guiqwt-4.4.0/sift/create_exe.py
--rw-rw-rw-   0        0        0   100952 2019-10-08 16:03:22.000000 guiqwt-4.4.0/sift/sift.ico
--rw-rw-rw-   0        0        0       64 2019-10-08 16:03:22.000000 guiqwt-4.4.0/sift/sift.pyw
-drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.663087 guiqwt-4.4.0/src/
--rw-rw-rw-   0        0        0     4647 2019-10-08 16:03:22.000000 guiqwt-4.4.0/src/arrays.hpp
--rw-rw-rw-   0        0        0      681 2019-10-08 16:03:22.000000 guiqwt-4.4.0/src/debug.hpp
--rw-rw-rw-   0        0        0   298411 2023-07-06 17:58:03.000000 guiqwt-4.4.0/src/histogram2d.c
--rw-rw-rw-   0        0        0     3434 2019-10-08 16:03:22.000000 guiqwt-4.4.0/src/histogram2d.pyx
--rw-rw-rw-   0        0        0   235857 2023-07-06 17:58:03.000000 guiqwt-4.4.0/src/mandelbrot.c
--rw-rw-rw-   0        0        0     1168 2019-10-08 16:03:22.000000 guiqwt-4.4.0/src/mandelbrot.pyx
--rw-rw-rw-   0        0        0    11581 2021-02-06 17:38:23.000000 guiqwt-4.4.0/src/pcolor.cpp
--rw-rw-rw-   0        0        0     6127 2019-10-08 16:03:22.000000 guiqwt-4.4.0/src/points.hpp
--rw-rw-rw-   0        0        0    22897 2021-02-06 17:38:23.000000 guiqwt-4.4.0/src/scaler.cpp
--rw-rw-rw-   0        0        0     2376 2019-10-08 16:03:22.000000 guiqwt-4.4.0/src/scaler.hpp
--rw-rw-rw-   0        0        0     4137 2022-08-01 14:49:33.000000 guiqwt-4.4.0/src/traits.hpp
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.685046 guiqwt-4.4.1/
+-rw-rw-rw-   0        0        0    37687 2023-07-21 16:11:27.000000 guiqwt-4.4.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0    21603 2019-10-08 16:03:22.000000 guiqwt-4.4.1/Licence_CeCILL_V2-en.txt
+-rw-rw-rw-   0        0        0      451 2021-02-06 17:38:23.000000 guiqwt-4.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2663 2023-07-21 16:19:09.685046 guiqwt-4.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2516 2022-08-01 14:49:33.000000 guiqwt-4.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.205038 guiqwt-4.4.1/doc/
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.207036 guiqwt-4.4.1/doc/_static/
+-rw-rw-rw-   0        0        0     7886 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/_static/favicon.ico
+-rw-rw-rw-   0        0        0     7119 2021-12-19 10:52:19.000000 guiqwt-4.4.1/doc/conf.py
+-rw-rw-rw-   0        0        0      512 2021-12-19 10:39:43.000000 guiqwt-4.4.1/doc/development.rst
+-rw-rw-rw-   0        0        0     1942 2023-07-06 13:56:54.000000 guiqwt-4.4.1/doc/disthelpers.rst
+-rw-rw-rw-   0        0        0     2648 2023-07-06 17:17:16.000000 guiqwt-4.4.1/doc/examples.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.216038 guiqwt-4.4.1/doc/images/
+-rw-rw-rw-   0        0        0    32373 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/images/curve_widgets.png
+-rw-rw-rw-   0        0        0     3360 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/guiqwt.png
+-rw-rw-rw-   0        0        0    49787 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/images/image_widgets.png
+-rw-rw-rw-   0        0        0    28528 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/my_plot_manager.png
+-rw-rw-rw-   0        0        0   142571 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/panorama.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.272039 guiqwt-4.4.1/doc/images/screenshots/
+-rw-rw-rw-   0        0        0    33973 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/__init__.png
+-rw-rw-rw-   0        0        0    32219 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/computations.png
+-rw-rw-rw-   0        0        0   103911 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/contrast.png
+-rw-rw-rw-   0        0        0   123005 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/cross_section.png
+-rw-rw-rw-   0        0        0   123510 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/cross_section2.png
+-rw-rw-rw-   0        0        0    68152 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/images/screenshots/dotarraydemo.png
+-rw-rw-rw-   0        0        0    52268 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/fit.png
+-rw-rw-rw-   0        0        0    33435 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/get_point.png
+-rw-rw-rw-   0        0        0    70160 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/hist2d.png
+-rw-rw-rw-   0        0        0   146225 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/image_plot_tools.png
+-rw-rw-rw-   0        0        0   114920 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/imagefilter.png
+-rw-rw-rw-   0        0        0    73527 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/imagesuperp.png
+-rw-rw-rw-   0        0        0   187178 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/imagexy.png
+-rw-rw-rw-   0        0        0   100238 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/manager.png
+-rw-rw-rw-   0        0        0   123059 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/mandelbrot.png
+-rw-rw-rw-   0        0        0    49104 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/pcolor.png
+-rw-rw-rw-   0        0        0    80158 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/plot.png
+-rw-rw-rw-   0        0        0    66602 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/sift1.png
+-rw-rw-rw-   0        0        0   139606 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/sift2.png
+-rw-rw-rw-   0        0        0    94356 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/sift3.png
+-rw-rw-rw-   0        0        0    47500 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/simple_dialog.png
+-rw-rw-rw-   0        0        0    76231 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/simple_window.png
+-rw-rw-rw-   0        0        0   391598 2019-10-08 16:03:22.000000 guiqwt-4.4.1/doc/images/screenshots/transform.png
+-rw-rw-rw-   0        0        0      824 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/index.rst
+-rw-rw-rw-   0        0        0     1503 2023-07-06 13:43:56.000000 guiqwt-4.4.1/doc/installation.rst
+-rw-rw-rw-   0        0        0     1360 2021-12-19 10:56:36.000000 guiqwt-4.4.1/doc/migrating_from_v2_to_v3.rst
+-rw-rw-rw-   0        0        0     5960 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/overview.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.303038 guiqwt-4.4.1/doc/reference/
+-rw-rw-rw-   0        0        0       36 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/annotations.rst
+-rw-rw-rw-   0        0        0       33 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/baseplot.rst
+-rw-rw-rw-   0        0        0       32 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/builder.rst
+-rw-rw-rw-   0        0        0       38 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/cross_section.rst
+-rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/curve.rst
+-rw-rw-rw-   0        0        0       34 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/histogram.rst
+-rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/image.rst
+-rw-rw-rw-   0        0        0      345 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/index.rst
+-rw-rw-rw-   0        0        0       27 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/io.rst
+-rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/label.rst
+-rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/panels.rst
+-rw-rw-rw-   0        0        0       29 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/plot.rst
+-rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/pyplot.rst
+-rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/shapes.rst
+-rw-rw-rw-   0        0        0       32 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/signals.rst
+-rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/styles.rst
+-rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/tools.rst
+-rw-rw-rw-   0        0        0       36 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/widgets_fit.rst
+-rw-rw-rw-   0        0        0       45 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/widgets_resizedialog.rst
+-rw-rw-rw-   0        0        0       43 2021-02-06 17:38:23.000000 guiqwt-4.4.1/doc/reference/widgets_rotatecrop.rst
+-rw-rw-rw-   0        0        0      903 2023-06-10 14:03:47.000000 guiqwt-4.4.1/doc/sift.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.352040 guiqwt-4.4.1/guiqwt/
+-rw-rw-rw-   0        0        0    26398 2023-07-19 09:59:53.000000 guiqwt-4.4.1/guiqwt/__init__.py
+-rw-rw-rw-   0        0        0   421487 2021-12-11 14:47:07.000000 guiqwt-4.4.1/guiqwt/_cm.py
+-rw-rw-rw-   0        0        0    24601 2023-07-06 13:47:44.000000 guiqwt-4.4.1/guiqwt/annotations.py
+-rw-rw-rw-   0        0        0    34494 2023-07-19 12:25:36.000000 guiqwt-4.4.1/guiqwt/baseplot.py
+-rw-rw-rw-   0        0        0    53108 2023-06-04 08:46:35.000000 guiqwt-4.4.1/guiqwt/builder.py
+-rw-rw-rw-   0        0        0     3798 2021-03-13 15:31:59.000000 guiqwt-4.4.1/guiqwt/colormap.py
+-rw-rw-rw-   0        0        0    33453 2023-05-14 09:35:27.000000 guiqwt-4.4.1/guiqwt/config.py
+-rw-rw-rw-   0        0        0    36835 2023-07-06 13:48:38.000000 guiqwt-4.4.1/guiqwt/cross_section.py
+-rw-rw-rw-   0        0        0    65731 2023-07-06 13:49:01.000000 guiqwt-4.4.1/guiqwt/curve.py
+-rw-rw-rw-   0        0        0     2189 2021-12-19 10:50:52.000000 guiqwt-4.4.1/guiqwt/debug.py
+-rw-rw-rw-   0        0        0    25456 2022-08-01 14:49:33.000000 guiqwt-4.4.1/guiqwt/events.py
+-rw-rw-rw-   0        0        0     3003 2021-12-11 14:46:59.000000 guiqwt-4.4.1/guiqwt/geometry.py
+-rw-rw-rw-   0        0        0    20183 2023-07-06 13:49:23.000000 guiqwt-4.4.1/guiqwt/histogram.py
+-rw-rw-rw-   0        0        0   103756 2023-07-06 13:54:21.000000 guiqwt-4.4.1/guiqwt/image.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.418041 guiqwt-4.4.1/guiqwt/images/
+-rw-rw-rw-   0        0        0      827 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/arrow_down.png
+-rw-rw-rw-   0        0        0      828 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/arrow_up.png
+-rw-rw-rw-   0        0        0     1095 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/autorefresh.png
+-rw-rw-rw-   0        0        0      739 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/axes.png
+-rw-rw-rw-   0        0        0      593 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/center.png
+-rw-rw-rw-   0        0        0      562 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/contrast.png
+-rw-rw-rw-   0        0        0     1227 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/copytoclipboard.png
+-rw-rw-rw-   0        0        0      953 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/csapplylut.png
+-rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/csautoscale.png
+-rw-rw-rw-   0        0        0      594 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/csection.png
+-rw-rw-rw-   0        0        0      558 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/csection_a.png
+-rw-rw-rw-   0        0        0      959 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/csection_oblique.png
+-rw-rw-rw-   0        0        0      408 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/csperimage.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.423044 guiqwt-4.4.1/guiqwt/images/curvestyles/
+-rw-rw-rw-   0        0        0      369 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/curvestyles/dots.png
+-rw-rw-rw-   0        0        0      412 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/curvestyles/lines.png
+-rw-rw-rw-   0        0        0      384 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/curvestyles/steps.png
+-rw-rw-rw-   0        0        0      435 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/curvestyles/sticks.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.428043 guiqwt-4.4.1/guiqwt/images/curvetypes/
+-rw-rw-rw-   0        0        0      570 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/curvetypes/xfy.png
+-rw-rw-rw-   0        0        0      570 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/curvetypes/yfx.png
+-rw-rw-rw-   0        0        0      430 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/eliminate_outliers.png
+-rw-rw-rw-   0        0        0      882 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/eraser.png
+-rw-rw-rw-   0        0        0     1108 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/export.png
+-rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/font.png
+-rw-rw-rw-   0        0        0      432 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/full_range.png
+-rw-rw-rw-   0        0        0     1112 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/funct.png
+-rw-rw-rw-   0        0        0    15224 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/guiqwt.svg
+-rw-rw-rw-   0        0        0      399 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/hcursor.png
+-rw-rw-rw-   0        0        0      660 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/hflip.png
+-rw-rw-rw-   0        0        0     1041 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/imagestats.png
+-rw-rw-rw-   0        0        0      684 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/item_list.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.441042 guiqwt-4.4.1/guiqwt/images/items/
+-rw-rw-rw-   0        0        0      877 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/items/annotation.png
+-rw-rw-rw-   0        0        0      551 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/items/curve.png
+-rw-rw-rw-   0        0        0      419 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/items/errorbar.png
+-rw-rw-rw-   0        0        0      368 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/items/grid.png
+-rw-rw-rw-   0        0        0      387 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/items/histogram.png
+-rw-rw-rw-   0        0        0     1104 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/items/histogram2d.png
+-rw-rw-rw-   0        0        0     1077 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/items/image.png
+-rw-rw-rw-   0        0        0      742 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/items/label.png
+-rw-rw-rw-   0        0        0      564 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/items/legend.png
+-rw-rw-rw-   0        0        0     2267 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/magnifier.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.459051 guiqwt-4.4.1/guiqwt/images/markers/
+-rw-rw-rw-   0        0        0      337 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markers/cross.png
+-rw-rw-rw-   0        0        0      420 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markers/diamond.png
+-rw-rw-rw-   0        0        0      468 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markers/ellipse.png
+-rw-rw-rw-   0        0        0      484 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markers/hexagon.png
+-rw-rw-rw-   0        0        0      331 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markers/point.png
+-rw-rw-rw-   0        0        0      363 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markers/square.png
+-rw-rw-rw-   0        0        0      357 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markers/star.png
+-rw-rw-rw-   0        0        0      449 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markers/triangle_d.png
+-rw-rw-rw-   0        0        0      445 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markers/triangle_l.png
+-rw-rw-rw-   0        0        0      438 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markers/triangle_r.png
+-rw-rw-rw-   0        0        0      449 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markers/triangle_u.png
+-rw-rw-rw-   0        0        0      349 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markers/xcross.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.464043 guiqwt-4.4.1/guiqwt/images/markerstyles/
+-rw-rw-rw-   0        0        0      343 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markerstyles/cross_marker.png
+-rw-rw-rw-   0        0        0      331 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markerstyles/horiz_marker.png
+-rw-rw-rw-   0        0        0      333 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/markerstyles/vert_marker.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.470043 guiqwt-4.4.1/guiqwt/images/mask/
+-rw-rw-rw-   0        0        0      619 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/mask/mask_circle.png
+-rw-rw-rw-   0        0        0      623 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/mask/mask_circle_outside.png
+-rw-rw-rw-   0        0        0      445 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/mask/mask_rectangle.png
+-rw-rw-rw-   0        0        0      446 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/mask/mask_rectangle_outside.png
+-rw-rw-rw-   0        0        0      411 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/mask/mask_tool.png
+-rw-rw-rw-   0        0        0      339 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/move.png
+-rw-rw-rw-   0        0        0      644 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/on_curve.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.495044 guiqwt-4.4.1/guiqwt/images/patterns/
+-rw-rw-rw-   0        0        0      325 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/bdiagpattern.png
+-rw-rw-rw-   0        0        0      311 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/crosspattern.png
+-rw-rw-rw-   0        0        0      303 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/dense1pattern.png
+-rw-rw-rw-   0        0        0      305 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/dense2pattern.png
+-rw-rw-rw-   0        0        0      309 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/dense3pattern.png
+-rw-rw-rw-   0        0        0      300 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/dense4pattern.png
+-rw-rw-rw-   0        0        0      307 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/dense5pattern.png
+-rw-rw-rw-   0        0        0      311 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/dense6pattern.png
+-rw-rw-rw-   0        0        0      308 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/dense7pattern.png
+-rw-rw-rw-   0        0        0      324 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/diagcrosspattern.png
+-rw-rw-rw-   0        0        0      330 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/fdiagpattern.png
+-rw-rw-rw-   0        0        0      306 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/horpattern.png
+-rw-rw-rw-   0        0        0      299 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/nobrush.png
+-rw-rw-rw-   0        0        0      296 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/solidpattern.png
+-rw-rw-rw-   0        0        0      304 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/patterns/verpattern.png
+-rw-rw-rw-   0        0        0      442 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/point_selection.png
+-rw-rw-rw-   0        0        0      913 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/print.png
+-rw-rw-rw-   0        0        0      967 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/refresh.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.501042 guiqwt-4.4.1/guiqwt/images/scales/
+-rw-rw-rw-   0        0        0      395 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/scales/lin_lin.png
+-rw-rw-rw-   0        0        0      402 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/scales/lin_log.png
+-rw-rw-rw-   0        0        0      403 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/scales/log_lin.png
+-rw-rw-rw-   0        0        0      407 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/scales/log_log.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.516043 guiqwt-4.4.1/guiqwt/images/shapes/
+-rw-rw-rw-   0        0        0      777 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/shapes/circle.png
+-rw-rw-rw-   0        0        0      794 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/shapes/ellipse_shape.png
+-rw-rw-rw-   0        0        0      552 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/shapes/freeform.png
+-rw-rw-rw-   0        0        0      568 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/shapes/gtaxes.png
+-rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/shapes/marker.png
+-rw-rw-rw-   0        0        0      898 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/shapes/oblique_rectangle.png
+-rw-rw-rw-   0        0        0      366 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/shapes/point_shape.png
+-rw-rw-rw-   0        0        0      479 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/shapes/polyline.png
+-rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/shapes/rectangle.png
+-rw-rw-rw-   0        0        0      467 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/shapes/segment.png
+-rw-rw-rw-   0        0        0    14258 2019-10-08 16:03:22.000000 guiqwt-4.4.1/guiqwt/images/sift.svg
+-rw-rw-rw-   0        0        0     1340 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/snapshot.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.525045 guiqwt-4.4.1/guiqwt/images/styles/
+-rw-rw-rw-   0        0        0      333 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/styles/dash.png
+-rw-rw-rw-   0        0        0      338 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/styles/dashdot.png
+-rw-rw-rw-   0        0        0      332 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/styles/dashdotdot.png
+-rw-rw-rw-   0        0        0      328 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/styles/dot.png
+-rw-rw-rw-   0        0        0      328 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/styles/solid.png
+-rw-rw-rw-   0        0        0      401 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/trash.png
+-rw-rw-rw-   0        0        0      407 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/vcursor.png
+-rw-rw-rw-   0        0        0      658 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/vflip.png
+-rw-rw-rw-   0        0        0      375 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/xcursor.png
+-rw-rw-rw-   0        0        0      417 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/images/xrange.png
+-rw-rw-rw-   0        0        0     9529 2021-12-11 14:46:59.000000 guiqwt-4.4.1/guiqwt/interfaces.py
+-rw-rw-rw-   0        0        0    21856 2023-07-19 09:59:11.000000 guiqwt-4.4.1/guiqwt/io.py
+-rw-rw-rw-   0        0        0    20156 2023-07-06 13:50:04.000000 guiqwt-4.4.1/guiqwt/label.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.530044 guiqwt-4.4.1/guiqwt/locale/
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.173035 guiqwt-4.4.1/guiqwt/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.538055 guiqwt-4.4.1/guiqwt/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    30153 2023-02-20 09:04:37.000000 guiqwt-4.4.1/guiqwt/locale/fr/LC_MESSAGES/guiqwt.mo
+-rw-rw-rw-   0        0        0    57708 2022-08-01 14:49:33.000000 guiqwt-4.4.1/guiqwt/locale/fr/LC_MESSAGES/guiqwt.po
+-rw-rw-rw-   0        0        0    44618 2023-02-20 09:03:54.000000 guiqwt-4.4.1/guiqwt/locale/guiqwt.pot
+-rw-rw-rw-   0        0        0     3242 2023-07-06 13:50:35.000000 guiqwt-4.4.1/guiqwt/panels.py
+-rw-rw-rw-   0        0        0    48599 2023-07-06 13:50:47.000000 guiqwt-4.4.1/guiqwt/plot.py
+-rw-rw-rw-   0        0        0    19841 2023-02-19 15:02:16.000000 guiqwt-4.4.1/guiqwt/pyplot.py
+-rw-rw-rw-   0        0        0     3361 2021-12-19 11:05:20.000000 guiqwt-4.4.1/guiqwt/qtdesigner.py
+-rw-rw-rw-   0        0        0     5824 2022-04-08 12:35:06.000000 guiqwt-4.4.1/guiqwt/qthelpers.py
+-rw-rw-rw-   0        0        0     1852 2021-12-11 14:47:00.000000 guiqwt-4.4.1/guiqwt/scaler.py
+-rw-rw-rw-   0        0        0    54040 2023-07-06 13:50:11.000000 guiqwt-4.4.1/guiqwt/shapes.py
+-rw-rw-rw-   0        0        0     4530 2023-05-13 07:53:17.000000 guiqwt-4.4.1/guiqwt/signals.py
+-rw-rw-rw-   0        0        0    62787 2022-08-01 14:49:33.000000 guiqwt-4.4.1/guiqwt/styles.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.640047 guiqwt-4.4.1/guiqwt/tests/
+-rw-rw-rw-   0        0        0      440 2021-12-11 14:47:02.000000 guiqwt-4.4.1/guiqwt/tests/__init__.py
+-rw-rw-rw-   0        0        0     4305 2023-06-10 14:04:27.000000 guiqwt-4.4.1/guiqwt/tests/benchmarks.py
+-rw-rw-rw-   0        0        0    39666 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/tests/brain.png
+-rw-rw-rw-   0        0        0    35354 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/tests/brain_cylinder.png
+-rw-rw-rw-   0        0        0     1374 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/computations.py
+-rw-rw-rw-   0        0        0     1088 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/contrast.py
+-rw-rw-rw-   0        0        0     1164 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/cross_section.py
+-rw-rw-rw-   0        0        0     2021 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/cross_section_oblique.py
+-rw-rw-rw-   0        0        0     1144 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/cursors.py
+-rw-rw-rw-   0        0        0     1742 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/customize_shape_tool.py
+-rw-rw-rw-   0        0        0      977 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/dicom_image.py
+-rw-rw-rw-   0        0        0     6069 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/dotarraydemo.py
+-rw-rw-rw-   0        0        0     2839 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/filtertest1.py
+-rw-rw-rw-   0        0        0     3590 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/filtertest2.py
+-rw-rw-rw-   0        0        0      807 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/fit.py
+-rw-rw-rw-   0        0        0     1153 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/fliprotate.py
+-rw-rw-rw-   0        0        0      401 2023-06-10 14:04:31.000000 guiqwt-4.4.1/guiqwt/tests/fontparam.py
+-rw-rw-rw-   0        0        0     1514 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/get_point.py
+-rw-rw-rw-   0        0        0     1517 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/get_segment.py
+-rw-rw-rw-   0        0        0      801 2023-06-10 14:04:35.000000 guiqwt-4.4.1/guiqwt/tests/highprecisionxy.py
+-rw-rw-rw-   0        0        0     1208 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/hist2d.py
+-rw-rw-rw-   0        0        0     1357 2021-12-11 14:47:02.000000 guiqwt-4.4.1/guiqwt/tests/hist2d_func.py
+-rw-rw-rw-   0        0        0      694 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/histogram.py
+-rw-rw-rw-   0        0        0     3046 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/image.py
+-rw-rw-rw-   0        0        0     1887 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/image_coords.py
+-rw-rw-rw-   0        0        0     1416 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/image_masked.py
+-rw-rw-rw-   0        0        0     1866 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/image_plot_tools.py
+-rw-rw-rw-   0        0        0      954 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/image_rgb.py
+-rw-rw-rw-   0        0        0     1635 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/imagefilter.py
+-rw-rw-rw-   0        0        0     1605 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/imagesuperp.py
+-rw-rw-rw-   0        0        0     1680 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/imagexy.py
+-rw-rw-rw-   0        0        0      875 2023-07-19 09:59:21.000000 guiqwt-4.4.1/guiqwt/tests/loadsaveitems_hdf5.py
+-rw-rw-rw-   0        0        0     1274 2023-07-19 09:59:25.000000 guiqwt-4.4.1/guiqwt/tests/loadsaveitems_json.py
+-rw-rw-rw-   0        0        0     3881 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/loadsaveitems_pickle.py
+-rw-rw-rw-   0        0        0     2710 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/loadtest.py
+-rw-rw-rw-   0        0        0     2402 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/manager.py
+-rw-rw-rw-   0        0        0     2617 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/mandelbrot.py
+-rw-rw-rw-   0        0        0   525620 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/tests/mr-brain.dcm
+-rw-rw-rw-   0        0        0     2660 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/pcolor.py
+-rw-rw-rw-   0        0        0     1802 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/plot.py
+-rw-rw-rw-   0        0        0      908 2023-06-10 14:04:39.000000 guiqwt-4.4.1/guiqwt/tests/plot_log.py
+-rw-rw-rw-   0        0        0    14151 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/plot_timecurve.py
+-rw-rw-rw-   0        0        0      785 2023-06-10 14:04:43.000000 guiqwt-4.4.1/guiqwt/tests/plot_yreverse.py
+-rw-rw-rw-   0        0        0      587 2023-06-10 14:04:47.000000 guiqwt-4.4.1/guiqwt/tests/png_test.py
+-rw-rw-rw-   0        0        0     2195 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/polygons.py
+-rw-rw-rw-   0        0        0     1887 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/pyplot.py
+-rw-rw-rw-   0        0        0     1032 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/qtdesigner.py
+-rw-rw-rw-   0        0        0      993 2021-02-06 17:38:23.000000 guiqwt-4.4.1/guiqwt/tests/qtdesigner.ui
+-rw-rw-rw-   0        0        0      617 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/resize.py
+-rw-rw-rw-   0        0        0     2810 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/rotatecrop.py
+-rw-rw-rw-   0        0        0    54603 2023-07-06 13:52:55.000000 guiqwt-4.4.1/guiqwt/tests/sift.py
+-rw-rw-rw-   0        0        0     3757 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/simple_dialog.py
+-rw-rw-rw-   0        0        0     9236 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/simple_window.py
+-rw-rw-rw-   0        0        0     2895 2023-06-10 14:04:54.000000 guiqwt-4.4.1/guiqwt/tests/styles.py
+-rw-rw-rw-   0        0        0     4809 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/syncplot.py
+-rw-rw-rw-   0        0        0     1280 2023-06-10 14:05:01.000000 guiqwt-4.4.1/guiqwt/tests/test_line.py
+-rw-rw-rw-   0        0        0     5352 2023-06-10 14:05:30.000000 guiqwt-4.4.1/guiqwt/tests/transform.py
+-rw-rw-rw-   0        0        0    88336 2023-06-10 14:03:47.000000 guiqwt-4.4.1/guiqwt/tools.py
+-rw-rw-rw-   0        0        0      749 2021-12-11 14:47:03.000000 guiqwt-4.4.1/guiqwt/transitional.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.650049 guiqwt-4.4.1/guiqwt/widgets/
+-rw-rw-rw-   0        0        0      578 2019-10-08 16:03:22.000000 guiqwt-4.4.1/guiqwt/widgets/__init__.py
+-rw-rw-rw-   0        0        0     8406 2021-12-11 14:47:03.000000 guiqwt-4.4.1/guiqwt/widgets/base.py
+-rw-rw-rw-   0        0        0    24376 2023-06-10 14:03:47.000000 guiqwt-4.4.1/guiqwt/widgets/fit.py
+-rw-rw-rw-   0        0        0     5169 2022-08-01 14:49:33.000000 guiqwt-4.4.1/guiqwt/widgets/fliprotate.py
+-rw-rw-rw-   0        0        0     5064 2021-12-19 10:53:14.000000 guiqwt-4.4.1/guiqwt/widgets/resizedialog.py
+-rw-rw-rw-   0        0        0     4550 2021-12-11 14:47:04.000000 guiqwt-4.4.1/guiqwt/widgets/rotatecrop.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.361039 guiqwt-4.4.1/guiqwt.egg-info/
+-rw-rw-rw-   0        0        0     2663 2023-07-21 16:19:08.000000 guiqwt-4.4.1/guiqwt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8112 2023-07-21 16:19:08.000000 guiqwt-4.4.1/guiqwt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 16:19:08.000000 guiqwt-4.4.1/guiqwt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-07-21 16:19:08.000000 guiqwt-4.4.1/guiqwt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      113 2023-07-21 16:19:08.000000 guiqwt-4.4.1/guiqwt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 16:19:08.000000 guiqwt-4.4.1/guiqwt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2022-08-01 14:49:33.000000 guiqwt-4.4.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.653047 guiqwt-4.4.1/qtdesigner/
+-rw-rw-rw-   0        0        0      446 2019-10-08 16:03:22.000000 guiqwt-4.4.1/qtdesigner/imageplotplugin.py
+-rw-rw-rw-   0        0        0      435 2019-10-08 16:03:22.000000 guiqwt-4.4.1/qtdesigner/plotplugin.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 16:19:09.686048 guiqwt-4.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     9571 2023-07-19 10:01:01.000000 guiqwt-4.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.660048 guiqwt-4.4.1/sift/
+-rw-rw-rw-   0        0        0     1136 2023-07-06 13:57:01.000000 guiqwt-4.4.1/sift/create_exe.py
+-rw-rw-rw-   0        0        0   100952 2019-10-08 16:03:22.000000 guiqwt-4.4.1/sift/sift.ico
+-rw-rw-rw-   0        0        0       64 2019-10-08 16:03:22.000000 guiqwt-4.4.1/sift/sift.pyw
+drwxrwxrwx   0        0        0        0 2023-07-21 16:19:09.683047 guiqwt-4.4.1/src/
+-rw-rw-rw-   0        0        0     4647 2019-10-08 16:03:22.000000 guiqwt-4.4.1/src/arrays.hpp
+-rw-rw-rw-   0        0        0      681 2019-10-08 16:03:22.000000 guiqwt-4.4.1/src/debug.hpp
+-rw-rw-rw-   0        0        0   295116 2023-07-21 16:18:50.000000 guiqwt-4.4.1/src/histogram2d.c
+-rw-rw-rw-   0        0        0     3434 2019-10-08 16:03:22.000000 guiqwt-4.4.1/src/histogram2d.pyx
+-rw-rw-rw-   0        0        0   232562 2023-07-21 16:18:50.000000 guiqwt-4.4.1/src/mandelbrot.c
+-rw-rw-rw-   0        0        0     1168 2019-10-08 16:03:22.000000 guiqwt-4.4.1/src/mandelbrot.pyx
+-rw-rw-rw-   0        0        0    11581 2021-02-06 17:38:23.000000 guiqwt-4.4.1/src/pcolor.cpp
+-rw-rw-rw-   0        0        0     6127 2019-10-08 16:03:22.000000 guiqwt-4.4.1/src/points.hpp
+-rw-rw-rw-   0        0        0    22897 2021-02-06 17:38:23.000000 guiqwt-4.4.1/src/scaler.cpp
+-rw-rw-rw-   0        0        0     2376 2019-10-08 16:03:22.000000 guiqwt-4.4.1/src/scaler.hpp
+-rw-rw-rw-   0        0        0     4137 2022-08-01 14:49:33.000000 guiqwt-4.4.1/src/traits.hpp
```

### Comparing `guiqwt-4.4.0/CHANGELOG.md` & `guiqwt-4.4.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # guiqwt Releases #
 
+## Version 4.4.1 ##
+
+Changes:
+
+* guiqwt now requires guidata >=v3.0.1 (API compatibility issue with guidata v3.0.0)
+
 ## Version 4.4.0 ##
 
 Changes:
 
 * guiqwt now requires guidata >=v3.0.
 * tests/syncplot: added image synchronization test
```

### Comparing `guiqwt-4.4.0/Licence_CeCILL_V2-en.txt` & `guiqwt-4.4.1/Licence_CeCILL_V2-en.txt`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/PKG-INFO` & `guiqwt-4.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: guiqwt
-Version: 4.4.0
+Version: 4.4.1
 Summary: guiqwt is a set of tools for curve and image plotting (extension to PythonQwt)
 Home-page: https://github.com/PierreRaybaut/guiqwt
 Author: Pierre Raybaut
 Author-email: pierre.raybaut@gmail.com
 License: CeCILL V2
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
@@ -64,7 +65,9 @@
 .. _NumPy: https://pypi.python.org/pypi/NumPy
 .. _SciPy: https://pypi.python.org/pypi/SciPy
 .. _Pillow: https://pypi.python.org/pypi/Pillow
 
 See the `README`_ and `documentation`_ for more details.
 
 .. _README: https://github.com/PierreRaybaut/guiqwt/blob/master/README.md
+
+
```

### Comparing `guiqwt-4.4.0/README.md` & `guiqwt-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/_static/favicon.ico` & `guiqwt-4.4.1/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/conf.py` & `guiqwt-4.4.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/development.rst` & `guiqwt-4.4.1/doc/development.rst`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/disthelpers.rst` & `guiqwt-4.4.1/doc/disthelpers.rst`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/examples.rst` & `guiqwt-4.4.1/doc/examples.rst`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/curve_widgets.png` & `guiqwt-4.4.1/doc/images/curve_widgets.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/guiqwt.png` & `guiqwt-4.4.1/doc/images/guiqwt.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/image_widgets.png` & `guiqwt-4.4.1/doc/images/image_widgets.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/my_plot_manager.png` & `guiqwt-4.4.1/doc/images/my_plot_manager.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/panorama.png` & `guiqwt-4.4.1/doc/images/panorama.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/__init__.png` & `guiqwt-4.4.1/doc/images/screenshots/__init__.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/computations.png` & `guiqwt-4.4.1/doc/images/screenshots/computations.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/contrast.png` & `guiqwt-4.4.1/doc/images/screenshots/contrast.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/cross_section.png` & `guiqwt-4.4.1/doc/images/screenshots/cross_section.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/cross_section2.png` & `guiqwt-4.4.1/doc/images/screenshots/cross_section2.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/dotarraydemo.png` & `guiqwt-4.4.1/doc/images/screenshots/dotarraydemo.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/fit.png` & `guiqwt-4.4.1/doc/images/screenshots/fit.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/get_point.png` & `guiqwt-4.4.1/doc/images/screenshots/get_point.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/hist2d.png` & `guiqwt-4.4.1/doc/images/screenshots/hist2d.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/image_plot_tools.png` & `guiqwt-4.4.1/doc/images/screenshots/image_plot_tools.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/imagefilter.png` & `guiqwt-4.4.1/doc/images/screenshots/imagefilter.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/imagesuperp.png` & `guiqwt-4.4.1/doc/images/screenshots/imagesuperp.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/imagexy.png` & `guiqwt-4.4.1/doc/images/screenshots/imagexy.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/manager.png` & `guiqwt-4.4.1/doc/images/screenshots/manager.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/mandelbrot.png` & `guiqwt-4.4.1/doc/images/screenshots/mandelbrot.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/pcolor.png` & `guiqwt-4.4.1/doc/images/screenshots/pcolor.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/plot.png` & `guiqwt-4.4.1/doc/images/screenshots/plot.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/sift1.png` & `guiqwt-4.4.1/doc/images/screenshots/sift1.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/sift2.png` & `guiqwt-4.4.1/doc/images/screenshots/sift2.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/sift3.png` & `guiqwt-4.4.1/doc/images/screenshots/sift3.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/simple_dialog.png` & `guiqwt-4.4.1/doc/images/screenshots/simple_dialog.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/simple_window.png` & `guiqwt-4.4.1/doc/images/screenshots/simple_window.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/images/screenshots/transform.png` & `guiqwt-4.4.1/doc/images/screenshots/transform.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/index.rst` & `guiqwt-4.4.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/installation.rst` & `guiqwt-4.4.1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/migrating_from_v2_to_v3.rst` & `guiqwt-4.4.1/doc/migrating_from_v2_to_v3.rst`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/overview.rst` & `guiqwt-4.4.1/doc/overview.rst`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/doc/sift.rst` & `guiqwt-4.4.1/doc/sift.rst`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/__init__.py` & `guiqwt-4.4.1/guiqwt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 .. _PyPI: https://pypi.python.org/pypi/guiqwt
 .. _GitHub: https://github.com/PierreRaybaut/guiqwt
 .. _GoogleGroup: http://groups.google.fr/group/guidata_guiqwt
 """
 
 
-__version__ = "4.4.0"  # Update here *AND* in setup.py!
+__version__ = "4.4.1"  # Update here *AND* in setup.py!
 # (Until setup.py has been fully retrofitted, this manual sync is mandatory)
 
 
 def about(html=True, copyright_only=False):
     """Return text about this package"""
     import sys, os, os.path as osp, platform, guidata, guiqwt, qwt
     from guiqwt.config import _
```

### Comparing `guiqwt-4.4.0/guiqwt/_cm.py` & `guiqwt-4.4.1/guiqwt/_cm.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/annotations.py` & `guiqwt-4.4.1/guiqwt/annotations.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/baseplot.py` & `guiqwt-4.4.1/guiqwt/baseplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,30 +608,30 @@
         items = pickle.load(iofile)
         for item in items:
             self.add_item(item)
 
     def serialize(self, writer, selected=False):
         """
         Save (serializable) items to HDF5 file:
-            * writer: :py:class:`guidata.dataset.hdf5io.HDF5Writer` object
+            * writer: :py:class:`guidata.dataset.io.HDF5Writer` object
             * selected=False: if True, will save only selected items
 
         See also :py:meth:`guiqwt.baseplot.BasePlot.restore_items_from_hdf5`
         """
         if selected:
             items = self.get_selected_items()
         else:
             items = self.items[:]
         items = [item for item in items if ISerializableType in item.types()]
         io.save_items(writer, items)
 
     def deserialize(self, reader):
         """
         Restore items from HDF5 file:
-            * reader: :py:class:`guidata.dataset.hdf5io.HDF5Reader` object
+            * reader: :py:class:`guidata.dataset.io.HDF5Reader` object
 
         See also :py:meth:`guiqwt.baseplot.BasePlot.save_items_to_hdf5`
         """
         for item in io.load_items(reader):
             self.add_item(item)
 
     def set_items(self, *args):
```

### Comparing `guiqwt-4.4.0/guiqwt/builder.py` & `guiqwt-4.4.1/guiqwt/builder.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/colormap.py` & `guiqwt-4.4.1/guiqwt/colormap.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/config.py` & `guiqwt-4.4.1/guiqwt/config.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/cross_section.py` & `guiqwt-4.4.1/guiqwt/cross_section.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/curve.py` & `guiqwt-4.4.1/guiqwt/curve.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/debug.py` & `guiqwt-4.4.1/guiqwt/debug.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/events.py` & `guiqwt-4.4.1/guiqwt/events.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/geometry.py` & `guiqwt-4.4.1/guiqwt/geometry.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/histogram.py` & `guiqwt-4.4.1/guiqwt/histogram.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/image.py` & `guiqwt-4.4.1/guiqwt/image.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/arrow_down.png` & `guiqwt-4.4.1/guiqwt/images/arrow_down.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/arrow_up.png` & `guiqwt-4.4.1/guiqwt/images/arrow_up.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/autorefresh.png` & `guiqwt-4.4.1/guiqwt/images/autorefresh.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/axes.png` & `guiqwt-4.4.1/guiqwt/images/axes.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/center.png` & `guiqwt-4.4.1/guiqwt/images/center.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/contrast.png` & `guiqwt-4.4.1/guiqwt/images/contrast.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/copytoclipboard.png` & `guiqwt-4.4.1/guiqwt/images/copytoclipboard.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/csapplylut.png` & `guiqwt-4.4.1/guiqwt/images/csapplylut.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/csection.png` & `guiqwt-4.4.1/guiqwt/images/csection.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/csection_a.png` & `guiqwt-4.4.1/guiqwt/images/csection_a.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/csection_oblique.png` & `guiqwt-4.4.1/guiqwt/images/csection_oblique.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/curvetypes/xfy.png` & `guiqwt-4.4.1/guiqwt/images/curvetypes/xfy.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/curvetypes/yfx.png` & `guiqwt-4.4.1/guiqwt/images/curvetypes/yfx.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/eraser.png` & `guiqwt-4.4.1/guiqwt/images/eraser.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/export.png` & `guiqwt-4.4.1/guiqwt/images/export.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/funct.png` & `guiqwt-4.4.1/guiqwt/images/funct.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/guiqwt.svg` & `guiqwt-4.4.1/guiqwt/images/guiqwt.svg`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/hflip.png` & `guiqwt-4.4.1/guiqwt/images/hflip.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/imagestats.png` & `guiqwt-4.4.1/guiqwt/images/imagestats.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/item_list.png` & `guiqwt-4.4.1/guiqwt/images/item_list.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/items/annotation.png` & `guiqwt-4.4.1/guiqwt/images/items/annotation.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/items/curve.png` & `guiqwt-4.4.1/guiqwt/images/items/curve.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/items/histogram2d.png` & `guiqwt-4.4.1/guiqwt/images/items/histogram2d.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/items/image.png` & `guiqwt-4.4.1/guiqwt/images/items/image.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/items/label.png` & `guiqwt-4.4.1/guiqwt/images/items/label.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/items/legend.png` & `guiqwt-4.4.1/guiqwt/images/items/legend.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/magnifier.png` & `guiqwt-4.4.1/guiqwt/images/magnifier.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/mask/mask_circle.png` & `guiqwt-4.4.1/guiqwt/images/mask/mask_circle.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/mask/mask_circle_outside.png` & `guiqwt-4.4.1/guiqwt/images/mask/mask_circle_outside.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/on_curve.png` & `guiqwt-4.4.1/guiqwt/images/on_curve.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/print.png` & `guiqwt-4.4.1/guiqwt/images/print.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/refresh.png` & `guiqwt-4.4.1/guiqwt/images/refresh.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/shapes/circle.png` & `guiqwt-4.4.1/guiqwt/images/shapes/circle.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/shapes/ellipse_shape.png` & `guiqwt-4.4.1/guiqwt/images/shapes/ellipse_shape.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/shapes/freeform.png` & `guiqwt-4.4.1/guiqwt/images/shapes/freeform.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/shapes/gtaxes.png` & `guiqwt-4.4.1/guiqwt/images/shapes/gtaxes.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/shapes/oblique_rectangle.png` & `guiqwt-4.4.1/guiqwt/images/shapes/oblique_rectangle.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/sift.svg` & `guiqwt-4.4.1/guiqwt/images/sift.svg`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/snapshot.png` & `guiqwt-4.4.1/guiqwt/images/snapshot.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/images/vflip.png` & `guiqwt-4.4.1/guiqwt/images/vflip.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/interfaces.py` & `guiqwt-4.4.1/guiqwt/interfaces.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/io.py` & `guiqwt-4.4.1/guiqwt/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -606,15 +606,15 @@
         item = klass()
         item.deserialize(reader)
     return item
 
 
 def save_items(writer, items):
     """Save items to HDF5 file:
-    * writer: :py:class:`guidata.dataset.hdf5io.HDF5Writer` object
+    * writer: :py:class:`guidata.dataset.io.HDF5Writer` object
     * items: serializable plot items"""
     counts = {}
     names = []
 
     def _get_name(item):
         basename = item_name_from_object(item)
         count = counts[basename] = counts.setdefault(basename, 0) + 1
@@ -627,16 +627,16 @@
             item.serialize(writer)
     with writer.group("plot_items"):
         writer.write_sequence(names)
 
 
 def load_items(reader):
     """Load items from file (HDF5, JSON, ...):
-    * reader: :py:class:`guidata.dataset.hdf5io.HDF5Reader` or
-      :py:class:`guidata.dataset.jsonio.JSONReader` object"""
+    * reader: :py:class:`guidata.dataset.io.HDF5Reader` or
+      :py:class:`guidata.dataset.io.JSONReader` object"""
     with reader.group("plot_items"):
         names = reader.read_sequence()
     items = []
     for name in names:
         try:
             name_str = name.decode()
         except AttributeError:
```

### Comparing `guiqwt-4.4.0/guiqwt/label.py` & `guiqwt-4.4.1/guiqwt/label.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/locale/fr/LC_MESSAGES/guiqwt.mo` & `guiqwt-4.4.1/guiqwt/locale/fr/LC_MESSAGES/guiqwt.mo`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/locale/fr/LC_MESSAGES/guiqwt.po` & `guiqwt-4.4.1/guiqwt/locale/fr/LC_MESSAGES/guiqwt.po`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/locale/guiqwt.pot` & `guiqwt-4.4.1/guiqwt/locale/guiqwt.pot`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/panels.py` & `guiqwt-4.4.1/guiqwt/panels.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/plot.py` & `guiqwt-4.4.1/guiqwt/plot.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/pyplot.py` & `guiqwt-4.4.1/guiqwt/pyplot.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/qtdesigner.py` & `guiqwt-4.4.1/guiqwt/qtdesigner.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/qthelpers.py` & `guiqwt-4.4.1/guiqwt/qthelpers.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/scaler.py` & `guiqwt-4.4.1/guiqwt/scaler.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/shapes.py` & `guiqwt-4.4.1/guiqwt/shapes.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/signals.py` & `guiqwt-4.4.1/guiqwt/signals.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/styles.py` & `guiqwt-4.4.1/guiqwt/styles.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/benchmarks.py` & `guiqwt-4.4.1/guiqwt/tests/benchmarks.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/brain.png` & `guiqwt-4.4.1/guiqwt/tests/brain.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/brain_cylinder.png` & `guiqwt-4.4.1/guiqwt/tests/brain_cylinder.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/computations.py` & `guiqwt-4.4.1/guiqwt/tests/computations.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/contrast.py` & `guiqwt-4.4.1/guiqwt/tests/contrast.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/cross_section.py` & `guiqwt-4.4.1/guiqwt/tests/cross_section.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/cross_section_oblique.py` & `guiqwt-4.4.1/guiqwt/tests/cross_section_oblique.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/cursors.py` & `guiqwt-4.4.1/guiqwt/tests/cursors.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/customize_shape_tool.py` & `guiqwt-4.4.1/guiqwt/tests/customize_shape_tool.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/dicom_image.py` & `guiqwt-4.4.1/guiqwt/tests/dicom_image.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/dotarraydemo.py` & `guiqwt-4.4.1/guiqwt/tests/dotarraydemo.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/filtertest1.py` & `guiqwt-4.4.1/guiqwt/tests/filtertest1.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/filtertest2.py` & `guiqwt-4.4.1/guiqwt/tests/filtertest2.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/fit.py` & `guiqwt-4.4.1/guiqwt/tests/fit.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/fliprotate.py` & `guiqwt-4.4.1/guiqwt/tests/fliprotate.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/get_point.py` & `guiqwt-4.4.1/guiqwt/tests/get_point.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/get_segment.py` & `guiqwt-4.4.1/guiqwt/tests/get_segment.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/highprecisionxy.py` & `guiqwt-4.4.1/guiqwt/tests/highprecisionxy.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/hist2d.py` & `guiqwt-4.4.1/guiqwt/tests/hist2d.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/hist2d_func.py` & `guiqwt-4.4.1/guiqwt/tests/hist2d_func.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/histogram.py` & `guiqwt-4.4.1/guiqwt/tests/histogram.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/image.py` & `guiqwt-4.4.1/guiqwt/tests/image.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/image_coords.py` & `guiqwt-4.4.1/guiqwt/tests/image_coords.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/image_masked.py` & `guiqwt-4.4.1/guiqwt/tests/image_masked.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/image_plot_tools.py` & `guiqwt-4.4.1/guiqwt/tests/image_plot_tools.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/image_rgb.py` & `guiqwt-4.4.1/guiqwt/tests/image_rgb.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/imagefilter.py` & `guiqwt-4.4.1/guiqwt/tests/imagefilter.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/imagesuperp.py` & `guiqwt-4.4.1/guiqwt/tests/imagesuperp.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/imagexy.py` & `guiqwt-4.4.1/guiqwt/tests/imagexy.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/loadsaveitems_hdf5.py` & `guiqwt-4.4.1/guiqwt/tests/loadsaveitems_hdf5.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """Load/save items from/to HDF5 file"""
 
 # guitest: show
 
 # WARNING:
 # This script requires read/write permissions on current directory
 
-from guidata.dataset.hdf5io import HDF5Reader, HDF5Writer
+from guidata.dataset.io import HDF5Reader, HDF5Writer
 
 from guiqwt.tests.loadsaveitems_pickle import IOTest
 
 
 class HDF5Test(IOTest):
     FNAME = "loadsavecanvas.h5"
```

### Comparing `guiqwt-4.4.0/guiqwt/tests/loadsaveitems_json.py` & `guiqwt-4.4.1/guiqwt/tests/loadsaveitems_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 """
 
 import os.path as osp
 
 from guiqwt.tests.loadsaveitems_pickle import IOTest
 
-from guidata.dataset.jsonio import JSONReader, JSONWriter
+from guidata.dataset.io import JSONReader, JSONWriter
 
 # guitest: show
 
 
 class JSONTest(IOTest):
     """Class for JSON I/O testing"""
```

### Comparing `guiqwt-4.4.0/guiqwt/tests/loadsaveitems_pickle.py` & `guiqwt-4.4.1/guiqwt/tests/loadsaveitems_pickle.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/loadtest.py` & `guiqwt-4.4.1/guiqwt/tests/loadtest.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/manager.py` & `guiqwt-4.4.1/guiqwt/tests/manager.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/mandelbrot.py` & `guiqwt-4.4.1/guiqwt/tests/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/mr-brain.dcm` & `guiqwt-4.4.1/guiqwt/tests/mr-brain.dcm`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/pcolor.py` & `guiqwt-4.4.1/guiqwt/tests/pcolor.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/plot.py` & `guiqwt-4.4.1/guiqwt/tests/plot.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/plot_log.py` & `guiqwt-4.4.1/guiqwt/tests/plot_log.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/plot_timecurve.py` & `guiqwt-4.4.1/guiqwt/tests/plot_timecurve.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/plot_yreverse.py` & `guiqwt-4.4.1/guiqwt/tests/plot_yreverse.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/png_test.py` & `guiqwt-4.4.1/guiqwt/tests/png_test.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/polygons.py` & `guiqwt-4.4.1/guiqwt/tests/polygons.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/pyplot.py` & `guiqwt-4.4.1/guiqwt/tests/pyplot.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/qtdesigner.py` & `guiqwt-4.4.1/guiqwt/tests/qtdesigner.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/qtdesigner.ui` & `guiqwt-4.4.1/guiqwt/tests/qtdesigner.ui`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/resize.py` & `guiqwt-4.4.1/guiqwt/tests/resize.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/rotatecrop.py` & `guiqwt-4.4.1/guiqwt/tests/rotatecrop.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/sift.py` & `guiqwt-4.4.1/guiqwt/tests/sift.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/simple_dialog.py` & `guiqwt-4.4.1/guiqwt/tests/simple_dialog.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/simple_window.py` & `guiqwt-4.4.1/guiqwt/tests/simple_window.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/styles.py` & `guiqwt-4.4.1/guiqwt/tests/styles.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/syncplot.py` & `guiqwt-4.4.1/guiqwt/tests/syncplot.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/test_line.py` & `guiqwt-4.4.1/guiqwt/tests/test_line.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tests/transform.py` & `guiqwt-4.4.1/guiqwt/tests/transform.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/tools.py` & `guiqwt-4.4.1/guiqwt/tools.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/transitional.py` & `guiqwt-4.4.1/guiqwt/transitional.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/widgets/__init__.py` & `guiqwt-4.4.1/guiqwt/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/widgets/base.py` & `guiqwt-4.4.1/guiqwt/widgets/base.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/widgets/fit.py` & `guiqwt-4.4.1/guiqwt/widgets/fit.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/widgets/fliprotate.py` & `guiqwt-4.4.1/guiqwt/widgets/fliprotate.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/widgets/resizedialog.py` & `guiqwt-4.4.1/guiqwt/widgets/resizedialog.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt/widgets/rotatecrop.py` & `guiqwt-4.4.1/guiqwt/widgets/rotatecrop.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/guiqwt.egg-info/PKG-INFO` & `guiqwt-4.4.1/guiqwt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: guiqwt
-Version: 4.4.0
+Version: 4.4.1
 Summary: guiqwt is a set of tools for curve and image plotting (extension to PythonQwt)
 Home-page: https://github.com/PierreRaybaut/guiqwt
 Author: Pierre Raybaut
 Author-email: pierre.raybaut@gmail.com
 License: CeCILL V2
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
@@ -64,7 +65,9 @@
 .. _NumPy: https://pypi.python.org/pypi/NumPy
 .. _SciPy: https://pypi.python.org/pypi/SciPy
 .. _Pillow: https://pypi.python.org/pypi/Pillow
 
 See the `README`_ and `documentation`_ for more details.
 
 .. _README: https://github.com/PierreRaybaut/guiqwt/blob/master/README.md
+
+
```

### Comparing `guiqwt-4.4.0/guiqwt.egg-info/SOURCES.txt` & `guiqwt-4.4.1/guiqwt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/setup.py` & `guiqwt-4.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,27 +224,27 @@
 # Compiling Cython modules to C source code: this is the only way I found to
 # be able to build both Fortran and Cython extensions together
 # (this could be changed now as there is no longer Fortran extensions here...)
 cythonize_all("src")
 
 setup(
     name=LIBNAME,
-    version="4.4.0",  # Update here *AND* in __init__.py!
+    version="4.4.1",  # Update here *AND* in __init__.py!
     # (Until setup.py has been fully retrofitted, this manual sync is mandatory)
     description=__description__,
     long_description=LONG_DESCRIPTION,
     packages=get_subpackages(LIBNAME),
     package_data={
         LIBNAME: get_package_data(LIBNAME, (".png", ".svg", ".mo", ".dcm", ".ui"))
     },
     data_files=[(r"Doc", [CHM_DOC])] if CHM_DOC else [],
     install_requires=[
         "NumPy>=1.3",
         "SciPy>=0.7",
-        "guidata>=3.0",
+        "guidata>=3.0.1",
         "PythonQwt>=0.10",
         "Pillow",
         "QtPy>=1.3",
     ],
     extras_require={
         "Doc": ["Sphinx>=1.1"],
         "DICOM": ["pydicom>=0.9.3"],
```

### Comparing `guiqwt-4.4.0/sift/create_exe.py` & `guiqwt-4.4.1/sift/create_exe.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/sift/sift.ico` & `guiqwt-4.4.1/sift/sift.ico`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/src/arrays.hpp` & `guiqwt-4.4.1/src/arrays.hpp`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/src/debug.hpp` & `guiqwt-4.4.1/src/debug.hpp`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/src/histogram2d.c` & `guiqwt-4.4.1/src/histogram2d.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.26 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_26"
+#define CYTHON_HEX_VERSION 0x001D1AF0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,15 +45,14 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -82,22 +81,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
-  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -127,67 +122,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
-#elif defined(PY_NOGIL)
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
-  #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 1
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYTYPE_LOOKUP
-  #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #ifndef CYTHON_USE_ASYNC_SLOTS
-    #define CYTHON_USE_ASYNC_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYLIST_INTERNALS
-  #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
-  #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
-  #ifndef CYTHON_AVOID_BORROWED_REFS
-    #define CYTHON_AVOID_BORROWED_REFS 0
-  #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
-  #undef CYTHON_FAST_THREAD_STATE
-  #define CYTHON_FAST_THREAD_STATE 0
-  #undef CYTHON_FAST_PYCALL
-  #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
-  #endif
-  #undef CYTHON_USE_DICT_VERSIONS
-  #define CYTHON_USE_DICT_VERSIONS 0
-  #undef CYTHON_USE_EXC_INFO_STACK
-  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -222,41 +168,32 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK 0
-  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+  #ifndef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
-  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -700,18 +637,16 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
-  #if !defined(_USE_MATH_DEFINES)
-    #define _USE_MATH_DEFINES
-  #endif
+#if defined(WIN32) || defined(MS_WINDOWS)
+  #define _USE_MATH_DEFINES
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -1020,195 +955,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":689
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":690
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":691
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":692
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":696
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":697
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":698
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":699
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":703
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":704
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":713
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":714
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":715
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":717
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":718
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":719
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":721
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":722
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":724
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":725
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":726
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1235,42 +1170,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":728
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":729
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":730
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":732
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3124,15 +3059,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_tmp.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":734
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3141,29 +3076,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3174,15 +3109,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":737
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3191,29 +3126,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3224,15 +3159,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":740
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3241,29 +3176,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3274,15 +3209,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":743
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3291,29 +3226,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3324,15 +3259,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":746
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3341,29 +3276,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3374,212 +3309,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":749
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":750
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":753
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":749
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":928
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":929
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":932
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":933
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":935
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":934
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":936
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":932
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":940
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3595,15 +3530,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":941
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3611,84 +3546,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":941
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":943
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":944
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":940
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3703,15 +3638,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":946
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3727,15 +3662,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":947
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3743,84 +3678,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":947
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":949
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":950
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":946
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3835,15 +3770,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":952
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3859,15 +3794,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":953
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3875,84 +3810,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":953
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":955
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":956
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":952
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3967,176 +3902,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":966
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":978
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":966
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":981
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":993
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":981
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":996
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":996
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1006
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1013
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4225,43 +4160,43 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_u, __pyx_k_u, sizeof(__pyx_k_u), 0, 0, 1, 1},
   {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 32, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "histogram2d.pyx":19
  * @cython.profile(False)
  * @cython.boundscheck(False)
  * def histogram2d(np.ndarray[double, ndim=1] X, np.ndarray[double, ndim=1] Y,             # <<<<<<<<<<<<<<
@@ -4353,46 +4288,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
   __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
   __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
   __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
   __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
   __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
   __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
   __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
   __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
   __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
   __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -4644,15 +4579,15 @@
  * # Copyright (C) 2012 CEA
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -6016,20 +5951,14 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -6085,32 +6014,22 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
-        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) {
-            /* If the code object creation fails, then we should clear the
-               fetched exception references and propagate the new exception */
-            Py_XDECREF(ptype);
-            Py_XDECREF(pvalue);
-            Py_XDECREF(ptraceback);
-            goto bad;
-        }
-        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
+        if (!py_code) goto bad;
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -7235,41 +7154,19 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
-        }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
-            break;
-        }
-    }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    char ctversion[4], rtversion[4];
+    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
+    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -7473,15 +7370,15 @@
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
     const digit* digits = ((PyLongObject*)b)->ob_digit;
     const Py_ssize_t size = Py_SIZE(b);
     if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
+        ival = likely(size) ? (Py_ssize_t)(digits[0]) : 0;
         if (size == -1) ival = -ival;
         return ival;
     } else {
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
```

### Comparing `guiqwt-4.4.0/src/histogram2d.pyx` & `guiqwt-4.4.1/src/histogram2d.pyx`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/src/mandelbrot.c` & `guiqwt-4.4.1/src/mandelbrot.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.26 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_26"
+#define CYTHON_HEX_VERSION 0x001D1AF0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,15 +45,14 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -82,22 +81,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
-  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -127,67 +122,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
-#elif defined(PY_NOGIL)
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
-  #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 1
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYTYPE_LOOKUP
-  #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #ifndef CYTHON_USE_ASYNC_SLOTS
-    #define CYTHON_USE_ASYNC_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYLIST_INTERNALS
-  #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
-  #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
-  #ifndef CYTHON_AVOID_BORROWED_REFS
-    #define CYTHON_AVOID_BORROWED_REFS 0
-  #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
-  #undef CYTHON_FAST_THREAD_STATE
-  #define CYTHON_FAST_THREAD_STATE 0
-  #undef CYTHON_FAST_PYCALL
-  #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
-  #endif
-  #undef CYTHON_USE_DICT_VERSIONS
-  #define CYTHON_USE_DICT_VERSIONS 0
-  #undef CYTHON_USE_EXC_INFO_STACK
-  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -222,41 +168,32 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK 0
-  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+  #ifndef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
-  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -700,18 +637,16 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
-  #if !defined(_USE_MATH_DEFINES)
-    #define _USE_MATH_DEFINES
-  #endif
+#if defined(WIN32) || defined(MS_WINDOWS)
+  #define _USE_MATH_DEFINES
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -983,195 +918,195 @@
 
 static const char *__pyx_f[] = {
   "src\\mandelbrot.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":689
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":690
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":691
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":692
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":696
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":697
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":698
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":699
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":703
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":704
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":713
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":714
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":715
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":717
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":718
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":719
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":721
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":722
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":724
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":725
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":726
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1198,42 +1133,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":728
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":729
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":730
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":732
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2147,15 +2082,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":734
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2164,29 +2099,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2197,15 +2132,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":737
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2214,29 +2149,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2247,15 +2182,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":740
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2264,29 +2199,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2297,15 +2232,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":743
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2314,29 +2249,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2347,15 +2282,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":746
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2364,29 +2299,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2397,212 +2332,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":749
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":750
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":753
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":749
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":928
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":929
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":932
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":933
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":935
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":934
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":936
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":932
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":940
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2618,15 +2553,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":941
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -2634,84 +2569,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":941
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":943
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":944
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":940
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2726,15 +2661,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":946
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2750,15 +2685,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":947
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -2766,84 +2701,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":947
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":949
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":950
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":946
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2858,15 +2793,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":952
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2882,15 +2817,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":953
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -2898,84 +2833,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":953
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":955
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":956
+      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":952
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2990,176 +2925,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":966
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":978
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":966
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":981
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":993
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":981
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":996
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":996
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1006
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1013
+/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -3239,43 +3174,43 @@
   {&__pyx_n_s_x2, __pyx_k_x2, sizeof(__pyx_k_x2), 0, 0, 1, 1},
   {&__pyx_n_s_y1, __pyx_k_y1, sizeof(__pyx_k_y1), 0, 0, 1, 1},
   {&__pyx_n_s_y2, __pyx_k_y2, sizeof(__pyx_k_y2), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 17, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "mandelbrot.pyx":25
  * 
  * @cython.boundscheck(False)
  * def mandelbrot(double x1, double y1, double x2, double y2,             # <<<<<<<<<<<<<<
@@ -3355,46 +3290,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
   __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
   __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
   __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
   __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
   __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
   __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
   __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
   __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
   __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
   __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -3634,15 +3569,15 @@
  * # Copyright (C) 2012 CEA
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4512,20 +4447,14 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -4581,32 +4510,22 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
-        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) {
-            /* If the code object creation fails, then we should clear the
-               fetched exception references and propagate the new exception */
-            Py_XDECREF(ptype);
-            Py_XDECREF(pvalue);
-            Py_XDECREF(ptraceback);
-            goto bad;
-        }
-        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
+        if (!py_code) goto bad;
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -5749,41 +5668,19 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
-        }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
-            break;
-        }
-    }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    char ctversion[4], rtversion[4];
+    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
+    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -5987,15 +5884,15 @@
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
     const digit* digits = ((PyLongObject*)b)->ob_digit;
     const Py_ssize_t size = Py_SIZE(b);
     if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
+        ival = likely(size) ? (Py_ssize_t)(digits[0]) : 0;
         if (size == -1) ival = -ival;
         return ival;
     } else {
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
```

### Comparing `guiqwt-4.4.0/src/mandelbrot.pyx` & `guiqwt-4.4.1/src/mandelbrot.pyx`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/src/pcolor.cpp` & `guiqwt-4.4.1/src/pcolor.cpp`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/src/points.hpp` & `guiqwt-4.4.1/src/points.hpp`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/src/scaler.cpp` & `guiqwt-4.4.1/src/scaler.cpp`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/src/scaler.hpp` & `guiqwt-4.4.1/src/scaler.hpp`

 * *Files identical despite different names*

### Comparing `guiqwt-4.4.0/src/traits.hpp` & `guiqwt-4.4.1/src/traits.hpp`

 * *Files identical despite different names*

