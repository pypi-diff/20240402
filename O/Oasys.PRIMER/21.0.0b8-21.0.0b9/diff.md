# Comparing `tmp/Oasys.PRIMER-21.0.0b8.tar.gz` & `tmp/Oasys.PRIMER-21.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Oasys.PRIMER-21.0.0b8.tar", last modified: Thu Feb  8 09:53:37 2024, max compression
+gzip compressed data, was "Oasys.PRIMER-21.0.0b9.tar", last modified: Thu Feb 22 16:21:56 2024, max compression
```

## Comparing `Oasys.PRIMER-21.0.0b8.tar` & `Oasys.PRIMER-21.0.0b9.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxrwxrwx   0        0        0        0 2024-02-08 09:53:37.476379 Oasys.PRIMER-21.0.0b8/
--rw-rw-rw-   0        0        0     1086 2024-01-18 09:17:34.000000 Oasys.PRIMER-21.0.0b8/LICENSE
--rw-rw-rw-   0        0        0     7334 2024-02-08 09:53:37.476379 Oasys.PRIMER-21.0.0b8/PKG-INFO
--rw-rw-rw-   0        0        0     5444 2024-01-04 08:21:46.000000 Oasys.PRIMER-21.0.0b8/README.rst
--rw-rw-rw-   0        0        0      778 2024-02-08 09:12:56.000000 Oasys.PRIMER-21.0.0b8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-08 09:53:37.477379 Oasys.PRIMER-21.0.0b8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-08 09:53:37.296271 Oasys.PRIMER-21.0.0b8/src/
-drwxrwxrwx   0        0        0        0 2024-02-08 09:53:37.296271 Oasys.PRIMER-21.0.0b8/src/Oasys/
-drwxrwxrwx   0        0        0        0 2024-02-08 09:53:37.473387 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/
--rw-rw-rw-   0        0        0     6627 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/__init__.py
--rw-rw-rw-   0        0        0    31623 2024-02-08 09:41:04.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/accelerometer.py
--rw-rw-rw-   0        0        0    31237 2024-02-08 09:41:04.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/airbag.py
--rw-rw-rw-   0        0        0     4706 2024-02-08 09:41:04.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/attached.py
--rw-rw-rw-   0        0        0    19225 2024-02-08 09:41:04.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/axialforcebeam.py
--rw-rw-rw-   0        0        0    35313 2024-02-08 09:41:04.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/beam.py
--rw-rw-rw-   0        0        0    33605 2024-02-08 09:41:04.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/belt.py
--rw-rw-rw-   0        0        0    29335 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/box.py
--rw-rw-rw-   0        0        0     2041 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/colour.py
--rw-rw-rw-   0        0        0    16926 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/comment.py
--rw-rw-rw-   0        0        0    25527 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/connectionproperties.py
--rw-rw-rw-   0        0        0    21402 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/constructionstages.py
--rw-rw-rw-   0        0        0    35979 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/contact.py
--rw-rw-rw-   0        0        0    30339 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/contactguidedcable.py
--rw-rw-rw-   0        0        0    45507 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/conx.py
--rw-rw-rw-   0        0        0    31349 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/coordinatesystem.py
--rw-rw-rw-   0        0        0    12069 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/core.py
--rw-rw-rw-   0        0        0    35848 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/crosssection.py
--rw-rw-rw-   0        0        0    27605 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/curve.py
--rw-rw-rw-   0        0        0    26622 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/dampingfrequencyrange.py
--rw-rw-rw-   0        0        0    26053 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/dampingpartmass.py
--rw-rw-rw-   0        0        0    25887 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/dampingpartstiffness.py
--rw-rw-rw-   0        0        0    25295 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/dampingrelative.py
--rw-rw-rw-   0        0        0    34426 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/deformabletorigid.py
--rw-rw-rw-   0        0        0    30818 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/discrete.py
--rw-rw-rw-   0        0        0    30205 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/discretesphere.py
--rw-rw-rw-   0        0        0    32879 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/dummy.py
--rw-rw-rw-   0        0        0    16964 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/elementdeath.py
--rw-rw-rw-   0        0        0    28219 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/extranodes.py
--rw-rw-rw-   0        0        0    16710 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/freqfrf.py
--rw-rw-rw-   0        0        0    24501 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/freqssd.py
--rw-rw-rw-   0        0        0    28572 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/freqvibration.py
--rw-rw-rw-   0        0        0    20306 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/funcs.py
--rw-rw-rw-   0        0        0    33751 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/generalizedweld.py
--rw-rw-rw-   0        0        0    28575 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/geometrysurface.py
--rw-rw-rw-   0        0        0    37576 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/group.py
--rw-rw-rw-   0        0        0    21832 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/hexspotweldassembly.py
--rw-rw-rw-   0        0        0    28613 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/history.py
--rw-rw-rw-   0        0        0    19747 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/hourglass.py
--rw-rw-rw-   0        0        0     5358 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/image.py
--rw-rw-rw-   0        0        0    24031 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/include.py
--rw-rw-rw-   0        0        0    22560 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/integrationbeam.py
--rw-rw-rw-   0        0        0    22252 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/integrationshell.py
--rw-rw-rw-   0        0        0    21343 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/interfacecomponent.py
--rw-rw-rw-   0        0        0    15255 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/interfacelinkingedge.py
--rw-rw-rw-   0        0        0    22963 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/interfacespringback.py
--rw-rw-rw-   0        0        0    38739 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/interpolation.py
--rw-rw-rw-   0        0        0    26262 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/interpolationspotweld.py
--rw-rw-rw-   0        0        0      537 2023-06-27 18:08:14.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/itemobject.py
--rw-rw-rw-   0        0        0    30298 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/joint.py
--rw-rw-rw-   0        0        0    32987 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/jointstiffness.py
--rw-rw-rw-   0        0        0    33438 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/linear.py
--rw-rw-rw-   0        0        0    26256 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadbeam.py
--rw-rw-rw-   0        0        0    27426 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadbodygeneralized.py
--rw-rw-rw-   0        0        0    25284 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadgravity.py
--rw-rw-rw-   0        0        0    24882 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadnode.py
--rw-rw-rw-   0        0        0    25428 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadremovepart.py
--rw-rw-rw-   0        0        0    25072 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadrigidbody.py
--rw-rw-rw-   0        0        0    28402 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadshell.py
--rw-rw-rw-   0        0        0    29694 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/mass.py
--rw-rw-rw-   0        0        0    27650 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/masspart.py
--rw-rw-rw-   0        0        0    41203 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/material.py
--rw-rw-rw-   0        0        0    34787 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/mechanism.py
--rw-rw-rw-   0        0        0    34504 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/model.py
--rw-rw-rw-   0        0        0    34455 2024-02-08 09:41:05.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/morphbox.py
--rw-rw-rw-   0        0        0    29329 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/morphflow.py
--rw-rw-rw-   0        0        0    28573 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/morphpoint.py
--rw-rw-rw-   0        0        0    24910 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/nodalforcegroup.py
--rw-rw-rw-   0        0        0    31959 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/nodalrigidbody.py
--rw-rw-rw-   0        0        0    34909 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/node.py
--rw-rw-rw-   0        0        0    30085 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/nodeset.py
--rw-rw-rw-   0        0        0     2473 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/options.py
--rw-rw-rw-   0        0        0    11790 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/parameter.py
--rw-rw-rw-   0        0        0    38255 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/part.py
--rw-rw-rw-   0        0        0    19493 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/prescribedaccelerometerrigid.py
--rw-rw-rw-   0        0        0    34734 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/prescribedfinalgeometry.py
--rw-rw-rw-   0        0        0    37897 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/prescribedmotion.py
--rw-rw-rw-   0        0        0    23313 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/prescribedorientationrigid.py
--rw-rw-rw-   0        0        0    31470 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/pretensioner.py
--rw-rw-rw-   0        0        0    29291 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/referencegeometry.py
--rw-rw-rw-   0        0        0    31340 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/retractor.py
--rw-rw-rw-   0        0        0    27537 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/rigidbodies.py
--rw-rw-rw-   0        0        0    32404 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/rigidwall.py
--rw-rw-rw-   0        0        0    30463 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/seatbelt1d.py
--rw-rw-rw-   0        0        0    29197 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/seatbelt2d.py
--rw-rw-rw-   0        0        0    36794 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/section.py
--rw-rw-rw-   0        0        0    30147 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/sensor.py
--rw-rw-rw-   0        0        0    25403 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/sensorcontrol.py
--rw-rw-rw-   0        0        0    22533 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/sensordefine.py
--rw-rw-rw-   0        0        0    23963 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/sensorswitch.py
--rw-rw-rw-   0        0        0    43924 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/set.py
--rw-rw-rw-   0        0        0    49986 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/shell.py
--rw-rw-rw-   0        0        0    30350 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/shellreferencegeometry.py
--rw-rw-rw-   0        0        0    30254 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/slipring.py
--rw-rw-rw-   0        0        0    37710 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/solid.py
--rw-rw-rw-   0        0        0    27698 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/spc.py
--rw-rw-rw-   0        0        0    29288 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/sph.py
--rw-rw-rw-   0        0        0    30116 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/spotweld.py
--rw-rw-rw-   0        0        0    23708 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/spr2.py
--rw-rw-rw-   0        0        0    28838 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/stagedconstructionpart.py
--rw-rw-rw-   0        0        0    22928 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/strainshell.py
--rw-rw-rw-   0        0        0    21645 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/strainsolid.py
--rw-rw-rw-   0        0        0    24685 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/stressbeam.py
--rw-rw-rw-   0        0        0    29144 2024-02-08 09:41:06.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/stresssection.py
--rw-rw-rw-   0        0        0    24396 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/stressshell.py
--rw-rw-rw-   0        0        0    24804 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/stresssolid.py
--rw-rw-rw-   0        0        0    17318 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/termination.py
--rw-rw-rw-   0        0        0    24028 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/tiebreak.py
--rw-rw-rw-   0        0        0    21314 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/transformation.py
--rw-rw-rw-   0        0        0    37279 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/tshell.py
--rw-rw-rw-   0        0        0     4465 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/utils.py
--rw-rw-rw-   0        0        0    29531 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/vector.py
--rw-rw-rw-   0        0        0    26251 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/velocity.py
--rw-rw-rw-   0        0        0    29270 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/velocitygeneration.py
--rw-rw-rw-   0        0        0     6942 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/view.py
--rw-rw-rw-   0        0        0    11675 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/window.py
--rw-rw-rw-   0        0        0     9837 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/workflow.py
--rw-rw-rw-   0        0        0     4023 2024-02-08 09:41:07.000000 Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/xrefs.py
-drwxrwxrwx   0        0        0        0 2024-02-08 09:53:37.475379 Oasys.PRIMER-21.0.0b8/src/Oasys.PRIMER.egg-info/
--rw-rw-rw-   0        0        0     7334 2024-02-08 09:53:37.000000 Oasys.PRIMER-21.0.0b8/src/Oasys.PRIMER.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3968 2024-02-08 09:53:37.000000 Oasys.PRIMER-21.0.0b8/src/Oasys.PRIMER.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-08 09:53:37.000000 Oasys.PRIMER-21.0.0b8/src/Oasys.PRIMER.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-02-08 09:53:37.000000 Oasys.PRIMER-21.0.0b8/src/Oasys.PRIMER.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-08 09:53:37.000000 Oasys.PRIMER-21.0.0b8/src/Oasys.PRIMER.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-02-22 16:21:56.755159 Oasys.PRIMER-21.0.0b9/
+-rw-rw-rw-   0        0        0     1086 2024-01-20 12:37:59.000000 Oasys.PRIMER-21.0.0b9/LICENSE
+-rw-rw-rw-   0        0        0     7334 2024-02-22 16:21:56.752167 Oasys.PRIMER-21.0.0b9/PKG-INFO
+-rw-rw-rw-   0        0        0     5444 2024-01-09 11:46:30.000000 Oasys.PRIMER-21.0.0b9/README.rst
+-rw-rw-rw-   0        0        0      778 2024-02-22 16:20:57.000000 Oasys.PRIMER-21.0.0b9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-02-22 16:21:56.756156 Oasys.PRIMER-21.0.0b9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-02-22 16:21:56.404567 Oasys.PRIMER-21.0.0b9/src/
+drwxrwxrwx   0        0        0        0 2024-02-22 16:21:56.404567 Oasys.PRIMER-21.0.0b9/src/Oasys/
+drwxrwxrwx   0        0        0        0 2024-02-22 16:21:56.746186 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/
+-rw-rw-rw-   0        0        0     6627 2024-02-22 14:38:38.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/__init__.py
+-rw-rw-rw-   0        0        0    31581 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/accelerometer.py
+-rw-rw-rw-   0        0        0    31225 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/airbag.py
+-rw-rw-rw-   0        0        0     4706 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/attached.py
+-rw-rw-rw-   0        0        0    19199 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/axialforcebeam.py
+-rw-rw-rw-   0        0        0    35307 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/beam.py
+-rw-rw-rw-   0        0        0    33599 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/belt.py
+-rw-rw-rw-   0        0        0    29333 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/box.py
+-rw-rw-rw-   0        0        0     2041 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/colour.py
+-rw-rw-rw-   0        0        0    16914 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/comment.py
+-rw-rw-rw-   0        0        0    25473 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/connectionproperties.py
+-rw-rw-rw-   0        0        0    21354 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/constructionstages.py
+-rw-rw-rw-   0        0        0    35961 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/contact.py
+-rw-rw-rw-   0        0        0    30291 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/contactguidedcable.py
+-rw-rw-rw-   0        0        0    45501 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/conx.py
+-rw-rw-rw-   0        0        0    31295 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/coordinatesystem.py
+-rw-rw-rw-   0        0        0    12070 2024-02-22 14:38:38.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/core.py
+-rw-rw-rw-   0        0        0    35810 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/crosssection.py
+-rw-rw-rw-   0        0        0    27595 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/curve.py
+-rw-rw-rw-   0        0        0    26565 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/dampingfrequencyrange.py
+-rw-rw-rw-   0        0        0    26014 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/dampingpartmass.py
+-rw-rw-rw-   0        0        0    25833 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/dampingpartstiffness.py
+-rw-rw-rw-   0        0        0    25256 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/dampingrelative.py
+-rw-rw-rw-   0        0        0    34366 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/deformabletorigid.py
+-rw-rw-rw-   0        0        0    30796 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/discrete.py
+-rw-rw-rw-   0        0        0    30159 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/discretesphere.py
+-rw-rw-rw-   0        0        0    32871 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/dummy.py
+-rw-rw-rw-   0        0        0    16934 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/elementdeath.py
+-rw-rw-rw-   0        0        0    28189 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/extranodes.py
+-rw-rw-rw-   0        0        0    16698 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/freqfrf.py
+-rw-rw-rw-   0        0        0    24486 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/freqssd.py
+-rw-rw-rw-   0        0        0    28539 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/freqvibration.py
+-rw-rw-rw-   0        0        0    20588 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/funcs.py
+-rw-rw-rw-   0        0        0    33701 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/generalizedweld.py
+-rw-rw-rw-   0        0        0    28547 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/geometrysurface.py
+-rw-rw-rw-   0        0        0    37566 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/group.py
+-rw-rw-rw-   0        0        0    21781 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/hexspotweldassembly.py
+-rw-rw-rw-   0        0        0    28603 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/history.py
+-rw-rw-rw-   0        0        0    19726 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/hourglass.py
+-rw-rw-rw-   0        0        0     5358 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/image.py
+-rw-rw-rw-   0        0        0    24025 2024-02-22 14:38:35.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/include.py
+-rw-rw-rw-   0        0        0    22521 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/integrationbeam.py
+-rw-rw-rw-   0        0        0    22210 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/integrationshell.py
+-rw-rw-rw-   0        0        0    21295 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/interfacecomponent.py
+-rw-rw-rw-   0        0        0    15217 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/interfacelinkingedge.py
+-rw-rw-rw-   0        0        0    22911 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/interfacespringback.py
+-rw-rw-rw-   0        0        0    38697 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/interpolation.py
+-rw-rw-rw-   0        0        0    26205 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/interpolationspotweld.py
+-rw-rw-rw-   0        0        0      537 2023-07-20 22:21:01.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/itemobject.py
+-rw-rw-rw-   0        0        0    30288 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/joint.py
+-rw-rw-rw-   0        0        0    32941 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/jointstiffness.py
+-rw-rw-rw-   0        0        0    33424 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/linear.py
+-rw-rw-rw-   0        0        0    26234 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadbeam.py
+-rw-rw-rw-   0        0        0    27375 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadbodygeneralized.py
+-rw-rw-rw-   0        0        0    25257 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadgravity.py
+-rw-rw-rw-   0        0        0    24864 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadnode.py
+-rw-rw-rw-   0        0        0    25392 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadremovepart.py
+-rw-rw-rw-   0        0        0    25039 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadrigidbody.py
+-rw-rw-rw-   0        0        0    28381 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadshell.py
+-rw-rw-rw-   0        0        0    29688 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/mass.py
+-rw-rw-rw-   0        0        0    27628 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/masspart.py
+-rw-rw-rw-   0        0        0    41181 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/material.py
+-rw-rw-rw-   0        0        0    34771 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/mechanism.py
+-rw-rw-rw-   0        0        0    34488 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/model.py
+-rw-rw-rw-   0        0        0    34437 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/morphbox.py
+-rw-rw-rw-   0        0        0    29303 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/morphflow.py
+-rw-rw-rw-   0        0        0    28549 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/morphpoint.py
+-rw-rw-rw-   0        0        0    24871 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/nodalforcegroup.py
+-rw-rw-rw-   0        0        0    31913 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/nodalrigidbody.py
+-rw-rw-rw-   0        0        0    34903 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/node.py
+-rw-rw-rw-   0        0        0    30067 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/nodeset.py
+-rw-rw-rw-   0        0        0     2473 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/options.py
+-rw-rw-rw-   0        0        0    11784 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/parameter.py
+-rw-rw-rw-   0        0        0    38249 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/part.py
+-rw-rw-rw-   0        0        0    19415 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/prescribedaccelerometerrigid.py
+-rw-rw-rw-   0        0        0    34652 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/prescribedfinalgeometry.py
+-rw-rw-rw-   0        0        0    37855 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/prescribedmotion.py
+-rw-rw-rw-   0        0        0    23241 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/prescribedorientationrigid.py
+-rw-rw-rw-   0        0        0    31432 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/pretensioner.py
+-rw-rw-rw-   0        0        0    29233 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/referencegeometry.py
+-rw-rw-rw-   0        0        0    31314 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/retractor.py
+-rw-rw-rw-   0        0        0    27503 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/rigidbodies.py
+-rw-rw-rw-   0        0        0    32378 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/rigidwall.py
+-rw-rw-rw-   0        0        0    30433 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/seatbelt1d.py
+-rw-rw-rw-   0        0        0    29167 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/seatbelt2d.py
+-rw-rw-rw-   0        0        0    36776 2024-02-22 14:38:36.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/section.py
+-rw-rw-rw-   0        0        0    30133 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/sensor.py
+-rw-rw-rw-   0        0        0    25370 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/sensorcontrol.py
+-rw-rw-rw-   0        0        0    22503 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/sensordefine.py
+-rw-rw-rw-   0        0        0    23933 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/sensorswitch.py
+-rw-rw-rw-   0        0        0    43927 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/set.py
+-rw-rw-rw-   0        0        0    49975 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/shell.py
+-rw-rw-rw-   0        0        0    30272 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/shellreferencegeometry.py
+-rw-rw-rw-   0        0        0    30232 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/slipring.py
+-rw-rw-rw-   0        0        0    37700 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/solid.py
+-rw-rw-rw-   0        0        0    27695 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/spc.py
+-rw-rw-rw-   0        0        0    29270 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/sph.py
+-rw-rw-rw-   0        0        0    30094 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/spotweld.py
+-rw-rw-rw-   0        0        0    23702 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/spr2.py
+-rw-rw-rw-   0        0        0    28760 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/stagedconstructionpart.py
+-rw-rw-rw-   0        0        0    22901 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/strainshell.py
+-rw-rw-rw-   0        0        0    21618 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/strainsolid.py
+-rw-rw-rw-   0        0        0    24661 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/stressbeam.py
+-rw-rw-rw-   0        0        0    29111 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/stresssection.py
+-rw-rw-rw-   0        0        0    24369 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/stressshell.py
+-rw-rw-rw-   0        0        0    24777 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/stresssolid.py
+-rw-rw-rw-   0        0        0    17291 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/termination.py
+-rw-rw-rw-   0        0        0    24010 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/tiebreak.py
+-rw-rw-rw-   0        0        0    21278 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/transformation.py
+-rw-rw-rw-   0        0        0    37265 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/tshell.py
+-rw-rw-rw-   0        0        0     4465 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/utils.py
+-rw-rw-rw-   0        0        0    29517 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/vector.py
+-rw-rw-rw-   0        0        0    26233 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/velocity.py
+-rw-rw-rw-   0        0        0    29208 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/velocitygeneration.py
+-rw-rw-rw-   0        0        0     6942 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/view.py
+-rw-rw-rw-   0        0        0    11675 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/window.py
+-rw-rw-rw-   0        0        0     9837 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/workflow.py
+-rw-rw-rw-   0        0        0     4023 2024-02-22 14:38:37.000000 Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/xrefs.py
+drwxrwxrwx   0        0        0        0 2024-02-22 16:21:56.750172 Oasys.PRIMER-21.0.0b9/src/Oasys.PRIMER.egg-info/
+-rw-rw-rw-   0        0        0     7334 2024-02-22 16:21:56.000000 Oasys.PRIMER-21.0.0b9/src/Oasys.PRIMER.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3968 2024-02-22 16:21:56.000000 Oasys.PRIMER-21.0.0b9/src/Oasys.PRIMER.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-22 16:21:56.000000 Oasys.PRIMER-21.0.0b9/src/Oasys.PRIMER.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-02-22 16:21:56.000000 Oasys.PRIMER-21.0.0b9/src/Oasys.PRIMER.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-02-22 16:21:56.000000 Oasys.PRIMER-21.0.0b9/src/Oasys.PRIMER.egg-info/top_level.txt
```

### Comparing `Oasys.PRIMER-21.0.0b8/LICENSE` & `Oasys.PRIMER-21.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/PKG-INFO` & `Oasys.PRIMER-21.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Oasys.PRIMER
-Version: 21.0.0b8
+Version: 21.0.0b9
 Summary: Python API for Oasys PRIMER
 Author: Miles Thornton
 Maintainer-email: DYNA support <dyna.support@arup.com>
 License: MIT License
         
         Copyright (c) 2024 Oasys Ltd
         
