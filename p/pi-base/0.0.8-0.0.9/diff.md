# Comparing `tmp/pi_base-0.0.8.tar.gz` & `tmp/pi_base-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi_base-0.0.8.tar", last modified: Fri Mar 15 15:19:51 2024, max compression
+gzip compressed data, was "pi_base-0.0.9.tar", last modified: Fri Mar 15 16:27:33 2024, max compression
```

## Comparing `pi_base-0.0.8.tar` & `pi_base-0.0.9.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.443604 pi_base-0.0.8/
--rw-rw-rw-   0        0        0      114 2024-03-15 15:19:46.000000 pi_base-0.0.8/AUTHORS.md
--rw-rw-rw-   0        0        0      835 2024-03-15 15:19:46.000000 pi_base-0.0.8/CHANGELOG.md
--rw-rw-rw-   0        0        0     1090 2024-03-15 15:19:46.000000 pi_base-0.0.8/EXAMPLE_.pypirc
--rw-rw-rw-   0        0        0      227 2024-03-15 15:19:46.000000 pi_base-0.0.8/EXAMPLE_develop.txt
--rw-rw-rw-   0        0        0     1063 2024-03-15 15:19:46.000000 pi_base-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      522 2024-03-15 15:19:46.000000 pi_base-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0    19183 2024-03-15 15:19:51.442603 pi_base-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      345 2024-03-15 15:19:46.000000 pi_base-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.314915 pi_base-0.0.8/blank/
--rw-rw-rw-   0        0        0     1514 2024-03-15 15:19:46.000000 pi_base-0.0.8/blank/README.md
--rw-rw-rw-   0        0        0     5364 2024-03-15 15:19:46.000000 pi_base-0.0.8/blank/blank.py
--rw-rw-rw-   0        0        0      735 2024-03-15 15:19:46.000000 pi_base-0.0.8/blank/conf.yaml
--rw-rw-rw-   0        0        0     6547 2024-03-15 15:19:46.000000 pi_base-0.0.8/blank/install.sh
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.315915 pi_base-0.0.8/blank/pkg/
--rw-rw-rw-   0        0        0        0 2024-03-15 15:19:46.000000 pi_base-0.0.8/blank/pkg/.keep
--rw-rw-rw-   0        0        0       14 2024-03-15 15:19:46.000000 pi_base-0.0.8/blank/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.316914 pi_base-0.0.8/lib/
--rw-rw-rw-   0        0        0        0 2024-03-15 15:19:46.000000 pi_base-0.0.8/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.336640 pi_base-0.0.8/pi_base/
--rw-rw-rw-   0        0        0       64 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/__init__.py
--rw-rw-rw-   0        0        0     2951 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/__main__.py
--rw-rw-rw-   0        0        0      544 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/_version.py
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.350588 pi_base-0.0.8/pi_base/common/
--rw-rw-rw-   0        0        0    22703 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/common_install.sh
--rw-rw-rw-   0        0        0      749 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/common_requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.353588 pi_base-0.0.8/pi_base/common/graphics/
--rw-rw-rw-   0        0        0    22408 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/graphics/splash.pi-base.png
--rw-rw-rw-   0        0        0     3698 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/graphics/splash.pi-base.svg
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.286915 pi_base-0.0.8/pi_base/common/pkg/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.356588 pi_base-0.0.8/pi_base/common/pkg/boot/
--rw-rw-rw-   0        0        0      216 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/boot/cmdline.txt.example
--rw-rw-rw-   0        0        0     2385 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/boot/config.txt
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.368588 pi_base-0.0.8/pi_base/common/pkg/etc/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.279916 pi_base-0.0.8/pi_base/common/pkg/etc/X11/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.370588 pi_base-0.0.8/pi_base/common/pkg/etc/X11/xorg.conf.d/
--rw-rw-rw-   0        0        0      247 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/X11/xorg.conf.d/10-blanking.conf
--rw-rw-rw-   0        0        0    46707 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/boot.jpg
--rw-rw-rw-   0        0        0  3463962 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/boot.wav
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.374597 pi_base-0.0.8/pi_base/common/pkg/etc/default/
--rw-rw-rw-   0        0        0       79 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/default/keyboard
--rw-rw-rw-   0        0        0       52 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/default/locale
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.375588 pi_base-0.0.8/pi_base/common/pkg/etc/lightdm/
--rw-rw-rw-   0        0        0        0 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/lightdm/.keep
--rw-rw-rw-   0        0        0     9372 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/locale.gen
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.376588 pi_base-0.0.8/pi_base/common/pkg/etc/samba/
--rw-rw-rw-   0        0        0     8798 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/samba/smb.conf.example
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.282915 pi_base-0.0.8/pi_base/common/pkg/etc/systemd/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.384588 pi_base-0.0.8/pi_base/common/pkg/etc/systemd/system/
--rw-rw-rw-   0        0        0     2343 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/systemd/system/app_manager_startup.service
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.385588 pi_base-0.0.8/pi_base/common/pkg/etc/systemd/system/getty@tty1.service.d/
--rw-rw-rw-   0        0        0        0 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/systemd/system/getty@tty1.service.d/.keep
--rw-rw-rw-   0        0        0      470 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/systemd/system/hdmi-sound-rpi3.target
--rw-rw-rw-   0        0        0      478 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/systemd/system/hdmi-sound-rpi4-c1.target
--rw-rw-rw-   0        0        0      478 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/systemd/system/hdmi-sound-rpi4-c2.target
--rw-rw-rw-   0        0        0      158 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/systemd/system/hdmi-sound.target
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.283915 pi_base-0.0.8/pi_base/common/pkg/etc/udev/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.387588 pi_base-0.0.8/pi_base/common/pkg/etc/udev/rules.d/
--rw-rw-rw-   0        0        0       63 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/udev/rules.d/60-watchdog.rules
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.389592 pi_base-0.0.8/pi_base/common/pkg/etc/wpa_supplicant/
--rw-rw-rw-   0        0        0      146 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/etc/wpa_supplicant/EXAMPLE_wpa_supplicant.conf
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.285915 pi_base-0.0.8/pi_base/common/pkg/home/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.392591 pi_base-0.0.8/pi_base/common/pkg/home/pi/
--rw-rw-rw-   0        0        0      299 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/home/pi/.bash_aliases
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.285915 pi_base-0.0.8/pi_base/common/pkg/home/pi/.config/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.393588 pi_base-0.0.8/pi_base/common/pkg/home/pi/.config/pulse/
--rw-rw-rw-   0        0        0        0 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/home/pi/.config/pulse/.keep
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.395587 pi_base-0.0.8/pi_base/common/pkg/home/pi/.ssh/
--rw-rw-rw-   0        0        0      399 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/home/pi/.ssh/authorized_keys
--rw-rw-rw-   0        0        0    33202 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/home/pi/block_xxl.flf
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.289915 pi_base-0.0.8/pi_base/common/pkg/usr/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.287915 pi_base-0.0.8/pi_base/common/pkg/usr/lib/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.287915 pi_base-0.0.8/pi_base/common/pkg/usr/lib/systemd/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.397587 pi_base-0.0.8/pi_base/common/pkg/usr/lib/systemd/system/
--rw-rw-rw-   0        0        0        0 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/usr/lib/systemd/system/.keep
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.288915 pi_base-0.0.8/pi_base/common/pkg/usr/local/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.398588 pi_base-0.0.8/pi_base/common/pkg/usr/local/bin/
--rw-rw-rw-   0        0        0     4326 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/usr/local/bin/app_manager_startup
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.289915 pi_base-0.0.8/pi_base/common/pkg/usr/share/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.289915 pi_base-0.0.8/pi_base/common/pkg/usr/share/plymouth/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.290915 pi_base-0.0.8/pi_base/common/pkg/usr/share/plymouth/themes/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.406587 pi_base-0.0.8/pi_base/common/pkg/usr/share/plymouth/themes/pix/
--rw-rw-rw-   0        0        0      187 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/usr/share/plymouth/themes/pix/pix.plymouth
--rw-rw-rw-   0        0        0     1477 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/usr/share/plymouth/themes/pix/pix.script
--rw-rw-rw-   0        0        0   196785 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/usr/share/plymouth/themes/pix/splash-power-off.png
--rw-rw-rw-   0        0        0   195321 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/common/pkg/usr/share/plymouth/themes/pix/splash-power-on.png
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.431588 pi_base-0.0.8/pi_base/lib/
--rw-rw-rw-   0        0        0        0 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/__init__.py
--rw-rw-rw-   0        0        0    18932 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/app_utils.py
--rw-rw-rw-   0        0        0    13186 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/deploy_site.py
--rw-rw-rw-   0        0        0    24471 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/gd_service.py
--rw-rw-rw-   0        0        0     4580 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/large.py
--rw-rw-rw-   0        0        0     3813 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/large.txt
--rw-rw-rw-   0        0        0    15804 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/loggr.py
--rw-rw-rw-   0        0        0     8910 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/manager.py
--rw-rw-rw-   0        0        0     5893 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/os_utils.py
--rw-rw-rw-   0        0        0      758 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/printer-print.sh
--rw-rw-rw-   0        0        0    36668 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/printer.py
--rw-rw-rw-   0        0        0    24136 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/remoteiot.py
--rw-rw-rw-   0        0        0     5798 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/tput.py
--rw-rw-rw-   0        0        0     6198 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/winserial.py
--rw-rw-rw-   0        0        0     9578 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/lib/zpl.ppd
--rw-rw-rw-   0        0        0    17160 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/make.py
--rw-rw-rw-   0        0        0    12984 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/modpath.py
--rwxrwxrwx   0        0        0     1306 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/net_rpi.cmd
--rw-rw-rw-   0        0        0       13 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/requirements-posix.txt
--rw-rw-rw-   0        0        0       14 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/requirements-win.txt
--rw-rw-rw-   0        0        0      530 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.437603 pi_base-0.0.8/pi_base/tests/
--rw-rw-rw-   0        0        0        0 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/tests/__init__.py
--rw-rw-rw-   0        0        0       96 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/tests/test_with_pytest.py
--rw-rw-rw-   0        0        0      352 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/tests/test_with_unittest.py
--rwxrwxrwx   0        0        0     2665 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/upload.cmd
--rw-rw-rw-   0        0        0    16821 2024-03-15 15:19:46.000000 pi_base-0.0.8/pi_base/upload.sh
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.347574 pi_base-0.0.8/pi_base.egg-info/
--rw-rw-rw-   0        0        0    19183 2024-03-15 15:19:51.000000 pi_base-0.0.8/pi_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2730 2024-03-15 15:19:51.000000 pi_base-0.0.8/pi_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 15:19:51.000000 pi_base-0.0.8/pi_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2024-03-15 15:19:51.000000 pi_base-0.0.8/pi_base.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      835 2024-03-15 15:19:51.000000 pi_base-0.0.8/pi_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-15 15:19:51.000000 pi_base-0.0.8/pi_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12044 2024-03-15 15:19:47.000000 pi_base-0.0.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-15 15:19:51.439621 pi_base-0.0.8/secrets/
--rw-rw-rw-   0        0        0      505 2024-03-15 15:19:47.000000 pi_base-0.0.8/secrets/EXAMPLE_remote_secrets.yaml
--rw-rw-rw-   0        0        0       42 2024-03-15 15:19:51.444603 pi_base-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     6255 2024-03-15 15:19:47.000000 pi_base-0.0.8/tox.ini
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.576770 pi_base-0.0.9/
+-rw-rw-rw-   0        0        0      114 2024-03-15 16:27:25.000000 pi_base-0.0.9/AUTHORS.md
+-rw-rw-rw-   0        0        0      889 2024-03-15 16:27:25.000000 pi_base-0.0.9/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1090 2024-03-15 16:27:25.000000 pi_base-0.0.9/EXAMPLE_.pypirc
+-rw-rw-rw-   0        0        0      227 2024-03-15 16:27:25.000000 pi_base-0.0.9/EXAMPLE_develop.txt
+-rw-rw-rw-   0        0        0     1063 2024-03-15 16:27:25.000000 pi_base-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      522 2024-03-15 16:27:25.000000 pi_base-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    19183 2024-03-15 16:27:33.575770 pi_base-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2024-03-15 16:27:25.000000 pi_base-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.438266 pi_base-0.0.9/blank/
+-rw-rw-rw-   0        0        0     1514 2024-03-15 16:27:25.000000 pi_base-0.0.9/blank/README.md
+-rw-rw-rw-   0        0        0     5364 2024-03-15 16:27:25.000000 pi_base-0.0.9/blank/blank.py
+-rw-rw-rw-   0        0        0      735 2024-03-15 16:27:25.000000 pi_base-0.0.9/blank/conf.yaml
+-rw-rw-rw-   0        0        0     6547 2024-03-15 16:27:25.000000 pi_base-0.0.9/blank/install.sh
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.439241 pi_base-0.0.9/blank/pkg/
+-rw-rw-rw-   0        0        0        0 2024-03-15 16:27:25.000000 pi_base-0.0.9/blank/pkg/.keep
+-rw-rw-rw-   0        0        0       14 2024-03-15 16:27:25.000000 pi_base-0.0.9/blank/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.441240 pi_base-0.0.9/lib/
+-rw-rw-rw-   0        0        0        0 2024-03-15 16:27:26.000000 pi_base-0.0.9/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.457965 pi_base-0.0.9/pi_base/
+-rw-rw-rw-   0        0        0       64 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/__init__.py
+-rw-rw-rw-   0        0        0     2951 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/__main__.py
+-rw-rw-rw-   0        0        0      544 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/_version.py
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.473146 pi_base-0.0.9/pi_base/common/
+-rw-rw-rw-   0        0        0    22703 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/common_install.sh
+-rw-rw-rw-   0        0        0      752 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/common_requirements.txt
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.477146 pi_base-0.0.9/pi_base/common/graphics/
+-rw-rw-rw-   0        0        0    22408 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/graphics/splash.pi-base.png
+-rw-rw-rw-   0        0        0     3698 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/graphics/splash.pi-base.svg
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.411240 pi_base-0.0.9/pi_base/common/pkg/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.481146 pi_base-0.0.9/pi_base/common/pkg/boot/
+-rw-rw-rw-   0        0        0      216 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/boot/cmdline.txt.example
+-rw-rw-rw-   0        0        0     2385 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/boot/config.txt
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.493147 pi_base-0.0.9/pi_base/common/pkg/etc/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.403240 pi_base-0.0.9/pi_base/common/pkg/etc/X11/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.495146 pi_base-0.0.9/pi_base/common/pkg/etc/X11/xorg.conf.d/
+-rw-rw-rw-   0        0        0      247 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/X11/xorg.conf.d/10-blanking.conf
+-rw-rw-rw-   0        0        0    46707 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/boot.jpg
+-rw-rw-rw-   0        0        0  3463962 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/boot.wav
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.499148 pi_base-0.0.9/pi_base/common/pkg/etc/default/
+-rw-rw-rw-   0        0        0       79 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/default/keyboard
+-rw-rw-rw-   0        0        0       52 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/default/locale
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.501148 pi_base-0.0.9/pi_base/common/pkg/etc/lightdm/
+-rw-rw-rw-   0        0        0        0 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/lightdm/.keep
+-rw-rw-rw-   0        0        0     9372 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/locale.gen
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.503146 pi_base-0.0.9/pi_base/common/pkg/etc/samba/
+-rw-rw-rw-   0        0        0     8798 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/samba/smb.conf.example
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.406240 pi_base-0.0.9/pi_base/common/pkg/etc/systemd/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.516145 pi_base-0.0.9/pi_base/common/pkg/etc/systemd/system/
+-rw-rw-rw-   0        0        0     2343 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/systemd/system/app_manager_startup.service
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.518148 pi_base-0.0.9/pi_base/common/pkg/etc/systemd/system/getty@tty1.service.d/
+-rw-rw-rw-   0        0        0        0 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/systemd/system/getty@tty1.service.d/.keep
+-rw-rw-rw-   0        0        0      470 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/systemd/system/hdmi-sound-rpi3.target
+-rw-rw-rw-   0        0        0      478 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/systemd/system/hdmi-sound-rpi4-c1.target
+-rw-rw-rw-   0        0        0      478 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/systemd/system/hdmi-sound-rpi4-c2.target
+-rw-rw-rw-   0        0        0      158 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/systemd/system/hdmi-sound.target
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.407240 pi_base-0.0.9/pi_base/common/pkg/etc/udev/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.519147 pi_base-0.0.9/pi_base/common/pkg/etc/udev/rules.d/
+-rw-rw-rw-   0        0        0       63 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/udev/rules.d/60-watchdog.rules
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.521169 pi_base-0.0.9/pi_base/common/pkg/etc/wpa_supplicant/
+-rw-rw-rw-   0        0        0      146 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/etc/wpa_supplicant/EXAMPLE_wpa_supplicant.conf
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.409241 pi_base-0.0.9/pi_base/common/pkg/home/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.524146 pi_base-0.0.9/pi_base/common/pkg/home/pi/
+-rw-rw-rw-   0        0        0      299 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/home/pi/.bash_aliases
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.409241 pi_base-0.0.9/pi_base/common/pkg/home/pi/.config/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.527174 pi_base-0.0.9/pi_base/common/pkg/home/pi/.config/pulse/
+-rw-rw-rw-   0        0        0        0 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/home/pi/.config/pulse/.keep
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.528147 pi_base-0.0.9/pi_base/common/pkg/home/pi/.ssh/
+-rw-rw-rw-   0        0        0      399 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/home/pi/.ssh/authorized_keys
+-rw-rw-rw-   0        0        0    33202 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/home/pi/block_xxl.flf
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.413240 pi_base-0.0.9/pi_base/common/pkg/usr/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.411240 pi_base-0.0.9/pi_base/common/pkg/usr/lib/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.411240 pi_base-0.0.9/pi_base/common/pkg/usr/lib/systemd/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.530151 pi_base-0.0.9/pi_base/common/pkg/usr/lib/systemd/system/
+-rw-rw-rw-   0        0        0        0 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/usr/lib/systemd/system/.keep
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.412240 pi_base-0.0.9/pi_base/common/pkg/usr/local/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.532148 pi_base-0.0.9/pi_base/common/pkg/usr/local/bin/
+-rw-rw-rw-   0        0        0     4326 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/usr/local/bin/app_manager_startup
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.413240 pi_base-0.0.9/pi_base/common/pkg/usr/share/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.413240 pi_base-0.0.9/pi_base/common/pkg/usr/share/plymouth/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.413240 pi_base-0.0.9/pi_base/common/pkg/usr/share/plymouth/themes/
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.540296 pi_base-0.0.9/pi_base/common/pkg/usr/share/plymouth/themes/pix/
+-rw-rw-rw-   0        0        0      187 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/usr/share/plymouth/themes/pix/pix.plymouth
+-rw-rw-rw-   0        0        0     1477 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/usr/share/plymouth/themes/pix/pix.script
+-rw-rw-rw-   0        0        0   196785 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/usr/share/plymouth/themes/pix/splash-power-off.png
+-rw-rw-rw-   0        0        0   195321 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/common/pkg/usr/share/plymouth/themes/pix/splash-power-on.png
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.568092 pi_base-0.0.9/pi_base/lib/
+-rw-rw-rw-   0        0        0        0 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/__init__.py
+-rw-rw-rw-   0        0        0    18932 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/app_utils.py
+-rw-rw-rw-   0        0        0    13186 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/deploy_site.py
+-rw-rw-rw-   0        0        0    24471 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/gd_service.py
+-rw-rw-rw-   0        0        0     4580 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/large.py
+-rw-rw-rw-   0        0        0     3813 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/large.txt
+-rw-rw-rw-   0        0        0    15804 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/loggr.py
+-rw-rw-rw-   0        0        0     8910 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/manager.py
+-rw-rw-rw-   0        0        0     5893 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/os_utils.py
+-rw-rw-rw-   0        0        0      758 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/printer-print.sh
+-rw-rw-rw-   0        0        0    36668 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/printer.py
+-rw-rw-rw-   0        0        0    24136 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/remoteiot.py
+-rw-rw-rw-   0        0        0     5798 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/tput.py
+-rw-rw-rw-   0        0        0     6198 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/winserial.py
+-rw-rw-rw-   0        0        0     9578 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/lib/zpl.ppd
+-rw-rw-rw-   0        0        0    17160 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/make.py
+-rw-rw-rw-   0        0        0    13945 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/modpath.py
+-rwxrwxrwx   0        0        0     1306 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/net_rpi.cmd
+-rw-rw-rw-   0        0        0       13 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/requirements-posix.txt
+-rw-rw-rw-   0        0        0       14 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/requirements-win.txt
+-rw-rw-rw-   0        0        0      530 2024-03-15 16:27:26.000000 pi_base-0.0.9/pi_base/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.572770 pi_base-0.0.9/pi_base/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-15 16:27:27.000000 pi_base-0.0.9/pi_base/tests/__init__.py
+-rw-rw-rw-   0        0        0       96 2024-03-15 16:27:27.000000 pi_base-0.0.9/pi_base/tests/test_with_pytest.py
+-rw-rw-rw-   0        0        0      352 2024-03-15 16:27:27.000000 pi_base-0.0.9/pi_base/tests/test_with_unittest.py
+-rwxrwxrwx   0        0        0     2665 2024-03-15 16:27:27.000000 pi_base-0.0.9/pi_base/upload.cmd
+-rw-rw-rw-   0        0        0    16821 2024-03-15 16:27:27.000000 pi_base-0.0.9/pi_base/upload.sh
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.469147 pi_base-0.0.9/pi_base.egg-info/
+-rw-rw-rw-   0        0        0    19183 2024-03-15 16:27:33.000000 pi_base-0.0.9/pi_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2730 2024-03-15 16:27:33.000000 pi_base-0.0.9/pi_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-15 16:27:33.000000 pi_base-0.0.9/pi_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2024-03-15 16:27:33.000000 pi_base-0.0.9/pi_base.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      835 2024-03-15 16:27:33.000000 pi_base-0.0.9/pi_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-03-15 16:27:33.000000 pi_base-0.0.9/pi_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12044 2024-03-15 16:27:27.000000 pi_base-0.0.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-03-15 16:27:33.573774 pi_base-0.0.9/secrets/
+-rw-rw-rw-   0        0        0      505 2024-03-15 16:27:27.000000 pi_base-0.0.9/secrets/EXAMPLE_remote_secrets.yaml
+-rw-rw-rw-   0        0        0       42 2024-03-15 16:27:33.577772 pi_base-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     6255 2024-03-15 16:27:27.000000 pi_base-0.0.9/tox.ini
```

### Comparing `pi_base-0.0.8/CHANGELOG.md` & `pi_base-0.0.9/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.0.9 (2024-03-15)
+
+* Fix modpath on Windows.
+
 ## 0.0.8 (2024-03-15)
 
 * Bugfixes in pi_base/modpath.py.
 
 ## 0.0.7 (2024-03-14)
 
 * Redo heuristics logic in pi_base/modpath.py.
