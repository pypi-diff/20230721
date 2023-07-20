# Comparing `tmp/reflex-0.2.2.tar.gz` & `tmp/reflex-0.2.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.2.2.tar", max compression
+gzip compressed data, was "reflex-0.2.2a1.tar", max compression
```

## Comparing `reflex-0.2.2.tar` & `reflex-0.2.2a1.tar`

### file list

```diff
@@ -1,178 +1,178 @@
--rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.2/LICENSE
--rw-r--r--   0        0        0     7766 2023-07-17 23:29:33.625723 reflex-0.2.2/README.md
--rw-r--r--   0        0        0     2000 2023-07-20 21:43:21.449188 reflex-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.2/reflex/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1337 2023-07-19 01:58:23.983993 reflex-0.2.2/reflex/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.2/reflex/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1225 2023-07-14 23:13:37.769942 reflex-0.2.2/reflex/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.2/reflex/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.2/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.2/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.2/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.2/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.2/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.2/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.2/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.2/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.2/reflex/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.2/reflex/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.2/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       65 2023-07-14 23:13:37.771678 reflex-0.2.2/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0     1287 2023-07-20 20:03:35.347093 reflex-0.2.2/reflex/.templates/web/package.json
--rw-r--r--   0        0        0      502 2023-07-14 23:13:37.771821 reflex-0.2.2/reflex/.templates/web/pages/404.js
--rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.2/reflex/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.2/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.2/reflex/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.2/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0    10110 2023-07-20 20:03:35.347375 reflex-0.2.2/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1965 2023-07-19 01:58:26.538410 reflex-0.2.2/reflex/__init__.py
--rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.2/reflex/admin.py
--rw-r--r--   0        0        0    23767 2023-07-20 20:03:35.348327 reflex-0.2.2/reflex/app.py
--rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.2/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.2/reflex/compiler/__init__.py
--rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.2/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     2725 2023-07-14 23:13:37.772848 reflex-0.2.2/reflex/compiler/templates.py
--rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.2/reflex/compiler/utils.py
--rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.2/reflex/components/__init__.py
--rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.2/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.2/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.2/reflex/components/base/body.py
--rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.2/reflex/components/base/document.py
--rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.2/reflex/components/base/head.py
--rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.2/reflex/components/base/link.py
--rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.2/reflex/components/base/meta.py
--rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.2/reflex/components/base/script.py
--rw-r--r--   0        0        0    24321 2023-07-14 23:13:37.773563 reflex-0.2.2/reflex/components/component.py
--rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.2/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.2/reflex/components/datadisplay/badge.py
--rw-r--r--   0        0        0     3495 2023-07-14 23:13:37.773785 reflex-0.2.2/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0     4025 2023-07-14 23:13:37.773859 reflex-0.2.2/reflex/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.2/reflex/components/datadisplay/divider.py
--rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.2/reflex/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.2/reflex/components/datadisplay/list.py
--rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.2/reflex/components/datadisplay/stat.py
--rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.2/reflex/components/datadisplay/table.py
--rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.2/reflex/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.2/reflex/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.2/reflex/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.2/reflex/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.2/reflex/components/disclosure/transition.py
--rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.2/reflex/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.2/reflex/components/feedback/__init__.py
--rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.2/reflex/components/feedback/alert.py
--rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.2/reflex/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.2/reflex/components/feedback/progress.py
--rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.2/reflex/components/feedback/skeleton.py
--rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.2/reflex/components/feedback/spinner.py
--rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.2/reflex/components/forms/__init__.py
--rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.2/reflex/components/forms/button.py
--rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.2/reflex/components/forms/checkbox.py
--rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.2/reflex/components/forms/colormodeswitch.py
--rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.2/reflex/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.2/reflex/components/forms/date_picker.py
--rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.2/reflex/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.2/reflex/components/forms/debounce.py
--rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.2/reflex/components/forms/editable.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.2/reflex/components/forms/email.py
--rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.2/reflex/components/forms/form.py
--rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.2/reflex/components/forms/iconbutton.py
--rw-r--r--   0        0        0     3246 2023-07-14 23:13:37.775648 reflex-0.2.2/reflex/components/forms/input.py
--rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.2/reflex/components/forms/multiselect.py
--rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.2/reflex/components/forms/numberinput.py
--rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.2/reflex/components/forms/password.py
--rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.2/reflex/components/forms/pininput.py
--rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.2/reflex/components/forms/radio.py
--rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.2/reflex/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.2/reflex/components/forms/select.py
--rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.2/reflex/components/forms/slider.py
--rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.2/reflex/components/forms/switch.py
--rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.2/reflex/components/forms/textarea.py
--rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.2/reflex/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.2/reflex/components/graphing/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.2/reflex/components/graphing/plotly.py
--rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.2/reflex/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.2/reflex/components/layout/__init__.py
--rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.2/reflex/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.2/reflex/components/layout/box.py
--rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.2/reflex/components/layout/card.py
--rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.2/reflex/components/layout/center.py
--rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.2/reflex/components/layout/cond.py
--rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.2/reflex/components/layout/container.py
--rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.2/reflex/components/layout/flex.py
--rw-r--r--   0        0        0     3159 2023-07-14 23:13:37.777060 reflex-0.2.2/reflex/components/layout/foreach.py
--rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.2/reflex/components/layout/fragment.py
--rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.2/reflex/components/layout/grid.py
--rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.2/reflex/components/layout/html.py
--rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.2/reflex/components/layout/responsive.py
--rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.2/reflex/components/layout/spacer.py
--rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.2/reflex/components/layout/stack.py
--rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.2/reflex/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.2/reflex/components/libs/__init__.py
--rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.2/reflex/components/libs/chakra.py
--rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.2/reflex/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.2/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.2/reflex/components/media/audio.py
--rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.2/reflex/components/media/avatar.py
--rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.2/reflex/components/media/icon.py
--rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.2/reflex/components/media/image.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.2/reflex/components/media/video.py
--rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.2/reflex/components/navigation/__init__.py
--rw-r--r--   0        0        0     2017 2023-07-14 23:13:37.778119 reflex-0.2.2/reflex/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.2/reflex/components/navigation/link.py
--rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.2/reflex/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.2/reflex/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.2/reflex/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.2/reflex/components/overlay/__init__.py
--rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.2/reflex/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.2/reflex/components/overlay/banner.py
--rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.2/reflex/components/overlay/drawer.py
--rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.2/reflex/components/overlay/menu.py
--rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.2/reflex/components/overlay/modal.py
--rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.2/reflex/components/overlay/popover.py
--rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.2/reflex/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.2/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.2/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-07-20 20:03:37.472790 reflex-0.2.2/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5008 2023-07-14 23:13:37.779125 reflex-0.2.2/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.2/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.2/reflex/components/typography/__init__.py
--rw-r--r--   0        0        0      278 2023-07-14 23:13:37.779315 reflex-0.2.2/reflex/components/typography/heading.py
--rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.2/reflex/components/typography/highlight.py
--rw-r--r--   0        0        0     3593 2023-07-14 23:13:37.779432 reflex-0.2.2/reflex/components/typography/markdown.py
--rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.2/reflex/components/typography/span.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.2/reflex/components/typography/text.py
--rw-r--r--   0        0        0     7692 2023-07-20 20:03:35.349661 reflex-0.2.2/reflex/config.py
--rw-r--r--   0        0        0    11103 2023-07-20 20:03:35.349925 reflex-0.2.2/reflex/constants.py
--rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.2/reflex/el/__init__.py
--rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.2/reflex/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.2/reflex/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.2/reflex/el/constants/react.py
--rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.2/reflex/el/constants/reflex.py
--rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.2/reflex/el/element.py
--rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.2/reflex/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.2/reflex/el/precompile.py
--rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.2/reflex/event.py
--rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.2/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.2/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.2/reflex/middleware/middleware.py
--rw-r--r--   0        0        0     9604 2023-07-19 23:09:19.472388 reflex-0.2.2/reflex/model.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.2/reflex/py.typed
--rw-r--r--   0        0        0    11041 2023-07-19 23:47:51.599199 reflex-0.2.2/reflex/reflex.py
--rw-r--r--   0        0        0     4104 2023-07-14 23:13:37.781214 reflex-0.2.2/reflex/route.py
--rw-r--r--   0        0        0    31805 2023-07-14 23:13:37.781402 reflex-0.2.2/reflex/state.py
--rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.2/reflex/style.py
--rw-r--r--   0        0        0    15063 2023-07-14 23:13:37.781613 reflex-0.2.2/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.2/reflex/utils/__init__.py
--rw-r--r--   0        0        0     7971 2023-07-20 20:03:35.350159 reflex-0.2.2/reflex/utils/build.py
--rw-r--r--   0        0        0     1692 2023-07-19 01:58:26.541439 reflex-0.2.2/reflex/utils/console.py
--rw-r--r--   0        0        0     4225 2023-07-17 23:29:33.628283 reflex-0.2.2/reflex/utils/exec.py
--rw-r--r--   0        0        0    11845 2023-07-14 23:13:37.782067 reflex-0.2.2/reflex/utils/format.py
--rw-r--r--   0        0        0      585 2023-07-14 23:13:37.782125 reflex-0.2.2/reflex/utils/imports.py
--rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.2/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    14056 2023-07-19 01:58:26.541782 reflex-0.2.2/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     4105 2023-07-17 23:29:33.628618 reflex-0.2.2/reflex/utils/processes.py
--rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.2/reflex/utils/telemetry.py
--rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.2/reflex/utils/types.py
--rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.2/reflex/utils/watch.py
--rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.2/reflex/vars.py
--rw-r--r--   0        0        0     9584 1970-01-01 00:00:00.000000 reflex-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.2a1/LICENSE
+-rw-r--r--   0        0        0     7766 2023-07-17 23:29:33.625723 reflex-0.2.2a1/README.md
+-rw-r--r--   0        0        0     2002 2023-07-20 20:03:43.742215 reflex-0.2.2a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.2a1/reflex/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1337 2023-07-19 01:58:23.983993 reflex-0.2.2a1/reflex/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.2a1/reflex/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1225 2023-07-14 23:13:37.769942 reflex-0.2.2a1/reflex/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.2a1/reflex/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.2a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.2a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.2a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.2a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.2a1/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.2a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.2a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.2a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.2a1/reflex/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.2a1/reflex/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.2a1/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       65 2023-07-14 23:13:37.771678 reflex-0.2.2a1/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1287 2023-07-20 20:03:35.347093 reflex-0.2.2a1/reflex/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-07-14 23:13:37.771821 reflex-0.2.2a1/reflex/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.2a1/reflex/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.2a1/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.2a1/reflex/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.2a1/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0    10110 2023-07-20 20:03:35.347375 reflex-0.2.2a1/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1965 2023-07-19 01:58:26.538410 reflex-0.2.2a1/reflex/__init__.py
+-rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.2a1/reflex/admin.py
+-rw-r--r--   0        0        0    23767 2023-07-20 20:03:35.348327 reflex-0.2.2a1/reflex/app.py
+-rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.2a1/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.2a1/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.2a1/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     2725 2023-07-14 23:13:37.772848 reflex-0.2.2a1/reflex/compiler/templates.py
+-rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.2a1/reflex/compiler/utils.py
+-rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.2a1/reflex/components/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.2a1/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.2a1/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.2a1/reflex/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.2a1/reflex/components/base/document.py
+-rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.2a1/reflex/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.2a1/reflex/components/base/link.py
+-rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.2a1/reflex/components/base/meta.py
+-rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.2a1/reflex/components/base/script.py
+-rw-r--r--   0        0        0    24321 2023-07-14 23:13:37.773563 reflex-0.2.2a1/reflex/components/component.py
+-rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.2a1/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.2a1/reflex/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     3495 2023-07-14 23:13:37.773785 reflex-0.2.2a1/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4025 2023-07-14 23:13:37.773859 reflex-0.2.2a1/reflex/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.2a1/reflex/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.2a1/reflex/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.2a1/reflex/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.2a1/reflex/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.2a1/reflex/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.2a1/reflex/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.2a1/reflex/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.2a1/reflex/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.2a1/reflex/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.2a1/reflex/components/disclosure/transition.py
+-rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.2a1/reflex/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.2a1/reflex/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.2a1/reflex/components/feedback/alert.py
+-rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.2a1/reflex/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.2a1/reflex/components/feedback/progress.py
+-rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.2a1/reflex/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.2a1/reflex/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.2a1/reflex/components/forms/__init__.py
+-rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.2a1/reflex/components/forms/button.py
+-rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.2a1/reflex/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.2a1/reflex/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.2a1/reflex/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.2a1/reflex/components/forms/date_picker.py
+-rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.2a1/reflex/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.2a1/reflex/components/forms/debounce.py
+-rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.2a1/reflex/components/forms/editable.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.2a1/reflex/components/forms/email.py
+-rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.2a1/reflex/components/forms/form.py
+-rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.2a1/reflex/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     3246 2023-07-14 23:13:37.775648 reflex-0.2.2a1/reflex/components/forms/input.py
+-rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.2a1/reflex/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.2a1/reflex/components/forms/numberinput.py
+-rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.2a1/reflex/components/forms/password.py
+-rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.2a1/reflex/components/forms/pininput.py
+-rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.2a1/reflex/components/forms/radio.py
+-rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.2a1/reflex/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.2a1/reflex/components/forms/select.py
+-rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.2a1/reflex/components/forms/slider.py
+-rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.2a1/reflex/components/forms/switch.py
+-rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.2a1/reflex/components/forms/textarea.py
+-rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.2a1/reflex/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.2a1/reflex/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.2a1/reflex/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.2a1/reflex/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.2a1/reflex/components/layout/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.2a1/reflex/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.2a1/reflex/components/layout/box.py
+-rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.2a1/reflex/components/layout/card.py
+-rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.2a1/reflex/components/layout/center.py
+-rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.2a1/reflex/components/layout/cond.py
+-rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.2a1/reflex/components/layout/container.py
+-rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.2a1/reflex/components/layout/flex.py
+-rw-r--r--   0        0        0     3159 2023-07-14 23:13:37.777060 reflex-0.2.2a1/reflex/components/layout/foreach.py
+-rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.2a1/reflex/components/layout/fragment.py
+-rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.2a1/reflex/components/layout/grid.py
+-rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.2a1/reflex/components/layout/html.py
+-rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.2a1/reflex/components/layout/responsive.py
+-rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.2a1/reflex/components/layout/spacer.py
+-rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.2a1/reflex/components/layout/stack.py
+-rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.2a1/reflex/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.2a1/reflex/components/libs/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.2a1/reflex/components/libs/chakra.py
+-rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.2a1/reflex/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.2a1/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.2a1/reflex/components/media/audio.py
+-rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.2a1/reflex/components/media/avatar.py
+-rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.2a1/reflex/components/media/icon.py
+-rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.2a1/reflex/components/media/image.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.2a1/reflex/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.2a1/reflex/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2017 2023-07-14 23:13:37.778119 reflex-0.2.2a1/reflex/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.2a1/reflex/components/navigation/link.py
+-rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.2a1/reflex/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.2a1/reflex/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.2a1/reflex/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.2a1/reflex/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.2a1/reflex/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.2a1/reflex/components/overlay/banner.py
+-rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.2a1/reflex/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.2a1/reflex/components/overlay/menu.py
+-rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.2a1/reflex/components/overlay/modal.py
+-rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.2a1/reflex/components/overlay/popover.py
+-rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.2a1/reflex/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.2a1/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.2a1/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-07-20 20:03:37.472790 reflex-0.2.2a1/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5008 2023-07-14 23:13:37.779125 reflex-0.2.2a1/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.2a1/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.2a1/reflex/components/typography/__init__.py
+-rw-r--r--   0        0        0      278 2023-07-14 23:13:37.779315 reflex-0.2.2a1/reflex/components/typography/heading.py
+-rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.2a1/reflex/components/typography/highlight.py
+-rw-r--r--   0        0        0     3593 2023-07-14 23:13:37.779432 reflex-0.2.2a1/reflex/components/typography/markdown.py
+-rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.2a1/reflex/components/typography/span.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.2a1/reflex/components/typography/text.py
+-rw-r--r--   0        0        0     7692 2023-07-20 20:03:35.349661 reflex-0.2.2a1/reflex/config.py
+-rw-r--r--   0        0        0    11103 2023-07-20 20:03:35.349925 reflex-0.2.2a1/reflex/constants.py
+-rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.2a1/reflex/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.2a1/reflex/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.2a1/reflex/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.2a1/reflex/el/constants/react.py
+-rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.2a1/reflex/el/constants/reflex.py
+-rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.2a1/reflex/el/element.py
+-rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.2a1/reflex/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.2a1/reflex/el/precompile.py
+-rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.2a1/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.2a1/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.2a1/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.2a1/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0     9604 2023-07-19 23:09:19.472388 reflex-0.2.2a1/reflex/model.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.2a1/reflex/py.typed
+-rw-r--r--   0        0        0    11041 2023-07-19 23:47:51.599199 reflex-0.2.2a1/reflex/reflex.py
+-rw-r--r--   0        0        0     4104 2023-07-14 23:13:37.781214 reflex-0.2.2a1/reflex/route.py
+-rw-r--r--   0        0        0    31805 2023-07-14 23:13:37.781402 reflex-0.2.2a1/reflex/state.py
+-rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.2a1/reflex/style.py
+-rw-r--r--   0        0        0    15063 2023-07-14 23:13:37.781613 reflex-0.2.2a1/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.2a1/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     7971 2023-07-20 20:03:35.350159 reflex-0.2.2a1/reflex/utils/build.py
+-rw-r--r--   0        0        0     1692 2023-07-19 01:58:26.541439 reflex-0.2.2a1/reflex/utils/console.py
+-rw-r--r--   0        0        0     4225 2023-07-17 23:29:33.628283 reflex-0.2.2a1/reflex/utils/exec.py
+-rw-r--r--   0        0        0    11845 2023-07-14 23:13:37.782067 reflex-0.2.2a1/reflex/utils/format.py
+-rw-r--r--   0        0        0      585 2023-07-14 23:13:37.782125 reflex-0.2.2a1/reflex/utils/imports.py
+-rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.2a1/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    14056 2023-07-19 01:58:26.541782 reflex-0.2.2a1/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     4105 2023-07-17 23:29:33.628618 reflex-0.2.2a1/reflex/utils/processes.py
+-rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.2a1/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.2a1/reflex/utils/types.py
+-rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.2a1/reflex/utils/watch.py
+-rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.2a1/reflex/vars.py
+-rw-r--r--   0        0        0     9586 1970-01-01 00:00:00.000000 reflex-0.2.2a1/PKG-INFO
```

### Comparing `reflex-0.2.2/LICENSE` & `reflex-0.2.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/README.md` & `reflex-0.2.2a1/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/pyproject.toml` & `reflex-0.2.2a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.2.2"
+version = "0.2.2a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `reflex-0.2.2/reflex/.templates/apps/counter/counter.py` & `reflex-0.2.2a1/reflex/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/.templates/apps/default/default.py` & `reflex-0.2.2a1/reflex/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/.templates/assets/favicon.ico` & `reflex-0.2.2a1/reflex/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/.templates/jinja/web/pages/index.js.jinja2` & `reflex-0.2.2a1/reflex/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.2.2a1/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/.templates/web/bun.lockb` & `reflex-0.2.2a1/reflex/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/.templates/web/package.json` & `reflex-0.2.2a1/reflex/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/.templates/web/pages/_app.js` & `reflex-0.2.2a1/reflex/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/.templates/web/styles/code/prism.js` & `reflex-0.2.2a1/reflex/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/.templates/web/utils/state.js` & `reflex-0.2.2a1/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/__init__.py` & `reflex-0.2.2a1/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/app.py` & `reflex-0.2.2a1/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/base.py` & `reflex-0.2.2a1/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/compiler/compiler.py` & `reflex-0.2.2a1/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/compiler/templates.py` & `reflex-0.2.2a1/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/compiler/utils.py` & `reflex-0.2.2a1/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/__init__.py` & `reflex-0.2.2a1/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/base/bare.py` & `reflex-0.2.2a1/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/base/document.py` & `reflex-0.2.2a1/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/base/link.py` & `reflex-0.2.2a1/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/base/meta.py` & `reflex-0.2.2a1/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/base/script.py` & `reflex-0.2.2a1/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/component.py` & `reflex-0.2.2a1/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/datadisplay/code.py` & `reflex-0.2.2a1/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/datadisplay/datatable.py` & `reflex-0.2.2a1/reflex/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/datadisplay/divider.py` & `reflex-0.2.2a1/reflex/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/datadisplay/list.py` & `reflex-0.2.2a1/reflex/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/datadisplay/stat.py` & `reflex-0.2.2a1/reflex/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/datadisplay/table.py` & `reflex-0.2.2a1/reflex/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/datadisplay/tag.py` & `reflex-0.2.2a1/reflex/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/disclosure/accordion.py` & `reflex-0.2.2a1/reflex/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/disclosure/tabs.py` & `reflex-0.2.2a1/reflex/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/disclosure/transition.py` & `reflex-0.2.2a1/reflex/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/feedback/alert.py` & `reflex-0.2.2a1/reflex/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/feedback/circularprogress.py` & `reflex-0.2.2a1/reflex/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/feedback/progress.py` & `reflex-0.2.2a1/reflex/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/feedback/skeleton.py` & `reflex-0.2.2a1/reflex/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/feedback/spinner.py` & `reflex-0.2.2a1/reflex/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/__init__.py` & `reflex-0.2.2a1/reflex/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/button.py` & `reflex-0.2.2a1/reflex/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/checkbox.py` & `reflex-0.2.2a1/reflex/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/colormodeswitch.py` & `reflex-0.2.2a1/reflex/components/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/copytoclipboard.py` & `reflex-0.2.2a1/reflex/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/debounce.py` & `reflex-0.2.2a1/reflex/components/forms/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/editable.py` & `reflex-0.2.2a1/reflex/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/form.py` & `reflex-0.2.2a1/reflex/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/iconbutton.py` & `reflex-0.2.2a1/reflex/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/input.py` & `reflex-0.2.2a1/reflex/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/multiselect.py` & `reflex-0.2.2a1/reflex/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/numberinput.py` & `reflex-0.2.2a1/reflex/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/pininput.py` & `reflex-0.2.2a1/reflex/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/radio.py` & `reflex-0.2.2a1/reflex/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/rangeslider.py` & `reflex-0.2.2a1/reflex/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/select.py` & `reflex-0.2.2a1/reflex/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/slider.py` & `reflex-0.2.2a1/reflex/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/switch.py` & `reflex-0.2.2a1/reflex/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/textarea.py` & `reflex-0.2.2a1/reflex/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/forms/upload.py` & `reflex-0.2.2a1/reflex/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/graphing/plotly.py` & `reflex-0.2.2a1/reflex/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/graphing/victory.py` & `reflex-0.2.2a1/reflex/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/layout/__init__.py` & `reflex-0.2.2a1/reflex/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/layout/box.py` & `reflex-0.2.2a1/reflex/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/layout/card.py` & `reflex-0.2.2a1/reflex/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/layout/cond.py` & `reflex-0.2.2a1/reflex/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/layout/flex.py` & `reflex-0.2.2a1/reflex/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/layout/foreach.py` & `reflex-0.2.2a1/reflex/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/layout/grid.py` & `reflex-0.2.2a1/reflex/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/layout/html.py` & `reflex-0.2.2a1/reflex/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/layout/responsive.py` & `reflex-0.2.2a1/reflex/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/layout/stack.py` & `reflex-0.2.2a1/reflex/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/layout/wrap.py` & `reflex-0.2.2a1/reflex/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/libs/react_player.py` & `reflex-0.2.2a1/reflex/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/media/avatar.py` & `reflex-0.2.2a1/reflex/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/media/icon.py` & `reflex-0.2.2a1/reflex/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/media/image.py` & `reflex-0.2.2a1/reflex/components/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/navigation/breadcrumb.py` & `reflex-0.2.2a1/reflex/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/navigation/link.py` & `reflex-0.2.2a1/reflex/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/navigation/linkoverlay.py` & `reflex-0.2.2a1/reflex/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/navigation/stepper.py` & `reflex-0.2.2a1/reflex/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/overlay/__init__.py` & `reflex-0.2.2a1/reflex/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/overlay/alertdialog.py` & `reflex-0.2.2a1/reflex/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/overlay/banner.py` & `reflex-0.2.2a1/reflex/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/overlay/drawer.py` & `reflex-0.2.2a1/reflex/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/overlay/menu.py` & `reflex-0.2.2a1/reflex/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/overlay/modal.py` & `reflex-0.2.2a1/reflex/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/overlay/popover.py` & `reflex-0.2.2a1/reflex/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/overlay/tooltip.py` & `reflex-0.2.2a1/reflex/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/tags/iter_tag.py` & `reflex-0.2.2a1/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/tags/tag.py` & `reflex-0.2.2a1/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/tags/tagless.py` & `reflex-0.2.2a1/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/typography/highlight.py` & `reflex-0.2.2a1/reflex/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/components/typography/markdown.py` & `reflex-0.2.2a1/reflex/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/config.py` & `reflex-0.2.2a1/reflex/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/constants.py` & `reflex-0.2.2a1/reflex/constants.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/el/constants/html.py` & `reflex-0.2.2a1/reflex/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/el/constants/react.py` & `reflex-0.2.2a1/reflex/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/el/constants/reflex.py` & `reflex-0.2.2a1/reflex/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/el/element.py` & `reflex-0.2.2a1/reflex/el/element.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/el/elements/__init__.py` & `reflex-0.2.2a1/reflex/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/el/precompile.py` & `reflex-0.2.2a1/reflex/el/precompile.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/event.py` & `reflex-0.2.2a1/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/middleware/hydrate_middleware.py` & `reflex-0.2.2a1/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/middleware/middleware.py` & `reflex-0.2.2a1/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/model.py` & `reflex-0.2.2a1/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/reflex.py` & `reflex-0.2.2a1/reflex/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/route.py` & `reflex-0.2.2a1/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/state.py` & `reflex-0.2.2a1/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/style.py` & `reflex-0.2.2a1/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/testing.py` & `reflex-0.2.2a1/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/utils/build.py` & `reflex-0.2.2a1/reflex/utils/build.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/utils/console.py` & `reflex-0.2.2a1/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/utils/exec.py` & `reflex-0.2.2a1/reflex/utils/exec.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/utils/format.py` & `reflex-0.2.2a1/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/utils/imports.py` & `reflex-0.2.2a1/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/utils/path_ops.py` & `reflex-0.2.2a1/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/utils/prerequisites.py` & `reflex-0.2.2a1/reflex/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/utils/processes.py` & `reflex-0.2.2a1/reflex/utils/processes.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/utils/telemetry.py` & `reflex-0.2.2a1/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/utils/types.py` & `reflex-0.2.2a1/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/utils/watch.py` & `reflex-0.2.2a1/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/reflex/vars.py` & `reflex-0.2.2a1/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.2/PKG-INFO` & `reflex-0.2.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.2.2
+Version: 0.2.2a1
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