@@ -30,15 +30,15 @@
 Project-URL: Homepage, https://www.oasys-software.com/dyna/software/primer/
 Project-URL: Linkedin, https://www.linkedin.com/company/oasys-ltd-software/
 Project-URL: YouTube, https://www.youtube.com/c/OasysLtd
 Keywords: Oasys,PRIMER
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Oasys.gRPC>=21.0.0b4
+Requires-Dist: Oasys.gRPC>=21.0.0b5
 
 The Oasys.PRIMER package allows Python scripts to control the Oasys LS-DYNA Environment
 software `PRIMER <https://www.oasys-software.com/dyna/software/primer/>`_.
 
 Basic Information
 -----------------
```

### Comparing `Oasys.PRIMER-21.0.0b8/README.rst` & `Oasys.PRIMER-21.0.0b9/README.rst`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/pyproject.toml` & `Oasys.PRIMER-21.0.0b9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "Oasys.PRIMER"
-version = "21.0.0b8"
+version = "21.0.0b9"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 keywords = ["Oasys", "PRIMER"]
 dependencies = [
-  "Oasys.gRPC >= 21.0.0b4"
+  "Oasys.gRPC >= 21.0.0b5"
 ]
 description = "Python API for Oasys PRIMER"
 readme = "README.rst"
 authors = [
   {name = "Miles Thornton"},
 ]
 maintainers = [
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/__init__.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/__init__.py`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/accelerometer.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/accelerometer.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         intopt : integer
             Optional. Integration option; velocities are integrated from global accelerations and transformed into local system if intopt is 0, they are integrated directly from local accelerations if intopt is 1
         mass : real
             Optional. Optional added mass for accelerometer
 
         Returns
         -------
-        Accelerometer
+        dict
             Accelerometer object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -141,15 +141,15 @@
             Model that the accelerometer will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Accelerometer
+        dict
             Accelerometer object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first accelerometer in the model
@@ -340,15 +340,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Accelerometer
+        dict
             Accelerometer object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the accelerometers in the model
@@ -746,15 +746,15 @@
         Parameters
         ----------
         prop : string
             accelerometer property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this accelerometer (\*ELEMENT_SEATBELT_ACCELEROMETER)
@@ -877,23 +877,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Accelerometer
+        dict
             Accelerometer object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this accelerometer
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/airbag.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/airbag.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         abid : integer
             Optional. Airbag number
         heading : string
             Optional. Airbag title
 
         Returns
         -------
-        Airbag
+        dict
             Airbag object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -108,15 +108,15 @@
             Model that the airbag will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Airbag
+        dict
             Airbag object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first airbag in the model
@@ -618,15 +618,15 @@
         Parameters
         ----------
         prop : string
             airbag property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetPropertyByIndex(self, index):
         """
         Returns the value of property at index index for this
@@ -899,23 +899,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Airbag
+        dict
             Airbag object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this airbag
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/attached.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/attached.py`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/axialforcebeam.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/axialforcebeam.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         lcid : integer
             Loadcurve ID defining preload versus time
         scale : float
             Optional. Scale factor on curve
 
         Returns
         -------
-        AxialForceBeam
+        dict
             AxialForceBeam object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -424,15 +424,15 @@
         Parameters
         ----------
         prop : string
             axial force beam property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this axial force beam (\*INITIAL_AXIAL_FORCE_BEAM).
@@ -544,23 +544,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        AxialForceBeam
+        dict
             AxialForceBeam object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this axial force beam
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/beam.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         n2 : integer
             Node number 2 (optional)
         n3 : integer
             Node number 3 (optional)
 
         Returns
         -------
-        Beam
+        dict
             Beam object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -137,15 +137,15 @@
             Model that the beam will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Beam
+        dict
             Beam object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def FindBeamInBox(model, xmin, xmax, ymin, ymax, zmin, zmax, flag=Oasys.gRPC.defaultArg, excl=Oasys.gRPC.defaultArg, vis_only=Oasys.gRPC.defaultArg):
         """
         Returns a list of Beam objects for the beams within a box.
@@ -381,15 +381,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Beam
+        dict
             Beam object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the beams in the model
@@ -804,15 +804,15 @@
         Parameters
         ----------
         prop : string
             beam property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this beam (\*BEAM, \*BEAM_SCALAR or \*BEAM_SCALAR_VALUE).
@@ -1010,23 +1010,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Beam
+        dict
             Beam object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this beam
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/belt.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/belt.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         structural_type : string
             Optional. Seatbelt will be fitted around this entity type. This will trigger creation of sets as required. Type can be one of MODEL, DUMMY, PART, any ELEMENT subtype such as SHELL, or any SET subtype such as SET_PART. See Appendix I of the PRIMER manual for more information on PRIMER types
         flag : integer
             Optional. Flag used to identify entities that the belt should fit around. This argument is ignored if structural_type is MODEL. Instead, the current model is used
 
         Returns
         -------