```

### Comparing `pi_base-0.0.8/EXAMPLE_.pypirc` & `pi_base-0.0.9/EXAMPLE_.pypirc`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/LICENSE` & `pi_base-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/MANIFEST.in` & `pi_base-0.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/PKG-INFO` & `pi_base-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi_base
-Version: 0.0.8
+Version: 0.0.9
 Summary: Framework for creating Raspberry Pi appliances.
 Author-email: Ilya Ivanchenko <iva2k@yahoo.com>
 License: MIT License
         
         Copyright (c) 2023 Ilya I
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pi_base-0.0.8/blank/README.md` & `pi_base-0.0.9/blank/README.md`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/blank/blank.py` & `pi_base-0.0.9/blank/blank.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/blank/conf.yaml` & `pi_base-0.0.9/blank/conf.yaml`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/blank/install.sh` & `pi_base-0.0.9/blank/install.sh`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/__main__.py` & `pi_base-0.0.9/pi_base/__main__.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/_version.py` & `pi_base-0.0.9/pi_base/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 import argparse
 import sys
 # import zest.releaser
 
 
 # Do not edit this line:
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 # instead, use commands from zest.releaser
 
 
 def main():
     parser = argparse.ArgumentParser("Version module for package pi_base")
     parser.add_argument("command", help="Command", choices=["current"])
     args = parser.parse_args()
