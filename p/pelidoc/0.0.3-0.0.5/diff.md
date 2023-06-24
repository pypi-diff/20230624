# Comparing `tmp/pelidoc-0.0.3.tar.gz` & `tmp/pelidoc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelidoc-0.0.3.tar", last modified: Sat Jun 24 05:04:18 2023, max compression
+gzip compressed data, was "pelidoc-0.0.5.tar", last modified: Sat Jun 24 05:10:13 2023, max compression
```

## Comparing `pelidoc-0.0.3.tar` & `pelidoc-0.0.5.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:18.514460 pelidoc-0.0.3/
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-06-24 05:03:58.000000 pelidoc-0.0.3/.version
--rw-r--r--   0 francispotter   (501) staff       (20)      414 2023-06-24 05:04:18.512990 pelidoc-0.0.3/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      168 2023-06-24 04:47:30.000000 pelidoc-0.0.3/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:17.823281 pelidoc-0.0.3/pelidoc/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-06-22 04:34:41.000000 pelidoc-0.0.3/pelidoc/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1209 2023-06-24 04:13:52.000000 pelidoc-0.0.3/pelidoc/conf.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:17.863140 pelidoc-0.0.3/pelidoc/theme/
--rw-r--r--   0 francispotter   (501) staff       (20)      799 2023-06-19 17:55:16.000000 pelidoc-0.0.3/pelidoc/theme/AUTHORS.md
--rw-r--r--   0 francispotter   (501) staff       (20)     1077 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/LICENSE
--rw-r--r--   0 francispotter   (501) staff       (20)    15125 2023-06-24 02:47:27.000000 pelidoc-0.0.3/pelidoc/theme/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:17.818230 pelidoc-0.0.3/pelidoc/theme/static/
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:18.315534 pelidoc-0.0.3/pelidoc/theme/static/css/
--rw-r--r--   0 francispotter   (501) staff       (20)   120090 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.cerulean.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   119768 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.cosmo.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   109602 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.cupid.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   116696 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.custom.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   119799 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.cyborg.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   121625 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.darkly.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   121354 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.flatly.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   118666 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.journal.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   124431 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.lumen.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   121457 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   132318 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.paper.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   105382 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.readable-old.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   118678 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.readable.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   118965 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.sandstone.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   101587 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.shamrock.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   120186 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.simplex.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   129014 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.slate.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   121499 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.spacelab.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   120731 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.superhero.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   117016 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.united.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)   121865 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.yeti.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)    37414 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/font-awesome.css
--rw-r--r--   0 francispotter   (501) staff       (20)    21778 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/font-awesome.css.map
--rw-r--r--   0 francispotter   (501) staff       (20)    31000 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/font-awesome.min.css
--rw-r--r--   0 francispotter   (501) staff       (20)     6853 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/html4css1.css
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:18.361218 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/
--rw-r--r--   0 francispotter   (501) staff       (20)     3875 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/autumn.css
--rw-r--r--   0 francispotter   (501) staff       (20)     3231 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/borland.css
--rw-r--r--   0 francispotter   (501) staff       (20)     2255 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/bw.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4527 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/colorful.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4217 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/default.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4216 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/emacs.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4244 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/friendly.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4909 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/fruity.css
--rw-r--r--   0 francispotter   (501) staff       (20)     3284 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/github.css
--rw-r--r--   0 francispotter   (501) staff       (20)     1852 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/igor.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4328 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/manni.css
--rw-r--r--   0 francispotter   (501) staff       (20)     3870 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/monokai.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4569 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/murphy.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4732 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/native.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4019 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/paraiso-dark.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4019 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/paraiso-light.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4622 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/pastie.css
--rw-r--r--   0 francispotter   (501) staff       (20)     3961 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/perldoc.css
--rw-r--r--   0 francispotter   (501) staff       (20)     1950 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/rrt.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4310 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/solarizeddark.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4310 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/solarizedlight.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4890 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/tango.css
--rw-r--r--   0 francispotter   (501) staff       (20)     3987 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/trac.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4447 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/vim.css
--rw-r--r--   0 francispotter   (501) staff       (20)     2069 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/vs.css
--rw-r--r--   0 francispotter   (501) staff       (20)     3407 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/xcode.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4370 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/pygments/zenburn.css
--rw-r--r--   0 francispotter   (501) staff       (20)     4249 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/style.css
--rw-r--r--   0 francispotter   (501) staff       (20)      190 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/css/typogrify.css
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:18.404821 pelidoc-0.0.3/pelidoc/theme/static/fonts/
--rw-r--r--   0 francispotter   (501) staff       (20)   134808 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/fonts/FontAwesome.otf
--rw-r--r--   0 francispotter   (501) staff       (20)   165742 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 francispotter   (501) staff       (20)   444379 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 francispotter   (501) staff       (20)   165548 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 francispotter   (501) staff       (20)    98024 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 francispotter   (501) staff       (20)    77160 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 francispotter   (501) staff       (20)    20127 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 francispotter   (501) staff       (20)   108738 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 francispotter   (501) staff       (20)    45404 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 francispotter   (501) staff       (20)    23424 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 francispotter   (501) staff       (20)    18028 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:18.412403 pelidoc-0.0.3/pelidoc/theme/static/js/
--rw-r--r--   0 francispotter   (501) staff       (20)       95 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/js/bodypadding.js
--rw-r--r--   0 francispotter   (501) staff       (20)    39680 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/js/bootstrap.min.js
--rw-r--r--   0 francispotter   (501) staff       (20)     1478 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/js/github.js
--rw-r--r--   0 francispotter   (501) staff       (20)     2474 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/js/jXHR.js
--rw-r--r--   0 francispotter   (501) staff       (20)    88145 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/js/jquery.min.js
--rw-r--r--   0 francispotter   (501) staff       (20)     4047 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/js/respond.min.js
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:18.418537 pelidoc-0.0.3/pelidoc/theme/static/tipuesearch/
--rwxr-xr-x   0 francispotter   (501) staff       (20)     6067 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/tipuesearch/tipuesearch.css
--rw-r--r--   0 francispotter   (501) staff       (20)    33038 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/tipuesearch/tipuesearch.js
--rw-r--r--   0 francispotter   (501) staff       (20)    10512 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/tipuesearch/tipuesearch.min.js
--rw-r--r--   0 francispotter   (501) staff       (20)     4797 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/tipuesearch/tipuesearch_content.js
--rw-r--r--   0 francispotter   (501) staff       (20)     3612 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/static/tipuesearch/tipuesearch_set.js
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:18.441437 pelidoc-0.0.3/pelidoc/theme/templates/
--rw-r--r--   0 francispotter   (501) staff       (20)      910 2023-06-19 17:53:48.000000 pelidoc-0.0.3/pelidoc/theme/templates/archives.html
--rw-r--r--   0 francispotter   (501) staff       (20)     4123 2023-06-19 17:56:28.000000 pelidoc-0.0.3/pelidoc/theme/templates/article.html
--rw-r--r--   0 francispotter   (501) staff       (20)      820 2023-06-19 17:52:09.000000 pelidoc-0.0.3/pelidoc/theme/templates/article_list.html
--rw-r--r--   0 francispotter   (501) staff       (20)     8517 2023-06-19 17:56:45.000000 pelidoc-0.0.3/pelidoc/theme/templates/base.html
--rw-r--r--   0 francispotter   (501) staff       (20)      725 2023-06-19 02:42:12.000000 pelidoc-0.0.3/pelidoc/theme/templates/category.html
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:18.464999 pelidoc-0.0.3/pelidoc/theme/templates/includes/
--rw-r--r--   0 francispotter   (501) staff       (20)      610 2023-06-18 20:35:35.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/addthis.html
--rw-r--r--   0 francispotter   (501) staff       (20)     1692 2023-06-19 15:31:51.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/article_info.html
--rw-r--r--   0 francispotter   (501) staff       (20)      332 2023-06-18 20:35:35.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/banner.html
--rw-r--r--   0 francispotter   (501) staff       (20)      336 2023-06-24 02:52:18.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/footer.html
--rw-r--r--   0 francispotter   (501) staff       (20)     1547 2023-06-18 20:35:35.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/ga.html
--rw-r--r--   0 francispotter   (501) staff       (20)      448 2023-06-18 20:35:35.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/liquid_tags_nb_footer.html
--rw-r--r--   0 francispotter   (501) staff       (20)     8765 2023-06-18 20:35:35.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/liquid_tags_nb_header.html
--rw-r--r--   0 francispotter   (501) staff       (20)      235 2023-06-18 20:35:35.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/minify_tipuesearch.html
--rw-r--r--   0 francispotter   (501) staff       (20)     1805 2023-06-19 17:45:10.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/pagination.html
--rw-r--r--   0 francispotter   (501) staff       (20)      851 2023-06-18 20:35:35.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/piwik.html
--rw-r--r--   0 francispotter   (501) staff       (20)      341 2023-06-18 20:35:35.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/related-posts.html
--rw-r--r--   0 francispotter   (501) staff       (20)      799 2023-06-18 20:35:35.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/series.html
--rw-r--r--   0 francispotter   (501) staff       (20)      304 2023-06-18 20:35:35.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/show_source.html
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:18.510495 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/
--rw-r--r--   0 francispotter   (501) staff       (20)      908 2023-06-19 17:45:56.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/archive.html
--rw-r--r--   0 francispotter   (501) staff       (20)       66 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/article-li.html
--rw-r--r--   0 francispotter   (501) staff       (20)      616 2023-06-19 17:49:44.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/categories.html
--rw-r--r--   0 francispotter   (501) staff       (20)      497 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/images.html
--rw-r--r--   0 francispotter   (501) staff       (20)      458 2023-06-19 17:52:32.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/links.html
--rw-r--r--   0 francispotter   (501) staff       (20)      215 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/macros.jinja
--rw-r--r--   0 francispotter   (501) staff       (20)     1049 2023-06-18 23:41:20.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/navigation.html
--rw-r--r--   0 francispotter   (501) staff       (20)      595 2023-06-19 17:51:06.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/recent_posts.html
--rw-r--r--   0 francispotter   (501) staff       (20)      786 2023-06-19 17:50:27.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/series.html
--rw-r--r--   0 francispotter   (501) staff       (20)      603 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/show_source.html
--rw-r--r--   0 francispotter   (501) staff       (20)     1069 2023-06-19 17:50:58.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/social.html
--rw-r--r--   0 francispotter   (501) staff       (20)      897 2023-06-19 17:50:49.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/tag_cloud.html
--rw-r--r--   0 francispotter   (501) staff       (20)      594 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/twitter_timeline.html
--rw-r--r--   0 francispotter   (501) staff       (20)      811 2023-06-19 17:52:54.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar.html
--rw-r--r--   0 francispotter   (501) staff       (20)      229 2023-06-19 17:45:23.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/taglist.html
--rw-r--r--   0 francispotter   (501) staff       (20)      274 2023-06-19 17:45:34.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/translations.html
--rw-r--r--   0 francispotter   (501) staff       (20)     1164 2023-06-18 20:35:35.000000 pelidoc-0.0.3/pelidoc/theme/templates/includes/twitter_cards.html
--rw-r--r--   0 francispotter   (501) staff       (20)      190 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/templates/index.html
--rw-r--r--   0 francispotter   (501) staff       (20)     2250 2023-06-19 15:35:22.000000 pelidoc-0.0.3/pelidoc/theme/templates/page.html
--rw-r--r--   0 francispotter   (501) staff       (20)      798 2023-06-19 15:28:57.000000 pelidoc-0.0.3/pelidoc/theme/templates/search.html
--rw-r--r--   0 francispotter   (501) staff       (20)      570 2023-06-17 01:11:39.000000 pelidoc-0.0.3/pelidoc/theme/templates/tag.html
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:04:17.832331 pelidoc-0.0.3/pelidoc.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)      414 2023-06-24 05:04:17.000000 pelidoc-0.0.3/pelidoc.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     5840 2023-06-24 05:04:17.000000 pelidoc-0.0.3/pelidoc.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-06-24 05:04:17.000000 pelidoc-0.0.3/pelidoc.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       50 2023-06-24 05:04:17.000000 pelidoc-0.0.3/pelidoc.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       25 2023-06-24 05:04:17.000000 pelidoc-0.0.3/pelidoc.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        8 2023-06-24 05:04:17.000000 pelidoc-0.0.3/pelidoc.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      622 2023-06-24 05:03:11.000000 pelidoc-0.0.3/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-06-24 05:04:18.514836 pelidoc-0.0.3/setup.cfg
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.598318 pelidoc-0.0.5/
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-06-24 05:09:57.000000 pelidoc-0.0.5/.version
+-rw-r--r--   0 francispotter   (501) staff       (20)      414 2023-06-24 05:10:13.597838 pelidoc-0.0.5/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      168 2023-06-24 04:47:30.000000 pelidoc-0.0.5/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.066137 pelidoc-0.0.5/pelidoc/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-06-22 04:34:41.000000 pelidoc-0.0.5/pelidoc/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1209 2023-06-24 04:13:52.000000 pelidoc-0.0.5/pelidoc/conf.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.100740 pelidoc-0.0.5/pelidoc/theme/
+-rw-r--r--   0 francispotter   (501) staff       (20)      799 2023-06-19 17:55:16.000000 pelidoc-0.0.5/pelidoc/theme/AUTHORS.md
+-rw-r--r--   0 francispotter   (501) staff       (20)     1077 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/LICENSE
+-rw-r--r--   0 francispotter   (501) staff       (20)    15125 2023-06-24 02:47:27.000000 pelidoc-0.0.5/pelidoc/theme/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.059553 pelidoc-0.0.5/pelidoc/theme/static/
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.305299 pelidoc-0.0.5/pelidoc/theme/static/css/
+-rw-r--r--   0 francispotter   (501) staff       (20)   120090 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.cerulean.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   119768 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.cosmo.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   109602 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.cupid.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   116696 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.custom.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   119799 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.cyborg.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   121625 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.darkly.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   121354 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.flatly.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   118666 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.journal.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   124431 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.lumen.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   121457 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   132318 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.paper.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   105382 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.readable-old.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   118678 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.readable.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   118965 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.sandstone.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   101587 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.shamrock.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   120186 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.simplex.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   129014 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.slate.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   121499 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.spacelab.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   120731 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.superhero.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   117016 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.united.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)   121865 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.yeti.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)    37414 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/font-awesome.css
+-rw-r--r--   0 francispotter   (501) staff       (20)    21778 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/font-awesome.css.map
+-rw-r--r--   0 francispotter   (501) staff       (20)    31000 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/font-awesome.min.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     6853 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/html4css1.css
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.490588 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/
+-rw-r--r--   0 francispotter   (501) staff       (20)     3875 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/autumn.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     3231 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/borland.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     2255 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/bw.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4527 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/colorful.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4217 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/default.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4216 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/emacs.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4244 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/friendly.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4909 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/fruity.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     3284 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/github.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     1852 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/igor.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4328 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/manni.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     3870 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/monokai.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4569 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/murphy.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4732 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/native.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4019 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/paraiso-dark.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4019 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/paraiso-light.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4622 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/pastie.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     3961 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/perldoc.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     1950 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/rrt.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4310 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/solarizeddark.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4310 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/solarizedlight.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4890 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/tango.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     3987 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/trac.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4447 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/vim.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     2069 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/vs.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     3407 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/xcode.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4370 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/pygments/zenburn.css
+-rw-r--r--   0 francispotter   (501) staff       (20)     4249 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/style.css
+-rw-r--r--   0 francispotter   (501) staff       (20)      190 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/css/typogrify.css
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.529351 pelidoc-0.0.5/pelidoc/theme/static/fonts/
+-rw-r--r--   0 francispotter   (501) staff       (20)   134808 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/fonts/FontAwesome.otf
+-rw-r--r--   0 francispotter   (501) staff       (20)   165742 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 francispotter   (501) staff       (20)   444379 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 francispotter   (501) staff       (20)   165548 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 francispotter   (501) staff       (20)    98024 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 francispotter   (501) staff       (20)    77160 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 francispotter   (501) staff       (20)    20127 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 francispotter   (501) staff       (20)   108738 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 francispotter   (501) staff       (20)    45404 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 francispotter   (501) staff       (20)    23424 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 francispotter   (501) staff       (20)    18028 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.541222 pelidoc-0.0.5/pelidoc/theme/static/js/
+-rw-r--r--   0 francispotter   (501) staff       (20)       95 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/js/bodypadding.js
+-rw-r--r--   0 francispotter   (501) staff       (20)    39680 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/js/bootstrap.min.js
+-rw-r--r--   0 francispotter   (501) staff       (20)     1478 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/js/github.js
+-rw-r--r--   0 francispotter   (501) staff       (20)     2474 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/js/jXHR.js
+-rw-r--r--   0 francispotter   (501) staff       (20)    88145 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/js/jquery.min.js
+-rw-r--r--   0 francispotter   (501) staff       (20)     4047 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/js/respond.min.js
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.546297 pelidoc-0.0.5/pelidoc/theme/static/tipuesearch/
+-rwxr-xr-x   0 francispotter   (501) staff       (20)     6067 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/tipuesearch/tipuesearch.css
+-rw-r--r--   0 francispotter   (501) staff       (20)    33038 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/tipuesearch/tipuesearch.js
+-rw-r--r--   0 francispotter   (501) staff       (20)    10512 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/tipuesearch/tipuesearch.min.js
+-rw-r--r--   0 francispotter   (501) staff       (20)     4797 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/tipuesearch/tipuesearch_content.js
+-rw-r--r--   0 francispotter   (501) staff       (20)     3612 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/static/tipuesearch/tipuesearch_set.js
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.561191 pelidoc-0.0.5/pelidoc/theme/templates/
+-rw-r--r--   0 francispotter   (501) staff       (20)      910 2023-06-19 17:53:48.000000 pelidoc-0.0.5/pelidoc/theme/templates/archives.html
+-rw-r--r--   0 francispotter   (501) staff       (20)     4123 2023-06-19 17:56:28.000000 pelidoc-0.0.5/pelidoc/theme/templates/article.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      820 2023-06-19 17:52:09.000000 pelidoc-0.0.5/pelidoc/theme/templates/article_list.html
+-rw-r--r--   0 francispotter   (501) staff       (20)     8517 2023-06-19 17:56:45.000000 pelidoc-0.0.5/pelidoc/theme/templates/base.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      725 2023-06-19 02:42:12.000000 pelidoc-0.0.5/pelidoc/theme/templates/category.html
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.583913 pelidoc-0.0.5/pelidoc/theme/templates/includes/
+-rw-r--r--   0 francispotter   (501) staff       (20)      610 2023-06-18 20:35:35.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/addthis.html
+-rw-r--r--   0 francispotter   (501) staff       (20)     1692 2023-06-19 15:31:51.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/article_info.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      332 2023-06-18 20:35:35.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/banner.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      336 2023-06-24 02:52:18.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/footer.html
+-rw-r--r--   0 francispotter   (501) staff       (20)     1547 2023-06-18 20:35:35.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/ga.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      448 2023-06-18 20:35:35.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/liquid_tags_nb_footer.html
+-rw-r--r--   0 francispotter   (501) staff       (20)     8765 2023-06-18 20:35:35.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/liquid_tags_nb_header.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      235 2023-06-18 20:35:35.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/minify_tipuesearch.html
+-rw-r--r--   0 francispotter   (501) staff       (20)     1805 2023-06-19 17:45:10.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/pagination.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      851 2023-06-18 20:35:35.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/piwik.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      341 2023-06-18 20:35:35.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/related-posts.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      799 2023-06-18 20:35:35.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/series.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      304 2023-06-18 20:35:35.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/show_source.html
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.596951 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/
+-rw-r--r--   0 francispotter   (501) staff       (20)      908 2023-06-19 17:45:56.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/archive.html
+-rw-r--r--   0 francispotter   (501) staff       (20)       66 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/article-li.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      616 2023-06-19 17:49:44.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/categories.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      497 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/images.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      458 2023-06-19 17:52:32.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/links.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      215 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/macros.jinja
+-rw-r--r--   0 francispotter   (501) staff       (20)     1049 2023-06-18 23:41:20.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/navigation.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      595 2023-06-19 17:51:06.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/recent_posts.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      786 2023-06-19 17:50:27.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/series.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      603 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/show_source.html
+-rw-r--r--   0 francispotter   (501) staff       (20)     1069 2023-06-19 17:50:58.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/social.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      897 2023-06-19 17:50:49.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/tag_cloud.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      594 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/twitter_timeline.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      811 2023-06-19 17:52:54.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      229 2023-06-19 17:45:23.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/taglist.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      274 2023-06-19 17:45:34.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/translations.html
+-rw-r--r--   0 francispotter   (501) staff       (20)     1164 2023-06-18 20:35:35.000000 pelidoc-0.0.5/pelidoc/theme/templates/includes/twitter_cards.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      190 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/templates/index.html
+-rw-r--r--   0 francispotter   (501) staff       (20)     2250 2023-06-19 15:35:22.000000 pelidoc-0.0.5/pelidoc/theme/templates/page.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      798 2023-06-19 15:28:57.000000 pelidoc-0.0.5/pelidoc/theme/templates/search.html
+-rw-r--r--   0 francispotter   (501) staff       (20)      570 2023-06-17 01:11:39.000000 pelidoc-0.0.5/pelidoc/theme/templates/tag.html
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-24 05:10:13.088117 pelidoc-0.0.5/pelidoc.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)      414 2023-06-24 05:10:13.000000 pelidoc-0.0.5/pelidoc.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)     5840 2023-06-24 05:10:13.000000 pelidoc-0.0.5/pelidoc.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-06-24 05:10:13.000000 pelidoc-0.0.5/pelidoc.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       50 2023-06-24 05:10:13.000000 pelidoc-0.0.5/pelidoc.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       41 2023-06-24 05:10:13.000000 pelidoc-0.0.5/pelidoc.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        8 2023-06-24 05:10:13.000000 pelidoc-0.0.5/pelidoc.egg-info/top_level.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)      645 2023-06-24 05:09:37.000000 pelidoc-0.0.5/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-06-24 05:10:13.598441 pelidoc-0.0.5/setup.cfg
```

### Comparing `pelidoc-0.0.3/pelidoc/conf.py` & `pelidoc-0.0.5/pelidoc/conf.py`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/AUTHORS.md` & `pelidoc-0.0.5/pelidoc/theme/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/LICENSE` & `pelidoc-0.0.5/pelidoc/theme/LICENSE`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/README.md` & `pelidoc-0.0.5/pelidoc/theme/README.md`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.cerulean.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.cerulean.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.cosmo.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.cosmo.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.cupid.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.cupid.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.custom.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.custom.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.cyborg.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.cyborg.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.darkly.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.darkly.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.flatly.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.flatly.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.journal.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.journal.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.lumen.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.lumen.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.paper.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.paper.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.readable-old.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.readable-old.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.readable.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.readable.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.sandstone.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.sandstone.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.shamrock.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.shamrock.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.simplex.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.simplex.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.slate.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.slate.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.spacelab.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.spacelab.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.superhero.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.superhero.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.united.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.united.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/bootstrap.yeti.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/bootstrap.yeti.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/font-awesome.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/font-awesome.css.map` & `pelidoc-0.0.5/pelidoc/theme/static/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/font-awesome.min.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/html4css1.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/html4css1.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/autumn.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/autumn.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/borland.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/borland.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/bw.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/bw.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/colorful.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/colorful.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/default.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/default.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/emacs.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/emacs.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/friendly.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/friendly.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/fruity.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/fruity.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/github.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/github.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/igor.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/igor.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/manni.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/manni.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/monokai.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/monokai.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/murphy.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/murphy.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/native.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/native.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/paraiso-dark.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/paraiso-dark.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/paraiso-light.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/paraiso-light.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/pastie.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/pastie.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/perldoc.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/perldoc.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/rrt.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/rrt.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/solarizeddark.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/solarizeddark.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/solarizedlight.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/solarizedlight.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/tango.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/tango.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/trac.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/trac.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/vim.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/vim.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/vs.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/vs.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/xcode.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/xcode.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/pygments/zenburn.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/pygments/zenburn.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/css/style.css` & `pelidoc-0.0.5/pelidoc/theme/static/css/style.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/fonts/FontAwesome.otf` & `pelidoc-0.0.5/pelidoc/theme/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/fonts/fontawesome-webfont.eot` & `pelidoc-0.0.5/pelidoc/theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/fonts/fontawesome-webfont.svg` & `pelidoc-0.0.5/pelidoc/theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/fonts/fontawesome-webfont.ttf` & `pelidoc-0.0.5/pelidoc/theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/fonts/fontawesome-webfont.woff` & `pelidoc-0.0.5/pelidoc/theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/fonts/fontawesome-webfont.woff2` & `pelidoc-0.0.5/pelidoc/theme/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/fonts/glyphicons-halflings-regular.eot` & `pelidoc-0.0.5/pelidoc/theme/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/fonts/glyphicons-halflings-regular.svg` & `pelidoc-0.0.5/pelidoc/theme/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/fonts/glyphicons-halflings-regular.ttf` & `pelidoc-0.0.5/pelidoc/theme/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/fonts/glyphicons-halflings-regular.woff` & `pelidoc-0.0.5/pelidoc/theme/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/fonts/glyphicons-halflings-regular.woff2` & `pelidoc-0.0.5/pelidoc/theme/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/js/bootstrap.min.js` & `pelidoc-0.0.5/pelidoc/theme/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/js/github.js` & `pelidoc-0.0.5/pelidoc/theme/static/js/github.js`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/js/jXHR.js` & `pelidoc-0.0.5/pelidoc/theme/static/js/jXHR.js`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/js/jquery.min.js` & `pelidoc-0.0.5/pelidoc/theme/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/js/respond.min.js` & `pelidoc-0.0.5/pelidoc/theme/static/js/respond.min.js`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/tipuesearch/tipuesearch.css` & `pelidoc-0.0.5/pelidoc/theme/static/tipuesearch/tipuesearch.css`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/tipuesearch/tipuesearch.js` & `pelidoc-0.0.5/pelidoc/theme/static/tipuesearch/tipuesearch.js`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/tipuesearch/tipuesearch.min.js` & `pelidoc-0.0.5/pelidoc/theme/static/tipuesearch/tipuesearch.min.js`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/tipuesearch/tipuesearch_content.js` & `pelidoc-0.0.5/pelidoc/theme/static/tipuesearch/tipuesearch_content.js`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/static/tipuesearch/tipuesearch_set.js` & `pelidoc-0.0.5/pelidoc/theme/static/tipuesearch/tipuesearch_set.js`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/archives.html` & `pelidoc-0.0.5/pelidoc/theme/templates/archives.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/article.html` & `pelidoc-0.0.5/pelidoc/theme/templates/article.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/article_list.html` & `pelidoc-0.0.5/pelidoc/theme/templates/article_list.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/base.html` & `pelidoc-0.0.5/pelidoc/theme/templates/base.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/category.html` & `pelidoc-0.0.5/pelidoc/theme/templates/category.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/addthis.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/addthis.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/article_info.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/article_info.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/ga.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/ga.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/liquid_tags_nb_header.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/liquid_tags_nb_header.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/pagination.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/piwik.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/piwik.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/series.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/series.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/archive.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/archive.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/categories.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/categories.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/navigation.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/navigation.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/recent_posts.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/recent_posts.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/series.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/series.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/show_source.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/show_source.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/social.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/social.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/tag_cloud.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/tag_cloud.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar/twitter_timeline.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar/twitter_timeline.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/sidebar.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/sidebar.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/includes/twitter_cards.html` & `pelidoc-0.0.5/pelidoc/theme/templates/includes/twitter_cards.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/page.html` & `pelidoc-0.0.5/pelidoc/theme/templates/page.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/search.html` & `pelidoc-0.0.5/pelidoc/theme/templates/search.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc/theme/templates/tag.html` & `pelidoc-0.0.5/pelidoc/theme/templates/tag.html`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pelidoc.egg-info/SOURCES.txt` & `pelidoc-0.0.5/pelidoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pelidoc-0.0.3/pyproject.toml` & `pelidoc-0.0.5/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     {name = "Steampunk Wizard", email = "pelidoc@steampunkwizard.ca"}
 ]
 description = "Static site generator for project documentation"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT"}
 dependencies = [
+    "Markdown==3.4.3",
     "pelican[markdown] ==4.8.0"
 ]
 dynamic = ["version"]
 
 [tool.setuptools.package-dir]
 pelidoc = "pelidoc"
```