-        Belt
+        dict
             Belt object
         """
 
 
 # Static methods
     def BlankAll(model, redraw=Oasys.gRPC.defaultArg):
         """
@@ -312,15 +312,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Belt
+        dict
             Belt object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the belts in the model
@@ -737,15 +737,15 @@
         Parameters
         ----------
         prop : string
             belt property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetPoint(self, index):
         """
         Returns the information for a path point (properties fixity, x, y, z, node, trx1, try1, trz1, tnx1, tny1, tnz1, tnode1, trx2, try2, trz2, tnx2, tny2, tnz2, tnode2).
@@ -935,23 +935,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Belt
+        dict
             Belt object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this belt
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/box.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/box.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         zmx : float
             Maximum Z coordinate
         heading : string
             Optional. Title for the box
 
         Returns
         -------
-        Box
+        dict
             Box object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -145,15 +145,15 @@
             Model that the box will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Box
+        dict
             Box object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first box in the model
@@ -344,15 +344,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Box
+        dict
             Box object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the boxs in the model
@@ -735,15 +735,15 @@
         Parameters
         ----------
         prop : string
             box property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this box (\*DEFINE_BOX).
@@ -866,23 +866,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Box
+        dict
             Box object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this box
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/colour.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/colour.py`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/comment.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/comment.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         header : string
             Optional. Comment number
         mode : constant
             Optional. Anchor: single or multiple
 
         Returns
         -------
-        Comment
+        dict
             Comment object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -400,15 +400,15 @@
         Parameters
         ----------
         prop : string
             comment property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this comment (\*COMMENT) and the header of the comment if there is one.
@@ -496,23 +496,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Comment
+        dict
             Comment object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this comment
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/connectionproperties.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/connectionproperties.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         con_id : integer
             \*DEFINE_CONNECTION_PROPERTIES id
         heading : string
             Optional. Title for the \*DEFINE_CONNECTION_PROPERTIES
 
         Returns
         -------
-        ConnectionProperties
+        dict
             ConnectionProperties object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -86,15 +86,15 @@
             Model that the \*DEFINE_CONNECTION_PROPERTIES will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        ConnectionProperties
+        dict
             ConnectionProperties object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first \*DEFINE_CONNECTION_PROPERTIES in the model
@@ -537,15 +537,15 @@
         Parameters
         ----------
         prop : string
             \*DEFINE_CONNECTION_PROPERTIES property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this \*DEFINE_CONNECTION_PROPERTIES
@@ -679,23 +679,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        ConnectionProperties
+        dict
             ConnectionProperties object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this \*DEFINE_CONNECTION_PROPERTIES
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/constructionstages.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/constructionstages.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         stage_id : integer
             ConstructionStages id
         heading : string
             Optional. Title for the \*DEFINE_CONSTRUCTION_STAGES
 
         Returns
         -------
-        ConstructionStages
+        dict
             ConstructionStages object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -86,15 +86,15 @@
             Model that the \*DEFINE_CONSTRUCTION_STAGES will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        ConstructionStages
+        dict
             ConstructionStages object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first \*DEFINE_CONSTRUCTION_STAGES in the model
@@ -510,15 +510,15 @@
         Parameters
         ----------
         prop : string
             \*DEFINE_CONSTRUCTION_STAGES property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this \*DEFINE_CONSTRUCTION_STAGES.
@@ -588,23 +588,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        ConstructionStages
+        dict
             ConstructionStages object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this \*DEFINE_CONSTRUCTION_STAGES
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/contact.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/contact.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         id : integer
             Optional. Contact number
         heading : string
             Optional. Title for the Contact
 
         Returns
         -------
-        Contact
+        dict
             Contact object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -135,15 +135,15 @@
             Model that the contact will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Contact
+        dict
             Contact object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first contact in the model
@@ -334,15 +334,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Contact
+        dict
             Contact object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the contacts in the model
@@ -756,15 +756,15 @@
         Parameters
         ----------
         prop : string
             contact property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Interactions(self, type=Oasys.gRPC.defaultArg):
         """
         Returns a list of objects describing the interactions which can either be penetrations
@@ -967,23 +967,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Contact
+        dict
             Contact object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this contact
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/contactguidedcable.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/contactguidedcable.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         heading : string
             Optional. ContactGuidedCable heading (Same as title)
         endtol : float
             Optional. Tolerance, in length units
 
         Returns
         -------
-        ContactGuidedCable
+        dict
             ContactGuidedCable object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -329,15 +329,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        ContactGuidedCable
+        dict
             ContactGuidedCable object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the contact guided_cables in the model
@@ -686,15 +686,15 @@
         Parameters
         ----------
         prop : string
             contact guided_cable property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this ContactGuidedCable (\*contact_guided_cable).
@@ -817,23 +817,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        ContactGuidedCable
+        dict
             ContactGuidedCable object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this contact guided_cable
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/conx.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/conx.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             Optional. Subtype of connection. See property subtype
             for valid values. If omitted subtype will be set to the default subtype for this type of connection
         title : string
             Optional. Title for the connection
 
         Returns
         -------
-        Conx
+        dict
             Conx object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -328,15 +328,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Conx
+        dict
             Conx object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RealizeAll(model):
         """
         Realizes all of the connections in the model
@@ -901,15 +901,15 @@
         Parameters
         ----------
         prop : string
             connection property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetPatchCoords(self, point):
         """
         Returns the data for a patch coordinate of an adhesive patch connection
@@ -1290,23 +1290,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Conx
+        dict
             Conx object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this connection
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/coordinatesystem.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/coordinatesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         dir : integer
             Axis defined by N1N2
         heading : string
             Optional. Title for the csys
 
         Returns
         -------
-        CoordinateSystem
+        dict
             CoordinateSystem object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -145,15 +145,15 @@
             Model that the csys will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        CoordinateSystem
+        dict
             CoordinateSystem object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first coordinate system in the model
@@ -344,15 +344,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        CoordinateSystem
+        dict
             CoordinateSystem object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the coordinate systems in the model
@@ -735,15 +735,15 @@
         Parameters
         ----------
         prop : string
             coordinate system property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this csys (\*DEFINE_COORDINATE).
@@ -866,23 +866,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        CoordinateSystem
+        dict
             CoordinateSystem object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this coordinate system
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/core.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         instance = object.__new__(Oasys.PRIMER.Sensor)
     elif t == "SensorControl":
         instance = object.__new__(Oasys.PRIMER.SensorControl)
     elif t == "SensorDefine":
         instance = object.__new__(Oasys.PRIMER.SensorDefine)
     elif t == "SensorSwitch":
         instance = object.__new__(Oasys.PRIMER.SensorSwitch)
-    elif t == "Set":
+    elif t == "SetK":
         instance = object.__new__(Oasys.PRIMER.Set)
     elif t == "Shell":
         instance = object.__new__(Oasys.PRIMER.Shell)
     elif t == "ShellReferenceGeometry":
         instance = object.__new__(Oasys.PRIMER.ShellReferenceGeometry)
     elif t == "Slipring":
         instance = object.__new__(Oasys.PRIMER.Slipring)
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/crosssection.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/crosssection.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         csid : integer
             Optional. Database cross_section number
         heading : string
             Optional. Database cross_section title
 
         Returns
         -------
-        CrossSection
+        dict
             CrossSection object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -152,15 +152,15 @@
             Model that the cross_section will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        CrossSection
+        dict
             CrossSection object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def CreateAlongFeatureLine(model, nid1, options):
         """
         Creates a set of cross sections along a feature line and returns them as a list of CrossSection objects. Use Options.edge_angle 
@@ -372,15 +372,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        CrossSection
+        dict
             CrossSection object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the cross sections in the model
@@ -827,15 +827,15 @@
         Parameters
         ----------
         prop : string
             cross section property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this cross_section (\*DATABASE_CROSS_SECTION).
@@ -988,23 +988,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        CrossSection
+        dict
             CrossSection object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this cross section
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/curve.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         heading : string
             Optional. Title for the curve
         lcint : integer
             Optional. Number of discretization points for the curve
 
         Returns
         -------
-        Curve
+        dict
             Curve object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -111,15 +111,15 @@
             Model that the curve will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Curve
+        dict
             Curve object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def CreateTable(model, modal=Oasys.gRPC.defaultArg):
         """
         Starts an interactive editing panel to create a table
@@ -130,15 +130,15 @@
             Model that the curve will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Curve
+        dict
             Curve object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "CreateTable", model, modal)
 
     def First(model):
         """
         Returns the first curve in the model
@@ -590,15 +590,15 @@
         Parameters
         ----------
         prop : string
             curve property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetPoint(self, row):
         """
         Returns x and y data for a point in a curve
@@ -821,23 +821,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Curve
+        dict
             Curve object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this curve
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/dampingfrequencyrange.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/dampingfrequencyrange.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         pidrel : integer
             Optional. Part ID
         iflg : integer
             Optional. Method used for internal calculation of damping constants
 
         Returns
         -------
-        DampingFrequencyRange
+        dict
             DampingFrequencyRange object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -255,15 +255,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        DampingFrequencyRange
+        dict
             DampingFrequencyRange object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select damping frequency ranges using standard PRIMER object menus
@@ -574,15 +574,15 @@
         Parameters
         ----------
         prop : string
             damping frequency range property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this damping frequency range (\*DAMPING_FREQUENCY_RANGE).
@@ -705,23 +705,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        DampingFrequencyRange
+        dict
             DampingFrequencyRange object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this damping frequency range
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/dampingpartmass.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/dampingpartmass.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         sry : float
             Optional. Rotational x scale factor
         srz : float
             Optional. Rotational x scale factor
 
         Returns
         -------
-        DampingPartMass
+        dict
             DampingPartMass object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -263,15 +263,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        DampingPartMass
+        dict
             DampingPartMass object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select damping part masss using standard PRIMER object menus
@@ -582,15 +582,15 @@
         Parameters
         ----------
         prop : string
             damping part mass property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this damping part mass (\*DAMPING_PART_MASS).
@@ -713,23 +713,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        DampingPartMass
+        dict
             DampingPartMass object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this damping part mass
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/dampingpartstiffness.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/dampingpartstiffness.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         id : integer
             Part/part set id
         coef : float
             Optional. Rayleigh damping coefficient
 
         Returns
         -------
-        DampingPartStiffness
+        dict
             DampingPartStiffness object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -247,15 +247,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        DampingPartStiffness
+        dict
             DampingPartStiffness object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select damping part stiffnesss using standard PRIMER object menus
@@ -566,15 +566,15 @@
         Parameters
         ----------
         prop : string
             damping part stiffness property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this damping part stiffness (\*DAMPING_PART_STIFFNESS).
@@ -697,23 +697,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        DampingPartStiffness
+        dict
             DampingPartStiffness object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this damping part stiffness
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/dampingrelative.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/dampingrelative.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         dv2 : float
             Optional. Constant for velocity squared term
         lcid : integer
             Optional. Fraction of cricitcal damping vs time
 
         Returns
         -------
-        DampingRelative
+        dict
             DampingRelative object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -250,15 +250,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        DampingRelative
+        dict
             DampingRelative object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select damping relatives using standard PRIMER object menus
@@ -569,15 +569,15 @@
         Parameters
         ----------
         prop : string
             damping relative property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this damping relative (\*DAMPING_RELATIVE).
@@ -700,23 +700,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        DampingRelative
+        dict
             DampingRelative object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this damping relative
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/deformabletorigid.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/deformabletorigid.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,30 +63,30 @@
             Model that deformable to rigid will be created in
         type : constant
             Specify the type of DeformableToRigid (Can be
             DeformableToRigid.SIMPLE or
             DeformableToRigid.AUTOMATIC or
             DeformableToRigid.INERTIA )
         pid : integer
-            Optional. Part  or Part set  ID which is switched to a rigid material. 
+            Optional. Part or Part set ID which is switched to a rigid material. 
             Depends on value of ptype. 
             Used only for DeformableToRigid.SIMPLE or 
             DeformableToRigid.INERTIA
         lrb : integer
             Optional. Part ID of the lead rigid body to which the part is merged. 
             Used only for DeformableToRigid.SIMPLE
         ptype : integer
             Optional. Type of PID. Valid values are: 
             DeformableToRigid.PART or 
             DeformableToRigid.PSET. 
             Used only for DeformableToRigid.SIMPLE
 
         Returns
         -------
-        DeformableToRigid
+        dict
             DeformableToRigid object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -147,15 +147,15 @@
             Model that the DeformableToRigid will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        DeformableToRigid
+        dict
             DeformableToRigid object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first deformable to rigid in the model
@@ -346,15 +346,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        DeformableToRigid
+        dict
             DeformableToRigid object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the deformable to rigids in the model
@@ -756,15 +756,15 @@
         Parameters
         ----------
         prop : string
             deformable to rigid property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this DeformableToRigid (\*DEFORMABLE_TO_RIGID_xxxx)
@@ -933,23 +933,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        DeformableToRigid
+        dict
             DeformableToRigid object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this deformable to rigid
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/discrete.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/discrete.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         pf : integer
             Optional. Print flag. Set to write forces to the DEFORC file
         offset : float
             Optional. Initial offset
 
         Returns
         -------
-        Discrete
+        dict
             Discrete object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -142,15 +142,15 @@
             Model that the discrete will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Discrete
+        dict
             Discrete object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first discrete in the model
@@ -341,15 +341,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Discrete
+        dict
             Discrete object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the discretes in the model
@@ -747,15 +747,15 @@
         Parameters
         ----------
         prop : string
             discrete property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this discrete (\*ELEMENT_DISCRETE).
@@ -889,23 +889,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Discrete
+        dict
             Discrete object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this discrete
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/discretesphere.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/discretesphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         inertia : real
             Mass moment of inertia
         radius : real
             Particle radius
 
         Returns
         -------