```

### Comparing `pi_base-0.0.8/pi_base/common/common_install.sh` & `pi_base-0.0.9/pi_base/common/common_install.sh`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/common_requirements.txt` & `pi_base-0.0.9/pi_base/common/common_requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # TODO: (now) Update this version number along with _version.py:
-pi_base>=0.0.8
+pi_base>=0.0.10
 # For now will use ">=" instead of "=="
 
+pyyaml~=6.0
+semver~=2.13.0
+
+#bleak==0.19.5
+#pyserial~=3.5
+
 #esptool==3.3
-bleak==0.19.5
 #coolname==2.2.0
 #fpdf~=1.7.2
 # Gooey~=1.0.8.1 # This pulls in `pip install wxpython>=4.1.0`, which involves compiling a ton of files that takes forever.
 #inquirer~=2.9.2
 #Pillow~=9.1.0
 #qrcode~=7.3.1
 #pyinstaller==5.7.0
 #pexpect~=4.8.0
 #pyinspect
-
-semver~=2.13.0
-pyserial~=3.5
-pyyaml~=6.0
-
 #slack_sdk~=3.21.0
 
 #? pyzmq
 
 # Linux only:
 # systemd~=0.16.1  # Install fails on 64-bit Rapberry OS. Instead use `apt-get install python3-systemd` in common_install.sh
 # systemd-python # Requires some apt packages so it could build. Instead use apt package 'python3-systemd`
