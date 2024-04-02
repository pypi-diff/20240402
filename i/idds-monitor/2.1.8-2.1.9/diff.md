# Comparing `tmp/idds-monitor-2.1.8.tar.gz` & `tmp/idds-monitor-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-monitor-2.1.8.tar", last modified: Wed Jan 31 16:35:26 2024, max compression
+gzip compressed data, was "idds-monitor-2.1.9.tar", last modified: Wed Jan 31 17:27:24 2024, max compression
```

## Comparing `idds-monitor-2.1.8.tar` & `idds-monitor-2.1.9.tar`

### file list

```diff
@@ -1,528 +1,528 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.915253 idds-monitor-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-01-31 16:35:26.915253 idds-monitor-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.819252 idds-monitor-2.1.8/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.823253 idds-monitor-2.1.8/data/backup/
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/backup/404.html
--rw-r--r--   0 runner    (1001) docker     (127)    19961 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/backup/basic-table.html
--rw-r--r--   0 runner    (1001) docker     (127)    16624 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/backup/blank.html
--rw-r--r--   0 runner    (1001) docker     (127)    38831 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/backup/dashboard.html.backup
--rw-r--r--   0 runner    (1001) docker     (127)    38831 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/backup/dashboard1.html
--rw-r--r--   0 runner    (1001) docker     (127)   232847 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/backup/fontawesome.html
--rw-r--r--   0 runner    (1001) docker     (127)    22743 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/backup/index.html.back
--rw-r--r--   0 runner    (1001) docker     (127)    59131 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/backup/map-google.html
--rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/backup/profile.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.811252 idds-monitor-2.1.8/data/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.823253 idds-monitor-2.1.8/data/bootstrap/dist/
--rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.831252 idds-monitor-2.1.8/data/bootstrap/dist/css/
--rw-r--r--   0 runner    (1001) docker     (127)    75728 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (127)   184946 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51515 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   115661 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    75801 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   184950 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51590 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   115738 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (127)    94576 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    34718 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)    94589 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    41119 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    71446 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.css
--rw-r--r--   0 runner    (1001) docker     (127)   111059 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    49492 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    28877 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    71303 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   111003 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    49419 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    28850 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   203731 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   500230 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   153117 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   422371 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   202974 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   500122 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   153222 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   622580 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.rtl.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.839253 idds-monitor-2.1.8/data/bootstrap/dist/js/
--rw-r--r--   0 runner    (1001) docker     (127)   216787 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   410135 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    80827 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   318338 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   147542 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.esm.js
--rw-r--r--   0 runner    (1001) docker     (127)   277557 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.esm.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    76585 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.esm.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   217908 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.esm.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   156888 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)   278810 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    62417 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   211771 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-01-31 16:35:26.000000 idds-monitor-2.1.8/data/conf.js
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/conf.js.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.839253 idds-monitor-2.1.8/data/css/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.839253 idds-monitor-2.1.8/data/css/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.811252 idds-monitor-2.1.8/data/css/icons/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.843253 idds-monitor-2.1.8/data/css/icons/font-awesome/css/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/css/fa-brands.css
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/css/fa-brands.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/css/fa-regular.css
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/css/fa-regular.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/css/fa-solid.css
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/css/fa-solid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    48879 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/css/fontawesome-all.css
--rw-r--r--   0 runner    (1001) docker     (127)    36993 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/css/fontawesome-all.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    47300 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/css/fontawesome.css
--rw-r--r--   0 runner    (1001) docker     (127)    35628 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/css/fontawesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.843253 idds-monitor-2.1.8/data/css/icons/font-awesome/less/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/_animated.less
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/_bordered-pulled.less
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/_core.less
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/_fixed-width.less
--rw-r--r--   0 runner    (1001) docker     (127)    59750 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/_icons.less
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/_larger.less
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/_list.less
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/_mixins.less
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/_rotated-flipped.less
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/_screen-reader.less
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/_stacked.less
--rw-r--r--   0 runner    (1001) docker     (127)    25724 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/_variables.less
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/fa-brands.less
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/fa-regular.less
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/fa-solid.less
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/less/fontawesome.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.847253 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_animated.scss
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_bordered-pulled.scss
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_core.scss
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_fixed-width.scss
--rw-r--r--   0 runner    (1001) docker     (127)    71096 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_larger.scss
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_list.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_rotated-flipped.scss
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_screen-reader.scss
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_stacked.scss
--rw-r--r--   0 runner    (1001) docker     (127)    24203 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/fa-brands.scss
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/fa-regular.scss
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/fa-solid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/scss/fontawesome.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.851253 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)    98940 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   510455 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)    98704 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    63904 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    54684 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30788 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   104302 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    14672 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   115152 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (127)   421894 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (127)   114932 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    55484 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (127)    44004 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.811252 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.855253 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/css/
--rw-r--r--   0 runner    (1001) docker     (127)    90505 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.css
--rw-r--r--   0 runner    (1001) docker     (127)    70850 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    77567 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/css/materialdesignicons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.859253 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    42495 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.eot
--rw-r--r--   0 runner    (1001) docker     (127)   239073 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.svg
--rw-r--r--   0 runner    (1001) docker     (127)    99212 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    50312 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff
--rw-r--r--   0 runner    (1001) docker     (127)    38384 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   261608 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)  1985766 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   261388 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   129588 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    99736 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.859253 idds-monitor-2.1.8/data/css/icons/themify-icons/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.859253 idds-monitor-2.1.8/data/css/icons/themify-icons/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    78748 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/themify-icons/fonts/themify.eot
--rw-r--r--   0 runner    (1001) docker     (127)   234630 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/themify-icons/fonts/themify.svg
--rw-r--r--   0 runner    (1001) docker     (127)    78584 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/themify-icons/fonts/themify.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    56108 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/themify-icons/fonts/themify.woff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.859253 idds-monitor-2.1.8/data/css/icons/themify-icons/ie7/
--rw-r--r--   0 runner    (1001) docker     (127)    36547 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/themify-icons/ie7/ie7.css
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/themify-icons/ie7/ie7.js
--rw-r--r--   0 runner    (1001) docker     (127)    17504 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/themify-icons/themify-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/themify-icons/themify-icons.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.811252 idds-monitor-2.1.8/data/css/icons/weather-icons/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.863253 idds-monitor-2.1.8/data/css/icons/weather-icons/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/css/weather-icons-core.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/css/weather-icons-variables.css
--rw-r--r--   0 runner    (1001) docker     (127)   150543 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/css/weather-icons-wind.css
--rw-r--r--   0 runner    (1001) docker     (127)   150543 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/css/weather-icons-wind.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    34012 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/css/weather-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    23146 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/css/weather-icons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.863253 idds-monitor-2.1.8/data/css/icons/weather-icons/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    99774 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   185225 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)    99564 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    56468 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    44720 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.863253 idds-monitor-2.1.8/data/css/icons/weather-icons/less/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.867253 idds-monitor-2.1.8/data/css/icons/weather-icons/less/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/css/variables-beaufort.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/css/variables-day.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/css/variables-direction.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/css/variables-misc.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/css/variables-moon.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/css/variables-neutral.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/css/variables-night.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/css/variables-time.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/css/variables-wind-names.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.867253 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-beaufort.less
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-day.less
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-direction.less
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-misc.less
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-moon-aliases.less
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-moon.less
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-neutral.less
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-night.less
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-time.less
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-wind-aliases.less
--rw-r--r--   0 runner    (1001) docker     (127)    30994 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-wind-degrees.less
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-wind.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.871253 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-beaufort.less
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-day.less
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-direction.less
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-misc.less
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-moon.less
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-neutral.less
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-night.less
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-time.less
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-wind-names.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.871253 idds-monitor-2.1.8/data/css/icons/weather-icons/less/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/mappings/wi-forecast-io.less
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/mappings/wi-owm.less
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/mappings/wi-wmo4680.less
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/mappings/wi-yahoo.less
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/weather-icons-classes.less
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/weather-icons-core.less
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/weather-icons-variables.less
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/weather-icons-wind.less
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/weather-icons-wind.min.less
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/weather-icons.less
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/less/weather-icons.min.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.871253 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.875253 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-beaufort.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-day.scss
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-direction.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-moon-aliases.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-moon.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-neutral.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-night.scss
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-time.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-wind-aliases.scss
--rw-r--r--   0 runner    (1001) docker     (127)    36834 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-wind-degrees.scss
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-wind.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.875253 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-beaufort.scss
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-day.scss
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-direction.scss
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-moon.scss
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-neutral.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-night.scss
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-time.scss
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-wind-names.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.875253 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/mappings/wi-forecast-io.scss
--rw-r--r--   0 runner    (1001) docker     (127)    19614 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/mappings/wi-owm.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/mappings/wi-wmo4680.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/mappings/wi-yahoo.scss
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/weather-icons-classes.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/weather-icons-core.scss
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/weather-icons-variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/weather-icons-wind.min.scss
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/weather-icons-wind.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/weather-icons.min.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/icons/weather-icons/sass/weather-icons.scss
--rw-r--r--   0 runner    (1001) docker     (127)   286030 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/style.extra.css
--rw-r--r--   0 runner    (1001) docker     (127)   245218 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/css/style.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    22026 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)    17695 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/detail_processing.html
--rw-r--r--   0 runner    (1001) docker     (127)    17882 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/detail_request.html
--rw-r--r--   0 runner    (1001) docker     (127)    18238 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/detail_transform.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.875253 idds-monitor-2.1.8/data/js/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/js/app-style-switcher.js
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.815252 idds-monitor-2.1.8/data/js/pages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.879253 idds-monitor-2.1.8/data/js/pages/dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/js/pages/dashboards/dashboard1.js
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/js/pages/dashboards/dashboard1.js.back
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/js/pages/dashboards/dashboard2.js.back
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/js/pages/dashboards/detail_processing.js
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/js/pages/dashboards/detail_request.js
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/js/pages/dashboards/detail_transform.js
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/js/pages/dashboards/processing.js
--rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/js/pages/dashboards/transform.js
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/js/sidebarmenu.js
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/js/waves.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.879253 idds-monitor-2.1.8/data/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.879253 idds-monitor-2.1.8/data/plugins/bower_components/
--rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.815252 idds-monitor-2.1.8/data/plugins/bower_components/chartist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.879253 idds-monitor-2.1.8/data/plugins/bower_components/chartist/dist/
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/chartist/dist/chartist.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    40223 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/chartist/dist/chartist.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.815252 idds-monitor-2.1.8/data/plugins/bower_components/chartist-plugin-tooltips/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.879253 idds-monitor-2.1.8/data/plugins/bower_components/chartist-plugin-tooltips/dist/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.css
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.879253 idds-monitor-2.1.8/data/plugins/bower_components/counterup/
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/counterup/jquery.counterup.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.879253 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/
--rw-r--r--   0 runner    (1001) docker     (127)    61030 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/gmaps.js
--rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/gmaps.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    42062 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/gmaps.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/jquery.gmaps.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.883253 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.controls.js
--rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.core.js
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.events.js
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.geofences.js
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.geometry.js
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.layers.js
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.map_types.js
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.markers.js
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.native_extensions.js
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.overlays.js
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.routes.js
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.static.js
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.streetview.js
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.styles.js
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.815252 idds-monitor-2.1.8/data/plugins/bower_components/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.883253 idds-monitor-2.1.8/data/plugins/bower_components/jquery/dist/
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/jquery/dist/core.js
--rw-r--r--   0 runner    (1001) docker     (127)    86929 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/jquery/dist/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    69919 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/jquery/dist/jquery.slim.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.883253 idds-monitor-2.1.8/data/plugins/bower_components/jquery-datatables/
--rw-r--r--   0 runner    (1001) docker     (127)    14202 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    86549 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.883253 idds-monitor-2.1.8/data/plugins/bower_components/jquery-sparkline/
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/jquery-sparkline/jquery.charts-sparkline.js
--rw-r--r--   0 runner    (1001) docker     (127)    43251 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/jquery-sparkline/jquery.sparkline.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.815252 idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.887253 idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.887253 idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/css/
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/css/perfect-scrollbar.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.887253 idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/js/
--rw-r--r--   0 runner    (1001) docker     (127)    25332 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    25011 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    35899 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.common.js
--rw-r--r--   0 runner    (1001) docker     (127)    35880 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.esm.js
--rw-r--r--   0 runner    (1001) docker     (127)    48633 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    18039 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.815252 idds-monitor-2.1.8/data/plugins/bower_components/popper.js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.887253 idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.887253 idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/esm/
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/esm/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    20319 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/esm/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    21236 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.887253 idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/umd/
--rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/umd/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    25280 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/umd/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.887253 idds-monitor-2.1.8/data/plugins/images/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (127)    14991 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/custom-select.png
--rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/idds.png
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/idds_log.png
--rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/idds_log_text.png
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/idds_log_text1.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.891253 idds-monitor-2.1.8/data/plugins/images/large/
--rw-r--r--   0 runner    (1001) docker     (127)    87878 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/large/img1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    17700 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/logo-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/logo-light-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/logo-light-text.png
--rw-r--r--   0 runner    (1001) docker     (127)    16541 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/logo-text.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.895253 idds-monitor-2.1.8/data/plugins/images/users/
--rw-r--r--   0 runner    (1001) docker     (127)    31418 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/1-old.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/1.png
--rw-r--r--   0 runner    (1001) docker     (127)    75554 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    23280 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/2.png
--rw-r--r--   0 runner    (1001) docker     (127)    43005 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/3.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    21452 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/3.png
--rw-r--r--   0 runner    (1001) docker     (127)    72937 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/4.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    78151 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/5.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    62316 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/6.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    80126 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/7.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    55544 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/8.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/agent.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/agent2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    25255 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/arijit.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    15693 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/d1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/d2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    14875 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/d3.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    16192 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/d4.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/d5.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    25699 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/genu.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    22312 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/govinda.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    21224 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/hritik.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    32130 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/pawandeep.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    32184 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/profile.png
--rw-r--r--   0 runner    (1001) docker     (127)    22359 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/ritesh.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    30783 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/sonu.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    19934 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/plugins/images/users/varun.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    19588 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/processing.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.895253 idds-monitor-2.1.8/data/scss/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.903253 idds-monitor-2.1.8/data/scss/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_accordion.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_button-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_card.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_carousel.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_close.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_containers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_functions.scss
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_helpers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_images.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_modal.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_popover.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)    13603 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_root.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_spinners.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_toasts.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_tooltip.scss
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_transitions.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_type.scss
--rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    59422 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/bootstrap-grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/bootstrap-reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/bootstrap-utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/bootstrap.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.903253 idds-monitor-2.1.8/data/scss/bootstrap/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/forms/_floating-labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/forms/_form-control.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/forms/_form-range.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/forms/_form-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/forms/_labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/forms/_validation.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.907253 idds-monitor-2.1.8/data/scss/bootstrap/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/helpers/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/helpers/_colored-links.scss
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/helpers/_position.scss
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/helpers/_ratio.scss
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/helpers/_stretched-link.scss
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/helpers/_text-truncation.scss
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/helpers/_visually-hidden.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/bootstrap/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_border-radius.scss
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_box-shadow.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_breakpoints.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_caret.scss
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_container.scss
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_deprecate.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_image.scss
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_reset-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_resize.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_table-variants.scss
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_text-truncate.scss
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_transition.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/mixins/_visually-hidden.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/bootstrap/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/utilities/_api.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/bootstrap/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/bootstrap/vendor/_rfs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/components.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/core/
--rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/core/animation/
--rw-r--r--   0 runner    (1001) docker     (127)    56455 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/animation/animation.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/core/breadcrumb/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/breadcrumb/breadcrumb.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/core/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/buttons/buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/core.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/core/extra/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/extra/extra.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/core/layout/
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/layout/layout.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/core/loader/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/loader/spinner.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/core/scafholdings/
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/scafholdings/scafholding.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/core/sidebar/
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/sidebar/sidebar.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/core/topbar/
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/topbar/header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/topbar/notify.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/core/wave-effects/
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/core/wave-effects/wave-effects.scss
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/custom.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/mixins/padding-margin.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/responsive.scss
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/style.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.911253 idds-monitor-2.1.8/data/scss/theme-colors/
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/theme-colors/theme-colors.scss
--rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/variable.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.915253 idds-monitor-2.1.8/data/scss/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/widgets/comments.scss
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/widgets/feeds.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/widgets/profile.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/widgets/steamline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/scss/widgets/widgets.scss
--rw-r--r--   0 runner    (1001) docker     (127)    26819 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/data/transform.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.819252 idds-monitor-2.1.8/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.915253 idds-monitor-2.1.8/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.915253 idds-monitor-2.1.8/lib/idds/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/lib/idds/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 16:35:22.000000 idds-monitor-2.1.8/lib/idds/monitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:26.915253 idds-monitor-2.1.8/lib/idds_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-01-31 16:35:26.000000 idds-monitor-2.1.8/lib/idds_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22199 2024-01-31 16:35:26.000000 idds-monitor-2.1.8/lib/idds_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 16:35:26.000000 idds-monitor-2.1.8/lib/idds_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 16:35:26.000000 idds-monitor-2.1.8/lib/idds_monitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 16:35:26.915253 idds-monitor-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-01-31 16:35:12.000000 idds-monitor-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.185896 idds-monitor-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-01-31 17:27:24.185896 idds-monitor-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.097896 idds-monitor-2.1.9/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.097896 idds-monitor-2.1.9/data/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/backup/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19961 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/backup/basic-table.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16624 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/backup/blank.html
+-rw-r--r--   0 runner    (1001) docker     (127)    38831 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/backup/dashboard.html.backup
+-rw-r--r--   0 runner    (1001) docker     (127)    38831 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/backup/dashboard1.html
+-rw-r--r--   0 runner    (1001) docker     (127)   232847 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/backup/fontawesome.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22743 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/backup/index.html.back
+-rw-r--r--   0 runner    (1001) docker     (127)    59131 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/backup/map-google.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/backup/profile.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.085896 idds-monitor-2.1.9/data/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.097896 idds-monitor-2.1.9/data/bootstrap/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.109896 idds-monitor-2.1.9/data/bootstrap/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    75728 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (127)   184946 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51515 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   115661 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    75801 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   184950 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51590 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   115738 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (127)    94576 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    34718 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)    94589 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    41119 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    71446 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.css
+-rw-r--r--   0 runner    (1001) docker     (127)   111059 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    49492 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    28877 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    71303 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   111003 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    49419 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    28850 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   203731 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   500230 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   153117 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   422371 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   202974 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   500122 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   153222 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   622580 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.rtl.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.113896 idds-monitor-2.1.9/data/bootstrap/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   216787 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   410135 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    80827 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   318338 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   147542 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.esm.js
+-rw-r--r--   0 runner    (1001) docker     (127)   277557 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.esm.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    76585 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.esm.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   217908 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.esm.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   156888 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)   278810 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    62417 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   211771 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-01-31 17:27:24.000000 idds-monitor-2.1.9/data/conf.js
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/conf.js.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.113896 idds-monitor-2.1.9/data/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.113896 idds-monitor-2.1.9/data/css/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.085896 idds-monitor-2.1.9/data/css/icons/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.117896 idds-monitor-2.1.9/data/css/icons/font-awesome/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/css/fa-brands.css
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/css/fa-brands.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/css/fa-regular.css
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/css/fa-regular.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/css/fa-solid.css
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/css/fa-solid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    48879 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/css/fontawesome-all.css
+-rw-r--r--   0 runner    (1001) docker     (127)    36993 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/css/fontawesome-all.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    47300 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/css/fontawesome.css
+-rw-r--r--   0 runner    (1001) docker     (127)    35628 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/css/fontawesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.121896 idds-monitor-2.1.9/data/css/icons/font-awesome/less/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/_animated.less
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/_bordered-pulled.less
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/_core.less
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/_fixed-width.less
+-rw-r--r--   0 runner    (1001) docker     (127)    59750 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/_icons.less
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/_larger.less
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/_list.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/_mixins.less
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/_rotated-flipped.less
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/_screen-reader.less
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/_stacked.less
+-rw-r--r--   0 runner    (1001) docker     (127)    25724 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/_variables.less
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/fa-brands.less
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/fa-regular.less
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/fa-solid.less
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/less/fontawesome.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.121896 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_animated.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_bordered-pulled.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_core.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_fixed-width.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    71096 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_larger.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_list.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_rotated-flipped.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_screen-reader.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_stacked.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    24203 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/fa-brands.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/fa-regular.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/fa-solid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/scss/fontawesome.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.125896 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    98940 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   510455 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    98704 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    63904 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    54684 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30788 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   104302 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    14672 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   115152 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   421894 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   114932 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    55484 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    44004 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.085896 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.125896 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    90505 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.css
+-rw-r--r--   0 runner    (1001) docker     (127)    70850 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    77567 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/css/materialdesignicons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.133896 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    42495 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   239073 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    99212 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    50312 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    38384 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   261608 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)  1985766 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   261388 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   129588 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    99736 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.133896 idds-monitor-2.1.9/data/css/icons/themify-icons/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.133896 idds-monitor-2.1.9/data/css/icons/themify-icons/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    78748 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/themify-icons/fonts/themify.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   234630 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/themify-icons/fonts/themify.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    78584 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/themify-icons/fonts/themify.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    56108 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/themify-icons/fonts/themify.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.133896 idds-monitor-2.1.9/data/css/icons/themify-icons/ie7/
+-rw-r--r--   0 runner    (1001) docker     (127)    36547 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/themify-icons/ie7/ie7.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/themify-icons/ie7/ie7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17504 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/themify-icons/themify-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/themify-icons/themify-icons.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.089896 idds-monitor-2.1.9/data/css/icons/weather-icons/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.137896 idds-monitor-2.1.9/data/css/icons/weather-icons/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/css/weather-icons-core.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/css/weather-icons-variables.css
+-rw-r--r--   0 runner    (1001) docker     (127)   150543 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/css/weather-icons-wind.css
+-rw-r--r--   0 runner    (1001) docker     (127)   150543 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/css/weather-icons-wind.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    34012 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/css/weather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    23146 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/css/weather-icons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.137896 idds-monitor-2.1.9/data/css/icons/weather-icons/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    99774 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   185225 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    99564 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    56468 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    44720 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.137896 idds-monitor-2.1.9/data/css/icons/weather-icons/less/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.141896 idds-monitor-2.1.9/data/css/icons/weather-icons/less/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/css/variables-beaufort.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/css/variables-day.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/css/variables-direction.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/css/variables-misc.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/css/variables-moon.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/css/variables-neutral.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/css/variables-night.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/css/variables-time.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/css/variables-wind-names.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.141896 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-beaufort.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-day.less
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-direction.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-misc.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-moon-aliases.less
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-moon.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-neutral.less
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-night.less
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-time.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-wind-aliases.less
+-rw-r--r--   0 runner    (1001) docker     (127)    30994 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-wind-degrees.less
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-wind.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.145896 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-beaufort.less
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-day.less
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-direction.less
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-misc.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-moon.less
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-neutral.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-night.less
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-time.less
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-wind-names.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.145896 idds-monitor-2.1.9/data/css/icons/weather-icons/less/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/mappings/wi-forecast-io.less
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/mappings/wi-owm.less
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/mappings/wi-wmo4680.less
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/mappings/wi-yahoo.less
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/weather-icons-classes.less
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/weather-icons-core.less
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/weather-icons-variables.less
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/weather-icons-wind.less
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/weather-icons-wind.min.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/weather-icons.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/less/weather-icons.min.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.145896 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.145896 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-beaufort.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-day.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-direction.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-moon-aliases.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-moon.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-neutral.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-night.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-time.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-wind-aliases.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    36834 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-wind-degrees.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-wind.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.149896 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-beaufort.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-day.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-direction.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-moon.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-neutral.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-night.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-time.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-wind-names.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.149896 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/mappings/wi-forecast-io.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    19614 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/mappings/wi-owm.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/mappings/wi-wmo4680.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/mappings/wi-yahoo.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/weather-icons-classes.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/weather-icons-core.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/weather-icons-variables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/weather-icons-wind.min.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/weather-icons-wind.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/weather-icons.min.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/icons/weather-icons/sass/weather-icons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)   286030 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/style.extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)   245218 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/css/style.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    22026 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17695 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/detail_processing.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17882 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/detail_request.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18238 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/detail_transform.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.149896 idds-monitor-2.1.9/data/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/js/app-style-switcher.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.089896 idds-monitor-2.1.9/data/js/pages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.153896 idds-monitor-2.1.9/data/js/pages/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/js/pages/dashboards/dashboard1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/js/pages/dashboards/dashboard1.js.back
+-rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/js/pages/dashboards/dashboard2.js.back
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/js/pages/dashboards/detail_processing.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/js/pages/dashboards/detail_request.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/js/pages/dashboards/detail_transform.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/js/pages/dashboards/processing.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/js/pages/dashboards/transform.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/js/sidebarmenu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/js/waves.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.153896 idds-monitor-2.1.9/data/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.153896 idds-monitor-2.1.9/data/plugins/bower_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.089896 idds-monitor-2.1.9/data/plugins/bower_components/chartist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.153896 idds-monitor-2.1.9/data/plugins/bower_components/chartist/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/chartist/dist/chartist.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    40223 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/chartist/dist/chartist.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.089896 idds-monitor-2.1.9/data/plugins/bower_components/chartist-plugin-tooltips/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.153896 idds-monitor-2.1.9/data/plugins/bower_components/chartist-plugin-tooltips/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.153896 idds-monitor-2.1.9/data/plugins/bower_components/counterup/
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/counterup/jquery.counterup.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.153896 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    61030 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/gmaps.js
+-rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/gmaps.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    42062 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/gmaps.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/jquery.gmaps.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.157896 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.controls.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.core.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.events.js
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.geofences.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.geometry.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.layers.js
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.map_types.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.markers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.native_extensions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.overlays.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.routes.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.static.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.streetview.js
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.styles.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.089896 idds-monitor-2.1.9/data/plugins/bower_components/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.157896 idds-monitor-2.1.9/data/plugins/bower_components/jquery/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/jquery/dist/core.js
+-rw-r--r--   0 runner    (1001) docker     (127)    86929 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/jquery/dist/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    69919 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/jquery/dist/jquery.slim.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.157896 idds-monitor-2.1.9/data/plugins/bower_components/jquery-datatables/
+-rw-r--r--   0 runner    (1001) docker     (127)    14202 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    86549 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.157896 idds-monitor-2.1.9/data/plugins/bower_components/jquery-sparkline/
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/jquery-sparkline/jquery.charts-sparkline.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43251 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/jquery-sparkline/jquery.sparkline.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.089896 idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.157896 idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.157896 idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/css/perfect-scrollbar.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.157896 idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    25332 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25011 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35899 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.common.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35880 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.esm.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48633 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18039 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.089896 idds-monitor-2.1.9/data/plugins/bower_components/popper.js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.161896 idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.161896 idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/esm/
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/esm/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20319 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/esm/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21236 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.161896 idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/umd/
+-rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/umd/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25280 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/umd/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.161896 idds-monitor-2.1.9/data/plugins/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)    14991 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/custom-select.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/idds.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/idds_log.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/idds_log_text.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/idds_log_text1.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.161896 idds-monitor-2.1.9/data/plugins/images/large/
+-rw-r--r--   0 runner    (1001) docker     (127)    87878 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/large/img1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    17700 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/logo-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/logo-light-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/logo-light-text.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16541 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/logo-text.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.169896 idds-monitor-2.1.9/data/plugins/images/users/
+-rw-r--r--   0 runner    (1001) docker     (127)    31418 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/1-old.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    75554 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    23280 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43005 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    21452 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72937 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/4.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    78151 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/5.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    62316 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/6.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    80126 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/7.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    55544 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/8.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/agent.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/agent2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    25255 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/arijit.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    15693 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/d1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/d2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    14875 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/d3.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    16192 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/d4.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/d5.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    25699 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/genu.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    22312 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/govinda.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    21224 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/hritik.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    32130 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/pawandeep.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    32184 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/profile.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22359 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/ritesh.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    30783 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/sonu.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    19934 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/plugins/images/users/varun.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    19588 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/processing.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.169896 idds-monitor-2.1.9/data/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.173896 idds-monitor-2.1.9/data/scss/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_accordion.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_button-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_card.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_carousel.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_close.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_containers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_functions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_helpers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_images.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_modal.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_popover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    13603 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_root.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_spinners.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_toasts.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_tooltip.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_transitions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_type.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    59422 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/bootstrap-grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/bootstrap-reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/bootstrap-utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/bootstrap.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.177897 idds-monitor-2.1.9/data/scss/bootstrap/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/forms/_floating-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/forms/_form-control.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/forms/_form-range.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/forms/_form-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/forms/_labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/forms/_validation.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.177897 idds-monitor-2.1.9/data/scss/bootstrap/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/helpers/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/helpers/_colored-links.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/helpers/_position.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/helpers/_ratio.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/helpers/_stretched-link.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/helpers/_text-truncation.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/helpers/_visually-hidden.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/bootstrap/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_border-radius.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_box-shadow.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_breakpoints.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_caret.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_container.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_deprecate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_reset-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_resize.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_table-variants.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_text-truncate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_transition.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/mixins/_visually-hidden.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/bootstrap/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/utilities/_api.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/bootstrap/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/bootstrap/vendor/_rfs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/components.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/core/animation/
+-rw-r--r--   0 runner    (1001) docker     (127)    56455 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/animation/animation.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/core/breadcrumb/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/breadcrumb/breadcrumb.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/core/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/buttons/buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/core.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/core/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/extra/extra.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/core/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/layout/layout.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/core/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/loader/spinner.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/core/scafholdings/
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/scafholdings/scafholding.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/core/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/sidebar/sidebar.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.181897 idds-monitor-2.1.9/data/scss/core/topbar/
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/topbar/header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/topbar/notify.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.185896 idds-monitor-2.1.9/data/scss/core/wave-effects/
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/core/wave-effects/wave-effects.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/custom.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.185896 idds-monitor-2.1.9/data/scss/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/mixins/padding-margin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/responsive.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/style.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.185896 idds-monitor-2.1.9/data/scss/theme-colors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/theme-colors/theme-colors.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/variable.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.185896 idds-monitor-2.1.9/data/scss/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/widgets/comments.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/widgets/feeds.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/widgets/profile.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/widgets/steamline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/scss/widgets/widgets.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    26819 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/data/transform.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.093896 idds-monitor-2.1.9/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.185896 idds-monitor-2.1.9/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.185896 idds-monitor-2.1.9/lib/idds/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/lib/idds/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 17:27:19.000000 idds-monitor-2.1.9/lib/idds/monitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:24.185896 idds-monitor-2.1.9/lib/idds_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-01-31 17:27:24.000000 idds-monitor-2.1.9/lib/idds_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22199 2024-01-31 17:27:24.000000 idds-monitor-2.1.9/lib/idds_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 17:27:24.000000 idds-monitor-2.1.9/lib/idds_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 17:27:24.000000 idds-monitor-2.1.9/lib/idds_monitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 17:27:24.185896 idds-monitor-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-01-31 17:27:09.000000 idds-monitor-2.1.9/setup.py
```

### Comparing `idds-monitor-2.1.8/PKG-INFO` & `idds-monitor-2.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-monitor
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-monitor-2.1.8/data/backup/404.html` & `idds-monitor-2.1.9/data/backup/404.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/backup/basic-table.html` & `idds-monitor-2.1.9/data/backup/basic-table.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/backup/blank.html` & `idds-monitor-2.1.9/data/backup/blank.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/backup/dashboard.html.backup` & `idds-monitor-2.1.9/data/backup/dashboard.html.backup`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/backup/dashboard1.html` & `idds-monitor-2.1.9/data/backup/dashboard1.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/backup/fontawesome.html` & `idds-monitor-2.1.9/data/backup/fontawesome.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/backup/index.html.back` & `idds-monitor-2.1.9/data/backup/index.html.back`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/backup/map-google.html` & `idds-monitor-2.1.9/data/backup/map-google.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/backup/profile.html` & `idds-monitor-2.1.9/data/backup/profile.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/.DS_Store` & `idds-monitor-2.1.9/data/bootstrap/dist/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.min.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.min.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.rtl.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.rtl.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.min.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.min.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.min.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.min.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.min.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.min.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.rtl.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.rtl.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.rtl.min.css` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/css/bootstrap.rtl.min.css.map` & `idds-monitor-2.1.9/data/bootstrap/dist/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.bundle.js` & `idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.bundle.js.map` & `idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.bundle.min.js` & `idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.bundle.min.js.map` & `idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.esm.js` & `idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.esm.js.map` & `idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.esm.min.js` & `idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.esm.min.js.map` & `idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.js` & `idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.js.map` & `idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.min.js` & `idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/bootstrap/dist/js/bootstrap.min.js.map` & `idds-monitor-2.1.9/data/bootstrap/dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/conf.js.template` & `idds-monitor-2.1.9/data/conf.js.template`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/.DS_Store` & `idds-monitor-2.1.9/data/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/.DS_Store` & `idds-monitor-2.1.9/data/css/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/css/fa-brands.css` & `idds-monitor-2.1.9/data/css/icons/font-awesome/css/fa-brands.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/css/fa-brands.min.css` & `idds-monitor-2.1.9/data/css/icons/font-awesome/css/fa-brands.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/css/fa-regular.css` & `idds-monitor-2.1.9/data/css/icons/font-awesome/css/fa-regular.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/css/fa-regular.min.css` & `idds-monitor-2.1.9/data/css/icons/font-awesome/css/fa-regular.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/css/fa-solid.css` & `idds-monitor-2.1.9/data/css/icons/font-awesome/css/fa-solid.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/css/fa-solid.min.css` & `idds-monitor-2.1.9/data/css/icons/font-awesome/css/fa-solid.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/css/fontawesome-all.css` & `idds-monitor-2.1.9/data/css/icons/font-awesome/css/fontawesome-all.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/css/fontawesome-all.min.css` & `idds-monitor-2.1.9/data/css/icons/font-awesome/css/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/css/fontawesome.css` & `idds-monitor-2.1.9/data/css/icons/font-awesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/css/fontawesome.min.css` & `idds-monitor-2.1.9/data/css/icons/font-awesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/less/_icons.less` & `idds-monitor-2.1.9/data/css/icons/font-awesome/less/_icons.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/less/_mixins.less` & `idds-monitor-2.1.9/data/css/icons/font-awesome/less/_mixins.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/less/_rotated-flipped.less` & `idds-monitor-2.1.9/data/css/icons/font-awesome/less/_rotated-flipped.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/less/_variables.less` & `idds-monitor-2.1.9/data/css/icons/font-awesome/less/_variables.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/less/fa-brands.less` & `idds-monitor-2.1.9/data/css/icons/font-awesome/less/fa-brands.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/less/fa-regular.less` & `idds-monitor-2.1.9/data/css/icons/font-awesome/less/fa-regular.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/less/fa-solid.less` & `idds-monitor-2.1.9/data/css/icons/font-awesome/less/fa-solid.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/less/fontawesome.less` & `idds-monitor-2.1.9/data/css/icons/font-awesome/less/fontawesome.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_icons.scss` & `idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_icons.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_mixins.scss` & `idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_rotated-flipped.scss` & `idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_rotated-flipped.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_stacked.scss` & `idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_stacked.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/scss/_variables.scss` & `idds-monitor-2.1.9/data/css/icons/font-awesome/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/scss/fa-brands.scss` & `idds-monitor-2.1.9/data/css/icons/font-awesome/scss/fa-brands.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/scss/fa-regular.scss` & `idds-monitor-2.1.9/data/css/icons/font-awesome/scss/fa-regular.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/scss/fa-solid.scss` & `idds-monitor-2.1.9/data/css/icons/font-awesome/scss/fa-solid.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-brands-400.eot` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-brands-400.svg` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-brands-400.ttf` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-brands-400.woff` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-brands-400.woff2` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-regular-400.eot` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-regular-400.svg` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-regular-400.ttf` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-regular-400.woff` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-regular-400.woff2` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-solid-900.eot` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-solid-900.svg` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-solid-900.ttf` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-solid-900.woff` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/font-awesome/webfonts/fa-solid-900.woff2` & `idds-monitor-2.1.9/data/css/icons/font-awesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.css` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.min.css` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/css/materialdesignicons.min.css` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/css/materialdesignicons.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.eot` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.svg` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.ttf` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff2` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff2`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.eot` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.svg` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.ttf` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff2` & `idds-monitor-2.1.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff2`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/themify-icons/fonts/themify.eot` & `idds-monitor-2.1.9/data/css/icons/themify-icons/fonts/themify.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/themify-icons/fonts/themify.svg` & `idds-monitor-2.1.9/data/css/icons/themify-icons/fonts/themify.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/themify-icons/fonts/themify.ttf` & `idds-monitor-2.1.9/data/css/icons/themify-icons/fonts/themify.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/themify-icons/fonts/themify.woff` & `idds-monitor-2.1.9/data/css/icons/themify-icons/fonts/themify.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/themify-icons/ie7/ie7.css` & `idds-monitor-2.1.9/data/css/icons/themify-icons/ie7/ie7.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/themify-icons/ie7/ie7.js` & `idds-monitor-2.1.9/data/css/icons/themify-icons/ie7/ie7.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/themify-icons/themify-icons.css` & `idds-monitor-2.1.9/data/css/icons/themify-icons/themify-icons.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/themify-icons/themify-icons.less` & `idds-monitor-2.1.9/data/css/icons/themify-icons/themify-icons.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/css/weather-icons-core.css` & `idds-monitor-2.1.9/data/css/icons/weather-icons/css/weather-icons-core.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/css/weather-icons-wind.css` & `idds-monitor-2.1.9/data/css/icons/weather-icons/css/weather-icons-wind.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/css/weather-icons-wind.min.css` & `idds-monitor-2.1.9/data/css/icons/weather-icons/css/weather-icons-wind.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/css/weather-icons.css` & `idds-monitor-2.1.9/data/css/icons/weather-icons/css/weather-icons.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/css/weather-icons.min.css` & `idds-monitor-2.1.9/data/css/icons/weather-icons/css/weather-icons.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.eot` & `idds-monitor-2.1.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.svg` & `idds-monitor-2.1.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.ttf` & `idds-monitor-2.1.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff` & `idds-monitor-2.1.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff2` & `idds-monitor-2.1.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-beaufort.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-beaufort.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-day.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-day.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-misc.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-misc.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-moon-aliases.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-moon-aliases.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-moon.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-moon.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-neutral.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-neutral.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-night.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-night.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-wind-aliases.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-wind-aliases.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-classes/classes-wind-degrees.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-classes/classes-wind-degrees.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-day.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-day.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-moon.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-moon.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-neutral.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-neutral.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/icon-variables/variables-night.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/icon-variables/variables-night.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/mappings/wi-forecast-io.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/mappings/wi-forecast-io.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/mappings/wi-owm.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/mappings/wi-owm.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/mappings/wi-wmo4680.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/mappings/wi-wmo4680.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/mappings/wi-yahoo.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/mappings/wi-yahoo.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/weather-icons-core.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/weather-icons-core.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/weather-icons.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/weather-icons.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/less/weather-icons.min.less` & `idds-monitor-2.1.9/data/css/icons/weather-icons/less/weather-icons.min.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-beaufort.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-beaufort.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-day.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-day.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-misc.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-misc.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-moon-aliases.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-moon-aliases.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-moon.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-moon.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-neutral.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-neutral.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-night.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-night.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-wind-aliases.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-wind-aliases.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-classes/classes-wind-degrees.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-classes/classes-wind-degrees.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-day.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-day.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-moon.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-moon.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-neutral.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-neutral.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/icon-variables/variables-night.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/icon-variables/variables-night.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/mappings/wi-forecast-io.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/mappings/wi-forecast-io.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/mappings/wi-owm.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/mappings/wi-owm.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/mappings/wi-wmo4680.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/mappings/wi-wmo4680.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/mappings/wi-yahoo.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/mappings/wi-yahoo.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/weather-icons-core.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/weather-icons-core.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/weather-icons.min.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/weather-icons.min.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/icons/weather-icons/sass/weather-icons.scss` & `idds-monitor-2.1.9/data/css/icons/weather-icons/sass/weather-icons.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/style.css` & `idds-monitor-2.1.9/data/css/style.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/style.extra.css` & `idds-monitor-2.1.9/data/css/style.extra.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/css/style.min.css` & `idds-monitor-2.1.9/data/css/style.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/dashboard.html` & `idds-monitor-2.1.9/data/dashboard.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/detail_processing.html` & `idds-monitor-2.1.9/data/detail_processing.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/detail_request.html` & `idds-monitor-2.1.9/data/detail_request.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/detail_transform.html` & `idds-monitor-2.1.9/data/detail_transform.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/js/custom.js` & `idds-monitor-2.1.9/data/js/custom.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/js/pages/dashboards/dashboard1.js` & `idds-monitor-2.1.9/data/js/pages/dashboards/dashboard1.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/js/pages/dashboards/dashboard1.js.back` & `idds-monitor-2.1.9/data/js/pages/dashboards/dashboard1.js.back`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/js/pages/dashboards/dashboard2.js.back` & `idds-monitor-2.1.9/data/js/pages/dashboards/dashboard2.js.back`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/js/pages/dashboards/detail_processing.js` & `idds-monitor-2.1.9/data/js/pages/dashboards/detail_processing.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/js/pages/dashboards/detail_request.js` & `idds-monitor-2.1.9/data/js/pages/dashboards/detail_request.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/js/pages/dashboards/detail_transform.js` & `idds-monitor-2.1.9/data/js/pages/dashboards/detail_transform.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/js/pages/dashboards/processing.js` & `idds-monitor-2.1.9/data/js/pages/dashboards/processing.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/js/pages/dashboards/transform.js` & `idds-monitor-2.1.9/data/js/pages/dashboards/transform.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/js/sidebarmenu.js` & `idds-monitor-2.1.9/data/js/sidebarmenu.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/js/waves.js` & `idds-monitor-2.1.9/data/js/waves.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/.DS_Store` & `idds-monitor-2.1.9/data/plugins/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/.DS_Store` & `idds-monitor-2.1.9/data/plugins/bower_components/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/chartist/dist/chartist.min.css` & `idds-monitor-2.1.9/data/plugins/bower_components/chartist/dist/chartist.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/chartist/dist/chartist.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/chartist/dist/chartist.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.css` & `idds-monitor-2.1.9/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/counterup/jquery.counterup.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/counterup/jquery.counterup.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/gmaps.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/gmaps.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/gmaps.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/gmaps.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/gmaps.min.js.map` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/gmaps.min.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.controls.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.controls.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.core.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.core.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.events.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.events.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.geometry.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.geometry.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.layers.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.layers.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.map_types.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.map_types.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.markers.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.markers.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.native_extensions.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.native_extensions.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.overlays.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.overlays.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.routes.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.routes.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.static.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.static.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.streetview.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.streetview.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/gmaps/lib/gmaps.utils.js` & `idds-monitor-2.1.9/data/plugins/bower_components/gmaps/lib/gmaps.utils.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/jquery/dist/core.js` & `idds-monitor-2.1.9/data/plugins/bower_components/jquery/dist/core.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/jquery/dist/jquery.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/jquery/dist/jquery.slim.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/jquery/dist/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.css` & `idds-monitor-2.1.9/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/jquery-sparkline/jquery.charts-sparkline.js` & `idds-monitor-2.1.9/data/plugins/bower_components/jquery-sparkline/jquery.charts-sparkline.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/jquery-sparkline/jquery.sparkline.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/jquery-sparkline/jquery.sparkline.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/css/perfect-scrollbar.min.css` & `idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/css/perfect-scrollbar.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.jquery.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.jquery.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.common.js` & `idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.common.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.esm.js` & `idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.esm.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.jquery.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.jquery.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/esm/popper-utils.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/esm/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/esm/popper.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/esm/popper.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/popper-utils.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/popper.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/popper.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/umd/popper-utils.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/umd/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/bower_components/popper.js/dist/umd/popper.min.js` & `idds-monitor-2.1.9/data/plugins/bower_components/popper.js/dist/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/.DS_Store` & `idds-monitor-2.1.9/data/plugins/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/custom-select.png` & `idds-monitor-2.1.9/data/plugins/images/custom-select.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/favicon.png` & `idds-monitor-2.1.9/data/plugins/images/favicon.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/idds.png` & `idds-monitor-2.1.9/data/plugins/images/idds.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/idds_log.png` & `idds-monitor-2.1.9/data/plugins/images/idds_log.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/idds_log_text.png` & `idds-monitor-2.1.9/data/plugins/images/idds_log_text.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/idds_log_text1.png` & `idds-monitor-2.1.9/data/plugins/images/idds_log_text1.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/large/img1.jpg` & `idds-monitor-2.1.9/data/plugins/images/large/img1.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/logo-icon.png` & `idds-monitor-2.1.9/data/plugins/images/logo-icon.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/logo-light-icon.png` & `idds-monitor-2.1.9/data/plugins/images/logo-light-icon.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/logo-light-text.png` & `idds-monitor-2.1.9/data/plugins/images/logo-light-text.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/logo-text.png` & `idds-monitor-2.1.9/data/plugins/images/logo-text.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/1-old.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/1-old.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/1.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/1.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/1.png` & `idds-monitor-2.1.9/data/plugins/images/users/1.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/2.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/2.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/2.png` & `idds-monitor-2.1.9/data/plugins/images/users/2.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/3.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/3.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/3.png` & `idds-monitor-2.1.9/data/plugins/images/users/3.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/4.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/4.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/5.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/5.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/6.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/6.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/7.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/7.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/8.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/8.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/agent.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/agent.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/agent2.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/agent2.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/arijit.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/arijit.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/d1.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/d1.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/d2.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/d2.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/d3.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/d3.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/d4.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/d4.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/d5.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/d5.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/genu.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/genu.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/govinda.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/govinda.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/hritik.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/hritik.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/pawandeep.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/pawandeep.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/profile.png` & `idds-monitor-2.1.9/data/plugins/images/users/profile.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/ritesh.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/ritesh.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/sonu.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/sonu.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/plugins/images/users/varun.jpg` & `idds-monitor-2.1.9/data/plugins/images/users/varun.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/processing.html` & `idds-monitor-2.1.9/data/processing.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/.DS_Store` & `idds-monitor-2.1.9/data/scss/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/.DS_Store` & `idds-monitor-2.1.9/data/scss/bootstrap/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_accordion.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_accordion.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_alert.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_alert.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_badge.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_badge.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_breadcrumb.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_button-group.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_button-group.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_buttons.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_card.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_card.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_carousel.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_close.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_containers.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_containers.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_dropdown.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_functions.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_images.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_images.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_list-group.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_mixins.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_modal.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_modal.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_nav.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_nav.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_navbar.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_pagination.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_popover.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_popover.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_progress.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_progress.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_reboot.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_reboot.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_root.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_root.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_spinners.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_spinners.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_tables.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_toasts.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_toasts.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_tooltip.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_type.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_utilities.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/_variables.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/bootstrap-grid.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/bootstrap-reboot.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/bootstrap-reboot.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/bootstrap.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/forms/_floating-labels.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/forms/_form-check.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/forms/_form-control.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/forms/_form-range.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/forms/_form-select.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/forms/_input-group.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/forms/_labels.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/forms/_validation.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/forms/_validation.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/helpers/_position.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_border-radius.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_breakpoints.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_buttons.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_caret.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_deprecate.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_forms.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_gradients.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_grid.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_pagination.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_pagination.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_reset-text.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_reset-text.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_table-variants.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_transition.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_utilities.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/mixins/_visually-hidden.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/utilities/_api.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/bootstrap/vendor/_rfs.scss` & `idds-monitor-2.1.9/data/scss/bootstrap/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/core/.DS_Store` & `idds-monitor-2.1.9/data/scss/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/core/animation/animation.scss` & `idds-monitor-2.1.9/data/scss/core/animation/animation.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/core/breadcrumb/breadcrumb.scss` & `idds-monitor-2.1.9/data/scss/core/breadcrumb/breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/core/buttons/buttons.scss` & `idds-monitor-2.1.9/data/scss/core/buttons/buttons.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/core/extra/extra.scss` & `idds-monitor-2.1.9/data/scss/core/extra/extra.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/core/layout/layout.scss` & `idds-monitor-2.1.9/data/scss/core/layout/layout.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/core/loader/spinner.scss` & `idds-monitor-2.1.9/data/scss/core/loader/spinner.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/core/scafholdings/scafholding.scss` & `idds-monitor-2.1.9/data/scss/core/scafholdings/scafholding.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/core/sidebar/sidebar.scss` & `idds-monitor-2.1.9/data/scss/core/sidebar/sidebar.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/core/topbar/header.scss` & `idds-monitor-2.1.9/data/scss/core/topbar/header.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/core/topbar/notify.scss` & `idds-monitor-2.1.9/data/scss/core/topbar/notify.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/core/wave-effects/wave-effects.scss` & `idds-monitor-2.1.9/data/scss/core/wave-effects/wave-effects.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/mixins/padding-margin.scss` & `idds-monitor-2.1.9/data/scss/mixins/padding-margin.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/responsive.scss` & `idds-monitor-2.1.9/data/scss/responsive.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/style.scss` & `idds-monitor-2.1.9/data/scss/style.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/theme-colors/theme-colors.scss` & `idds-monitor-2.1.9/data/scss/theme-colors/theme-colors.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/variable.scss` & `idds-monitor-2.1.9/data/scss/variable.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/widgets/comments.scss` & `idds-monitor-2.1.9/data/scss/widgets/comments.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/widgets/feeds.scss` & `idds-monitor-2.1.9/data/scss/widgets/feeds.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/widgets/profile.scss` & `idds-monitor-2.1.9/data/scss/widgets/profile.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/scss/widgets/steamline.scss` & `idds-monitor-2.1.9/data/scss/widgets/steamline.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/data/transform.html` & `idds-monitor-2.1.9/data/transform.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/lib/idds_monitor.egg-info/PKG-INFO` & `idds-monitor-2.1.9/lib/idds_monitor.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-monitor
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-monitor-2.1.8/lib/idds_monitor.egg-info/SOURCES.txt` & `idds-monitor-2.1.9/lib/idds_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-monitor-2.1.8/setup.py` & `idds-monitor-2.1.9/setup.py`

 * *Files identical despite different names*