-        DiscreteSphere
+        dict
             DiscreteSphere object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -136,15 +136,15 @@
             Model that the discrete sphere will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        DiscreteSphere
+        dict
             DiscreteSphere object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first discrete sphere in the model
@@ -335,15 +335,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        DiscreteSphere
+        dict
             DiscreteSphere object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select discrete spheres using standard PRIMER object menus
@@ -703,15 +703,15 @@
         Parameters
         ----------
         prop : string
             discrete sphere property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this discrete sphere (\*ELEMENT_DISCRETE_SPHERE or \*ELEMENT_DISCRETE_SPHERE_VOLUME).
@@ -834,23 +834,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        DiscreteSphere
+        dict
             DiscreteSphere object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this discrete sphere
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/dummy.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/dummy.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Dummy
+        dict
             Dummy object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the dummys in the model
@@ -705,15 +705,15 @@
         Parameters
         ----------
         prop : string
             dummy property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetPoint(self, index):
         """
         Returns the information for a reference point
@@ -969,23 +969,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Dummy
+        dict
             Dummy object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this dummy
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/elementdeath.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/elementdeath.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             ElementDeath.THICK_SHELL or
             ElementDeath.THICK_SHELL_SET
         eid_sid : integer
             Element or element set ID
 
         Returns
         -------
-        ElementDeath
+        dict
             ElementDeath object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -97,15 +97,15 @@
             Model that the element death will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        ElementDeath
+        dict
             ElementDeath object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first element death in the model
@@ -415,15 +415,15 @@
         Parameters
         ----------
         prop : string
             element death property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this element death (\*DEFINE_ELEMENT_DEATH).
@@ -493,23 +493,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        ElementDeath
+        dict
             ElementDeath object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this element death
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/extranodes.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/extranodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         id : integer
             Node node ID or node set ID
         iflag : boolean
             Flag for adding node mass inertia to PART_INERTIA
 
         Returns
         -------
-        ExtraNodes
+        dict
             ExtraNodes object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -139,15 +139,15 @@
             Model that the constrained extra nodes card will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        ExtraNodes
+        dict
             ExtraNodes object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first constrained extra node in the model
@@ -270,15 +270,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        ExtraNodes
+        dict
             ExtraNodes object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select constrained extra nodes using standard PRIMER object menus
@@ -638,15 +638,15 @@
         Parameters
         ----------
         prop : string
             constrained extra node property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this constrained extra nodes (\*CONSTRAINED_EXTRA_NODES).
@@ -769,23 +769,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        ExtraNodes
+        dict
             ExtraNodes object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this constrained extra node
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/freqfrf.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/freqfrf.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             Type of n2. 
             Values can be FreqFRF.NODE,
             FreqFRF.NODE_SET or 
             FreqFRF.SEGMENT_SET
 
         Returns
         -------
-        FreqFRF
+        dict
             FreqFRF object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -398,15 +398,15 @@
         Parameters
         ----------
         prop : string
             \*FREQUENCY_DOMAIN_FRF property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this \*FREQUENCY_DOMAIN_FRF
@@ -476,23 +476,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        FreqFRF
+        dict
             FreqFRF object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this \*FREQUENCY_DOMAIN_FRF
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/freqssd.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/freqssd.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             FreqSSD.FATIGUE,
             FreqSSD.FRF,
             FreqSSD.ERP or
             FreqSSD.SUBCASE
 
         Returns
         -------
-        FreqSSD
+        dict
             FreqSSD object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -93,15 +93,15 @@
             Model that the \*FREQUENCY_DOMAIN_SSD card will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        FreqSSD
+        dict
             FreqSSD object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first \*FREQUENCY_DOMAIN_SSD in the model
@@ -558,15 +558,15 @@
         Parameters
         ----------
         prop : string
             \*FREQUENCY_DOMAIN_SSD property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this \*FREQUENCY_DOMAIN_SSD.
@@ -671,23 +671,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        FreqSSD
+        dict
             FreqSSD object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this \*FREQUENCY_DOMAIN_SSD
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/freqvibration.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/freqvibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         option : constant
             Specify the type of \*FREQUENCY_DOMAIN_RANDOM_VIBRATION. Can be
             FreqVibration.VIBRATION,
             FreqVibration.FATIGUE
 
         Returns
         -------
-        FreqVibration
+        dict
             FreqVibration object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -89,15 +89,15 @@
             Model that the \*FREQUENCY_DOMAIN_RANDOM_VIBRATION card will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        FreqVibration
+        dict
             FreqVibration object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first \*FREQUENCY_DOMAIN_RANDOM_VIBRATION in the model
@@ -604,15 +604,15 @@
         Parameters
         ----------
         prop : string
             \*FREQUENCY_DOMAIN_RANDOM_VIBRATION property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this \*FREQUENCY_DOMAIN_RANDOM_VIBRATION.
@@ -748,23 +748,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        FreqVibration
+        dict
             FreqVibration object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this \*FREQUENCY_DOMAIN_RANDOM_VIBRATION
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/funcs.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,18 @@
         Flag
     """
     return Oasys.PRIMER._connection.functionCall("AllocateFlag")
 
 
 def BatchMode():
     """
-    Check if PRIMER is running in batch mode (i.e. menus are not active)
+    Check if PRIMER is running in "batch mode" (i.e. menus are not active).
+    Menus will not be active if PRIMER is started with the -d=tty command line argument.
+    Note that this is different to starting PRIMER with the -batch command line argument. When using -batch,
+    the menu system is still running, but the main PRIMER window is not shown
 
     Returns
     -------
     bool
         True if in batch mode, False if not
     """
     return Oasys.PRIMER._connection.functionCall("BatchMode")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/generalizedweld.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/generalizedweld.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         nprt : integer
             Optional. Printout option
         wid : integer
             Optional. Constrained Generalized weld number
 
         Returns
         -------
-        GeneralizedWeld
+        dict
             GeneralizedWeld object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -145,15 +145,15 @@
             Model that the gwld will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        GeneralizedWeld
+        dict
             GeneralizedWeld object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first generalized weld in the model
@@ -344,15 +344,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        GeneralizedWeld
+        dict
             GeneralizedWeld object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the generalized welds in the model
@@ -767,15 +767,15 @@
         Parameters
         ----------
         prop : string
             generalized weld property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this gwld (\*CONSTRAINED_GENERALIZED_WELD_xxxx).
@@ -934,23 +934,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        GeneralizedWeld
+        dict
             GeneralizedWeld object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this generalized weld
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/geometrysurface.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/geometrysurface.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        GeometrySurface
+        dict
             GeometrySurface object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the surfaces in the model
@@ -686,15 +686,15 @@
         Parameters
         ----------
         prop : string
             surface property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetTriaIndices(self):
         """
         Return a list of all the tria indices for a surface (in triplets)
@@ -833,23 +833,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        GeometrySurface
+        dict
             GeometrySurface object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this surface
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/group.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         label : integer
             Group number
         title : string
             Optional. Title for the group
 
         Returns
         -------
-        Group
+        dict
             Group object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -133,15 +133,15 @@
             Model that the group will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Group
+        dict
             Group object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first group in the model
@@ -332,15 +332,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Group
+        dict
             Group object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the groups in the model
@@ -780,15 +780,15 @@
         Parameters
         ----------
         prop : string
             group property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetTotalAll(self, type):
         """
         Returns the total number of 'all' rows for a type in a group
@@ -1117,23 +1117,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Group
+        dict
             Group object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this group
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/hexspotweldassembly.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/hexspotweldassembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         eid4 : integer
             EID 4
         title : string
             Optional. Define hex spotweld assembly title
 
         Returns
         -------
-        HexSpotweldAssembly
+        dict
             HexSpotweldAssembly object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -96,15 +96,15 @@
             Model that the Hex Spotweld Assembly will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        HexSpotweldAssembly
+        dict
             HexSpotweldAssembly object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first DEFINE_HEX_SPOTWELD_ASSEMBLY in the model
@@ -520,15 +520,15 @@
         Parameters
         ----------
         prop : string
             DEFINE_HEX_SPOTWELD_ASSEMBLY property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this HexSpotweldAssembly (\*DEFINE_HEX_SPOTWELD_ASSEMBLY).
@@ -598,23 +598,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        HexSpotweldAssembly
+        dict
             HexSpotweldAssembly object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this DEFINE_HEX_SPOTWELD_ASSEMBLY
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/history.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/history.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         id : integer
             ID of the item
         heading : string
             Optional. Optional heading
 
         Returns
         -------
-        History
+        dict
             History object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -190,15 +190,15 @@
             History.TSHELL_SET
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        History
+        dict
             History object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, type, modal)
 
     def First(model, type=Oasys.gRPC.defaultArg):
         """
         Returns the first database history in the model
@@ -375,15 +375,15 @@
             from any model
         modal : boolean
             Optional. If picking is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the pick will be modal
 
         Returns
         -------
-        History
+        dict
             History object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select database histories using standard PRIMER object menus
@@ -805,12 +805,12 @@
 
     def Xrefs(self):
         """
         Returns the cross references for this database history
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/hourglass.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/hourglass.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         hgid : integer or string
             Hourglass number or character label
         title : string
             Optional. Title for the hourglass
 
         Returns
         -------
-        Hourglass
+        dict
             Hourglass object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -86,15 +86,15 @@
             Model that the hourglass will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Hourglass
+        dict
             Hourglass object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first hourglass in the model
@@ -510,15 +510,15 @@
         Parameters
         ----------
         prop : string
             hourglass property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this hourglass (\*HOURGLASS).
@@ -588,23 +588,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Hourglass
+        dict
             Hourglass object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this hourglass
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/image.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/image.py`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/include.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/include.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         name : string
             Include filename
         parent : integer
             Optional. Parent include file number. If omitted parent will be 0 (main file)
 
         Returns
         -------
-        Include
+        dict
             Include object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -239,15 +239,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Include
+        dict
             Include object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, model=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select includes using standard PRIMER object menus
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/integrationbeam.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/integrationbeam.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         icst : integer
             Optional. Standard cross section type. If omitted icst will be 0. If icst is non-zero, nip should be zero and vice-versa
         k : integer
             Optional. Integration refinement parameter for standard cross section types. If omitted k will be 0
 
         Returns
         -------
-        IntegrationBeam
+        dict
             IntegrationBeam object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -92,15 +92,15 @@
             Model that the intb will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        IntegrationBeam
+        dict
             IntegrationBeam object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first integration beam in the model
@@ -532,15 +532,15 @@
         Parameters
         ----------
         prop : string
             integration beam property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this intb (\*INTEGRATION_BEAM).
@@ -634,23 +634,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        IntegrationBeam
+        dict
             IntegrationBeam object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this integration beam
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/integrationshell.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/integrationshell.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         esop : integer
             Optional. Equal spacing of integration points option. If omitted esop will be 0
         failopt : integer
             Optional. Treatment of failure when mixing different constitutive types. If omitted failopt will be 0
 
         Returns
         -------
-        IntegrationShell
+        dict
             IntegrationShell object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -90,15 +90,15 @@
             Model that the ints will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        IntegrationShell
+        dict
             IntegrationShell object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first integration shell in the model
@@ -530,15 +530,15 @@
         Parameters
         ----------
         prop : string
             integration shell property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this ints (\*INTEGRATION_SHELL).
@@ -630,23 +630,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        IntegrationShell
+        dict
             IntegrationShell object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this integration shell
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/interfacecomponent.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/interfacecomponent.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         label : integer
             Optional. InterfaceComponent number
         title : string
             Optional. Title for this interface
 
         Returns
         -------
-        InterfaceComponent
+        dict
             InterfaceComponent object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -99,15 +99,15 @@
             Model that the InterfaceComponent will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        InterfaceComponent
+        dict
             InterfaceComponent object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first interface component in the model
@@ -523,15 +523,15 @@
         Parameters
         ----------
         prop : string
             interface component property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this InterfaceComponent (\*INTERFACE_COMPONENT).
@@ -601,23 +601,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        InterfaceComponent
+        dict
             InterfaceComponent object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this interface component
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/interfacelinkingedge.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/interfacelinkingedge.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         nsid : integer
             Node set ID
         ifid : integer
             Interface ID
 
         Returns
         -------
-        InterfaceLinkingEdge
+        dict
             InterfaceLinkingEdge object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -351,15 +351,15 @@
         Parameters
         ----------
         prop : string
             Interface Linking Edge property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this Interface Linking Edge (\*INTERFACE_LINKING_EDGE).
@@ -429,23 +429,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        InterfaceLinkingEdge
+        dict
             InterfaceLinkingEdge object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this Interface Linking Edge
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/interfacespringback.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/interfacespringback.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         type : constant
             Specify the type of InterfaceSpringback (Can be
             InterfaceSpringback.NIKE3D or
             InterfaceSpringback.LSDYNA or
             InterfaceSpringback.NASTRAN or
             InterfaceSpringback.SEAMLESS )
         psid : integer
-            Optional. Part set  ID for springback
+            Optional. Part set ID for springback
         nshv : integer
             Optional. Num additional Shell/Solid history variables number
         ftype : integer
             Optional. Filetype (0-3, 10-12)
         ftensr : integer
             Optional. Flag for dumping tensor data from the element history variables into the dynain file (0/1)
         nthhsv : integer
@@ -91,15 +91,15 @@
         ndflag : integer
             Optional. Flag to dump nodes into dynain file
         cflag : integer
             Optional. Output contact state
 
         Returns
         -------
-        InterfaceSpringback
+        dict
             InterfaceSpringback object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -116,15 +116,15 @@
             Model that the InterfaceSpringback will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        InterfaceSpringback
+        dict
             InterfaceSpringback object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first interface springback in the model
@@ -466,15 +466,15 @@
         Parameters
         ----------
         prop : string
             interface springback property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this Interface Springback (\*INTERFACE_SPRINGBACK_xxxx_xxxx)
@@ -619,23 +619,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        InterfaceSpringback
+        dict
             InterfaceSpringback object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this interface springback
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/interpolation.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/interpolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         rwghtz : float
             Optional. Weighting factor for INID. Scales the z-rotational component. The default value is twghtx
         cidi : integer
             Optional. Coordinate System ID if LOCAL option is active. The default value is 0
 
         Returns
         -------
-        Interpolation
+        dict
             Interpolation object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -162,15 +162,15 @@
             Model that the constrainedInterpolation will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Interpolation
+        dict
             Interpolation object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first constrained interpolation in the model
@@ -361,15 +361,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Interpolation
+        dict
             Interpolation object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the constrained interpolations in the model
@@ -784,15 +784,15 @@
         Parameters
         ----------
         prop : string
             constrained interpolation property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetRowData(self, row_index):
         """
         Returns independent node cards and local coordinate cards (if ITYP is Interpolation.NODE_SET) for the selected row of the \*CONSTRAINED_INTERPOLATION
@@ -984,23 +984,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Interpolation
+        dict
             Interpolation object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this constrained interpolation
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/interpolationspotweld.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/interpolationspotweld.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         pid2 : integer
             Part ID of second sheet
         nsid : integer
             Node Set ID of spotweld location nodes
 
         Returns
         -------
-        InterpolationSpotweld
+        dict
             InterpolationSpotweld object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -247,15 +247,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        InterpolationSpotweld
+        dict
             InterpolationSpotweld object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select interpolation spotwelds using standard PRIMER object menus
@@ -566,15 +566,15 @@
         Parameters
         ----------
         prop : string
             interpolation spotweld property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this interpolation spotweld (\*CONSTRAINED_INTERPOLATION_SPOTWELD).
@@ -697,23 +697,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        InterpolationSpotweld
+        dict
             InterpolationSpotweld object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this interpolation spotweld
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/itemobject.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/itemobject.py`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/joint.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/joint.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         jid : integer
             Optional. Constrained joint number
         heading : string
             Optional. Constrained joint title
 
         Returns
         -------