```

### Comparing `pi_base-0.0.8/pi_base/common/graphics/splash.pi-base.png` & `pi_base-0.0.9/pi_base/common/graphics/splash.pi-base.png`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/graphics/splash.pi-base.svg` & `pi_base-0.0.9/pi_base/common/graphics/splash.pi-base.svg`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/pkg/boot/config.txt` & `pi_base-0.0.9/pi_base/common/pkg/boot/config.txt`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/pkg/etc/boot.jpg` & `pi_base-0.0.9/pi_base/common/pkg/etc/boot.jpg`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/pkg/etc/boot.wav` & `pi_base-0.0.9/pi_base/common/pkg/etc/boot.wav`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/pkg/etc/locale.gen` & `pi_base-0.0.9/pi_base/common/pkg/etc/locale.gen`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/pkg/etc/samba/smb.conf.example` & `pi_base-0.0.9/pi_base/common/pkg/etc/samba/smb.conf.example`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/pkg/etc/systemd/system/app_manager_startup.service` & `pi_base-0.0.9/pi_base/common/pkg/etc/systemd/system/app_manager_startup.service`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/pkg/home/pi/block_xxl.flf` & `pi_base-0.0.9/pi_base/common/pkg/home/pi/block_xxl.flf`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/pkg/usr/local/bin/app_manager_startup` & `pi_base-0.0.9/pi_base/common/pkg/usr/local/bin/app_manager_startup`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/pkg/usr/share/plymouth/themes/pix/pix.script` & `pi_base-0.0.9/pi_base/common/pkg/usr/share/plymouth/themes/pix/pix.script`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/pkg/usr/share/plymouth/themes/pix/splash-power-off.png` & `pi_base-0.0.9/pi_base/common/pkg/usr/share/plymouth/themes/pix/splash-power-off.png`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/common/pkg/usr/share/plymouth/themes/pix/splash-power-on.png` & `pi_base-0.0.9/pi_base/common/pkg/usr/share/plymouth/themes/pix/splash-power-on.png`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/app_utils.py` & `pi_base-0.0.9/pi_base/lib/app_utils.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/deploy_site.py` & `pi_base-0.0.9/pi_base/lib/deploy_site.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/gd_service.py` & `pi_base-0.0.9/pi_base/lib/gd_service.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/large.py` & `pi_base-0.0.9/pi_base/lib/large.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/large.txt` & `pi_base-0.0.9/pi_base/lib/large.txt`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/loggr.py` & `pi_base-0.0.9/pi_base/lib/loggr.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/manager.py` & `pi_base-0.0.9/pi_base/lib/manager.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/os_utils.py` & `pi_base-0.0.9/pi_base/lib/os_utils.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/printer-print.sh` & `pi_base-0.0.9/pi_base/lib/printer-print.sh`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/printer.py` & `pi_base-0.0.9/pi_base/lib/printer.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/remoteiot.py` & `pi_base-0.0.9/pi_base/lib/remoteiot.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/tput.py` & `pi_base-0.0.9/pi_base/lib/tput.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/winserial.py` & `pi_base-0.0.9/pi_base/lib/winserial.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/lib/zpl.ppd` & `pi_base-0.0.9/pi_base/lib/zpl.ppd`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/make.py` & `pi_base-0.0.9/pi_base/make.py`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/modpath.py` & `pi_base-0.0.9/pi_base/modpath.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 Exports:
 - app_dir             (str): Location of the app main script and app data files.
 - app_conf_dir        (str): Location of the app configuration file app_conf.yaml (for dev: it is generated by `pi_base make`)
 - app_shared_lib_dir  (str): Location of lib (common modules from app_workspace/lib shared by all app projects in the app workspace, on the target location of all copied modules)
 - testscript_dir      (str): Location of tester script .csv files
 - results_dir         (str): Location where to save result files
-- running_on          (str): Detected environment, one of ['target', 'sources', 'pibase_sources', 'build']
+- running_on          (str): Detected environment, one of ['target', 'sources', 'pibase_sources_in_app_workspace', 'pibase_sources', 'build']
 - workspace_dir       (str): Location of package workspace (for dev)
 - module_dirname      (str): Location of this module / script
 - site_id             (str): What site ID to use (for dev)
 - project             (str): What project name to use (for dev)
 
 Functions:
 - is_raspberrypi()
@@ -107,21 +107,21 @@
     return sys.platform == "darwin"
 
 
 def is_win() -> bool:
     return os.name == "nt"
 
 
-def get_top_module() -> tuple[str, str]:
+def get_top_module() -> tuple[str, str, str]:
     # import __main__ as m  # pylint: disable=import-outside-toplevel
     m = sys.modules["__main__"]
     top_filename = (m.__file__ if hasattr(m, "__file__") else None) or sys.argv[0]
     top_module_path = os.path.dirname(os.path.realpath(top_filename))
     top_module_name = os.path.splitext(os.path.basename(top_filename))[0]
-    return top_module_path, top_module_name
+    return top_filename, top_module_path, top_module_name
 
 
 def get_script_dir(file_or_object_or_func: str | inspect._SourceObjectType, follow_symlinks: bool = True) -> str:
     if not file_or_object_or_func:
         raise ValueError("Please provide file_or_object_or_func argument (can be __file__).")
     if getattr(sys, "frozen", False):  # py2exe, PyInstaller, cx_Freeze
         path = os.path.realpath(sys.executable)
@@ -179,21 +179,26 @@
     my_vars = [
         "__file__",
         "__name__",
         "running_on",
         "workspace_dir",
         "module_path",
         "module_dirname",
+        "module_is_from_editable",
         "module_is_from_package",
-        "in_pibase_source",
-        "project_dir",
-        "_app_workspace_path",
+        "app_filename",
         "app_module_path",
         "app_module_dir",
         "app_module_name",
+        "is_pibase_script",
+        "in_pibase_source",
+        "project_dir",
+        "caller_dir",
+        "caller_has_develop_file",
+        "_app_workspace_path",
         "app_dir",
         "app_conf_dir",
         "app_shared_lib_dir",
         "testscript_dir",
         "results_dir",
     ]
 
@@ -214,39 +219,46 @@
 # From modpath.py we can distinguish only these options:
 # 1. Debugging pi_base modules in pi_base {workspace}
 # 2. If it is ran from a package by a client of pi_base
 # When:                      __file__             # {workspace}/pi_base/modpath.py # {site_packages}/pi_base-X.X.X/pi_base/modpath.
 module_path = get_script_dir(__file__)  #         # {workspace}/pi_base            # {site_packages}/pi_base-X.X.X/pi_base
 module_dirname = os.path.basename(module_path)  # # pi_base                        # pi_base
 workspace_dir = os.path.dirname(module_path)  #   # {workspace}                    # {site_packages}/pi_base-X.X.X
-module_is_from_package = "/dist-packages/" in module_path or "/site_packages/" in module_path or "\\site_packages\\" in module_path or os.path.isfile(os.path.join(module_path, "is_editable.md"))
+module_is_from_editable = os.path.isfile(os.path.join(module_path, "is_editable.md"))
+module_is_from_package = "/dist-packages/" in module_path or "/site-packages/" in module_path or "\\site-packages\\" in module_path or module_is_from_editable
 
 # From top-level module we can infer:
 # 1. sources of app                      (app_module_dir == app_module_name)
 # 2. ?sources of {app_workspace}/lib     (app_module_dir == "lib" and ?)
 # 3. ?sources of {workspace}/lib         (app_module_dir == "lib" and ?)
 # 4. ?sources of {workspace}/pi_base/lib (app_module_dir == "lib" and ?)
-app_module_path, app_module_name = get_top_module()
+# 5. pi_base script with pi_base editable (app_filename == "{venv}\{Scripts|bin}\pi[-_]base{.exe}\__main__.py")
+app_filename, app_module_path, app_module_name = get_top_module()
+is_pibase_script = "__main__" in app_filename
 app_module_dir = os.path.basename(app_module_path)
-in_pibase_source = app_module_path.startswith(workspace_dir)  # This is surefire way to know that something run from pi_base {workspace}.
+in_pibase_source = is_pibase_script or app_module_path.startswith(workspace_dir)  # This is surefire way to know that something run from pi_base {workspace}.
 
-# `caller_dir` is mostly irrelevant, we should not rely on it.
-caller_dir = os.getcwd()
+# `caller_dir` is the only way to learn where {app_workspace} is when running pi_base script with editable pi_base.
+caller_dir = os.path.realpath(os.getcwd())
+caller_has_develop_file = (caller_dir != workspace_dir) and os.path.isfile(os.path.realpath(os.path.join(caller_dir, "develop.txt")))
+# caller_has_develop_file keep False if caller is pi_base {workspace}. develop_filename will still be found in workspace_dir.
 
 # Now from all the above, do some heuristics to arrive to all the answers.
 
 _app_workspace_path = ""
 pibase_shared_lib_dir = os.path.join(workspace_dir, "lib")
 additional_python_paths = []
 if not module_is_from_package or in_pibase_source:
     DEBUG = True
-    running_on: str = "pibase_sources"  # This is legacy way of running pi_base.
+    running_on: str = (
+        "pibase_sources_in_app_workspace" if caller_has_develop_file else "pibase_sources"
+    )  # This is either a legacy way of running pi_base, or running pi_base script from editable pi_base package.
 
     # In pi_base, we currently have one app - `blank`
-    _app_workspace_path = workspace_dir
+    _app_workspace_path = caller_dir if caller_has_develop_file else workspace_dir
 
     # Detect developer setup
     # If present, 'develop.txt' file (see 'SAMPLE_develop.txt') defines which app is running and choose where to find app_conf.yaml file
     develop_filename = os.path.realpath(os.path.join(_app_workspace_path, "develop.txt"))
     has_develop_file, site_id, project, additional_python_paths = _get_developer_setup(develop_filename, "BASE", "blank")
     additional_python_paths = [os.path.realpath(path) for path in additional_python_paths]
     project_dir = os.path.join(_app_workspace_path, f"build/{site_id}/{project}/pkg{PI_BASE_DIR}")
@@ -278,15 +290,15 @@
         app_conf_dir = project_dir
         app_shared_lib_dir = os.path.join(_app_workspace_path, "lib")
         testscript_dir = os.path.join(_app_workspace_path, "testscripts")
         results_dir: str = os.path.join(_app_workspace_path, "testresults")
     else:
         # Unknown situation
         print_info()
-        raise RuntimeError("Unknown situation, cannot deterrmine what is running and how to setup import paths and all locations.")
+        raise RuntimeError("Unknown situation, cannot determine what is running and how to setup import paths and all locations.")
 
 elif app_module_dir == APP_DIRNAME and not is_raspberrypi():
     # Running build but not on target
     DEBUG = True
     running_on = "build"
 
     _app_workspace_path = None  # There's no good reason to try to figure out app_workspace_path for running on "build". If anyone asks, cause an exception.
```

### Comparing `pi_base-0.0.8/pi_base/net_rpi.cmd` & `pi_base-0.0.9/pi_base/net_rpi.cmd`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/requirements.txt` & `pi_base-0.0.9/pi_base/requirements.txt`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/upload.cmd` & `pi_base-0.0.9/pi_base/upload.cmd`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base/upload.sh` & `pi_base-0.0.9/pi_base/upload.sh`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base.egg-info/PKG-INFO` & `pi_base-0.0.9/pi_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-base
-Version: 0.0.8
+Version: 0.0.9
 Summary: Framework for creating Raspberry Pi appliances.
 Author-email: Ilya Ivanchenko <iva2k@yahoo.com>
 License: MIT License
         
         Copyright (c) 2023 Ilya I
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pi_base-0.0.8/pi_base.egg-info/SOURCES.txt` & `pi_base-0.0.9/pi_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pi_base.egg-info/requires.txt` & `pi_base-0.0.9/pi_base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/pyproject.toml` & `pi_base-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pi_base-0.0.8/tox.ini` & `pi_base-0.0.9/tox.ini`

 * *Files identical despite different names*