-        Joint
+        dict
             Joint object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -139,15 +139,15 @@
             Model that the joint will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Joint
+        dict
             Joint object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first joint in the model
@@ -338,15 +338,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Joint
+        dict
             Joint object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the joints in the model
@@ -744,15 +744,15 @@
         Parameters
         ----------
         prop : string
             joint property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this joint (\*CONSTRAINED_JOINT).
@@ -875,23 +875,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Joint
+        dict
             Joint object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this joint
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/jointstiffness.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/jointstiffness.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         nsaps : float
             Stop angle for -ve Psi rotation
         psaps : float
             Stop angle for +ve Psi rotation
 
         Returns
         -------
-        JointStiffness
+        dict
             JointStiffness object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -180,15 +180,15 @@
             Model that the jstf will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        JointStiffness
+        dict
             JointStiffness object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first joint stiffness in the model
@@ -379,15 +379,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        JointStiffness
+        dict
             JointStiffness object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the joint stiffnesss in the model
@@ -770,15 +770,15 @@
         Parameters
         ----------
         prop : string
             joint stiffness property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this jstf (\*CONSTRAINED_JOINT_STIFFNESS).
@@ -901,23 +901,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        JointStiffness
+        dict
             JointStiffness object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this joint stiffness
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/linear.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         coeff : float
             Non-zero coefficient
         cid : integer
             Optional. Coordinate System ID if format is Linear.LOCAL. The default value is 0
 
         Returns
         -------
-        Linear
+        dict
             Linear object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -143,15 +143,15 @@
             Model that the constrainedLinear will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Linear
+        dict
             Linear object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first constrained linear in the model
@@ -342,15 +342,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Linear
+        dict
             Linear object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the constrained linears in the model
@@ -755,15 +755,15 @@
         Parameters
         ----------
         prop : string
             constrained linear property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetRowData(self, row_index):
         """
         Returns independent card 2 for the selected row of the \*CONSTRAINED_LINEAR
@@ -945,23 +945,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Linear
+        dict
             Linear object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this constrained linear
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadbeam.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadbeam.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         lcid : integer
             Curve ID
         sf : float
             Optional. Load curve scale factor
 
         Returns
         -------
-        LoadBeam
+        dict
             LoadBeam object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -141,15 +141,15 @@
             Model that the load beam will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        LoadBeam
+        dict
             LoadBeam object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first load beam in the model
@@ -272,15 +272,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        LoadBeam
+        dict
             LoadBeam object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select load beams using standard PRIMER object menus
@@ -625,15 +625,15 @@
         Parameters
         ----------
         prop : string
             load beam property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this load beam (\*LOAD_BEAM_xxxx).
@@ -756,23 +756,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        LoadBeam
+        dict
             LoadBeam object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this load beam
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadbodygeneralized.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadbodygeneralized.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         cid : integer
             Optional. Coordinate system ID to define acceleration
         angtyp : string
             Optional. Type of body loads
 
         Returns
         -------
-        LoadBodyGeneralized
+        dict
             LoadBodyGeneralized object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -276,15 +276,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        LoadBodyGeneralized
+        dict
             LoadBodyGeneralized object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select load body generalizeds using standard PRIMER object menus
@@ -595,15 +595,15 @@
         Parameters
         ----------
         prop : string
             load body generalized property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this load body generalized (\*LOAD_NODE_xxxx).
@@ -726,23 +726,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        LoadBodyGeneralized
+        dict
             LoadBodyGeneralized object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this load body generalized
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadgravity.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadgravity.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         stga : integer
             Optional. Construction Stage ID at which part is added (optional)
         stgr : integer
             Optional. Construction Stage ID at which part is removed (optional)
 
         Returns
         -------
-        LoadGravity
+        dict
             LoadGravity object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -259,15 +259,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        LoadGravity
+        dict
             LoadGravity object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select load gravitys using standard PRIMER object menus
@@ -578,15 +578,15 @@
         Parameters
         ----------
         prop : string
             load gravity property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this LoadGravity (\*LOAD_GRAVITY_PART).
@@ -709,23 +709,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        LoadGravity
+        dict
             LoadGravity object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this load gravity
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadnode.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadnode.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         m3 : integer
             Optional. Node 3 ID
         lcidsf : integer
             Optional. Curve ID
 
         Returns
         -------
-        LoadNode
+        dict
             LoadNode object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -264,15 +264,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        LoadNode
+        dict
             LoadNode object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select load nodes using standard PRIMER object menus
@@ -583,15 +583,15 @@
         Parameters
         ----------
         prop : string
             load node property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this load node (\*LOAD_NODE_xxxx).
@@ -714,23 +714,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        LoadNode
+        dict
             LoadNode object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this load node
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadremovepart.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadremovepart.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         time1 : float
             Optional. Time at which stresses become zero and elements are deleted
         stgr : integer
             Optional. Construction Stage ID at which part is removed
 
         Returns
         -------
-        LoadRemovePart
+        dict
             LoadRemovePart object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -253,15 +253,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        LoadRemovePart
+        dict
             LoadRemovePart object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select load remove_parts using standard PRIMER object menus
@@ -572,15 +572,15 @@
         Parameters
         ----------
         prop : string
             load remove_part property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this LoadRemovePart (\*LOAD_REMOVE_PART).
@@ -703,23 +703,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        LoadRemovePart
+        dict
             LoadRemovePart object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this load remove_part
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadrigidbody.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadrigidbody.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         m2 : integer
             Optional. Node 2 ID
         m3 : integer
             Optional. Node 3 ID
 
         Returns
         -------
-        LoadRigidBody
+        dict
             LoadRigidBody object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -254,15 +254,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        LoadRigidBody
+        dict
             LoadRigidBody object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select load rigidbodys using standard PRIMER object menus
@@ -573,15 +573,15 @@
         Parameters
         ----------
         prop : string
             load rigidbody property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this load rigidbody (\*LOAD_RIGIDBODY).
@@ -704,23 +704,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        LoadRigidBody
+        dict
             LoadRigidBody object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this load rigidbody
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/loadshell.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/loadshell.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         lsid : integer
             Optional. LoadShell number
         heading : string
             Optional. Title for the LoadShell
 
         Returns
         -------
-        LoadShell
+        dict
             LoadShell object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -325,15 +325,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        LoadShell
+        dict
             LoadShell object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the load shells in the model
@@ -682,15 +682,15 @@
         Parameters
         ----------
         prop : string
             load shell property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this LoadShell (\*LOAD_SHELL_xxxx).
@@ -813,23 +813,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        LoadShell
+        dict
             LoadShell object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this load shell
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/mass.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/mass.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         mass : float
             Mass value
         node_set : integer
             Optional. Only used if a node set is used
 
         Returns
         -------
-        Mass
+        dict
             Mass object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -137,15 +137,15 @@
             Model that the mass will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Mass
+        dict
             Mass object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first mass in the model
@@ -336,15 +336,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Mass
+        dict
             Mass object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the masss in the model
@@ -742,15 +742,15 @@
         Parameters
         ----------
         prop : string
             mass property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this mass (\*ELEMENT_MASS or \*ELEMENT_MASS_NODE_SET).
@@ -873,23 +873,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Mass
+        dict
             Mass object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this mass
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/masspart.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/masspart.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         addmass : real
             Optional. Added translational mass
         finmass : real
             Optional. Final translational mass
 
         Returns
         -------
-        MassPart
+        dict
             MassPart object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -139,15 +139,15 @@
             Model that the mass part will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        MassPart
+        dict
             MassPart object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first element mass part in the model
@@ -270,15 +270,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        MassPart
+        dict
             MassPart object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select element mass parts using standard PRIMER object menus
@@ -638,15 +638,15 @@
         Parameters
         ----------
         prop : string
             element mass part property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this mass part (\*ELEMENT_MASS_PART)
@@ -769,23 +769,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        MassPart
+        dict
             MassPart object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this element mass part
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/material.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/material.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             Material number or character label
         type : string
             Material type. Either give the LS-DYNA material name or
             3 digit number
 
         Returns
         -------
-        Material
+        dict
             Material object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -131,15 +131,15 @@
             Model that the material will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Material
+        dict
             Material object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first material in the model
@@ -330,15 +330,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Material
+        dict
             Material object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the materials in the model
@@ -794,15 +794,15 @@
         Parameters
         ----------
         prop : string
             material property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetPropertyByIndex(self, index):
         """
         Returns the value of property at index index for this
@@ -1141,26 +1141,26 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Material
+        dict
             Material object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this material
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
 
     def YieldStress(self):
         """
         Get Yield stress for the material
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/mechanism.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/mechanism.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Mechanism
+        dict
             Mechanism object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the mechanisms in the model
@@ -728,15 +728,15 @@
         Parameters
         ----------
         prop : string
             mechanism property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetPoint(self, index):
         """
         Returns the information for a reference point
@@ -1006,23 +1006,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Mechanism
+        dict
             Mechanism object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this mechanism
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/model.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         Parameters
         ----------
         number : integer
             Optional. Model number to create. If omitted the next free model number will be used
 
         Returns
         -------
-        Model
+        dict
             Model object
         """
 
 
 # Static methods
     def BlankAll():
         """
@@ -264,15 +264,15 @@
             Optional. Filetype you want to read. Can be Model.LSDYNA,
             Model.ABAQUS,
             Model.NASTRAN,
             Model.RADIOSS or
             Model.IGES.
             If omitted the file is assumed to be a DYNA3D file.
             For Model.NASTRAN there are options that change how the model is read.
-            See Options>` for details
+            See for details
         number : integer
             Optional. Model number to read file into. If omitted the next free model number will be used
 
         Returns
         -------
         Model
             Model object (or None if error)
@@ -472,15 +472,15 @@
         ----------
         update : boolean
             Optional. If the graphics should be updated after the model is copied.
             If omitted update will be set to false
 
         Returns
         -------
-        Model
+        dict
             Model object for new model
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Copy", update)
 
     def CopyFlagged(self, flag, update=Oasys.gRPC.defaultArg):
         """
         Copy flagged items in a model to the next free model in PRIMER
@@ -491,15 +491,15 @@
             Flag set on items that you want to copy
         update : boolean
             Optional. If the graphics should be updated after the model is copied.
             If omitted update will be set to false
 
         Returns
         -------
-        Model
+        dict
             Model object for new model
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "CopyFlagged", flag, update)
 
     def Delete(self):
         """
         Deletes a model in PRIMER
@@ -529,23 +529,23 @@
         Returns
         -------
         None
             No return value
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "DeleteFlagged", flag, recursive)
 
-    def DeleteInclude(self, _py_class_include__label, method=Oasys.gRPC.defaultArg, force=Oasys.gRPC.defaultArg):
+    def DeleteInclude(self, _py_class_include___label, method=Oasys.gRPC.defaultArg, force=Oasys.gRPC.defaultArg):
         """
         Tries to delete an include file from the model. Note that this may not actually
         delete the include file. For example if some of the items in the include file are required
         by other things in different includes then the include file will not be deleted
 
         Parameters
         ----------
-        _py_class_include__label : integer
+        _py_class_include___label : integer
             label of include file that you want to delete
         method : constant
             Optional. Method for deleting items. Must be Model.REMOVE_FROM_SETS (default),
             Model.REMOVE_JUNIOR or
             Model.REMOVE_INCLUDE_ONLY.
             Model.REMOVE_FROM_SETS will only delete items within
             the include selected but may remove items from sets in other includes.
@@ -560,15 +560,15 @@
             from the model. If this argument is omitted, force will be set to false
 
         Returns
         -------
         bool
             True if include successfully deleted, False otherwise
         """
-        return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "DeleteInclude", _py_class_include__label, method, force)
+        return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "DeleteInclude", _py_class_include___label, method, force)
 
     def FlagDuplicate(self, flag):
         """
         Flag all nodes referenced in two different includes
 
         Parameters
         ----------
@@ -640,15 +640,15 @@
         source : String OR Include Object
             Can either be a Filename of the LS-DYNA include file you want to import, OR Include object of another model you want to import
         target : Include Object
             Optional. Include file object of current model if the Import has to be done in an existing include
 
         Returns
         -------
-        Include
+        dict
             Include object for include file
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ImportInclude", source, target)
 
     def ImportIncludeTransform(self, filename, idnoff, ideoff, idpoff, idmoff, idsoff, idfoff, iddoff, idroff):
         """
         Imports a file as an include transform file for model m. The labels of any items
@@ -673,15 +673,15 @@
         iddoff : integer
             Offset for defines in the file
         idroff : integer
             Offset for other labels in the file
 
         Returns
         -------
-        Include
+        dict
             Include object if successful, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ImportIncludeTransform", filename, idnoff, ideoff, idpoff, idmoff, idsoff, idfoff, iddoff, idroff)
 
     def Mass(self):
         """
         Returns the mass for a model
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/morphbox.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/morphbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         flag : Flag
             Flag set on the entities (for example nodes, elements and/or parts) that you want to create the box around
         options : dict
             Optional. Options to create the box
 
         Returns
         -------
-        MorphBox
+        dict
             MorphBox object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -331,15 +331,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        MorphBox
+        dict
             MorphBox object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the boxs in the model
@@ -748,15 +748,15 @@
         Parameters
         ----------
         prop : string
             box property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetPoint(self, xindex, yindex, zindex):
         """
         Returns the morph point ID on the morph box at indices in X, Y and Z
@@ -971,23 +971,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        MorphBox
+        dict
             MorphBox object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this box
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/morphflow.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/morphflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         model : Model
             Model that morph flow will be created in
         name : string
             MorphFlow name
 
         Returns
         -------
-        MorphFlow
+        dict
             MorphFlow object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -128,15 +128,15 @@
             Model that the morph flow card will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        MorphFlow
+        dict
             MorphFlow object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first flow in the model
@@ -279,15 +279,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        MorphFlow
+        dict
             MorphFlow object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select flows using standard PRIMER object menus
@@ -632,15 +632,15 @@
         Parameters
         ----------
         prop : string
             flow property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetRow(self, row):
         """
         Returns the data for a row in the morph flow
@@ -871,23 +871,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        MorphFlow
+        dict
             MorphFlow object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this flow
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/morphpoint.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/morphpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         y : float
             Y coordinate
         z : float
             Z coordinate
 
         Returns
         -------
-        MorphPoint
+        dict
             MorphPoint object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -345,15 +345,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        MorphPoint
+        dict
             MorphPoint object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the points in the model
@@ -702,15 +702,15 @@
         Parameters
         ----------
         prop : string
             point property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this morph point (\*MORPH_POINT).
@@ -833,23 +833,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        MorphPoint
+        dict
             MorphPoint object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this point
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/nodalforcegroup.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/nodalforcegroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         nsid : integer
             Set Node Set ID
         cid : integer
             Optional. Coordinate System ID
 
         Returns
         -------
-        NodalForceGroup
+        dict
             NodalForceGroup object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -242,15 +242,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        NodalForceGroup
+        dict
             NodalForceGroup object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select nodal force groups using standard PRIMER object menus
@@ -561,15 +561,15 @@
         Parameters
         ----------
         prop : string
             nodal force group property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this nodal force group.
@@ -692,23 +692,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        NodalForceGroup
+        dict
             NodalForceGroup object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this nodal force group
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/nodalrigidbody.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/nodalrigidbody.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         drflag : integer
             Optional. Displacement release flag
         rrflag : integer
             Optional. Rotation release flag
 
         Returns
         -------
-        NodalRigidBody
+        dict
             NodalRigidBody object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -141,15 +141,15 @@
             Model that the nrb will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        NodalRigidBody
+        dict
             NodalRigidBody object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first nodal rigid body in the model
@@ -340,15 +340,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        NodalRigidBody
+        dict
             NodalRigidBody object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the nodal rigid bodys in the model
@@ -746,15 +746,15 @@
         Parameters
         ----------
         prop : string
             nodal rigid body property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this nrb (\*CONSTRAINED_NODAL_RIGID_BODY_xxxx).
@@ -877,23 +877,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        NodalRigidBody
+        dict
             NodalRigidBody object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this nodal rigid body
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/node.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         tc : integer
             Optional. Translational constraint (0-7). If omitted tc will be set to 0
         rc : integer
             Optional. Rotational constraint (0-7). If omitted rc will be set to 0
 
         Returns
         -------
-        Node
+        dict
             Node object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -141,15 +141,15 @@
             Model that the node will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Node
+        dict
             Node object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first node in the model
@@ -372,15 +372,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Node
+        dict
             Node object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the nodes in the model
@@ -833,15 +833,15 @@
         Parameters
         ----------
         prop : string
             node property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetReferenceGeometry(self):
         """
         Returns the airbag reference geometry of the node
@@ -989,23 +989,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Node
+        dict
             Node object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this node
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/nodeset.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/nodeset.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         tf : float
             Failure time
         label : integer
             Optional. Constrained node set number
 
         Returns
         -------
-        NodeSet
+        dict
             NodeSet object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -134,15 +134,15 @@
             Model that the node_set will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        NodeSet
+        dict
             NodeSet object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first node set in the model
@@ -333,15 +333,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        NodeSet
+        dict
             NodeSet object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the node sets in the model
@@ -739,15 +739,15 @@
         Parameters
         ----------
         prop : string
             node set property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this node_set (\*CONSTRAINED_NODE_SET).
@@ -870,23 +870,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        NodeSet
+        dict
             NodeSet object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this node set
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/options.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/options.py`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/parameter.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             Parameter.MUTABLE for \*PARAMETER_..._MUTABLE, or
             Parameter.NOECHO for \*PARAMETER_..._NOECHO.
             These may be bitwise ORed together, ie Parameter.LOCAL | Parameter.MUTABLE | Parameter.NOECHO.
             If omitted the parameter will not be local or mutable
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -341,12 +341,12 @@
 
     def Xrefs(self):
         """
         Returns the cross references for this parameter
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/part.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/part.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         mid : integer or string
             Material number or character label
         heading : string
             Optional. Title for the part
 
         Returns
         -------
-        Part
+        dict
             Part object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -155,15 +155,15 @@
             Model that the part will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Part
+        dict
             Part object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first part in the model
@@ -414,15 +414,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Part
+        dict
             Part object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the parts in the model
@@ -872,15 +872,15 @@
         Parameters
         ----------
         prop : string
             part property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this part (\*PART, \*PART_SCALAR or \*PART_SCALAR_VALUE).
@@ -1086,23 +1086,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Part
+        dict
             Part object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this part
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/prescribedaccelerometerrigid.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/prescribedaccelerometerrigid.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         pid : integer
             Part ID for rigid body whose motion is prescribed
         solv : integer
             Optional. Solver type
 
         Returns
         -------
-        PrescribedAccelerometerRigid
+        dict
             PrescribedAccelerometerRigid object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -86,15 +86,15 @@
             Model that the prescribed accelerometer rigid will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        PrescribedAccelerometerRigid
+        dict
             PrescribedAccelerometerRigid object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first prescribed accelerometer rigid in the model
@@ -404,15 +404,15 @@
         Parameters
         ----------
         prop : string
             prescribed accelerometer rigid property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetRow(self, row):
         """
         Returns the data for a row in the prescribed accelerometer rigid
@@ -534,23 +534,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        PrescribedAccelerometerRigid
+        dict
             PrescribedAccelerometerRigid object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this prescribed accelerometer rigid
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/prescribedfinalgeometry.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/prescribedfinalgeometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         model : Model
             Model that PrescribedFinalGeometry will be created in
         bpfgid : PrescribedFinalGeometry
             PrescribedFinalGeometry number
 
         Returns
         -------
-        PrescribedFinalGeometry
+        dict
             PrescribedFinalGeometry object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -128,15 +128,15 @@
             Model that the bpfg will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        PrescribedFinalGeometry
+        dict
             PrescribedFinalGeometry object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first boundary prescribed final geometry in the model
@@ -327,15 +327,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        PrescribedFinalGeometry
+        dict
             PrescribedFinalGeometry object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the boundary prescribed final geometrys in the model
@@ -735,15 +735,15 @@
         Parameters
         ----------
         prop : string
             boundary prescribed final geometry property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this PrescribedFinalGeometry (\*BOUNDARY_PRESCRIBED_FINAL_GEOMETRY).
@@ -912,23 +912,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        PrescribedFinalGeometry
+        dict
             PrescribedFinalGeometry object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this boundary prescribed final geometry
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/prescribedmotion.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/prescribedmotion.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         label : integer
             Optional. PrescribedMotion number
         heading : string
             Optional. Title for the PrescribedMotion
 
         Returns
         -------
-        PrescribedMotion
+        dict
             PrescribedMotion object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -517,15 +517,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        PrescribedMotion
+        dict
             PrescribedMotion object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the boundary prescribed motions in the model
@@ -874,15 +874,15 @@
         Parameters
         ----------
         prop : string
             boundary prescribed motion property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this PrescribedMotion (\*BOUNDARY_PRESCRIBED_MOTION_xxxx).
@@ -1005,23 +1005,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        PrescribedMotion
+        dict
             PrescribedMotion object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this boundary prescribed motion
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/prescribedorientationrigid.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/prescribedorientationrigid.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         label : integer
             Optional. PrescribedOrientationRigid number
         heading : string
             Optional. Title for the PrescribedOrientationRigid
 
         Returns
         -------
-        PrescribedOrientationRigid
+        dict
             PrescribedOrientationRigid object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -97,15 +97,15 @@
             Model that the prescribed orientation rigid will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        PrescribedOrientationRigid
+        dict
             PrescribedOrientationRigid object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first prescribed orientation rigid in the model
@@ -486,15 +486,15 @@
         Parameters
         ----------
         prop : string
             prescribed orientation rigid property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this prescribed orientation rigid.
@@ -606,23 +606,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        PrescribedOrientationRigid
+        dict
             PrescribedOrientationRigid object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this prescribed orientation rigid
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/pretensioner.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/pretensioner.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         time : float
             Optional. Time between sensor triggering and pretensioner acting
         lmtfrc : float
             Optional. Limiting force
 
         Returns
         -------
-        Pretensioner
+        dict
             Pretensioner object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -146,15 +146,15 @@
             Model that the pretensioner will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Pretensioner
+        dict
             Pretensioner object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first pretensioner in the model
@@ -345,15 +345,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Pretensioner
+        dict
             Pretensioner object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the pretensioners in the model
@@ -751,15 +751,15 @@
         Parameters
         ----------
         prop : string
             pretensioner property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this pretensioner (\*ELEMENT_SEATBELT_PRETEROMETER)
@@ -882,23 +882,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Pretensioner
+        dict
             Pretensioner object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this pretensioner
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/referencegeometry.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/referencegeometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         model : Model
             Model that ReferenceGeometry will be created in
         aid : integer
             Optional. ReferenceGeometry number to set _ID suffix
 
         Returns
         -------
-        ReferenceGeometry
+        dict
             ReferenceGeometry object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -84,15 +84,15 @@
             Model that the ardt will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        ReferenceGeometry
+        dict
             ReferenceGeometry object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first airbag reference geometry in the model
@@ -283,15 +283,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        ReferenceGeometry
+        dict
             ReferenceGeometry object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the airbag reference geometrys in the model
@@ -624,15 +624,15 @@
         Parameters
         ----------
         prop : string
             airbag reference geometry property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this reference_geometry (\*AIRBAG_REFERENCE_GEOMETRY).
@@ -805,23 +805,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        ReferenceGeometry
+        dict
             ReferenceGeometry object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this airbag reference geometry
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/retractor.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/retractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         ulcid : integer
             Optional. Loadcurve for unloading (pull-out vs force)
         lfed : float
             Optional. Fed length
 
         Returns
         -------
-        Retractor
+        dict
             Retractor object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -151,15 +151,15 @@
             Model that the retractor will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Retractor
+        dict
             Retractor object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first retractor in the model
@@ -350,15 +350,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Retractor
+        dict
             Retractor object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the retractors in the model
@@ -756,15 +756,15 @@
         Parameters
         ----------
         prop : string
             retractor property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this retractor (\*ELEMENT_SEATBELT_RETREROMETER)
@@ -887,23 +887,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Retractor
+        dict
             Retractor object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this retractor
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/rigidbodies.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/rigidbodies.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         model : Model
             Model that constrained rigid bodies will be created in
         options : dict
             Options specifying which properties would be used to create the keyword. If optional values are not used, then the default values below will be used
 
         Returns
         -------
-        RigidBodies
+        dict
             RigidBodies object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -131,15 +131,15 @@
             Model that the constrained rigid bodies definition will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        RigidBodies
+        dict
             RigidBodies object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first rigid body merge in the model
@@ -262,15 +262,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        RigidBodies
+        dict
             RigidBodies object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select rigid body merges using standard PRIMER object menus
@@ -630,15 +630,15 @@
         Parameters
         ----------
         prop : string
             rigid body merge property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this constrained rigid bodies (\*CONSTRAINED_RIGID_BODIES).
@@ -761,23 +761,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        RigidBodies
+        dict
             RigidBodies object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this rigid body merge
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/rigidwall.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/rigidwall.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         rwid : integer
             Optional. Rigidwall number
         heading : string
             Optional. Title for the Rigidwall
 
         Returns
         -------
-        Rigidwall
+        dict
             Rigidwall object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -142,15 +142,15 @@
             Model that the rigidwall will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Rigidwall
+        dict
             Rigidwall object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first rigidwall in the model
@@ -341,15 +341,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Rigidwall
+        dict
             Rigidwall object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the rigidwalls in the model
@@ -748,15 +748,15 @@
         Parameters
         ----------
         prop : string
             rigidwall property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetRow(self, row):
         """
         Returns the data for an NSEGS card row in the rigidwall
@@ -931,23 +931,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Rigidwall
+        dict
             Rigidwall object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this rigidwall
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/seatbelt1d.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/seatbelt1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         n1 : integer
             Node 1 ID
         n2 : integer
             Node 2 ID
 
         Returns
         -------
-        Seatbelt1D
+        dict
             Seatbelt1D object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -134,15 +134,15 @@
             Model that the seatbelt will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Seatbelt1D
+        dict
             Seatbelt1D object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first seatbelt in the model
@@ -333,15 +333,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Seatbelt1D
+        dict
             Seatbelt1D object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the seatbelts in the model
@@ -739,15 +739,15 @@
         Parameters
         ----------
         prop : string
             seatbelt property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this seatbelt (\*ELEMENT_SEATBELT)
@@ -881,23 +881,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Seatbelt1D
+        dict
             Seatbelt1D object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this seatbelt
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/seatbelt2d.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/seatbelt2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         n3 : integer
             Node 3 ID
         n4 : integer
             Node 4 ID
 
         Returns
         -------
-        Seatbelt2D
+        dict
             Seatbelt2D object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -138,15 +138,15 @@
             Model that the seatbelt will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Seatbelt2D
+        dict
             Seatbelt2D object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first seatbelt in the model
@@ -337,15 +337,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Seatbelt2D
+        dict
             Seatbelt2D object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select seatbelts using standard PRIMER object menus
@@ -705,15 +705,15 @@
         Parameters
         ----------
         prop : string
             seatbelt property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this seatbelt (\*ELEMENT_SEATBELT)
@@ -836,23 +836,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Seatbelt2D
+        dict
             Seatbelt2D object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this seatbelt
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/section.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/section.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             Section.SPH or
             Section.TSHELL
         title : string
             Optional. Title for the section
 
         Returns
         -------
-        Section
+        dict
             Section object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -142,15 +142,15 @@
             Model that the sect will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Section
+        dict
             Section object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first section in the model
@@ -341,15 +341,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Section
+        dict
             Section object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the sections in the model
@@ -779,15 +779,15 @@
         Parameters
         ----------
         prop : string
             section property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetPointData(self, ipt):
         """
         Returns the point data for a single point in \*SECTION_POINT_SOURCE
@@ -1029,23 +1029,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Section
+        dict
             Section object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this section
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/sensor.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         nid : integer
             Optional. Optional node ID: Compulsory for types 1 and 4
         nid2 : integer
             Optional. Optional node ID 2: Compulsory for type 4
 
         Returns
         -------
-        Sensor
+        dict
             Sensor object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -136,15 +136,15 @@
             Model that the sensor will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Sensor
+        dict
             Sensor object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first sensor in the model
@@ -335,15 +335,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Sensor
+        dict
             Sensor object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the sensors in the model
@@ -741,15 +741,15 @@
         Parameters
         ----------
         prop : string
             sensor property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this sensor (\*ELEMENT_SEATBELT_SENSEROMETER)
@@ -872,23 +872,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Sensor
+        dict
             Sensor object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this sensor
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/sensorcontrol.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/sensorcontrol.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         type_id : integer
             Optional. ID of entity to be controlled if type is not FUNCTION or input value for FUNCTION
         estyp : string
             Optional. Element Set Type to be controlled. Can be "BEAM", "DISC", "SHELL", "SOLID", "TSHELL". Required only if Type argument is "ELESET"
 
         Returns
         -------
-        SensorControl
+        dict
             SensorControl object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -93,15 +93,15 @@
             Model that the \*SENSOR_CONTROL will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        SensorControl
+        dict
             SensorControl object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first \*SENSOR_CONTROL in the model
@@ -588,15 +588,15 @@
         Parameters
         ----------
         prop : string
             \*SENSOR_CONTROL property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this \*SENSOR_CONTROL.
@@ -708,23 +708,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        SensorControl
+        dict
             SensorControl object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this \*SENSOR_CONTROL
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/sensordefine.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/sensordefine.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             It is NODE or NODE set ID for SensorDefine.DEFINE_NODE or SensorDefine.DEFINE_NODE_SET respectively,
             Sensor Define ID for SensorDefine.DEFINE_CALC_MATH,
             Element ID or Element set ID for SensorDefine.DEFINE_ELEMENT or SensorDefine.DEFINE_ELEMENT_SET respectively or
             Type ID for SensorDefine.DEFINE_FORCE
 
         Returns
         -------
-        SensorDefine
+        dict
             SensorDefine object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -114,15 +114,15 @@
             Model that the \*SENSOR_DEFINE will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        SensorDefine
+        dict
             SensorDefine object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first \*SENSOR_DEFINE in the model
@@ -538,15 +538,15 @@
         Parameters
         ----------
         prop : string
             \*SENSOR_DEFINE property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this \*SENSOR_DEFINE.
@@ -616,23 +616,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        SensorDefine
+        dict
             SensorDefine object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this \*SENSOR_DEFINE
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/sensorswitch.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/sensorswitch.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             SensorSwitch id. This is required for the
             SensorSwitch.SWITCH and
             SensorSwitch.SWITCH_CALC_LOGIC options and ignored for
             SensorSwitch.SWITCH_SHELL_TO_VENT
 
         Returns
         -------
-        SensorSwitch
+        dict
             SensorSwitch object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -94,15 +94,15 @@
             Model that the \*SENSOR_SWITCH will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        SensorSwitch
+        dict
             SensorSwitch object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first \*SENSOR_SWITCH in the model
@@ -518,15 +518,15 @@
         Parameters
         ----------
         prop : string
             \*SENSOR_SWITCH property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetRow(self, row):
         """
         Returns the data for a row in the SENSOR_SWITCH_SHELL_TO_VENT
@@ -700,23 +700,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        SensorSwitch
+        dict
             SensorSwitch object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this \*SENSOR_SWITCH
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/set.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/set.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             Set.ADD,
             Set.INTERSECT,
             Set.GENERAL or
             Set.GENERATE
 
         Returns
         -------
-        Set
+        dict
             Set object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -201,15 +201,15 @@
             Set.TSHELL
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Set
+        dict
             Set object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, type, modal)
 
     def First(model, type):
         """
         Returns the first set in the model
@@ -550,15 +550,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Set
+        dict
             Set object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", type, prompt, limit, modal, button_text)
 
     def RenumberAll(model, start, type=Oasys.gRPC.defaultArg):
         """
         Renumbers all of the sets in the model
@@ -1089,15 +1089,15 @@
         Parameters
         ----------
         number : Integer
             The index of the child collect set to return. Note that indices start at 0, not 1
 
         Returns
         -------
-        Set
+        dict
             Set object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetCollectChild", number)
 
     def GetGeneralData(self, index):
         """
         Returns a line of data for a GENERAL set
@@ -1338,12 +1338,12 @@
 
     def Xrefs(self):
         """
         Returns the cross references for this set
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/shell.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         n7 : integer
             Optional. Node number 7
         n8 : integer
             Optional. Node number 8
 
         Returns
         -------
-        Shell
+        dict
             Shell object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -152,15 +152,15 @@
             Model that the shell will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Shell
+        dict
             Shell object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def FillHolesOnFlagged(model, flag, remeshhole, pid=Oasys.gRPC.defaultArg, max_hole_size=Oasys.gRPC.defaultArg, mesh_element_size=Oasys.gRPC.defaultArg, planarsurface=Oasys.gRPC.defaultArg):
         """
         Fills multiple holes using flagged shells
@@ -446,15 +446,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Shell
+        dict
             Shell object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def PickIsoparametric(prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg, button_text=Oasys.gRPC.defaultArg):
         """
         Allows the user to pick a point on a shell. The isoparametric coordinates of the point picked on the
@@ -478,15 +478,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Shell
+        dict
             List containing Shell object and isoparametric coordinates (or None if not picked or the point is not on a shell)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "PickIsoparametric", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the shells in the model
@@ -1054,15 +1054,15 @@
         Parameters
         ----------
         prop : string
             shell property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetShellReferenceGeometry(self):
         """
         Returns the airbag shell reference geometry of the shell
@@ -1362,15 +1362,15 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Shell
+        dict
             Shell object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Warpage(self):
         """
         Calculates the warpage for the shell
@@ -1402,12 +1402,12 @@
 
     def Xrefs(self):
         """
         Returns the cross references for this shell
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/shellreferencegeometry.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/shellreferencegeometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         model : Model
             Model that ShellReferenceGeometry will be created in
         aid : integer
             Optional. ShellReferenceGeometry number to set _ID suffix
 
         Returns
         -------
-        ShellReferenceGeometry
+        dict
             ShellReferenceGeometry object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -84,15 +84,15 @@
             Model that the asrg will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        ShellReferenceGeometry
+        dict
             ShellReferenceGeometry object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first airbag shell reference geometry in the model
@@ -283,15 +283,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        ShellReferenceGeometry
+        dict
             ShellReferenceGeometry object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the airbag shell reference geometrys in the model
@@ -608,15 +608,15 @@
         Parameters
         ----------
         prop : string
             airbag shell reference geometry property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetShell(self, eid):
         """
         Returns the shell reference geometry nodes and pid for the shell
@@ -809,23 +809,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        ShellReferenceGeometry
+        dict
             ShellReferenceGeometry object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this airbag shell reference geometry
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/slipring.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/slipring.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         sbid2 : integer
             Seatbelt number 2
         sbrnid : integer
             Slipring Node number
 
         Returns
         -------
-        Slipring
+        dict
             Slipring object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -134,15 +134,15 @@
             Model that the slipring will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Slipring
+        dict
             Slipring object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first slipring in the model
@@ -333,15 +333,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Slipring
+        dict
             Slipring object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the sliprings in the model
@@ -739,15 +739,15 @@
         Parameters
         ----------
         prop : string
             slipring property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this slipring (\*ELEMENT_SEATBELT_SLIPEROMETER)
@@ -870,23 +870,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Slipring
+        dict
             Slipring object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this slipring
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/solid.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/solid.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         n7 : integer
             Optional. Node number 7
         n8 : integer
             Optional. Node number 8
 
         Returns
         -------
-        Solid
+        dict
             Solid object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -182,15 +182,15 @@
             Model that the solid will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Solid
+        dict
             Solid object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def FindSolidInBox(model, xmin, xmax, ymin, ymax, zmin, zmax, flag=Oasys.gRPC.defaultArg, excl=Oasys.gRPC.defaultArg, vis_only=Oasys.gRPC.defaultArg):
         """
         Returns a list of Solid objects for the solids within a box.
@@ -425,15 +425,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Solid
+        dict
             Solid object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the solids in the model
@@ -858,15 +858,15 @@
         Parameters
         ----------
         prop : string
             solid property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Jacobian(self):
         """
         Calculates the jacobian for the solid
@@ -1044,15 +1044,15 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Solid
+        dict
             Solid object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Volume(self):
         """
         Calculates the volume for the solid
@@ -1077,12 +1077,12 @@
 
     def Xrefs(self):
         """
         Returns the cross references for this solid
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/spc.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/spc.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         label : integer
             Optional. Spc number
         heading : string
             Optional. Title for the spc
 
         Returns
         -------
-        Spc
+        dict
             Spc object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -333,15 +333,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Spc
+        dict
             Spc object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the boundary SPCs in the model
@@ -675,15 +675,15 @@
         Parameters
         ----------
         prop : string
             boundary SPC property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this spc (\*BOUNDARY_SPC_xxxx).
@@ -804,23 +804,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Spc
+        dict
             Spc object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this boundary SPC
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/sph.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/sph.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,30 +48,30 @@
 
 
 # Constructor
     def __init__(self, model, nid, pid, mass):
         handle = Oasys.PRIMER._connection.constructor(self.__class__.__name__, model, nid, pid, mass)
         Oasys.gRPC.OasysItem.__init__(self, self.__class__.__name__, handle)
         """
-        Create a new :py:class:`Sph<>` object
+        Create a new   object
 
         Parameters
         ----------
         model : Model
             Model that sph will be created in
         nid : integer
             Node ID and Element ID are the same for the SPH option
         pid : integer
             Part ID to which this element belongs
         mass : real
             Mass value
 
         Returns
         -------
-        Sph
+        dict
             Sph object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -132,15 +132,15 @@
             Model that the sph will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Sph
+        dict
             Sph object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first sph in the model
@@ -331,15 +331,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Sph
+        dict
             Sph object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the sphs in the model
@@ -737,15 +737,15 @@
         Parameters
         ----------
         prop : string
             sph property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this sph (\*ELEMENT_SPH)
@@ -868,23 +868,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Sph
+        dict
             Sph object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this sph
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/spotweld.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/spotweld.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         n2 : integer
             Node ID 2
         label : integer
             Optional. Constrained spotweld number
 
         Returns
         -------
-        Spotweld
+        dict
             Spotweld object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -132,15 +132,15 @@
             Model that the spotweld will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Spotweld
+        dict
             Spotweld object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first spotweld in the model
@@ -331,15 +331,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Spotweld
+        dict
             Spotweld object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the spotwelds in the model
@@ -737,15 +737,15 @@
         Parameters
         ----------
         prop : string
             spotweld property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this spotweld (\*CONSTRAINED_SPOTWELD).
@@ -868,23 +868,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Spotweld
+        dict
             Spotweld object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this spotweld
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/spr2.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/spr2.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         lpid : integer
             Lower Sheet Part ID
         nsid : integer
             Node Set ID of rivet location nodes
 
         Returns
         -------
-        Spr2
+        dict
             Spr2 object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -247,15 +247,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Spr2
+        dict
             Spr2 object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select spr2s using standard PRIMER object menus
@@ -566,15 +566,15 @@
         Parameters
         ----------
         prop : string
             spr2 property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this spr2 (\*CONSTRAINED_SPR2).
@@ -697,23 +697,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Spr2
+        dict
             Spr2 object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this spr2
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/stagedconstructionpart.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/stagedconstructionpart.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         stga : integer
             Construction stage at which part is added
         stgr : integer
             Construction stage at which part is removed
 
         Returns
         -------
-        StagedConstructionPart
+        dict
             StagedConstructionPart object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -139,15 +139,15 @@
             Model that the Define staged construction parts card will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        StagedConstructionPart
+        dict
             StagedConstructionPart object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first Define staged construction part in the model
@@ -270,15 +270,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        StagedConstructionPart
+        dict
             StagedConstructionPart object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select Define staged construction parts using standard PRIMER object menus
@@ -623,15 +623,15 @@
         Parameters
         ----------
         prop : string
             Define staged construction part property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this Define staged construction parts (\*Define_staged_construction_part).
@@ -754,23 +754,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        StagedConstructionPart
+        dict
             StagedConstructionPart object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this Define staged construction part
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/strainshell.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/strainshell.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         large : integer
             Large format flag, set 0 to turn it off or 1 to enable it. It is optional and set to 0 by default
         ilocal : integer
             Flag for coordinate system of strain components. Set to 0 for global or 1 to enable local. It is optional and set to 0 by default
 
         Returns
         -------
-        StrainShell
+        dict
             StrainShell object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -211,15 +211,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        StrainShell
+        dict
             StrainShell object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select initial strain shells using standard PRIMER object menus
@@ -481,15 +481,15 @@
         Parameters
         ----------
         prop : string
             initial strain shell property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this initial strain shell (\*INITIAL_STRAIN_SHELL).
@@ -620,23 +620,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        StrainShell
+        dict
             StrainShell object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this initial strain shell
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/strainsolid.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/strainsolid.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         epsyz : real
             The yzth strain component in the global cartesian system
         epszx : real
             The zxth strain component in the global cartesian system
 
         Returns
         -------
-        StrainSolid
+        dict
             StrainSolid object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -215,15 +215,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        StrainSolid
+        dict
             StrainSolid object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select initial strain solids using standard PRIMER object menus
@@ -468,15 +468,15 @@
         Parameters
         ----------
         prop : string
             initial strain solid property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this initial strain solid (\*INITIAL_STRESS_SOLID).
@@ -588,23 +588,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        StrainSolid
+        dict
             StrainSolid object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this initial strain solid
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/stressbeam.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/stressbeam.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             Optional. Number of variables giving beam local axes.
             Valid values are:
             StressBeam.NAXES_0 or
             StressBeam.NAXES_12
 
         Returns
         -------
-        StressBeam
+        dict
             StressBeam object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -222,15 +222,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        StressBeam
+        dict
             StressBeam object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select initial stress beams using standard PRIMER object menus
@@ -506,15 +506,15 @@
         Parameters
         ----------
         prop : string
             initial stress beam property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this initial stress beam (\*INITIAL_STRESS_BEAM).
@@ -666,23 +666,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        StressBeam
+        dict
             StressBeam object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this initial stress beam
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/stresssection.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/stresssection.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         izshear : integer
             Shear stress flag
         istiff : integer
             Optional. Load curve ID defining artificial stress fraction versus time
 
         Returns
         -------
-        StressSection
+        dict
             StressSection object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -140,15 +140,15 @@
             Model that the stress section will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        StressSection
+        dict
             StressSection object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first stress section in the model
@@ -701,15 +701,15 @@
         Parameters
         ----------
         prop : string
             stress section property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this stress section.
@@ -832,23 +832,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        StressSection
+        dict
             StressSection object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this stress section
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/stressshell.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/stressshell.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         nhisv : integer
             Number of additional history variables
         ntensr : integer
             Number of components of tensor data taken from the element history variables stored
 
         Returns
         -------
-        StressShell
+        dict
             StressShell object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -211,15 +211,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        StressShell
+        dict
             StressShell object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select initial stress shells using standard PRIMER object menus
@@ -483,15 +483,15 @@
         Parameters
         ----------
         prop : string
             initial stress shell property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetThermalIntegrationPoint(self, index):
         """
         Returns the thermal data for a specific integration point as a list. For each integration point there will be
@@ -665,23 +665,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        StressShell
+        dict
             StressShell object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this initial stress shell
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/stresssolid.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/stresssolid.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         large : boolean
             true if large format, false otherwise
         iveflg : integer
             Initial volume energy flag (only used if large is TRUE). Valid values are 0, 1 and 2 only
 
         Returns
         -------
-        StressSolid
+        dict
             StressSolid object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -212,15 +212,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        StressSolid
+        dict
             StressSolid object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select initial stress solids using standard PRIMER object menus
@@ -484,15 +484,15 @@
         Parameters
         ----------
         prop : string
             initial stress solid property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetThermalIntegrationPoint(self, index):
         """
         Returns the thermal data for a specific integration point as a list. For each integration point there will be
@@ -667,23 +667,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        StressSolid
+        dict
             StressSolid object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this initial stress solid
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/termination.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/termination.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             Curve ID for Termination.CURVE, OR
             Part Set ID for Termination.DELETED_SHELLS_SET or 
             Termination.DELETED_SOLIDS_SET, OR
             Sensor Switch ID for Termination.SENSOR
 
         Returns
         -------
-        Termination
+        dict
             Termination object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -104,15 +104,15 @@
             Model that the Termination will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Termination
+        dict
             Termination object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first termination in the model
@@ -422,15 +422,15 @@
         Parameters
         ----------
         prop : string
             termination property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this Termination (\*TERMINATION_xxxx)
@@ -500,23 +500,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Termination
+        dict
             Termination object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this termination
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/tiebreak.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/tiebreak.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         nsid2 : integer
             Second Node Set ID
         eppf : float
             Optional. Plastic strain at failure
 
         Returns
         -------
-        TieBreak
+        dict
             TieBreak object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -244,15 +244,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        TieBreak
+        dict
             TieBreak object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select tie-breaks using standard PRIMER object menus
@@ -563,15 +563,15 @@
         Parameters
         ----------
         prop : string
             tie-break property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this tie-break (\*\*CONSTRAINED_TIE_BREAK).
@@ -694,23 +694,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        TieBreak
+        dict
             TieBreak object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this tie-break
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/transformation.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         tranid : integer
             Transformation label
         title : string
             Optional. Transformation title
 
         Returns
         -------
-        Transformation
+        dict
             Transformation object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -86,15 +86,15 @@
             Model that the transformation will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Transformation
+        dict
             Transformation object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first transformation in the model
@@ -492,15 +492,15 @@
         Parameters
         ----------
         prop : string
             transformation property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def GetRow(self, row):
         """
         Returns the data for a row in the transformation
@@ -622,23 +622,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Transformation
+        dict
             Transformation object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this transformation
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/tshell.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/tshell.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         n7 : integer
             Optional. Node number 7
         n8 : integer
             Optional. Node number 8
 
         Returns
         -------
-        Tshell
+        dict
             Tshell object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -147,15 +147,15 @@
             Model that the thick shell will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Tshell
+        dict
             Tshell object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def FindTshellInBox(model, xmin, xmax, ymin, ymax, zmin, zmax, flag=Oasys.gRPC.defaultArg, excl=Oasys.gRPC.defaultArg, vis_only=Oasys.gRPC.defaultArg):
         """
         Returns a list of Tshell objects for the thick shells within a box.
@@ -390,15 +390,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Tshell
+        dict
             Tshell object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the thick shells in the model
@@ -863,15 +863,15 @@
         Parameters
         ----------
         prop : string
             thick shell property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Jacobian(self):
         """
         Calculates the jacobian for the thick shell
@@ -1056,15 +1056,15 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Tshell
+        dict
             Tshell object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Warpage(self):
         """
         Calculates the warpage for the thick shell
@@ -1078,12 +1078,12 @@
 
     def Xrefs(self):
         """
         Returns the cross references for this thick shell
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/utils.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/utils.py`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/vector.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         cid : int
             Optional. Coordinate system ID
         heading : string
             Optional. Title for the vector
 
         Returns
         -------
-        Vector
+        dict
             Vector object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -144,15 +144,15 @@
             Model that the vector will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        Vector
+        dict
             Vector object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first vector in the model
@@ -343,15 +343,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Vector
+        dict
             Vector object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def RenumberAll(model, start):
         """
         Renumbers all of the vectors in the model
@@ -734,15 +734,15 @@
         Parameters
         ----------
         prop : string
             vector property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this vector (\*DEFINE_VECTOR).
@@ -865,23 +865,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Vector
+        dict
             Vector object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this vector
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/velocity.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/velocity.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         vzre : float
             Optional. Initial rotational velocity about Z axis of exempted nodes
         icid : float
             Optional. Local coordinate system nodes
 
         Returns
         -------
-        Velocity
+        dict
             Velocity object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -272,15 +272,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        Velocity
+        dict
             Velocity object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select initial velocitys using standard PRIMER object menus
@@ -591,15 +591,15 @@
         Parameters
         ----------
         prop : string
             initial velocity property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this initial velocity (\*INITIAL_VELOCITY).
@@ -722,23 +722,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        Velocity
+        dict
             Velocity object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this initial velocity
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/velocitygeneration.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/velocitygeneration.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         irigid : integer
             Overide part inertia flag
         icid : integer
             Local coordinate system
 
         Returns
         -------
-        VelocityGeneration
+        dict
             VelocityGeneration object
         """
 
 
 # String representation
     def __repr__(self):
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "toString")
@@ -164,15 +164,15 @@
             Model that the initial velocity generation definition will be created in
         modal : boolean
             Optional. If this window is modal (blocks the user from doing anything else in PRIMER
             until this window is dismissed). If omitted the window will be modal
 
         Returns
         -------
-        VelocityGeneration
+        dict
             VelocityGeneration object (or None if not made)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Create", model, modal)
 
     def First(model):
         """
         Returns the first initial velocity generation in the model
@@ -295,15 +295,15 @@
         button_text : string
             Optional. By default the window with the prompt will have a button labelled 'Cancel'
             which if pressed will cancel the pick and return None. If you want to change the
             text on the button use this argument. If omitted 'Cancel' will be used
 
         Returns
         -------
-        VelocityGeneration
+        dict
             VelocityGeneration object (or None if not picked)
         """
         return Oasys.PRIMER._connection.classMethod(__class__.__name__, "Pick", prompt, limit, modal, button_text)
 
     def Select(flag, prompt, limit=Oasys.gRPC.defaultArg, modal=Oasys.gRPC.defaultArg):
         """
         Allows the user to select initial velocity generations using standard PRIMER object menus
@@ -648,15 +648,15 @@
         Parameters
         ----------
         prop : string
             initial velocity generation property to get parameter for
 
         Returns
         -------
-        Parameter
+        dict
             Parameter object if property is a parameter, None if not
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "GetParameter", prop)
 
     def Keyword(self):
         """
         Returns the keyword for this initial velocity (\*INITIAL_VELOCITY_GENERATION).
@@ -779,23 +779,23 @@
         Object properties that are parameters are normally returned as the integer or
         float parameter values as that is virtually always what the user would want. This function temporarily
         changes the behaviour so that if a property is a parameter the parameter name is returned instead.
         This can be used with 'method chaining' (see the example below) to make sure a property argument is correct
 
         Returns
         -------
-        VelocityGeneration
+        dict
             VelocityGeneration object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "ViewParameters")
 
     def Xrefs(self):
         """
         Returns the cross references for this initial velocity generation
 
         Returns
         -------
-        Xrefs
+        dict
             Xrefs object
         """
         return Oasys.PRIMER._connection.instanceMethod(self.__class__.__name__, self._handle, "Xrefs")
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/view.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/view.py`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/window.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/window.py`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/workflow.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/workflow.py`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys/PRIMER/xrefs.py` & `Oasys.PRIMER-21.0.0b9/src/Oasys/PRIMER/xrefs.py`

 * *Files identical despite different names*

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys.PRIMER.egg-info/PKG-INFO` & `Oasys.PRIMER-21.0.0b9/src/Oasys.PRIMER.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Oasys.PRIMER
-Version: 21.0.0b8
+Version: 21.0.0b9
 Summary: Python API for Oasys PRIMER
 Author: Miles Thornton
 Maintainer-email: DYNA support <dyna.support@arup.com>
 License: MIT License
         
         Copyright (c) 2024 Oasys Ltd
         
@@ -30,15 +30,15 @@
 Project-URL: Homepage, https://www.oasys-software.com/dyna/software/primer/
 Project-URL: Linkedin, https://www.linkedin.com/company/oasys-ltd-software/
 Project-URL: YouTube, https://www.youtube.com/c/OasysLtd
 Keywords: Oasys,PRIMER
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Oasys.gRPC>=21.0.0b4
+Requires-Dist: Oasys.gRPC>=21.0.0b5
 
 The Oasys.PRIMER package allows Python scripts to control the Oasys LS-DYNA Environment
 software `PRIMER <https://www.oasys-software.com/dyna/software/primer/>`_.
 
 Basic Information
 -----------------
```

### Comparing `Oasys.PRIMER-21.0.0b8/src/Oasys.PRIMER.egg-info/SOURCES.txt` & `Oasys.PRIMER-21.0.0b9/src/Oasys.PRIMER.egg-info/SOURCES.txt`

 * *Files identical despite different names*

