# Comparing `tmp/field-compression-benchmark-0.0.1.tar.gz` & `tmp/field-compression-benchmark-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "field-compression-benchmark-0.0.1.tar", last modified: Fri Mar 15 07:44:22 2024, max compression
+gzip compressed data, was "field-compression-benchmark-0.0.2.tar", last modified: Tue Apr  2 09:27:31 2024, max compression
```

## Comparing `field-compression-benchmark-0.0.1.tar` & `field-compression-benchmark-0.0.2.tar`

### file list

```diff
@@ -1,301 +1,316 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.930295 field-compression-benchmark-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.898295 field-compression-benchmark-0.0.1/.cargo/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/.cargo/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)    90132 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-03-15 07:44:22.930295 field-compression-benchmark-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.890295 field-compression-benchmark-0.0.1/codecs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/bit-round/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/bit-round/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/bit-round/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/bit-round/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/bit-transpose/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/bit-transpose/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/bit-transpose/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/bit-transpose/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/build/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/build/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/build/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/build/src/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/build/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/core/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/core/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core/src/buffer.rs
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core/src/casts.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core/src/map.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core/src/slice.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core/src/ty.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/core-host/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core-host/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/core-host/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core-host/src/codec.rs
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core-host/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core-host/src/plugin.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/core-wasm/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core-wasm/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/core-wasm/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core-wasm/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core-wasm/src/convert.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/core-wasm/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.902295 field-compression-benchmark-0.0.1/codecs/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/frontend/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/frontend/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12411 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/frontend/src/codec.rs
--rw-r--r--   0 runner    (1001) docker     (127)    21555 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/frontend/src/engine.rs
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/frontend/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/frontend/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)    24170 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/frontend/src/template.rs
--rw-r--r--   0 runner    (1001) docker     (127)    44307 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/frontend/src/transform.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/identity/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/identity/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/identity/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/identity/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/linear-quantize/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/linear-quantize/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/linear-quantize/src/
--rw-r--r--   0 runner    (1001) docker     (127)    16918 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/linear-quantize/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/log/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/log/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/log/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/log/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/reinterpret/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/reinterpret/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/reinterpret/src/
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/reinterpret/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/sz3/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/sz3/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/sz3/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/sz3/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/wit/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/wit/world.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/zfp/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/zfp/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/zfp/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/zfp/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)    13353 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/zfp/src/zfp.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/zlib/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/zlib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/zlib/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/zlib/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/zstd/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/zstd/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/codecs/zstd/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/codecs/zstd/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.894295 field-compression-benchmark-0.0.1/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.906295 field-compression-benchmark-0.0.1/core/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/benchmark/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/benchmark/src/
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/benchmark/src/case.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/benchmark/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/benchmark/src/goodness.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/benchmark/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11021 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/benchmark/src/measuring.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/benchmark/src/performance.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/benchmark/src/report.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/benchmark/src/reporter.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/benchmark/src/settings.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/compressor/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/compressor/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/compressor/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/compressor/src/codec/
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/compressor/src/codec/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/compressor/src/codec/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/compressor/src/compress.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/compressor/src/compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/compressor/src/compressor/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/compressor/src/compressor/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/compressor/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/compressor/src/numcodecs.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/compressor/src/parameter/
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/compressor/src/parameter/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/compressor/src/parameter/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/dataset/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/dataset/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/dataset/src/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/dataset/src/dataset/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/dataset/src/dataset/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/dataset/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)    29808 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/dataset/src/units.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/dataset/src/variable/
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/dataset/src/variable/config.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/dataset/src/variable/derivative/
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/dataset/src/variable/derivative/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/dataset/src/variable/derivative/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/dataset/src/variable/dimension/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/dataset/src/variable/dimension/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/dataset/src/variable/dimension/config/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/dataset/src/variable/dimension/config/slice.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/dataset/src/variable/dimension/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/dataset/src/variable/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/error/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/error/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.910295 field-compression-benchmark-0.0.1/core/error/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/error/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.914295 field-compression-benchmark-0.0.1/core/goodness/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/goodness/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.914295 field-compression-benchmark-0.0.1/core/goodness/src/
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/goodness/src/bit_information.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/goodness/src/correlation.rs
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/goodness/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/goodness/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/goodness/src/pca.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/goodness/src/uniformity.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.914295 field-compression-benchmark-0.0.1/core/measure/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/measure/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.914295 field-compression-benchmark-0.0.1/core/measure/src/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/measure/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/measure/src/measurement.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/measure/src/stats.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.914295 field-compression-benchmark-0.0.1/core/model/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.914295 field-compression-benchmark-0.0.1/core/model/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.914295 field-compression-benchmark-0.0.1/core/model/src/boundary/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/boundary/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/boundary/noop.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/boundary/periodic.rs
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/boundary/zero.rs
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.914295 field-compression-benchmark-0.0.1/core/model/src/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/model/linadv.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/model/lorenz_63.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/model/lorenz_96.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/model/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/num.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.918295 field-compression-benchmark-0.0.1/core/model/src/timestep/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/timestep/direct.rs
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/timestep/euler_smoothing.rs
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/timestep/leapfrog.rs
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/timestep/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/core/model/src/timestep/runge_kutta.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.894295 field-compression-benchmark-0.0.1/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.918295 field-compression-benchmark-0.0.1/data/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/data/codecs/wasmtime.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.918295 field-compression-benchmark-0.0.1/fcbench/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.926295 field-compression-benchmark-0.0.1/fcbench/fcbench/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/fcbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/fcbench/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/fcbench/codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/fcbench/compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/fcbench/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/fcbench/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    29655 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/fcbench/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.918295 field-compression-benchmark-0.0.1/fcbench/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/src/benchmark.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/src/compressor.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/src/dataclass.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/src/dataset.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fcbench/src/model.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.930295 field-compression-benchmark-0.0.1/field_compression_benchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-03-15 07:44:22.000000 field-compression-benchmark-0.0.1/field_compression_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-03-15 07:44:22.000000 field-compression-benchmark-0.0.1/field_compression_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 07:44:22.000000 field-compression-benchmark-0.0.1/field_compression_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-15 07:44:22.000000 field-compression-benchmark-0.0.1/field_compression_benchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-15 07:44:22.000000 field-compression-benchmark-0.0.1/field_compression_benchmark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.918295 field-compression-benchmark-0.0.1/fork/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fork/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.918295 field-compression-benchmark-0.0.1/fork/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fork/src/fork.rs
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fork/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.918295 field-compression-benchmark-0.0.1/fork/src/reaper/
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fork/src/reaper/canary.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fork/src/reaper/handler.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fork/src/reaper/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fork/src/reaper/worker.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/fork/src/work.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/rust-toolchain
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/rustfmt.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 07:44:22.930295 field-compression-benchmark-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.918295 field-compression-benchmark-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/src/args.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.918295 field-compression-benchmark-0.0.1/src/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/src/benchmarking/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/src/benchmarking/prepare.rs
--rw-r--r--   0 runner    (1001) docker     (127)    15259 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/src/benchmarking/report.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/src/fcpy.rs
--rw-r--r--   0 runner    (1001) docker     (127)    15989 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.898295 field-compression-benchmark-0.0.1/wasi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.918295 field-compression-benchmark-0.0.1/wasi/build/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/build/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/build/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.918295 field-compression-benchmark-0.0.1/wasi/build/src/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/build/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.918295 field-compression-benchmark-0.0.1/wasi/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/cli/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/cli/src/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/cli/src/environment.rs
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/cli/src/exit.rs
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/cli/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/cli/src/stdio.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/cli/src/terminal.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/clocks/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/clocks/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/clocks/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/clocks/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/filesystem/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/filesystem/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/filesystem/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/io/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/io/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/io/src/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/io/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/io/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/io/src/poll.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/io/src/streams.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/random/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/random/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/random/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/random/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/wit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.898295 field-compression-benchmark-0.0.1/wasi/wit/deps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/wit/deps/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/cli/command.wit
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/cli/environment.wit
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/cli/exit.wit
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/cli/imports.wit
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/cli/run.wit
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/cli/stdio.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/cli/terminal.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/wit/deps/clocks/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/clocks/monotonic-clock.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/clocks/wall-clock.wit
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/clocks/world.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.922295 field-compression-benchmark-0.0.1/wasi/wit/deps/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/filesystem/preopens.wit
--rw-r--r--   0 runner    (1001) docker     (127)    27621 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/filesystem/types.wit
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/filesystem/world.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.926295 field-compression-benchmark-0.0.1/wasi/wit/deps/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/http/handler.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/http/proxy.wit
--rw-r--r--   0 runner    (1001) docker     (127)    24187 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/http/types.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.926295 field-compression-benchmark-0.0.1/wasi/wit/deps/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/io/error.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/io/poll.wit
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/io/streams.wit
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/io/world.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.926295 field-compression-benchmark-0.0.1/wasi/wit/deps/random/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/random/insecure-seed.wit
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/random/insecure.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/random/random.wit
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/random/world.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:44:22.926295 field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/instance-network.wit
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/ip-name-lookup.wit
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/network.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/tcp-create-socket.wit
--rw-r--r--   0 runner    (1001) docker     (127)    20199 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/tcp.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/udp-create-socket.wit
--rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/udp.wit
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/world.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-15 07:44:07.000000 field-compression-benchmark-0.0.1/wasi/wit/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.738675 field-compression-benchmark-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/.cargo/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    88816 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-02 09:27:31.738675 field-compression-benchmark-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.698675 field-compression-benchmark-0.0.2/codecs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/bit-round/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/bit-round/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/bit-round/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/bit-round/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/bit-transpose/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/bit-transpose/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/bit-transpose/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/bit-transpose/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/build/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/build/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/build/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/build/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/build/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/core/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/src/buffer.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/src/casts.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/src/map.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/src/slice.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/src/ty.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/core-host/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-host/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/core-host/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    11816 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-host/src/codec.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-host/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-host/src/plugin.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/core-wasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-wasm/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/core-wasm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-wasm/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-wasm/src/convert.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-wasm/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/frontend/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/src/codec.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    21585 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/src/engine.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    24426 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/src/template.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    44331 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/src/transform.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/identity/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/identity/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/identity/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/linear-quantize/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/linear-quantize/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/linear-quantize/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    18818 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/linear-quantize/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/log/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/log/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/log/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/reinterpret/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/reinterpret/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/reinterpret/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/reinterpret/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/sz3/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/sz3/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/sz3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/sz3/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/uniform-noise/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/uniform-noise/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/uniform-noise/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/uniform-noise/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/wit/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/wit/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/zfp/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zfp/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/zfp/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zfp/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    13336 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zfp/src/zfp.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/zlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zlib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/zlib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zlib/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/zstd/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zstd/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/zstd/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zstd/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.702675 field-compression-benchmark-0.0.2/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/core/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/core/benchmark/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/case.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/goodness.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/measuring.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/performance.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/report.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/reporter.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/settings.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/core/compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/core/compressor/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/core/compressor/src/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/codec/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/codec/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/compress.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/compressor/src/compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/compressor/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/compressor/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/numcodecs.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/compressor/src/parameter/
+-rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/parameter/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    24245 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/parameter/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/src/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/dataset/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/dataset/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    29862 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/units.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/src/variable/
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/config.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/src/variable/derivative/
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/derivative/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/derivative/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/config/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/config/slice.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/error/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/error/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/error/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/goodness/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/goodness/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/src/bit_information.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/src/correlation.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/src/pca.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/src/uniformity.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/measure/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/measure/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/core/measure/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/measure/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/measure/src/measurement.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/measure/src/stats.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/core/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/core/model/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/core/model/src/boundary/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/boundary/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/boundary/noop.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/boundary/periodic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/boundary/zero.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/core/model/src/extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/extrapolation/direct.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/extrapolation/euler_smoothing.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/extrapolation/leapfrog.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/extrapolation/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/extrapolation/runge_kutta.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/core/model/src/model/
+-rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/any.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/linadv.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/lorenz_63.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/lorenz_96.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/onedsw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/twodsw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/num.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.702675 field-compression-benchmark-0.0.2/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/data/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/data/codecs/wasmtime.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/fcbench/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/fcbench/fcbench/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/fcbench/fcbench/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/benchmark/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/codecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/fcbench/fcbench/compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/compressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/compressor/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/fcbench/fcbench/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/dataset/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/fcbench/fcbench/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29660 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/fcbench/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/src/benchmark.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/src/compressor.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    21741 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/src/dataclass.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11940 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/src/dataset.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    26212 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/src/model.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-02 09:27:31.000000 field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-02 09:27:31.000000 field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:27:31.000000 field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-02 09:27:31.000000 field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 09:27:31.000000 field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/fork/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/fork/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/fork.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/fork/src/reaper/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/reaper/canary.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/reaper/handler.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/reaper/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/reaper/worker.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/work.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/rust-toolchain
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/rustfmt.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:27:31.738675 field-compression-benchmark-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/src/args.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/src/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/src/benchmarking/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/src/benchmarking/prepare.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    15158 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/src/benchmarking/report.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/src/fcpy.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    18774 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.702675 field-compression-benchmark-0.0.2/wasi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/build/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/build/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/build/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/build/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/build/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/cli/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/cli/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/cli/src/environment.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/cli/src/exit.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/cli/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/cli/src/stdio.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/cli/src/terminal.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/clocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/clocks/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/clocks/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/clocks/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/filesystem/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/filesystem/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/filesystem/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/io/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/io/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/io/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/io/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/io/src/poll.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/io/src/streams.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/random/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/random/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/random/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/wit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.702675 field-compression-benchmark-0.0.2/wasi/wit/deps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/command.wit
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/environment.wit
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/exit.wit
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/imports.wit
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/run.wit
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/stdio.wit
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/terminal.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/wit/deps/clocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/clocks/monotonic-clock.wit
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/clocks/wall-clock.wit
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/clocks/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/wit/deps/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/filesystem/preopens.wit
+-rw-r--r--   0 runner    (1001) docker     (127)    27621 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/filesystem/types.wit
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/filesystem/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/wit/deps/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/http/handler.wit
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/http/proxy.wit
+-rw-r--r--   0 runner    (1001) docker     (127)    24187 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/http/types.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/wasi/wit/deps/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/io/error.wit
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/io/poll.wit
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/io/streams.wit
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/io/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/wasi/wit/deps/random/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/random/insecure-seed.wit
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/random/insecure.wit
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/random/random.wit
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/random/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/instance-network.wit
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/ip-name-lookup.wit
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/network.wit
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/tcp-create-socket.wit
+-rw-r--r--   0 runner    (1001) docker     (127)    20199 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/tcp.wit
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/udp-create-socket.wit
+-rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/udp.wit
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/world.wit
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/world.wit
```

### Comparing `field-compression-benchmark-0.0.1/Cargo.lock` & `field-compression-benchmark-0.0.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anstream"
 version = "0.6.13"
@@ -104,17 +104,17 @@
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
@@ -135,51 +135,51 @@
 
 [[package]]
 name = "bindgen"
 version = "0.68.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "726e4313eb6ec35d2730258ad4e15b547ee75d6afaa1361a922e78e59b7d8078"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cexpr",
  "clang-sys",
  "lazy_static",
  "lazycell",
  "log",
  "peeking_take_while",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.52",
+ "syn 2.0.55",
  "which",
 ]
 
 [[package]]
 name = "bindgen"
 version = "0.69.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a00dc851838a2120612785d195287475a3ac45514741da670b735818822129a0"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cexpr",
  "clang-sys",
- "itertools 0.12.1",
+ "itertools",
  "lazy_static",
  "lazycell",
  "log",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.52",
+ "syn 2.0.55",
  "which",
 ]
 
 [[package]]
 name = "bit-round-codec"
 version = "0.1.0"
 dependencies = [
@@ -207,17 +207,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bitvec"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
 dependencies = [
@@ -245,33 +245,33 @@
  "bit-vec",
  "getrandom",
  "siphasher",
 ]
 
 [[package]]
 name = "borsh"
-version = "1.3.1"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f58b559fd6448c6e2fd0adb5720cd98a2506594cafa4737ff98c396f3e82f667"
+checksum = "0901fc8eb0aca4c83be0106d6f2db17d86a08dfc2c25f0e84464bf381158add6"
 dependencies = [
  "borsh-derive",
  "cfg_aliases",
 ]
 
 [[package]]
 name = "borsh-derive"
-version = "1.3.1"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7aadb5b6ccbd078890f6d7003694e33816e6b784358f18e15e7e6d9f065a57cd"
+checksum = "51670c3aa053938b0ee3bd67c3817e471e626151131b934038e83c5bf8de48f5"
 dependencies = [
  "once_cell",
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
  "syn_derive",
 ]
 
 [[package]]
 name = "bumpalo"
 version = "3.15.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -320,17 +320,17 @@
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
 version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
 dependencies = [
@@ -368,17 +368,17 @@
  "glob",
  "libc",
  "libloading",
 ]
 
 [[package]]
 name = "clap"
-version = "4.5.2"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b230ab84b0ffdf890d5a10abdbc8b83ae1c4918275daea1ab8801f71536b2651"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
 ]
 
 [[package]]
 name = "clap_builder"
@@ -390,22 +390,22 @@
  "anstyle",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.5.0"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "307bc0538d5f0f83b8248db3087aa92fe504e4691294d0c96c0eabc33f47ba47"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
- "heck 0.4.1",
+ "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
@@ -427,15 +427,15 @@
 
 [[package]]
 name = "codecs-build"
 version = "0.1.0"
 dependencies = [
  "flate2",
  "tar",
- "wit-component 0.201.0",
+ "wit-component 0.202.0",
 ]
 
 [[package]]
 name = "codecs-core"
 version = "0.1.0"
 dependencies = [
  "serde",
@@ -459,44 +459,44 @@
 name = "codecs-core-wasm"
 version = "0.1.0"
 dependencies = [
  "codecs-core",
  "format_serde_error",
  "serde",
  "serde_json",
- "wit-bindgen 0.22.0 (git+https://github.com/alexcrichton/witx-bindgen.git?branch=fix-rust-ctors)",
+ "wit-bindgen",
 ]
 
 [[package]]
 name = "codecs-frontend"
 version = "0.1.0"
 dependencies = [
  "anyhow",
  "codecs-core",
  "codecs-core-host",
  "convert_case",
  "core-error",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "numpy",
  "polonius-the-crab",
  "pyo3",
  "pyodide-webassembly-runtime-layer",
  "semver",
  "thiserror",
  "topological-sort",
  "vecmap-rs",
  "virtual-wasi-build",
  "wac-parser",
  "walrus",
  "wasm_component_layer",
  "wasm_runtime_layer",
- "wasmparser 0.201.0",
+ "wasmparser 0.202.0",
  "wasmtime",
- "wit-component 0.201.0",
- "wit-parser 0.201.0",
+ "wit-component 0.202.0",
+ "wit-parser 0.202.0",
 ]
 
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
@@ -534,43 +534,45 @@
 
 [[package]]
 name = "core-compressor"
 version = "0.1.0"
 dependencies = [
  "core-error",
  "core-measure",
+ "evalexpr",
  "nonempty",
  "numpy",
  "pyo3",
  "serde",
  "thiserror",
- "toml 0.8.11",
+ "toml 0.8.12",
  "vecmap-rs",
 ]
 
 [[package]]
 name = "core-dataset"
 version = "0.1.0"
 dependencies = [
  "byte-unit",
  "core-error",
  "nonempty",
  "pyo3",
  "serde",
  "sorted-vec",
  "thiserror",
- "toml 0.8.11",
+ "toml 0.8.12",
  "vecmap-rs",
 ]
 
 [[package]]
 name = "core-error"
 version = "0.1.0"
 dependencies = [
  "serde",
+ "serde-name",
 ]
 
 [[package]]
 name = "core-goodness"
 version = "0.1.0"
 dependencies = [
  "core-error",
@@ -586,14 +588,15 @@
 name = "core-measure"
 version = "0.1.0"
 dependencies = [
  "core-error",
  "human_bytes",
  "rand",
  "serde",
+ "serde-name",
  "thiserror",
 ]
 
 [[package]]
 name = "core-model"
 version = "0.1.0"
 dependencies = [
@@ -711,15 +714,15 @@
 version = "0.105.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4135b0ab01fd16aa8f8821196e9e2fe15953552ccaef8ba5153be0ced04ef757"
 dependencies = [
  "cranelift-codegen",
  "cranelift-entity",
  "cranelift-frontend",
- "itertools 0.10.5",
+ "itertools",
  "log",
  "smallvec",
  "wasmparser 0.121.2",
  "wasmtime-types",
 ]
 
 [[package]]
@@ -834,47 +837,59 @@
 checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "evalexpr"
+version = "11.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "63b41cb9dd076076058a4523f009c900c582279536d0b2e45a29aa930e083cc5"
+
+[[package]]
 name = "fallible-iterator"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4443176a9f2c162692bd3d352d745ef9413eec5782a80d8fd6f8a1ac692a07f7"
 
 [[package]]
 name = "fallible-iterator"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2acce4a10f12dc2fb14a218589d4f1f62ef011b2d0cc4b3cb1bba8e94da14649"
 
 [[package]]
 name = "fastrand"
-version = "2.0.1"
+version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
 
 [[package]]
 name = "fcbench"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "codecs-build",
  "codecs-frontend",
  "core-benchmark",
  "core-compressor",
  "core-dataset",
  "core-error",
  "core-model",
  "ndarray",
  "numpy",
  "pyo3",
  "pythonize",
+ "rand",
+ "rand_chacha",
+ "rand_distr",
  "serde",
+ "serde-reflection",
+ "serde_path_to_error",
+ "uuid",
  "vecmap-rs",
 ]
 
 [[package]]
 name = "field-compression-benchmark"
 version = "0.1.0"
 dependencies = [
@@ -942,14 +957,15 @@
 name = "fork"
 version = "0.1.0"
 dependencies = [
  "core-error",
  "ipc-channel",
  "libc",
  "log",
+ "rustix",
  "serde",
  "signal-hook",
  "thiserror",
 ]
 
 [[package]]
 name = "form_urlencoded"
@@ -1032,15 +1048,15 @@
 [[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 dependencies = [
  "fallible-iterator 0.3.0",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1088,14 +1104,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 dependencies = [
  "unicode-segmentation",
 ]
 
 [[package]]
+name = "heck"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
+
+[[package]]
 name = "hermit-abi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hexf"
@@ -1176,28 +1198,28 @@
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.2.5"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown 0.14.3",
  "serde",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "ipc-channel"
 version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ab3a34c91b7e84a72643bd75d1bac3afd241f78f9859fe0b5e5b2a6a75732c2"
 dependencies = [
@@ -1231,27 +1253,18 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
-name = "itertools"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
-dependencies = [
- "either",
-]
-
-[[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
 version = "0.1.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
 dependencies = [
@@ -1309,15 +1322,15 @@
 
 [[package]]
 name = "libredox"
 version = "0.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85c833ca1e66078851dba29046874e38f08b2c883700aa29a03ddd3b23814ee8"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "libc",
  "redox_syscall",
 ]
 
 [[package]]
 name = "linear-quantize-codec"
 version = "0.1.0"
@@ -1358,40 +1371,41 @@
  "codecs-core",
  "codecs-core-wasm",
  "serde",
 ]
 
 [[package]]
 name = "logos"
-version = "0.13.0"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c000ca4d908ff18ac99b93a062cb8958d331c3220719c52e77cb19cc6ac5d2c1"
+checksum = "161971eb88a0da7ae0c333e1063467c5b5727e7fb6b710b8db4814eade3a42e8"
 dependencies = [
  "logos-derive",
 ]
 
 [[package]]
 name = "logos-codegen"
-version = "0.13.0"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc487311295e0002e452025d6b580b77bb17286de87b57138f3b5db711cded68"
+checksum = "8e31badd9de5131fdf4921f6473d457e3dd85b11b7f091ceb50e4df7c3eeb12a"
 dependencies = [
  "beef",
  "fnv",
+ "lazy_static",
  "proc-macro2",
  "quote",
- "regex-syntax 0.6.29",
- "syn 2.0.52",
+ "regex-syntax",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "logos-derive"
-version = "0.13.0"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbfc0d229f1f42d790440136d941afd806bc9e949e2bcb8faa813b0f00d1267e"
+checksum = "1c2a69b3eb68d5bd595107c9ee58d7e07fe2bb5e360cc85b0f084dedac80de0a"
 dependencies = [
  "logos-codegen",
 ]
 
 [[package]]
 name = "mach"
 version = "0.3.2"
@@ -1409,56 +1423,58 @@
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memfd"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2cffa4ad52c6f791f4f8b15f0c05f9824b2ced1160e88cc393d64fff9a8ac64"
 dependencies = [
  "rustix",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miette"
 version = "7.2.0"
-source = "git+https://github.com/zkat/miette#ca646f3119790900c737ee8620d12ca8867c3bb4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4edc8853320c2a0dab800fbda86253c8938f6ea88510dc92c5f1ed20e794afc1"
 dependencies = [
  "cfg-if",
  "miette-derive",
  "serde",
  "thiserror",
  "unicode-width",
 ]
 
 [[package]]
 name = "miette-derive"
 version = "7.2.0"
-source = "git+https://github.com/zkat/miette#ca646f3119790900c737ee8620d12ca8867c3bb4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dcf09caffaac8068c346b6df2a7fc27a177fd20b39421a39ce0a211bde679a6c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
@@ -1569,15 +1585,15 @@
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "crc32fast",
  "hashbrown 0.14.3",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1670,20 +1686,20 @@
 dependencies = [
  "env_logger",
  "log",
 ]
 
 [[package]]
 name = "prettyplease"
-version = "0.2.16"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a41cf62165e97c7f814d2221421dbb9afcbcdb0a88068e5ea206e19951c2cbb5"
+checksum = "8d3928fb5db768cb86f891ff014f0144589297e3c6a1aba6ed7cecfdace270c7"
 dependencies = [
  "proc-macro2",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "proc-macro-crate"
 version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
@@ -1802,28 +1818,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "pyodide-webassembly-runtime-layer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38c50baf5fe8876a5dbd044875621dd47c3d5f0af182ae176dcbdd3e2006e275"
@@ -1835,15 +1851,15 @@
  "wasmparser 0.201.0",
  "wobbly",
 ]
 
 [[package]]
 name = "pythonize"
 version = "0.20.0"
-source = "git+https://github.com/juntyr/pythonize?rev=f1b3275#f1b3275b12837dc80463cbb09fe2daf51bcf0495"
+source = "git+https://github.com/juntyr/pythonize?rev=3a1fb05#3a1fb055bbad61ce04da8d66dff17194dbe364b6"
 dependencies = [
  "pyo3",
  "serde",
 ]
 
 [[package]]
 name = "quote"
@@ -1865,14 +1881,15 @@
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
 dependencies = [
  "libc",
  "rand_chacha",
  "rand_core",
+ "serde",
 ]
 
 [[package]]
 name = "rand_chacha"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
@@ -1884,24 +1901,26 @@
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
+ "serde",
 ]
 
 [[package]]
 name = "rand_distr"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "32cb0b9bc82b0a0876c2dd994a7e7a2683d3e7390ca40e6886785ef0c7e3ee31"
 dependencies = [
  "num-traits",
  "rand",
+ "serde",
 ]
 
 [[package]]
 name = "rand_pcg"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "59cad018caf63deb318e5a4586d99a24424a364f40f1e5778c29aca23f4fc73e"
@@ -1948,15 +1967,15 @@
 name = "ref-cast-impl"
 version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5fddb4f8d99b0a2ebafc65a87a69a7b9875e4b1ae1f00db265d300ef7f28bccc"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "regalloc2"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad156d539c879b7a24a363a2016d77961786e71f48f2e2fc8302a92abd2429a6"
@@ -1966,46 +1985,40 @@
  "rustc-hash",
  "slice-group-by",
  "smallvec",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
- "regex-syntax 0.8.2",
+ "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax 0.8.2",
+ "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
-
-[[package]]
-name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reinterpret-codec"
 version = "0.1.0"
 dependencies = [
  "codecs-core",
  "codecs-core-wasm",
@@ -2048,17 +2061,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "rust_decimal"
-version = "1.34.3"
+version = "1.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b39449a79f45e8da28c57c341891b69a183044b29518bb8f86dbac9df60bb7df"
+checksum = "1790d1c4c0ca81211399e0e0af16333276f375209e71a37b67698a373db5b47a"
 dependencies = [
  "arrayvec",
  "borsh",
  "bytes",
  "num-traits",
  "rand",
  "rkyv",
@@ -2070,19 +2083,19 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
@@ -2118,44 +2131,74 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
+name = "serde-name"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b5b14ebbcc4e4f2b3642fa99c388649da58d1dc3308c7d109f39f565d1710f0"
+dependencies = [
+ "serde",
+ "thiserror",
+]
+
+[[package]]
+name = "serde-reflection"
+version = "0.3.6"
+source = "git+https://github.com/juntyr/serde-reflection.git?rev=4490f20#4490f20958a7c2880a8018dafcb5f6f52b5cd115"
+dependencies = [
+ "once_cell",
+ "serde",
+ "thiserror",
+]
+
+[[package]]
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_path_to_error"
+version = "0.1.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af99884400da37c88f5e9146b7f1fd0fbcae8f6eec4e9da38b67d05486f814a6"
+dependencies = [
+ "itoa",
+ "serde",
+]
+
+[[package]]
 name = "serde_repr"
 version = "0.1.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b2e6b945e9d3df726b65d6ee24060aff8e3533d431f677a9695db04eff9dfdb"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "serde_spanned"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eb3622f419d1296904700073ea6cc23ad690adbd66f13ea683df73298736f0c1"
@@ -2203,17 +2246,17 @@
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "siphasher"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54ac45299ccbd390721be55b412d41931911f654fa99e2cb8bfb57184b2061fe"
+checksum = "56199f7ddabf13fe5074ce809e7d3f42b42ae711800501b5b16ea82ad029c39d"
 
 [[package]]
 name = "slab"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
@@ -2224,17 +2267,17 @@
 name = "slice-group-by"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "826167069c09b99d56f31e9ae5c99049e932a98c9dc2dac47645b08dbbf76ba7"
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "sorted-vec"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6734caf0b6f51addd5eeacca12fb39b2c6c14e8d4f3ac42f3a78955c0467458"
 
@@ -2274,17 +2317,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.55"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2292,15 +2335,15 @@
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1329189c02ff984e9736652b1631330da25eaa6bc639089ed4915d25446cbe7b"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "sz3"
 version = "0.1.0+3.1.5.3"
 source = "git+https://github.com/juntyr/sz3-rs.git?rev=475d6e0#475d6e0d1b0a0c94b7647bc96eeff4ac79bc16a8"
 dependencies = [
@@ -2313,14 +2356,15 @@
 version = "0.1.0"
 dependencies = [
  "codecs-core",
  "codecs-core-wasm",
  "postcard",
  "serde",
  "sz3",
+ "zstd-sys",
 ]
 
 [[package]]
 name = "sz3-sys"
 version = "0.1.0+SZ3-3.1.5.3"
 source = "git+https://github.com/juntyr/sz3-rs.git?rev=475d6e0#475d6e0d1b0a0c94b7647bc96eeff4ac79bc16a8"
 dependencies = [
@@ -2385,15 +2429,15 @@
 name = "thiserror-impl"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -2414,23 +2458,23 @@
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml"
-version = "0.8.11"
+version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af06656561d28735e9c1cd63dfd57132c8155426aa6af24f36a00a351f88c48e"
+checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
 dependencies = [
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "serde",
  "serde_spanned",
  "toml_datetime",
- "toml_edit 0.22.7",
+ "toml_edit 0.22.9",
 ]
 
 [[package]]
 name = "toml_datetime"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
@@ -2440,26 +2484,26 @@
 
 [[package]]
 name = "toml_edit"
 version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a8534fd7f78b5405e860340ad6575217ce99f38d4d5c8f2442cb5ecb50090e1"
 dependencies = [
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "toml_datetime",
  "winnow 0.5.40",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.22.7"
+version = "0.22.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "18769cd1cec395d70860ceb4d932812a0b4d06b1a4bb336745a4d21b9496e992"
+checksum = "8e40bb779c5187258fd7aad0eb68cb8706a0a81fa712fbea808ab43c4b8374c4"
 dependencies = [
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow 0.6.5",
 ]
 
 [[package]]
@@ -2521,14 +2565,25 @@
 [[package]]
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
 [[package]]
+name = "uniform-noise-codec"
+version = "0.1.0"
+dependencies = [
+ "codecs-core",
+ "codecs-core-wasm",
+ "rand",
+ "rand_chacha",
+ "serde",
+]
+
+[[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "url"
@@ -2551,17 +2606,17 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "getrandom",
  "serde",
 ]
 
 [[package]]
 name = "vecmap-rs"
@@ -2578,97 +2633,97 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "virtual-wasi-build"
 version = "0.1.0"
 dependencies = [
- "wit-component 0.201.0",
+ "wit-component 0.202.0",
 ]
 
 [[package]]
 name = "virtual-wasi-cli"
 version = "0.1.0"
 dependencies = [
- "wit-bindgen 0.22.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "wit-bindgen",
 ]
 
 [[package]]
 name = "virtual-wasi-clocks"
 version = "0.1.0"
 dependencies = [
- "wit-bindgen 0.22.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "wit-bindgen",
 ]
 
 [[package]]
 name = "virtual-wasi-filesystem"
 version = "0.1.0"
 dependencies = [
- "wit-bindgen 0.22.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "wit-bindgen",
 ]
 
 [[package]]
 name = "virtual-wasi-io"
 version = "0.1.0"
 dependencies = [
- "wit-bindgen 0.22.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "wit-bindgen",
 ]
 
 [[package]]
 name = "virtual-wasi-random"
 version = "0.1.0"
 dependencies = [
  "rand_core",
  "rand_pcg",
- "wit-bindgen 0.22.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "wit-bindgen",
 ]
 
 [[package]]
 name = "wac-parser"
 version = "0.1.0"
-source = "git+https://github.com/peterhuene/wac.git?rev=0b44c06#0b44c0654e0d7d1c4f90e1569f6203376b00f73a"
+source = "git+https://github.com/peterhuene/wac.git?rev=7b2f728#7b2f7283d3b3044419eafbc5c82d9877d8b0dc60"
 dependencies = [
  "anyhow",
  "id-arena",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "log",
  "logos",
  "miette",
  "semver",
  "serde",
  "thiserror",
- "wasm-encoder 0.38.1",
- "wasm-metadata 0.10.20",
- "wasmparser 0.118.2",
+ "wasm-encoder 0.201.0",
+ "wasm-metadata 0.201.0",
+ "wasmparser 0.201.0",
 ]
 
 [[package]]
 name = "walrus"
 version = "0.20.3"
-source = "git+https://github.com/rustwasm/walrus.git?branch=update#4efdb5c8951a83deb64d02a8822f9442948a6401"
+source = "git+https://github.com/rustwasm/walrus.git?rev=4efdb5c#4efdb5c8951a83deb64d02a8822f9442948a6401"
 dependencies = [
  "anyhow",
  "gimli 0.26.2",
  "id-arena",
  "leb128",
  "log",
  "walrus-macro",
  "wasm-encoder 0.41.2",
  "wasmparser 0.100.0",
 ]
 
 [[package]]
 name = "walrus-macro"
 version = "0.19.0"
-source = "git+https://github.com/rustwasm/walrus.git?branch=update#4efdb5c8951a83deb64d02a8822f9442948a6401"
+source = "git+https://github.com/rustwasm/walrus.git?rev=4efdb5c#4efdb5c8951a83deb64d02a8822f9442948a6401"
 dependencies = [
  "heck 0.3.3",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
@@ -2690,15 +2745,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2712,36 +2767,27 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "wasm-encoder"
-version = "0.38.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ad2b51884de9c7f4fe2fd1043fccb8dcad4b1e29558146ee57a144d15779f3f"
-dependencies = [
- "leb128",
-]
-
-[[package]]
-name = "wasm-encoder"
 version = "0.41.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "972f97a5d8318f908dded23594188a90bcd09365986b1163e66d70170e5287ae"
 dependencies = [
  "leb128",
 ]
 
@@ -2760,37 +2806,30 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9c7d2731df60006819b013f64ccc2019691deccf6e11a1804bc850cd6748f1a"
 dependencies = [
  "leb128",
 ]
 
 [[package]]
-name = "wasm-metadata"
-version = "0.10.20"
+name = "wasm-encoder"
+version = "0.202.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "18ebaa7bd0f9e7a5e5dd29b9a998acf21c4abed74265524dd7e85934597bfb10"
+checksum = "bfd106365a7f5f7aa3c1916a98cbb3ad477f5ff96ddb130285a91c6e7429e67a"
 dependencies = [
- "anyhow",
- "indexmap 2.2.5",
- "serde",
- "serde_derive",
- "serde_json",
- "spdx",
- "wasm-encoder 0.41.2",
- "wasmparser 0.121.2",
+ "leb128",
 ]
 
 [[package]]
 name = "wasm-metadata"
 version = "0.200.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c31b8cc0c21f46d55b0aaa419cacce1eadcf28eaebd0e1488d6a6313ee71a586"
 dependencies = [
  "anyhow",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "serde",
  "serde_derive",
  "serde_json",
  "spdx",
  "wasm-encoder 0.200.0",
  "wasmparser 0.200.0",
 ]
@@ -2798,27 +2837,43 @@
 [[package]]
 name = "wasm-metadata"
 version = "0.201.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fd83062c17b9f4985d438603cde0a5e8c5c8198201a6937f778b607924c7da2"
 dependencies = [
  "anyhow",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "serde",
  "serde_derive",
  "serde_json",
  "spdx",
  "wasm-encoder 0.201.0",
  "wasmparser 0.201.0",
 ]
 
 [[package]]
+name = "wasm-metadata"
+version = "0.202.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "094aea3cb90e09f16ee25a4c0e324b3e8c934e7fd838bfa039aef5352f44a917"
+dependencies = [
+ "anyhow",
+ "indexmap 2.2.6",
+ "serde",
+ "serde_derive",
+ "serde_json",
+ "spdx",
+ "wasm-encoder 0.202.0",
+ "wasmparser 0.202.0",
+]
+
+[[package]]
 name = "wasm_component_layer"
 version = "0.1.16"
-source = "git+https://github.com/juntyr/wasm_component_layer.git?branch=resource-transfer#0d6d5e5d5a261a88756f36fb0d1da3377a6b17a3"
+source = "git+https://github.com/juntyr/wasm_component_layer.git?rev=0d6d5e5#0d6d5e5d5a261a88756f36fb0d1da3377a6b17a3"
 dependencies = [
  "anyhow",
  "bytemuck",
  "fxhash",
  "id-arena",
  "ref-cast",
  "semver",
@@ -2850,52 +2905,53 @@
 dependencies = [
  "indexmap 1.9.3",
  "url",
 ]
 
 [[package]]
 name = "wasmparser"
-version = "0.118.2"
+version = "0.121.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77f1154f1ab868e2a01d9834a805faca7bf8b50d041b4ca714d005d0dab1c50c"
+checksum = "9dbe55c8f9d0dbd25d9447a5a889ff90c0cc3feaa7395310d3d826b2c703eaab"
 dependencies = [
- "indexmap 2.2.5",
+ "bitflags 2.5.0",
+ "indexmap 2.2.6",
  "semver",
 ]
 
 [[package]]
 name = "wasmparser"
-version = "0.121.2"
+version = "0.200.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9dbe55c8f9d0dbd25d9447a5a889ff90c0cc3feaa7395310d3d826b2c703eaab"
+checksum = "a03f65ac876612140c57ff6c3b8fe4990067cce97c2cfdb07368a3cc3354b062"
 dependencies = [
- "bitflags 2.4.2",
- "indexmap 2.2.5",
+ "bitflags 2.5.0",
+ "indexmap 2.2.6",
  "semver",
 ]
 
 [[package]]
 name = "wasmparser"
-version = "0.200.0"
+version = "0.201.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a03f65ac876612140c57ff6c3b8fe4990067cce97c2cfdb07368a3cc3354b062"
+checksum = "84e5df6dba6c0d7fafc63a450f1738451ed7a0b52295d83e868218fa286bf708"
 dependencies = [
- "bitflags 2.4.2",
- "indexmap 2.2.5",
+ "bitflags 2.5.0",
+ "indexmap 2.2.6",
  "semver",
 ]
 
 [[package]]
 name = "wasmparser"
-version = "0.201.0"
+version = "0.202.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84e5df6dba6c0d7fafc63a450f1738451ed7a0b52295d83e868218fa286bf708"
+checksum = "d6998515d3cf3f8b980ef7c11b29a9b1017d4cf86b99ae93b546992df9931413"
 dependencies = [
- "bitflags 2.4.2",
- "indexmap 2.2.5",
+ "bitflags 2.5.0",
+ "indexmap 2.2.6",
  "semver",
 ]
 
 [[package]]
 name = "wasmprinter"
 version = "0.2.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2913,15 +2969,15 @@
 dependencies = [
  "anyhow",
  "bincode",
  "bumpalo",
  "cfg-if",
  "encoding_rs",
  "gimli 0.28.1",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "libc",
  "log",
  "object",
  "once_cell",
  "paste",
  "rustix",
  "serde",
@@ -2974,15 +3030,15 @@
 version = "18.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d3786c0531565ec6c9852c0e46299f06cb6e4b58d36e30f3c234cfa69bde376"
 dependencies = [
  "anyhow",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
  "wasmtime-component-util",
  "wasmtime-wit-bindgen",
  "wit-parser 0.13.2",
 ]
 
 [[package]]
 name = "wasmtime-component-util"
@@ -3037,15 +3093,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3279d510005358141550d8a90a5fc989d7e81748e5759d582fe6bfdcbf074a04"
 dependencies = [
  "anyhow",
  "bincode",
  "cranelift-entity",
  "gimli 0.28.1",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "log",
  "object",
  "serde",
  "serde_derive",
  "target-lexicon",
  "thiserror",
  "wasm-encoder 0.41.2",
@@ -3072,15 +3128,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e11185c88cadf595d228f5ae4ff9b4badbf9ca98dcb37b0310c36e31fa74867f"
 dependencies = [
  "anyhow",
  "cc",
  "cfg-if",
  "encoding_rs",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "libc",
  "log",
  "mach",
  "memfd",
  "memoffset",
  "paste",
  "psm",
@@ -3111,15 +3167,15 @@
 name = "wasmtime-versioned-export-macros"
 version = "18.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ab8d7566d206c42f8cf1d4ac90c5e40d3582e8eabad9b3b67e9e73c61fc47a1"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "wasmtime-winch"
 version = "18.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba5a97bfccc241d1769cef75eb16f472a893982704d5f3c9c71c431c1484344a"
@@ -3139,15 +3195,15 @@
 name = "wasmtime-wit-bindgen"
 version = "18.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "faf2c76781a27e07802669f6f0e11eb4441546407eb65be60c3d862200988b92"
 dependencies = [
  "anyhow",
  "heck 0.4.1",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "wit-parser 0.13.2",
 ]
 
 [[package]]
 name = "wasmtime-wmemcheck"
 version = "18.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3369,164 +3425,116 @@
 checksum = "dffa400e67ed5a4dd237983829e66475f0a4a26938c4b04c21baede6262215b8"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "wit-bindgen"
-version = "0.22.0"
+version = "0.23.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "288f992ea30e6b5c531b52cdd5f3be81c148554b09ea416f058d16556ba92c27"
-dependencies = [
- "bitflags 2.4.2",
- "wit-bindgen-rt 0.22.0 (registry+https://github.com/rust-lang/crates.io-index)",
- "wit-bindgen-rust-macro 0.22.0 (registry+https://github.com/rust-lang/crates.io-index)",
-]
-
-[[package]]
-name = "wit-bindgen"
-version = "0.22.0"
-source = "git+https://github.com/alexcrichton/witx-bindgen.git?branch=fix-rust-ctors#b484e6f3342add6715209f10fff1788c502d5023"
+checksum = "041a3276f25dce240b10f5b34d9d490b007f18e8ead05984ae7948b283b4059e"
 dependencies = [
- "bitflags 2.4.2",
- "wit-bindgen-rt 0.22.0 (git+https://github.com/alexcrichton/witx-bindgen.git?branch=fix-rust-ctors)",
- "wit-bindgen-rust-macro 0.22.0 (git+https://github.com/alexcrichton/witx-bindgen.git?branch=fix-rust-ctors)",
+ "wit-bindgen-rt",
+ "wit-bindgen-rust-macro",
 ]
 
 [[package]]
 name = "wit-bindgen-core"
-version = "0.22.0"
+version = "0.23.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e85e72719ffbccf279359ad071497e47eb0675fe22106dea4ed2d8a7fcb60ba4"
-dependencies = [
- "anyhow",
- "wit-parser 0.201.0",
-]
-
-[[package]]
-name = "wit-bindgen-core"
-version = "0.22.0"
-source = "git+https://github.com/alexcrichton/witx-bindgen.git?branch=fix-rust-ctors#b484e6f3342add6715209f10fff1788c502d5023"
+checksum = "b0834150cd852e64e1eddcff4fea9524b788161b4111d83a94c9eda715f8f442"
 dependencies = [
  "anyhow",
- "wit-parser 0.201.0",
+ "wit-parser 0.202.0",
 ]
 
 [[package]]
 name = "wit-bindgen-rt"
-version = "0.22.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcb8738270f32a2d6739973cbbb7c1b6dd8959ce515578a6e19165853272ee64"
-
-[[package]]
-name = "wit-bindgen-rt"
-version = "0.22.0"
-source = "git+https://github.com/alexcrichton/witx-bindgen.git?branch=fix-rust-ctors#b484e6f3342add6715209f10fff1788c502d5023"
-
-[[package]]
-name = "wit-bindgen-rust"
-version = "0.22.0"
+version = "0.23.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8a39a15d1ae2077688213611209849cad40e9e5cccf6e61951a425850677ff3"
+checksum = "d6ccd4c6a69667c75474ddb30c36773c5e70cdca099ec2e293005458886ac81b"
 dependencies = [
- "anyhow",
- "heck 0.4.1",
- "indexmap 2.2.5",
- "wasm-metadata 0.201.0",
- "wit-bindgen-core 0.22.0 (registry+https://github.com/rust-lang/crates.io-index)",
- "wit-component 0.201.0",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "wit-bindgen-rust"
-version = "0.22.0"
-source = "git+https://github.com/alexcrichton/witx-bindgen.git?branch=fix-rust-ctors#b484e6f3342add6715209f10fff1788c502d5023"
+version = "0.23.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "60620df421d4c787e2660f0159fd58f2ae6998dc42ccf2e09b8d9d96d16885a9"
 dependencies = [
  "anyhow",
  "heck 0.4.1",
- "indexmap 2.2.5",
- "wasm-metadata 0.201.0",
- "wit-bindgen-core 0.22.0 (git+https://github.com/alexcrichton/witx-bindgen.git?branch=fix-rust-ctors)",
- "wit-component 0.201.0",
+ "indexmap 2.2.6",
+ "wasm-metadata 0.202.0",
+ "wit-bindgen-core",
+ "wit-component 0.202.0",
 ]
 
 [[package]]
 name = "wit-bindgen-rust-macro"
-version = "0.22.0"
+version = "0.23.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d376d3ae5850526dfd00d937faea0d81a06fa18f7ac1e26f386d760f241a8f4b"
-dependencies = [
- "anyhow",
- "proc-macro2",
- "quote",
- "syn 2.0.52",
- "wit-bindgen-core 0.22.0 (registry+https://github.com/rust-lang/crates.io-index)",
- "wit-bindgen-rust 0.22.0 (registry+https://github.com/rust-lang/crates.io-index)",
-]
-
-[[package]]
-name = "wit-bindgen-rust-macro"
-version = "0.22.0"
-source = "git+https://github.com/alexcrichton/witx-bindgen.git?branch=fix-rust-ctors#b484e6f3342add6715209f10fff1788c502d5023"
+checksum = "96e875e7dd09a0d2acc1a27df6a4b0586288741d940b40a717e2daed3bc3d979"
 dependencies = [
  "anyhow",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
- "wit-bindgen-core 0.22.0 (git+https://github.com/alexcrichton/witx-bindgen.git?branch=fix-rust-ctors)",
- "wit-bindgen-rust 0.22.0 (git+https://github.com/alexcrichton/witx-bindgen.git?branch=fix-rust-ctors)",
+ "syn 2.0.55",
+ "wit-bindgen-core",
+ "wit-bindgen-rust",
 ]
 
 [[package]]
 name = "wit-component"
 version = "0.200.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "39979723340baea490b87b11b2abae05f149d86f2b55c18d41d78a2a2b284c16"
 dependencies = [
  "anyhow",
- "bitflags 2.4.2",
- "indexmap 2.2.5",
+ "bitflags 2.5.0",
+ "indexmap 2.2.6",
  "log",
  "serde",
  "serde_derive",
  "serde_json",
  "wasm-encoder 0.200.0",
  "wasm-metadata 0.200.0",
  "wasmparser 0.200.0",
  "wit-parser 0.200.0",
 ]
 
 [[package]]
 name = "wit-component"
-version = "0.201.0"
+version = "0.202.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "421c0c848a0660a8c22e2fd217929a0191f14476b68962afd2af89fd22e39825"
+checksum = "0c836b1fd9932de0431c1758d8be08212071b6bba0151f7bac826dbc4312a2a9"
 dependencies = [
  "anyhow",
- "bitflags 2.4.2",
- "indexmap 2.2.5",
+ "bitflags 2.5.0",
+ "indexmap 2.2.6",
  "log",
  "serde",
  "serde_derive",
  "serde_json",
- "wasm-encoder 0.201.0",
- "wasm-metadata 0.201.0",
- "wasmparser 0.201.0",
- "wit-parser 0.201.0",
+ "wasm-encoder 0.202.0",
+ "wasm-metadata 0.202.0",
+ "wasmparser 0.202.0",
+ "wit-parser 0.202.0",
 ]
 
 [[package]]
 name = "wit-parser"
 version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "316b36a9f0005f5aa4b03c39bc3728d045df136f8c13a73b7db4510dec725e08"
 dependencies = [
  "anyhow",
  "id-arena",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "log",
  "semver",
  "serde",
  "serde_derive",
  "serde_json",
  "unicode-xid",
 ]
@@ -3535,40 +3543,40 @@
 name = "wit-parser"
 version = "0.200.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f717576b37f01c15696bda7f6f13868367b9c5913485f9f0ec8e59fd28c8e13"
 dependencies = [
  "anyhow",
  "id-arena",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "log",
  "semver",
  "serde",
  "serde_derive",
  "serde_json",
  "unicode-xid",
  "wasmparser 0.200.0",
 ]
 
 [[package]]
 name = "wit-parser"
-version = "0.201.0"
+version = "0.202.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "196d3ecfc4b759a8573bf86a9b3f8996b304b3732e4c7de81655f875f6efdca6"
+checksum = "744237b488352f4f27bca05a10acb79474415951c450e52ebd0da784c1df2bcc"
 dependencies = [
  "anyhow",
  "id-arena",
- "indexmap 2.2.5",
+ "indexmap 2.2.6",
  "log",
  "semver",
  "serde",
  "serde_derive",
  "serde_json",
  "unicode-xid",
- "wasmparser 0.201.0",
+ "wasmparser 0.202.0",
 ]
 
 [[package]]
 name = "wobbly"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "10c47ee6b4260f6a7cee6cd6b7a34edf5b3e16ce2f309b5168d6fdb6c0dbbdd6"
@@ -3595,15 +3603,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.55",
 ]
 
 [[package]]
 name = "zfp-codec"
 version = "0.1.0"
 dependencies = [
  "codecs-core",
```

### Comparing `field-compression-benchmark-0.0.1/Cargo.toml` & `field-compression-benchmark-0.0.2/fcbench/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,41 @@
-[workspace]
-members = [
-    ".", "fork",
-    "wasi/build", "wasi/cli", "wasi/clocks", "wasi/filesystem", "wasi/io",
-    "wasi/random",
-    "core/benchmark", "core/compressor", "core/dataset", "core/error",
-    "core/goodness", "core/measure", "core/model",
-    "codecs/build", "codecs/core", "codecs/core-host", "codecs/core-wasm",
-    "codecs/frontend",
-    "codecs/bit-round", "codecs/bit-transpose", "codecs/identity",
-    "codecs/linear-quantize", "codecs/log", "codecs/reinterpret",
-    "codecs/sz3", "codecs/zfp", "codecs/zlib", "codecs/zstd",
-    "fcbench",
-]
-
 [package]
-name = "field-compression-benchmark"
-version = "0.1.0"
+name = "fcbench"
+version = "0.0.2"
 edition = "2021"
-authors = ["Juniper Tyree <juniper.tyree@helsinki.fi>"]
-homepage = "https://github.com/juntyr/field-compression-benchmarkt"
-repository = "https://github.com/juntyr/field-compression-benchmark"
-readme = "README.md"
-license = "MIT OR Apache-2.0"
-rust-version = "1.76"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
+[lib]
+name = "fcbench"
+crate-type = ["cdylib"]
 
 [dependencies]
-byte-unit = { version = "5.1", default-features = false, features = ["std"] }
-clap = { version = "4.3", default-features = false, features = ["derive", "std", "color", "help", "usage", "error-context", "suggestions", "string"] }
-codecs-build = { path = "codecs/build", default-features = false }
-codecs-frontend = { path = "codecs/frontend", default-features = false, features = ["wasmtime"] }
-core-benchmark = { path = "core/benchmark", default-features = false }
-core-compressor = { path = "core/compressor", default-features = false }
-core-dataset = { path = "core/dataset", default-features = false }
-core-error = { path = "core/error", default-features = false }
-fork = { version = "0.1", path = "fork" }
-gag = { version = "1.0", default-features = false }
-getrandom = { version = "0.2", default-features = false, features = ["std"] }
-log = { version = "0.4", default-features = false }
-nonempty = { version = "0.10", default-features = false, features = ["serialize"] }
-pretty_env_logger = { version = "0.5", default-features = false }
-pyo3 = { version = "0.20", default-features = false, features = ["abi3"] }
-serde = { version = "1.0", default-features = false, features = ["derive"] }
-serde_json = { version = "1.0", default-features = false, features = ["std"] }
-thiserror = { version = "1.0", default-features = false }
-vecmap-rs = { version = "0.2", default-features = false, features = ["serde"] }
+codecs-build = { path = "../codecs/build", default-features = false }
+core-benchmark = { path = "../core/benchmark", default-features = false }
+core-compressor = { path = "../core/compressor", default-features = false }
+core-dataset = { path = "../core/dataset", default-features = false }
+core-error = { path = "../core/error", default-features = false }
+core-model = { path = "../core/model", default-features = false }
+ndarray = { version = "0.15", default-features = false, features = ["std"] }
+numpy = { version = "0.20", default-features = false }
+pyo3 = { version = "0.20", default-features = false, features = ["macros", "abi3", "extension-module"] }
+pythonize = { git = "https://github.com/juntyr/pythonize", rev = "3a1fb05", version = "0.20", default-features = false }
+rand = { version = "0.8", default-features = false }
+rand_chacha = { version = "0.3", default-features = false }
+rand_distr = { version = "0.4", default-features = false, features = ["serde1"] }
+serde = { version = "1.0", default-features = false, features = ["std"] }
+serde_path_to_error = { version = "0.1", default-features = false }
+serde-reflection = { git = "https://github.com/juntyr/serde-reflection.git", rev = "4490f20", version = "0.3", default-features = false }
+uuid = { version = "1.5", default-features = false, features = ["std", "v8", "serde"] }
+vecmap-rs = { version = "0.2", default-features = false }
+
+[target.'cfg(target_arch = "wasm32")'.dependencies]
+codecs-frontend = { path = "../codecs/frontend", default-features = false, features = ["pyodide"] }
+
+[target.'cfg(not(target_arch = "wasm32"))'.dependencies]
+codecs-frontend = { path = "../codecs/frontend", default-features = false, features = ["wasmtime"] }
+
+[lints]
+workspace = true
 
 [package.metadata.cargo-udeps.ignore]
 normal = ["codecs-build"]
```

### Comparing `field-compression-benchmark-0.0.1/LICENSE-APACHE` & `field-compression-benchmark-0.0.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/LICENSE-MIT` & `field-compression-benchmark-0.0.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/PKG-INFO` & `field-compression-benchmark-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: field-compression-benchmark
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data compression methods and benchmarks for Cli/Met datasets
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 Maintainer-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `field-compression-benchmark-0.0.1/README.md` & `field-compression-benchmark-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/codecs/bit-round/src/lib.rs` & `field-compression-benchmark-0.0.2/codecs/bit-round/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,8 @@
-#![deny(clippy::pedantic)]
-#![cfg_attr(not(test), deny(clippy::unwrap_used))]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
+#![cfg_attr(test, allow(clippy::unwrap_used))]
 #![allow(clippy::missing_errors_doc)]
 #![cfg_attr(not(test), no_main)]
 
 pub fn bit_round<T: Float>(data: &[T], keepbits: u8) -> Result<Vec<T>, String> {
     if u32::from(keepbits) > T::MANITSSA_BITS {
         return Err(format!(
             "{keepbits} bits exceed the mantissa size for {}",
```

### Comparing `field-compression-benchmark-0.0.1/codecs/bit-transpose/src/lib.rs` & `field-compression-benchmark-0.0.2/codecs/bit-transpose/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
 #![cfg_attr(not(test), no_main)]
 
 #[must_use]
 pub fn bit_transpose<T: Float>(data: &[T]) -> Vec<T::Unsigned> {
     // Adapted from Milan Klöwer's BitInformation.jl's bittranspose
     //  (MIT licensed)
     // https://github.com/milankl/BitInformation.jl/blob/9a599e343bc127f73b6b1f77ac497a829d0a4a5f/src/bittranspose.jl#L3-L54
```

### Comparing `field-compression-benchmark-0.0.1/codecs/build/build.rs` & `field-compression-benchmark-0.0.2/codecs/build/build.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,26 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
-
 use std::{
     ffi::OsString,
     fs, io,
     path::{Path, PathBuf},
     process::Command,
 };
 
 const WASI_VERSION: u32 = 20;
 const WASMTIME_VERSION_FULL: &str = "18.0.0";
 
 fn main() -> io::Result<()> {
     // Check for `clippy` and return early in this case
     //  since `clippy` pollutes the `RUSTFLAGS` between rebuilds
-    if match std::env::var_os("RUSTC_WRAPPER")
+    if std::env::var_os("RUSTC_WRAPPER")
         .or_else(|| std::env::var_os("RUSTC_WORKSPACE_WRAPPER"))
+        .map_or(false, |wrapper| {
+            Path::new(&wrapper).ends_with("clippy-driver")
+        })
     {
-        Some(wrapper) => Path::new(&wrapper).ends_with("clippy-driver"),
-        None => false,
-    } {
         return Ok(());
     }
 
     std::env::remove_var("CARGO_ENCODED_RUSTFLAGS");
 
     let out_dir = PathBuf::from(std::env::var_os("OUT_DIR").ok_or_else(|| {
         io::Error::new(io::ErrorKind::NotFound, "missing env variable `OUT_DIR`")
@@ -52,14 +42,15 @@
         ("bit-round-codec", "bit-round"),
         ("bit-transpose-codec", "bit-transpose"),
         ("identity-codec", "identity"),
         ("linear-quantize-codec", "linear-quantize"),
         ("log-codec", "log"),
         ("reinterpret-codec", "reinterpret"),
         ("sz3-codec", "sz3"),
+        ("uniform-noise-codec", "uniform-noise"),
         ("zfp-codec", "zfp"),
         ("zlib-codec", "zlib"),
         ("zstd-codec", "zstd"),
     ] {
         let wasm = build_wasm_codec(&wasi_sdk_path, &target_dir, crate_name)?;
         add_change_dependencies(&wasm)?;
         let wasm = adapt_wasi_snapshot_to_preview2(&wasm, &adapter_path)?;
@@ -211,15 +202,15 @@
         return Err(io::Error::new(
             io::ErrorKind::InvalidData,
             "invalid deps file format",
         ));
     };
 
     for dep in deps.split_whitespace() {
-        println!("cargo:rerun-if-changed={dep}");
+        println!("cargo::rerun-if-changed={dep}");
     }
 
     Ok(())
 }
 
 fn adapt_wasi_snapshot_to_preview2(wasm: &Path, adapter: &Path) -> io::Result<PathBuf> {
     let wasm_preview2 = wasm.with_extension("preview2.wasm");
```

### Comparing `field-compression-benchmark-0.0.1/codecs/core/src/buffer.rs` & `field-compression-benchmark-0.0.2/codecs/core/src/buffer.rs`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     I64(B::Buffer<i64>),
     F32(B::Buffer<f32>),
     F64(B::Buffer<f64>),
 }
 
 impl<B: OwnedBuffer> BufferVec<B> {
     #[must_use]
+    #[allow(clippy::trait_duplication_in_bounds)]
     pub fn map<F: HigherOrderMap, R>(self, map: F) -> R
     where
         F: HigherOrderMap<Args<u8> = B::Buffer<u8>, Output<u8> = R>
             + HigherOrderMap<Args<u16> = B::Buffer<u16>, Output<u16> = R>
             + HigherOrderMap<Args<u32> = B::Buffer<u32>, Output<u32> = R>
             + HigherOrderMap<Args<u64> = B::Buffer<u64>, Output<u64> = R>
             + HigherOrderMap<Args<i8> = B::Buffer<i8>, Output<i8> = R>
@@ -48,14 +49,15 @@
             Self::I64(b) => map.map::<i64>(b),
             Self::F32(b) => map.map::<f32>(b),
             Self::F64(b) => map.map::<f64>(b),
         }
     }
 
     #[must_use]
+    #[allow(clippy::trait_duplication_in_bounds)]
     pub fn map_ref<'a, F: HigherOrderMap, R>(&'a self, map: F) -> R
     where
         F: HigherOrderMap<Args<u8> = &'a [u8], Output<u8> = R>
             + HigherOrderMap<Args<u16> = &'a [u16], Output<u16> = R>
             + HigherOrderMap<Args<u32> = &'a [u32], Output<u32> = R>
             + HigherOrderMap<Args<u64> = &'a [u64], Output<u64> = R>
             + HigherOrderMap<Args<i8> = &'a [i8], Output<i8> = R>
@@ -81,24 +83,14 @@
 
     #[must_use]
     pub fn as_slice(&self) -> BufferSlice {
         self.map_ref(map_with!(for<'a, T> |v: &'a [T]| -> BufferSlice<'a> {
             BufferSlice::from(v)
         }))
     }
-
-    #[doc(hidden)]
-    #[must_use]
-    pub unsafe fn get_data_ty_len(&self) -> (*const u8, BufferTy, usize) {
-        self.map_ref(map_with!(
-            for<'a, T> |v: &'a [T]| -> (*const u8, BufferTy, usize) {
-                (v.as_ptr().cast::<u8>(), T::TY, v.len())
-            }
-        ))
-    }
 }
 
 impl<B: OwnedBuffer> BufferVec<B>
 where
     B::Buffer<u8>: core::ops::DerefMut<Target = [u8]>,
     B::Buffer<u16>: core::ops::DerefMut<Target = [u16]>,
     B::Buffer<u32>: core::ops::DerefMut<Target = [u32]>,
@@ -107,14 +99,15 @@
     B::Buffer<i16>: core::ops::DerefMut<Target = [i16]>,
     B::Buffer<i32>: core::ops::DerefMut<Target = [i32]>,
     B::Buffer<i64>: core::ops::DerefMut<Target = [i64]>,
     B::Buffer<f32>: core::ops::DerefMut<Target = [f32]>,
     B::Buffer<f64>: core::ops::DerefMut<Target = [f64]>,
 {
     #[must_use]
+    #[allow(clippy::trait_duplication_in_bounds)]
     pub fn map_ref_mut<'a, F: HigherOrderMap, R>(&'a mut self, map: F) -> R
     where
         F: HigherOrderMap<Args<u8> = &'a mut [u8], Output<u8> = R>
             + HigherOrderMap<Args<u16> = &'a mut [u16], Output<u16> = R>
             + HigherOrderMap<Args<u32> = &'a mut [u32], Output<u32> = R>
             + HigherOrderMap<Args<u64> = &'a mut [u64], Output<u64> = R>
             + HigherOrderMap<Args<i8> = &'a mut [i8], Output<i8> = R>
@@ -138,44 +131,34 @@
         }
     }
 
     #[must_use]
     pub fn as_bytes_mut(&mut self) -> &mut [u8] {
         self.map_ref_mut(map_with!(for<'a, T> |v: &'a mut [T]| -> &'a mut [u8] {
             let (data, len) = (v.as_mut_ptr().cast::<u8>(), core::mem::size_of_val(v));
-            unsafe { core::slice::from_raw_parts_mut(data, len) }
+            #[allow(unsafe_code)]
+            // Safety:
+            // - we have a mutable reference to self
+            // - all slice element types can be modified on a per-byte basis
+            unsafe {
+                core::slice::from_raw_parts_mut(data, len)
+            }
         }))
     }
 }
 
 impl BufferVec<VecBuffer> {
     #[must_use]
     pub fn zeros_with_ty_len(ty: BufferTy, len: usize) -> Self {
         ty.map(
             map_with!(for<T> move(len: usize) || -> BufferVec<VecBuffer> {
                 BufferVec::from(vec![T::ZERO; len])
             }),
         )
     }
-
-    #[doc(hidden)]
-    #[allow(unused)]
-    #[must_use]
-    pub unsafe fn copy_from_data_ty_len(src: *const u8, ty: BufferTy, len: usize) -> Self {
-        let align = ty.layout().align();
-        assert_eq!(crate::casts::ptr_addr(src) % align, 0);
-
-        let mut buf = Self::zeros_with_ty_len(ty, len);
-        let dst = buf.as_bytes_mut().as_mut_ptr();
-        let count = buf.as_slice().as_bytes().len();
-
-        unsafe { core::ptr::copy_nonoverlapping(src, dst, count) };
-
-        buf
-    }
 }
 
 impl<B: OwnedBufferImpl> From<B> for BufferVec<B::Provider> {
     fn from(buffer: B) -> Self {
         <B::Item as BufferTyBound>::into_buffer_vec(buffer)
     }
 }
```

### Comparing `field-compression-benchmark-0.0.1/codecs/core/src/map.rs` & `field-compression-benchmark-0.0.2/codecs/core/src/map.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/codecs/core/src/slice.rs` & `field-compression-benchmark-0.0.2/codecs/core/src/slice.rs`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     I64(&'a [i64]),
     F32(&'a [f32]),
     F64(&'a [f64]),
 }
 
 impl<'a> BufferSlice<'a> {
     #[must_use]
+    #[allow(clippy::trait_duplication_in_bounds)]
     pub fn map<F: HigherOrderMap, R>(self, map: F) -> R
     where
         F: HigherOrderMap<Args<u8> = &'a [u8], Output<u8> = R>
             + HigherOrderMap<Args<u16> = &'a [u16], Output<u16> = R>
             + HigherOrderMap<Args<u32> = &'a [u32], Output<u32> = R>
             + HigherOrderMap<Args<u64> = &'a [u64], Output<u64> = R>
             + HigherOrderMap<Args<i8> = &'a [i8], Output<i8> = R>
@@ -75,39 +76,30 @@
         }))
     }
 
     #[must_use]
     pub fn as_bytes(&self) -> &'a [u8] {
         self.map(map_with!(for<'a, T> |v: &'a [T]| -> &'a [u8] {
             let (data, len) = (v.as_ptr().cast::<u8>(), core::mem::size_of_val(v));
-            unsafe { core::slice::from_raw_parts(data, len) }
+            #[allow(unsafe_code)]
+            // Safety:
+            // - we have a reference to self
+            // - all slice element types can be modified on a per-byte basis
+            unsafe {
+                core::slice::from_raw_parts(data, len)
+            }
         }))
     }
 
     #[must_use]
     pub fn to_vec(&self) -> BufferVec {
         self.map(map_with!(for<'a, T> |v: &'a [T]| -> BufferVec {
             BufferVec::from(Vec::from(v))
         }))
     }
-
-    #[doc(hidden)]
-    #[must_use]
-    pub unsafe fn from_data_ty_len(data: *const u8, ty: BufferTy, len: usize) -> Self {
-        let align = ty.layout().align();
-        assert_eq!(crate::casts::ptr_addr(data) % align, 0);
-
-        ty.map(
-            map_with!(for<'a, T> move(data: *const u8, len: usize) || -> BufferSlice<'a> {
-                BufferSlice::from(
-                    unsafe { core::slice::from_raw_parts(data.cast::<T>(), len) }
-                )
-            }),
-        )
-    }
 }
 
 impl<'a, T: BufferTyBound> From<&'a [T]> for BufferSlice<'a> {
     fn from(slice: &'a [T]) -> Self {
         T::into_buffer_slice(slice)
     }
 }
```

### Comparing `field-compression-benchmark-0.0.1/codecs/core/src/ty.rs` & `field-compression-benchmark-0.0.2/codecs/core/src/ty.rs`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,20 @@
     F32 = 32 | 2,
     #[serde(rename = "float64")]
     F64 = 64 | 2,
 }
 
 impl BufferTy {
     #[must_use]
-    pub fn new<T: BufferTyBound>() -> Self {
+    pub const fn new<T: BufferTyBound>() -> Self {
         T::TY
     }
 
     #[must_use]
+    #[allow(clippy::trait_duplication_in_bounds)]
     pub fn map<F: HigherOrderMap, R>(self, map: F) -> R
     where
         F: HigherOrderMap<Args<u8> = (), Output<u8> = R>
             + HigherOrderMap<Args<u16> = (), Output<u16> = R>
             + HigherOrderMap<Args<u32> = (), Output<u32> = R>
             + HigherOrderMap<Args<u64> = (), Output<u64> = R>
             + HigherOrderMap<Args<i8> = (), Output<i8> = R>
@@ -75,15 +76,15 @@
     }
 }
 
 pub struct TryBufferTyFromU32Error;
 
 impl From<BufferTy> for u32 {
     fn from(value: BufferTy) -> Self {
-        value as u32
+        value as Self
     }
 }
 
 impl TryFrom<u32> for BufferTy {
     type Error = TryBufferTyFromU32Error;
 
     fn try_from(value: u32) -> Result<Self, Self::Error> {
@@ -113,24 +114,24 @@
         }
     }
 }
 
 impl fmt::Display for BufferTy {
     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
         let str = match self {
-            BufferTy::U8 => "uint8",
-            BufferTy::U16 => "uint16",
-            BufferTy::U32 => "uint32",
-            BufferTy::U64 => "uint64",
-            BufferTy::I8 => "int8",
-            BufferTy::I16 => "int16",
-            BufferTy::I32 => "int32",
-            BufferTy::I64 => "int64",
-            BufferTy::F32 => "float32",
-            BufferTy::F64 => "float64",
+            Self::U8 => "uint8",
+            Self::U16 => "uint16",
+            Self::U32 => "uint32",
+            Self::U64 => "uint64",
+            Self::I8 => "int8",
+            Self::I16 => "int16",
+            Self::I32 => "int32",
+            Self::I64 => "int64",
+            Self::F32 => "float32",
+            Self::F64 => "float64",
         };
 
         fmt.write_str(str)
     }
 }
 
 pub trait BufferTyBound: 'static + Copy + sealed::Sealed {
```

### Comparing `field-compression-benchmark-0.0.1/codecs/core-host/Cargo.toml` & `field-compression-benchmark-0.0.2/codecs/core-host/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -8,9 +8,12 @@
 [dependencies]
 anyhow = { version = "1.0", default-features = false }
 codecs-core = { path = "../core", default-features = false }
 core-error = { path = "../../core/error", default-features = false }
 semver = { version = "1.0", default-features = false }
 serde = { version = "1.0", default-features = false, features = ["alloc", "derive"] }
 thiserror = { version = "1.0", default-features = false }
-wasm_component_layer = { git = "https://github.com/juntyr/wasm_component_layer.git", branch = "resource-transfer", version = "0.1", default-features = false }
+wasm_component_layer = { git = "https://github.com/juntyr/wasm_component_layer.git", rev = "0d6d5e5", version = "0.1", default-features = false }
 wasm_runtime_layer = { version = "0.3", default-features = false }
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/codecs/core-host/src/codec.rs` & `field-compression-benchmark-0.0.2/codecs/core-host/src/codec.rs`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     pub(crate) plugin: P,
     pub(crate) instruction_counter: u64,
     pub(crate) _marker: PhantomData<E>,
 }
 
 impl<E: WasmEngine, P: BorrowMut<CodecPlugin<E>>> WasmCodec<E, P> {
     #[must_use]
-    pub fn instruction_counter(&self) -> u64 {
+    pub const fn instruction_counter(&self) -> u64 {
         self.instruction_counter
     }
 
     #[allow(clippy::type_complexity, clippy::too_many_lines)]
     fn process(
         &mut self,
         buf: BufferSlice,
@@ -61,44 +61,24 @@
                 ("buffer", ValueType::Variant(buffer_ty.clone())),
                 ("shape", ValueType::List(ListType::new(ValueType::U32))),
             ],
         )
         .map_err(LocationError::from2)?;
 
         let buffer = match buf {
-            BufferSlice::U8(buf) => {
-                Variant::new(buffer_ty.clone(), 0, Some(Value::List(List::from(buf))))
-            },
-            BufferSlice::U16(buf) => {
-                Variant::new(buffer_ty.clone(), 1, Some(Value::List(List::from(buf))))
-            },
-            BufferSlice::U32(buf) => {
-                Variant::new(buffer_ty.clone(), 2, Some(Value::List(List::from(buf))))
-            },
-            BufferSlice::U64(buf) => {
-                Variant::new(buffer_ty.clone(), 3, Some(Value::List(List::from(buf))))
-            },
-            BufferSlice::I8(buf) => {
-                Variant::new(buffer_ty.clone(), 4, Some(Value::List(List::from(buf))))
-            },
-            BufferSlice::I16(buf) => {
-                Variant::new(buffer_ty.clone(), 5, Some(Value::List(List::from(buf))))
-            },
-            BufferSlice::I32(buf) => {
-                Variant::new(buffer_ty.clone(), 6, Some(Value::List(List::from(buf))))
-            },
-            BufferSlice::I64(buf) => {
-                Variant::new(buffer_ty.clone(), 7, Some(Value::List(List::from(buf))))
-            },
-            BufferSlice::F32(buf) => {
-                Variant::new(buffer_ty.clone(), 8, Some(Value::List(List::from(buf))))
-            },
-            BufferSlice::F64(buf) => {
-                Variant::new(buffer_ty.clone(), 9, Some(Value::List(List::from(buf))))
-            },
+            BufferSlice::U8(buf) => Variant::new(buffer_ty, 0, Some(Value::List(List::from(buf)))),
+            BufferSlice::U16(buf) => Variant::new(buffer_ty, 1, Some(Value::List(List::from(buf)))),
+            BufferSlice::U32(buf) => Variant::new(buffer_ty, 2, Some(Value::List(List::from(buf)))),
+            BufferSlice::U64(buf) => Variant::new(buffer_ty, 3, Some(Value::List(List::from(buf)))),
+            BufferSlice::I8(buf) => Variant::new(buffer_ty, 4, Some(Value::List(List::from(buf)))),
+            BufferSlice::I16(buf) => Variant::new(buffer_ty, 5, Some(Value::List(List::from(buf)))),
+            BufferSlice::I32(buf) => Variant::new(buffer_ty, 6, Some(Value::List(List::from(buf)))),
+            BufferSlice::I64(buf) => Variant::new(buffer_ty, 7, Some(Value::List(List::from(buf)))),
+            BufferSlice::F32(buf) => Variant::new(buffer_ty, 8, Some(Value::List(List::from(buf)))),
+            BufferSlice::F64(buf) => Variant::new(buffer_ty, 9, Some(Value::List(List::from(buf)))),
             buf => Err(anyhow::Error::msg(format!(
                 "unknown buffer type {}",
                 buf.ty()
             ))),
         }
         .map_err(LocationError::from2)?;
```

### Comparing `field-compression-benchmark-0.0.1/codecs/core-host/src/plugin.rs` & `field-compression-benchmark-0.0.2/codecs/core-host/src/plugin.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/codecs/core-wasm/Cargo.toml` & `field-compression-benchmark-0.0.2/fork/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 [package]
-name = "codecs-core-wasm"
+name = "fork"
 version = "0.1.0"
 edition = "2021"
+authors = ["Juniper Tyree <juniper.tyree@helsinki.fi>"]
+homepage = "https://github.com/juntyr/field-compression-benchmarkt"
+repository = "https://github.com/juntyr/field-compression-benchmark"
+readme = "README.md"
+license = "MIT OR Apache-2.0"
+rust-version = "1.77"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-codecs-core = { path = "../core" }
-format_serde_error = { version = "0.3", default-features = false, features = ["serde_json"] }
-serde = { version = "1.0", default-features = false, features = ["alloc", "derive"] }
-serde_json = { version = "1.0", default-features = false, features = ["alloc"] }
-wit-bindgen = { git = "https://github.com/alexcrichton/witx-bindgen.git", branch = "fix-rust-ctors", version = "0.22", default-features = false, features = ["macros", "realloc"] }
+core-error = { path = "../core/error", default-features = false }
+ipc-channel = { version = "0.18", default-features = false }
+libc = { version = "0.2", default-features = false }
+log = { version = "0.4", default-features = false }
+rustix = { version = "0.38", default-features = false, features = ["process", "use-libc"] }
+serde = { version = "1.0", default-features = false, features = ["std"] }
+signal-hook = { version = "0.3", default-features = false, features = ["iterator"] }
+thiserror = { version = "1.0", default-features = false }
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/codecs/core-wasm/src/config.rs` & `field-compression-benchmark-0.0.2/codecs/core-wasm/src/config.rs`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 pub struct CodecId<C: codecs_core::Codec> {
     _marker: core::marker::PhantomData<C>,
 }
 
 impl<C: codecs_core::Codec> CodecId<C> {
     #[must_use]
-    pub fn new() -> Self {
+    pub const fn new() -> Self {
         Self {
             _marker: core::marker::PhantomData::<C>,
         }
     }
 }
 
 impl<C: codecs_core::Codec> Default for CodecId<C> {
```

### Comparing `field-compression-benchmark-0.0.1/codecs/core-wasm/src/convert.rs` & `field-compression-benchmark-0.0.2/codecs/core-wasm/src/convert.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/codecs/core-wasm/src/lib.rs` & `field-compression-benchmark-0.0.2/codecs/core-wasm/src/lib.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
 #![allow(clippy::missing_errors_doc)]
 
 mod config;
 #[cfg(target_arch = "wasm32")]
 mod convert;
 
 #[doc(hidden)]
```

### Comparing `field-compression-benchmark-0.0.1/codecs/frontend/Cargo.toml` & `field-compression-benchmark-0.0.2/codecs/frontend/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,27 @@
 numpy = { version = "0.20", default-features = false }
 polonius-the-crab = { version = "0.4", default-features = false }
 pyodide-webassembly-runtime-layer = { version = ">=0.2.1", default-features = false, optional = true }
 pyo3 = { version = "0.20", default-features = false, features = ["abi3"] }
 semver = { version = "1.0", default-features = false }
 thiserror = { version = "1.0", default-features = false }
 topological-sort = { version = "0.2", default-features = false }
-wac-parser = { git = "https://github.com/peterhuene/wac.git", rev = "0b44c06", version = "0.1", default-features = false }
-walrus = { git = "https://github.com/rustwasm/walrus.git", branch = "update", version = "0.20", default-features = false }
-wasm_component_layer = { git = "https://github.com/juntyr/wasm_component_layer.git", branch = "resource-transfer", version = "0.1", default-features = false }
+wac-parser = { git = "https://github.com/peterhuene/wac.git", rev = "7b2f728", version = "0.1", default-features = false }
+walrus = { git = "https://github.com/rustwasm/walrus.git", rev = "4efdb5c", version = "0.20", default-features = false }
+wasm_component_layer = { git = "https://github.com/juntyr/wasm_component_layer.git", rev = "0d6d5e5", version = "0.1", default-features = false }
 wasm_runtime_layer = { version = "0.3", default-features = false }
-wasmparser = { version = "0.201", default-features = false }
+wasmparser = { version = "0.202", default-features = false }
 # wasmtime requires `component-model` feature since wasm_component_layer
 #  enables the feature in the common wasmtime-environ dependency
 wasmtime = { version = "18.0", default-features = false, features = ["runtime", "cranelift", "cache", "component-model"], optional = true }
-wit-component = { version = "0.201", default-features = false }
-wit-parser = { version = "0.201", default-features = false }
+wit-component = { version = "0.202", default-features = false }
+wit-parser = { version = "0.202", default-features = false }
 vecmap-rs = { version = "0.2", default-features = false }
 virtual-wasi-build = { path = "../../wasi/build" }
 
 [features]
 default = []
 wasmtime = ["dep:wasmtime", "wasm_runtime_layer/backend_wasmtime"]
 pyodide = ["dep:pyodide-webassembly-runtime-layer"]
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/codecs/frontend/src/codec.rs` & `field-compression-benchmark-0.0.2/codecs/frontend/src/codec.rs`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
         repr.push(')');
 
         Ok(repr)
     }
 
     #[getter]
-    fn instruction_counter(&self) -> u64 {
+    const fn instruction_counter(&self) -> u64 {
         self.codec.instruction_counter()
     }
 }
 
 impl WasmCodec {
     fn process<'py>(
         &mut self,
```

### Comparing `field-compression-benchmark-0.0.1/codecs/frontend/src/engine.rs` & `field-compression-benchmark-0.0.2/codecs/frontend/src/engine.rs`

 * *Files 1% similar despite different names*

```diff
@@ -24,24 +24,24 @@
     type StoreContext<'a, T: 'a> = ValidatedStoreContext<'a, T, E>;
     type StoreContextMut<'a, T: 'a> = ValidatedStoreContextMut<'a, T, E>;
     type Table = ValidatedTable<E>;
 }
 
 impl<E: WasmEngine> ValidatedEngine<E> {
     cfg_single_wasm! {
-        pub fn new(engine: E) -> Self {
+        pub const fn new(engine: E) -> Self {
             Self(engine)
         }
     }
 
-    fn as_ref(&self) -> &E {
+    const fn as_ref(&self) -> &E {
         &self.0
     }
 
-    fn from_ref(engine: &E) -> &Self {
+    const fn from_ref(engine: &E) -> &Self {
         // Safety: Self is a transparent newtype around E
         #[allow(unsafe_code)]
         unsafe {
             &*(engine as *const E).cast()
         }
     }
 }
@@ -586,15 +586,15 @@
             ctx.as_context_mut().as_inner_context_mut(),
             index,
             into_value(value),
         )
     }
 }
 
-fn as_values<E: WasmEngine>(values: &[Value<ValidatedEngine<E>>]) -> &[Value<E>] {
+const fn as_values<E: WasmEngine>(values: &[Value<ValidatedEngine<E>>]) -> &[Value<E>] {
     // Safety: all of our WASM runtime type wrappers are transparent newtypes
     #[allow(unsafe_code)]
     unsafe {
         std::slice::from_raw_parts(values.as_ptr().cast(), values.len())
     }
 }
 
@@ -602,15 +602,15 @@
     // Safety: all of our WASM runtime type wrappers are transparent newtypes
     #[allow(unsafe_code)]
     unsafe {
         std::slice::from_raw_parts_mut(values.as_mut_ptr().cast(), values.len())
     }
 }
 
-fn from_values<E: WasmEngine>(values: &[Value<E>]) -> &[Value<ValidatedEngine<E>>] {
+const fn from_values<E: WasmEngine>(values: &[Value<E>]) -> &[Value<ValidatedEngine<E>>] {
     // Safety: all of our WASM runtime type wrappers are transparent newtypes
     #[allow(unsafe_code)]
     unsafe {
         std::slice::from_raw_parts(values.as_ptr().cast(), values.len())
     }
 }
```

### Comparing `field-compression-benchmark-0.0.1/codecs/frontend/src/error.rs` & `field-compression-benchmark-0.0.2/codecs/frontend/src/error.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/codecs/frontend/src/lib.rs` & `field-compression-benchmark-0.0.2/codecs/frontend/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
-#![allow(clippy::module_name_repetitions)]
 #![allow(clippy::missing_errors_doc)] // FIXME
 
 macro_rules! cfg_single_wasm {
     ($item:item) => {
         #[cfg(any(
             all(feature = "wasmtime", not(feature = "pyodide")),
             all(feature = "pyodide", not(feature = "wasmtime")),
```

### Comparing `field-compression-benchmark-0.0.1/codecs/frontend/src/template.rs` & `field-compression-benchmark-0.0.2/codecs/frontend/src/template.rs`

 * *Files 2% similar despite different names*

```diff
@@ -91,18 +91,18 @@
 
     #[staticmethod]
     pub fn import_codec_class<'py>(
         py: Python<'py>,
         path: PathBuf,
         module: &'py PyModule,
     ) -> Result<&'py PyAny, PyLocationErr> {
-        let template = WasmCodecTemplate::load(py, path)?;
+        let template = Self::load(py, path)?;
         let template = PyCell::new(py, template)?;
 
-        WasmCodecTemplate::create_codec_class(template.borrow(), py, module)
+        Self::create_codec_class(template.borrow(), py, module)
     }
 }
 
 impl WasmCodecTemplate {
     pub fn new(path: PathBuf) -> Result<Self, LocationError<WasmCodecError>> {
         let wasm_module = Self::load_and_transform_wasm_module(&path)?;
 
@@ -167,17 +167,19 @@
             .collect::<Result<Vec<_>, _>>()?;
 
         let mut required_packages_queue = imports
             .iter()
             .map(|(package, _interface)| package.clone())
             .collect::<std::collections::VecDeque<_>>();
         let mut sorted_components = topological_sort::TopologicalSort::new();
+        #[allow(clippy::iter_on_single_items)]
         let mut package_providers = [(String::from(ROOT_COMPONENT), String::from(ROOT_COMPONENT))]
             .into_iter()
             .collect::<vecmap::VecMap<_, _>>();
+        #[allow(clippy::iter_on_single_items)]
         let mut required_components = [(String::from(ROOT_COMPONENT), imports.into_vec())]
             .into_iter()
             .collect::<vecmap::VecMap<_, _>>();
 
         while let Some(required_package) = required_packages_queue.pop_front() {
             if package_providers.contains_key(&required_package) {
                 continue;
@@ -508,14 +510,15 @@
     let mut module = create_instruction_counter_module();
 
     let mut resolve = wit_parser::Resolve::new();
 
     let interface = resolve.interfaces.alloc(wit_parser::Interface {
         name: Some(String::from("perf")),
         types: indexmap::IndexMap::new(),
+        #[allow(clippy::iter_on_single_items)]
         functions: [(
             String::from("instruction-counter"),
             wit_parser::Function {
                 name: String::from("instruction-counter"),
                 kind: wit_parser::FunctionKind::Freestanding,
                 params: Vec::new(),
                 results: wit_parser::Results::Anon(wit_parser::Type::U64),
@@ -532,26 +535,28 @@
         namespace: String::from("wasi"),
         name: String::from("perf"),
         version: Some(semver::Version::new(0, 1, 0)),
     };
     let package = resolve.packages.alloc(wit_parser::Package {
         name: package_name.clone(),
         docs: wit_parser::Docs { contents: None },
+        #[allow(clippy::iter_on_single_items)]
         interfaces: [(String::from("perf"), interface)].into_iter().collect(),
         worlds: indexmap::IndexMap::new(),
     });
     resolve.package_names.insert(package_name, package);
 
     if let Some(interface) = resolve.interfaces.get_mut(interface) {
         interface.package = Some(package);
     }
 
     let world = resolve.worlds.alloc(wit_parser::World {
         name: String::from("root"),
         imports: indexmap::IndexMap::new(),
+        #[allow(clippy::iter_on_single_items)]
         exports: [(
             wit_parser::WorldKey::Interface(interface),
             wit_parser::WorldItem::Interface(interface),
         )]
         .into_iter()
         .collect(),
         package: None, // The package is linked up below
@@ -565,14 +570,15 @@
         name: String::from("component"),
         version: None,
     };
     let root = resolve.packages.alloc(wit_parser::Package {
         name: root_name.clone(),
         docs: wit_parser::Docs { contents: None },
         interfaces: indexmap::IndexMap::new(),
+        #[allow(clippy::iter_on_single_items)]
         worlds: [(String::from("root"), world)].into_iter().collect(),
     });
     resolve.package_names.insert(root_name, root);
 
     if let Some(world) = resolve.worlds.get_mut(world) {
         world.package = Some(root);
     }
```

### Comparing `field-compression-benchmark-0.0.1/codecs/frontend/src/transform.rs` & `field-compression-benchmark-0.0.2/codecs/frontend/src/transform.rs`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                 entry,
             );
         }
 
         instruction_counter
     }
 
-    fn instruction_needs_counter_update(instr: &walrus::ir::Instr) -> bool {
+    const fn instruction_needs_counter_update(instr: &walrus::ir::Instr) -> bool {
         #[allow(clippy::match_same_arms)]
         match instr {
             walrus::ir::Instr::Block(_)
             | walrus::ir::Instr::Loop(_)
             | walrus::ir::Instr::Br(_)
             | walrus::ir::Instr::BrIf(_)
             | walrus::ir::Instr::IfElse(_)
@@ -184,15 +184,15 @@
 
             std::mem::replace(&mut visitor.result, Ok(()))?;
         }
 
         Ok(())
     }
 
-    fn may_produce_non_deterministic_nan(
+    const fn may_produce_non_deterministic_nan(
         instr: &walrus::ir::Instr,
     ) -> Result<Option<MaybeNaNKind>, NaNCanonicaliserError> {
         #[allow(clippy::match_same_arms)]
         match instr {
             walrus::ir::Instr::Block(_)
             | walrus::ir::Instr::Loop(_)
             | walrus::ir::Instr::Br(_)
@@ -245,15 +245,15 @@
             | walrus::ir::Instr::TableInit(_)
             | walrus::ir::Instr::ElemDrop(_)
             | walrus::ir::Instr::TableCopy(_) => Ok(None),
         }
     }
 
     #[allow(clippy::too_many_lines)]
-    fn unop_may_produce_non_deterministic_nan(
+    const fn unop_may_produce_non_deterministic_nan(
         unop: walrus::ir::UnaryOp,
     ) -> Result<Option<MaybeNaNKind>, NaNCanonicaliserError> {
         #[allow(clippy::match_same_arms)]
         match unop {
             // integer operations never produce NaNs
             walrus::ir::UnaryOp::I32Eqz
             | walrus::ir::UnaryOp::I32Clz
@@ -432,15 +432,15 @@
             | walrus::ir::UnaryOp::I32x4WidenLowI16x8U
             | walrus::ir::UnaryOp::I32x4WidenHighI16x8S
             | walrus::ir::UnaryOp::I32x4WidenHighI16x8U => Ok(None),
         }
     }
 
     #[allow(clippy::too_many_lines)]
-    fn binop_may_produce_non_deterministic_nan(
+    const fn binop_may_produce_non_deterministic_nan(
         binop: walrus::ir::BinaryOp,
     ) -> Result<Option<MaybeNaNKind>, NaNCanonicaliserError> {
         #[allow(clippy::match_same_arms)]
         match binop {
             // integer operations never produce NaNs
             walrus::ir::BinaryOp::I32Eq
             | walrus::ir::BinaryOp::I32Ne
```

### Comparing `field-compression-benchmark-0.0.1/codecs/identity/src/lib.rs` & `field-compression-benchmark-0.0.2/codecs/identity/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
 #![cfg_attr(not(test), no_main)]
 
 #[derive(Clone, serde::Serialize, serde::Deserialize)]
 pub struct IdentityCodec {
     // empty
 }
```

### Comparing `field-compression-benchmark-0.0.1/codecs/linear-quantize/Cargo.toml` & `field-compression-benchmark-0.0.2/codecs/zstd/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 [package]
-name = "linear-quantize-codec"
+name = "zstd-codec"
 version = "0.1.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 crate-type = ["cdylib"]
 
 [dependencies]
 codecs-core = { path = "../core", default-features = false }
 codecs-core-wasm = { path = "../core-wasm", default-features = false }
 postcard = { version = "1.0", default-features = false }
 serde = { version = "1.0", default-features = false, features = ["std", "derive"] }
-twofloat = { version = "0.7", default-features = false, features = ["std"] }
+# FIXME: enable the `no_wasm_shim` feature once published
+zstd = { version = "0.13", default-features = false }
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/codecs/linear-quantize/src/lib.rs` & `field-compression-benchmark-0.0.2/codecs/linear-quantize/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
 #![allow(clippy::missing_errors_doc)]
 #![cfg_attr(not(test), no_main)]
 
 use std::fmt;
 
 use twofloat::TwoFloat;
 
@@ -33,31 +25,40 @@
         },
         Vec::new(),
     )
     .map_err(|err| format!("LinearQuantize failed to write header: {err}"))?;
 
     let mut encoded =
         vec![Q::ZERO; (header.len() + std::mem::size_of::<Q>() - 1) / std::mem::size_of::<Q>()];
+    #[allow(unsafe_code)]
+    // Safety: encoded is at least header.len() bytes long and propely aligned for Q
     unsafe {
         std::ptr::copy_nonoverlapping(header.as_ptr(), encoded.as_mut_ptr().cast(), header.len());
     }
     encoded.reserve(data.len());
 
-    encoded.extend(
-        data.iter()
-            .map(|x| quantize((*x - minimum) / (maximum - minimum))),
-    );
+    if maximum == minimum {
+        let zero = quantize(T::ZERO);
+        encoded.extend(data.iter().map(|_x| zero));
+    } else {
+        encoded.extend(
+            data.iter()
+                .map(|x| quantize((*x - minimum) / (maximum - minimum))),
+        );
+    }
 
     Ok(encoded)
 }
 
 pub fn decompress<T: Float, Q: Unsigned>(
     data: &[Q],
     floatify: impl Fn(Q) -> T,
 ) -> Result<(Vec<T>, Vec<usize>), String> {
+    #[allow(unsafe_code)]
+    // Safety: data is data.len()*size_of::<Q> bytes long and propely aligned for Q
     let (header, remaining) = postcard::take_from_bytes::<CompressionHeader<T>>(unsafe {
         std::slice::from_raw_parts(data.as_ptr().cast(), std::mem::size_of_val(data))
     })
     .map_err(|err| format!("LinearQuantize failed to read header: {err}"))?;
     let data = data
         .get(data.len() - (remaining.len() / std::mem::size_of::<Q>())..)
         .unwrap_or(&[]);
@@ -112,51 +113,79 @@
         shape: &[usize],
     ) -> Result<codecs_core::ShapedBuffer<Self::EncodedBuffer>, String> {
         let encoded = match (buf, self.dtype) {
             (codecs_core::BufferSlice::F32(data), DType::F32) => match self.bits {
                 bits @ ..=8 => codecs_core::BufferVec::U8(compress(data, shape, |x| {
                     let max = f32::from(u8::MAX >> (8 - bits));
                     let x = (x * f32::scale_for_bits(bits)).clamp(0.0, max);
-                    unsafe { x.to_int_unchecked::<u8>() }
+                    #[allow(unsafe_code)]
+                    // Safety: x is clamped beforehand
+                    unsafe {
+                        x.to_int_unchecked::<u8>()
+                    }
                 })?),
                 bits @ ..=16 => codecs_core::BufferVec::U16(compress(data, shape, |x| {
                     let max = f32::from(u16::MAX >> (16 - bits));
                     let x = (x * f32::scale_for_bits(bits)).clamp(0.0, max);
-                    unsafe { x.to_int_unchecked::<u16>() }
+                    #[allow(unsafe_code)]
+                    // Safety: x is clamped beforehand
+                    unsafe {
+                        x.to_int_unchecked::<u16>()
+                    }
                 })?),
                 bits => codecs_core::BufferVec::U32(compress(data, shape, |x| {
                     // we need to use f64 here to have sufficient precision
                     let max = f64::from(u32::MAX >> (32 - bits));
                     let x = (f64::from(x) * f64::scale_for_bits(bits)).clamp(0.0, max);
-                    unsafe { x.to_int_unchecked::<u32>() }
+                    #[allow(unsafe_code)]
+                    // Safety: x is clamped beforehand
+                    unsafe {
+                        x.to_int_unchecked::<u32>()
+                    }
                 })?),
             },
             (codecs_core::BufferSlice::F64(data), DType::F64) => match self.bits {
                 bits @ ..=8 => codecs_core::BufferVec::U8(compress(data, shape, |x| {
                     let max = f64::from(u8::MAX >> (8 - bits));
                     let x = (x * f64::scale_for_bits(bits)).clamp(0.0, max);
-                    unsafe { x.to_int_unchecked::<u8>() }
+                    #[allow(unsafe_code)]
+                    // Safety: x is clamped beforehand
+                    unsafe {
+                        x.to_int_unchecked::<u8>()
+                    }
                 })?),
                 bits @ ..=16 => codecs_core::BufferVec::U16(compress(data, shape, |x| {
                     let max = f64::from(u16::MAX >> (16 - bits));
                     let x = (x * f64::scale_for_bits(bits)).clamp(0.0, max);
-                    unsafe { x.to_int_unchecked::<u16>() }
+                    #[allow(unsafe_code)]
+                    // Safety: x is clamped beforehand
+                    unsafe {
+                        x.to_int_unchecked::<u16>()
+                    }
                 })?),
                 bits @ ..=32 => codecs_core::BufferVec::U32(compress(data, shape, |x| {
                     let max = f64::from(u32::MAX >> (32 - bits));
                     let x = (x * f64::scale_for_bits(bits)).clamp(0.0, max);
-                    unsafe { x.to_int_unchecked::<u32>() }
+                    #[allow(unsafe_code)]
+                    // Safety: x is clamped beforehand
+                    unsafe {
+                        x.to_int_unchecked::<u32>()
+                    }
                 })?),
                 bits => codecs_core::BufferVec::U64(compress(data, shape, |x| {
                     // we need to use TwoFloat here to have sufficient precision
                     let max = TwoFloat::from(u64::MAX >> (64 - bits));
                     let x = (TwoFloat::from(x) * f64::scale_for_bits(bits))
                         .max(TwoFloat::from(0.0))
                         .min(max);
-                    unsafe { u64::try_from(x).unwrap_unchecked() }
+                    #[allow(unsafe_code)]
+                    // Safety: x is clamped beforehand
+                    unsafe {
+                        u64::try_from(x).unwrap_unchecked()
+                    }
                 })?),
             },
             (buf, _) => {
                 return Err(format!(
                     "LinearQuantize::encode buffer dtype `{}` does not match the configured dtype \
                      `{}`",
                     buf.ty(),
@@ -288,14 +317,15 @@
     Copy
     + serde::Serialize
     + serde::de::DeserializeOwned
     + std::ops::Sub<Self, Output = Self>
     + std::ops::Div<Self, Output = Self>
     + std::ops::Add<Self, Output = Self>
     + std::ops::Mul<Self, Output = Self>
+    + PartialEq
 {
     const ZERO: Self;
     const ONE: Self;
 
     #[must_use]
     fn minimum(self, other: Self) -> Self;
 
@@ -503,8 +533,33 @@
                 // FIXME: there seem to be some rounding errors
                 assert!((o - d).abs() < 2.0);
             }
         }
 
         Ok(())
     }
+
+    #[test]
+    fn const_data_roundtrip() -> Result<(), String> {
+        for bits in 1..=64 {
+            let data = [42.0, 42.0, 42.0, 42.0];
+
+            let codec = LinearQuantizeCodec {
+                dtype: DType::F64,
+                bits,
+            };
+
+            let encoded = codec.encode(BufferSlice::F64(&data), &[data.len()])?;
+            let decoded = codec.decode(encoded.buffer.as_slice(), &encoded.shape)?;
+
+            let BufferSlice::F64(decoded) = decoded.buffer.as_slice() else {
+                return Err(String::from("wrong decode output type"));
+            };
+
+            for (o, d) in data.iter().zip(decoded.iter()) {
+                assert_eq!(o.to_bits(), d.to_bits());
+            }
+        }
+
+        Ok(())
+    }
 }
```

### Comparing `field-compression-benchmark-0.0.1/codecs/log/src/lib.rs` & `field-compression-benchmark-0.0.2/codecs/log/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
 #![allow(clippy::missing_errors_doc)]
 #![cfg_attr(not(test), no_main)]
 
 pub fn ln_1p<T: Float>(data: &[T]) -> Result<Vec<T>, String> {
     if data.iter().copied().any(T::is_negative) {
         return Err(String::from("Log cannot encode negative data"));
     }
@@ -72,28 +63,28 @@
     }
 
     fn decode(
         &self,
         buf: codecs_core::BufferSlice,
         shape: &[usize],
     ) -> Result<codecs_core::ShapedBuffer<Self::DecodedBuffer>, String> {
-        let encoded = match buf {
+        let decoded = match buf {
             codecs_core::BufferSlice::F32(data) => codecs_core::BufferVec::F32(exp_m1(data)?),
             codecs_core::BufferSlice::F64(data) => codecs_core::BufferVec::F64(exp_m1(data)?),
             buf => {
                 return Err(format!(
                     "Log::decode does not support the buffer dtype `{}`",
                     buf.ty(),
                 ))
             },
         };
 
         Ok(codecs_core::ShapedBuffer {
             shape: Vec::from(shape),
-            buffer: encoded,
+            buffer: decoded,
         })
     }
 
     fn get_config<S: serde::Serializer>(&self, serializer: S) -> Result<S::Ok, S::Error> {
         serde::Serialize::serialize(&self, serializer)
     }
 }
```

### Comparing `field-compression-benchmark-0.0.1/codecs/reinterpret/src/lib.rs` & `field-compression-benchmark-0.0.2/codecs/reinterpret/src/lib.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
 #![allow(clippy::missing_errors_doc)]
 #![cfg_attr(not(test), no_main)]
 
 #[derive(Clone, serde::Serialize, serde::Deserialize)]
 pub struct ReinterpretCodec {
     encode_dtype: codecs_core::BufferTy,
     decode_dtype: codecs_core::BufferTy,
@@ -62,63 +54,73 @@
                  `{}`",
                 buf.ty(),
                 self.decode_dtype
             ));
         }
 
         let (encoded, shape) = match (&buf, self.encode_dtype) {
-            (buf, ty) if buf.ty() == ty => (*buf, Vec::from(shape)),
+            (buf, ty) if buf.ty() == ty => (buf.to_vec(), Vec::from(shape)),
             (buf, codecs_core::BufferTy::U8) => {
                 let mut shape = Vec::from(shape);
                 if let Some(last) = shape.last_mut() {
                     *last *= buf.ty().layout().size();
                 }
-                (codecs_core::BufferSlice::U8(buf.as_bytes()), shape)
+                (codecs_core::BufferVec::U8(buf.as_bytes().to_vec()), shape)
             },
             (codecs_core::BufferSlice::I16(v), codecs_core::BufferTy::U16) => (
-                codecs_core::BufferSlice::U16(unsafe {
-                    std::slice::from_raw_parts(v.as_ptr().cast(), v.len())
-                }),
+                codecs_core::BufferVec::U16(
+                    v.iter()
+                        .map(|x| u16::from_ne_bytes(x.to_ne_bytes()))
+                        .collect(),
+                ),
                 Vec::from(shape),
             ),
             (codecs_core::BufferSlice::I32(v), codecs_core::BufferTy::U32) => (
-                codecs_core::BufferSlice::U32(unsafe {
-                    std::slice::from_raw_parts(v.as_ptr().cast(), v.len())
-                }),
+                codecs_core::BufferVec::U32(
+                    v.iter()
+                        .map(|x| u32::from_ne_bytes(x.to_ne_bytes()))
+                        .collect(),
+                ),
                 Vec::from(shape),
             ),
             (codecs_core::BufferSlice::F32(v), codecs_core::BufferTy::U32) => (
-                codecs_core::BufferSlice::U32(unsafe {
-                    std::slice::from_raw_parts(v.as_ptr().cast(), v.len())
-                }),
+                codecs_core::BufferVec::U32(
+                    v.iter()
+                        .map(|x| u32::from_ne_bytes(x.to_ne_bytes()))
+                        .collect(),
+                ),
                 Vec::from(shape),
             ),
             (codecs_core::BufferSlice::I64(v), codecs_core::BufferTy::U64) => (
-                codecs_core::BufferSlice::U64(unsafe {
-                    std::slice::from_raw_parts(v.as_ptr().cast(), v.len())
-                }),
+                codecs_core::BufferVec::U64(
+                    v.iter()
+                        .map(|x| u64::from_ne_bytes(x.to_ne_bytes()))
+                        .collect(),
+                ),
                 Vec::from(shape),
             ),
             (codecs_core::BufferSlice::F64(v), codecs_core::BufferTy::U64) => (
-                codecs_core::BufferSlice::U64(unsafe {
-                    std::slice::from_raw_parts(v.as_ptr().cast(), v.len())
-                }),
+                codecs_core::BufferVec::U64(
+                    v.iter()
+                        .map(|x| u64::from_ne_bytes(x.to_ne_bytes()))
+                        .collect(),
+                ),
                 Vec::from(shape),
             ),
             (buf, ty) => {
                 return Err(format!(
                     "Reinterpret::encode reinterpreting buffer dtype `{}` as `{ty}` is not allowed",
                     buf.ty(),
                 ));
             },
         };
 
         Ok(codecs_core::ShapedBuffer {
             shape,
-            buffer: encoded.to_vec(),
+            buffer: encoded,
         })
     }
 
     fn decode(
         &self,
         buf: codecs_core::BufferSlice,
         shape: &[usize],
@@ -129,79 +131,91 @@
                  `{}`",
                 buf.ty(),
                 self.encode_dtype
             ));
         }
 
         let (decoded, shape) = match (&buf, self.decode_dtype) {
-            (buf, ty) if buf.ty() == ty => (*buf, Vec::from(shape)),
+            (buf, ty) if buf.ty() == ty => (buf.to_vec(), Vec::from(shape)),
             (codecs_core::BufferSlice::U8(v), ty) => {
                 let mut shape = Vec::from(shape);
                 if let Some(last) = shape.last_mut() {
                     if *last % ty.layout().size() != 0 {
                         return Err(format!(
                             "Reinterpret::decode byte buffer with shape {shape:?} cannot be \
                              reinterpreted as {ty}"
                         ));
                     }
 
                     *last /= ty.layout().size();
                 }
-                (
-                    unsafe {
-                        codecs_core::BufferSlice::from_data_ty_len(
-                            v.as_ptr(),
-                            ty,
-                            v.len() / ty.layout().size(),
-                        )
-                    },
-                    shape,
-                )
+                let mut buffer =
+                    codecs_core::BufferVec::zeros_with_ty_len(ty, v.len() / ty.layout().size());
+                #[allow(unsafe_code)]
+                // Safety: buffer is v.len() bytes long and propely aligned for ty
+                unsafe {
+                    std::ptr::copy_nonoverlapping(
+                        v.as_ptr(),
+                        buffer.as_bytes_mut().as_mut_ptr().cast(),
+                        v.len(),
+                    );
+                }
+                (buffer, shape)
             },
             (codecs_core::BufferSlice::U16(v), codecs_core::BufferTy::I16) => (
-                codecs_core::BufferSlice::I16(unsafe {
-                    std::slice::from_raw_parts(v.as_ptr().cast(), v.len())
-                }),
+                codecs_core::BufferVec::I16(
+                    v.iter()
+                        .map(|x| i16::from_ne_bytes(x.to_ne_bytes()))
+                        .collect(),
+                ),
                 Vec::from(shape),
             ),
             (codecs_core::BufferSlice::U32(v), codecs_core::BufferTy::I32) => (
-                codecs_core::BufferSlice::I32(unsafe {
-                    std::slice::from_raw_parts(v.as_ptr().cast(), v.len())
-                }),
+                codecs_core::BufferVec::I32(
+                    v.iter()
+                        .map(|x| i32::from_ne_bytes(x.to_ne_bytes()))
+                        .collect(),
+                ),
                 Vec::from(shape),
             ),
             (codecs_core::BufferSlice::U32(v), codecs_core::BufferTy::F32) => (
-                codecs_core::BufferSlice::F32(unsafe {
-                    std::slice::from_raw_parts(v.as_ptr().cast(), v.len())
-                }),
+                codecs_core::BufferVec::F32(
+                    v.iter()
+                        .map(|x| f32::from_ne_bytes(x.to_ne_bytes()))
+                        .collect(),
+                ),
                 Vec::from(shape),
             ),
             (codecs_core::BufferSlice::U64(v), codecs_core::BufferTy::I64) => (
-                codecs_core::BufferSlice::I64(unsafe {
-                    std::slice::from_raw_parts(v.as_ptr().cast(), v.len())
-                }),
+                codecs_core::BufferVec::I64(
+                    v.iter()
+                        .map(|x| i64::from_ne_bytes(x.to_ne_bytes()))
+                        .collect(),
+                ),
                 Vec::from(shape),
             ),
             (codecs_core::BufferSlice::U64(v), codecs_core::BufferTy::F64) => (
-                codecs_core::BufferSlice::F64(unsafe {
-                    std::slice::from_raw_parts(v.as_ptr().cast(), v.len())
-                }),
+                codecs_core::BufferVec::F64(
+                    v.iter()
+                        .map(|x| f64::from_ne_bytes(x.to_ne_bytes()))
+                        .collect(),
+                ),
                 Vec::from(shape),
             ),
             (buf, ty) => {
                 return Err(format!(
                     "Reinterpret::decode reinterpreting buffer dtype `{}` as `{ty}` is not allowed",
                     buf.ty(),
                 ));
             },
         };
 
         Ok(codecs_core::ShapedBuffer {
             shape,
-            buffer: decoded.to_vec(),
+            buffer: decoded,
         })
     }
 
     fn get_config<S: serde::Serializer>(&self, serializer: S) -> Result<S::Ok, S::Error> {
         serde::Serialize::serialize(&self, serializer)
     }
 }
```

### Comparing `field-compression-benchmark-0.0.1/codecs/sz3/Cargo.toml` & `field-compression-benchmark-0.0.2/codecs/uniform-noise/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [package]
-name = "sz3-codec"
+name = "uniform-noise-codec"
 version = "0.1.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 crate-type = ["cdylib"]
 
 [dependencies]
 codecs-core = { path = "../core", default-features = false }
 codecs-core-wasm = { path = "../core-wasm", default-features = false }
-postcard = { version = "1.0", default-features = false }
+rand = { version = "0.8", default-features = false }
+rand_chacha = { version = "0.3", default-features = false }
 serde = { version = "1.0", default-features = false, features = ["std", "derive"] }
-sz3 = { git = "https://github.com/juntyr/sz3-rs.git", rev = "475d6e0", version = "0.1", default-features = false }
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/codecs/sz3/src/lib.rs` & `field-compression-benchmark-0.0.2/codecs/sz3/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
 #![allow(clippy::missing_errors_doc)]
 #![cfg_attr(not(test), no_main)]
 
 use std::fmt;
 
 pub fn compress<T: Sz3Element>(
     data: &[T],
```

### Comparing `field-compression-benchmark-0.0.1/codecs/wit/world.wit` & `field-compression-benchmark-0.0.2/codecs/wit/world.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/codecs/zfp/src/lib.rs` & `field-compression-benchmark-0.0.2/codecs/zfp/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
 #![allow(clippy::missing_errors_doc)]
 #![cfg_attr(not(test), no_main)]
 
 pub mod zfp;
 
 pub fn compress<T: zfp::ZfpCompressible>(
     data: &[T],
```

### Comparing `field-compression-benchmark-0.0.1/codecs/zfp/src/zfp.rs` & `field-compression-benchmark-0.0.2/codecs/zfp/src/zfp.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#![allow(clippy::module_name_repetitions)]
+#![allow(unsafe_code)] // FFI
 
 use std::marker::PhantomData;
 
 #[derive(Clone, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "mode")]
 #[serde(deny_unknown_fields)]
 pub enum ZfpCompressionMode {
@@ -113,15 +113,15 @@
             shape => {
                 return Err(format!(
                     "Zfp only supports 1-4-dimensional data, found {shape:?}"
                 ))
             },
         };
 
-        Ok(ZfpField {
+        Ok(Self {
             field,
             dims,
             _marker: PhantomData::<T>,
         })
     }
 }
```

### Comparing `field-compression-benchmark-0.0.1/codecs/zlib/Cargo.toml` & `field-compression-benchmark-0.0.2/codecs/linear-quantize/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [package]
-name = "zlib-codec"
+name = "linear-quantize-codec"
 version = "0.1.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 crate-type = ["cdylib"]
 
 [dependencies]
 codecs-core = { path = "../core", default-features = false }
 codecs-core-wasm = { path = "../core-wasm", default-features = false }
-miniz_oxide = { version = "0.7", default-features = false, features = ["with-alloc"] }
 postcard = { version = "1.0", default-features = false }
 serde = { version = "1.0", default-features = false, features = ["std", "derive"] }
-serde_repr = { version = "0.1", default-features = false }
+twofloat = { version = "0.7", default-features = false, features = ["std"] }
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/codecs/zlib/src/lib.rs` & `field-compression-benchmark-0.0.2/codecs/zlib/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
 #![allow(clippy::missing_errors_doc)]
 #![cfg_attr(not(test), no_main)]
 
 pub fn compress(
     buf: codecs_core::BufferSlice,
     shape: &[usize],
     level: ZlibLevel,
```

### Comparing `field-compression-benchmark-0.0.1/codecs/zstd/Cargo.toml` & `field-compression-benchmark-0.0.2/codecs/zlib/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [package]
-name = "zstd-codec"
+name = "zlib-codec"
 version = "0.1.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 crate-type = ["cdylib"]
 
 [dependencies]
 codecs-core = { path = "../core", default-features = false }
 codecs-core-wasm = { path = "../core-wasm", default-features = false }
+miniz_oxide = { version = "0.7", default-features = false, features = ["with-alloc"] }
 postcard = { version = "1.0", default-features = false }
 serde = { version = "1.0", default-features = false, features = ["std", "derive"] }
-# FIXME: enable the `no_wasm_shim` feature once published
-zstd = { version = "0.13", default-features = false }
+serde_repr = { version = "0.1", default-features = false }
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/codecs/zstd/src/lib.rs` & `field-compression-benchmark-0.0.2/codecs/zstd/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
 #![cfg_attr(not(test), no_main)]
 
 #[derive(Clone, serde::Serialize, serde::Deserialize)]
 pub struct ZstdCodec {
     level: ZstdLevel,
 }
```

### Comparing `field-compression-benchmark-0.0.1/core/benchmark/Cargo.toml` & `field-compression-benchmark-0.0.2/core/benchmark/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -18,7 +18,10 @@
 rand = { version = "0.8", default-features = false }
 rand_chacha = { version = "0.3", default-features = false }
 serde = { version = "1.0", default-features = false, features = ["derive"] }
 sorted-vec = { version = "0.8", default-features = false }
 thiserror = { version = "1.0", default-features = false }
 uuid = { version = "1.5", default-features = false, features = ["std", "v8", "serde"] }
 vecmap-rs = { version = "0.2", default-features = false, features = ["serde"] }
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/core/benchmark/src/case.rs` & `field-compression-benchmark-0.0.2/core/benchmark/src/case.rs`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         case.variable
             .dimensions()
             .for_each(|(name, _)| name.hash(&mut checksum));
         case.compressor.config_path().hash(&mut checksum);
         case.compressor.name().hash(&mut checksum);
         case.compressor.codecs().len().hash(&mut checksum);
         case.compressor.codecs().for_each(|codec| {
-            codec.import().hash(&mut checksum);
+            codec.import_path().hash(&mut checksum);
             codec.kind().hash(&mut checksum);
             codec.parameters().count().hash(&mut checksum);
             codec.parameters().for_each(|(name, param)| {
                 name.hash(&mut checksum);
                 param.hash(&mut checksum);
             });
         });
@@ -86,15 +86,15 @@
             compressor,
             codec_params,
             checksum,
         }
     }
 
     #[must_use]
-    pub fn from_uuid(uuid: Uuid) -> Self {
+    pub const fn from_uuid(uuid: Uuid) -> Self {
         let bytes = uuid.into_bytes();
 
         let mut checksum_bytes = [0u8; 4];
         checksum_bytes[0] = bytes[12];
         checksum_bytes[1] = bytes[13];
         checksum_bytes[2] = bytes[14];
         checksum_bytes[3] = bytes[15];
@@ -204,25 +204,29 @@
         // include UUIDv8 variant field
         (hash & (u32::MAX >> 2)) | (0b10_u32 << 30)
     }
 }
 
 impl serde::Serialize for BenchmarkCaseId {
     fn serialize<S: serde::Serializer>(&self, serializer: S) -> Result<S::Ok, S::Error> {
-        self.into_uuid().serialize(serializer)
+        BenchmarkCaseIdUuid(self.into_uuid()).serialize(serializer)
     }
 }
 
 impl<'de> serde::Deserialize<'de> for BenchmarkCaseId {
     fn deserialize<D: serde::Deserializer<'de>>(deserializer: D) -> Result<Self, D::Error> {
-        let uuid = Uuid::deserialize(deserializer)?;
+        let BenchmarkCaseIdUuid(uuid) = BenchmarkCaseIdUuid::deserialize(deserializer)?;
         Ok(Self::from_uuid(uuid))
     }
 }
 
+#[derive(Copy, Clone, serde::Serialize, serde::Deserialize)]
+#[serde(rename = "BenchmarkCaseId")]
+struct BenchmarkCaseIdUuid(Uuid);
+
 pub struct BenchmarkCaseFilter {
     ids: HashSet<BenchmarkCaseId>,
     dataset: Bloom<u32>,
     variable: Bloom<u16>,
     compressor: Bloom<u16>,
     codec_params: Bloom<u32>,
 }
```

### Comparing `field-compression-benchmark-0.0.1/core/benchmark/src/error.rs` & `field-compression-benchmark-0.0.2/core/benchmark/src/error.rs`

 * *Files 27% similar despite different names*

```diff
@@ -68,74 +68,140 @@
                 err.set_cause(py, Some(python.into_error()));
                 err
             }),
         }
     }
 }
 
-#[derive(Debug, Clone, Error, serde::Serialize, serde::Deserialize)]
-#[serde(rename_all = "kebab-case")]
+#[derive(Debug, Clone, Error)]
 pub enum BenchmarkCaseError {
     #[error("failed to execute Python code")]
     Python(#[source] LocationError<PyErrString>),
     #[error("failed to analyse some measurements")]
     Analysis(#[source] LocationError<StringifiedError>),
     #[error("failed to distribute a benchmark case")]
     Distributed(#[source] LocationError<StringifiedError>),
 }
 
+// FIXME: eliminate extraneous clones
+impl serde::Serialize for BenchmarkCaseError {
+    fn serialize<S: serde::Serializer>(&self, serializer: S) -> Result<S::Ok, S::Error> {
+        if serializer.is_human_readable() {
+            match self {
+                Self::Python(source) => BenchmarkCaseErrorHumanReadable::Python(source.clone()),
+                Self::Analysis(source) => BenchmarkCaseErrorHumanReadable::Analysis(source.clone()),
+                Self::Distributed(source) => {
+                    BenchmarkCaseErrorHumanReadable::Distributed(source.clone())
+                },
+            }
+            .serialize(serializer)
+        } else {
+            match self {
+                Self::Python(source) => BenchmarkCaseErrorBinary::Python {
+                    python: source.clone(),
+                },
+                Self::Analysis(source) => BenchmarkCaseErrorBinary::Analysis {
+                    analysis: source.clone(),
+                },
+                Self::Distributed(source) => BenchmarkCaseErrorBinary::Distributed {
+                    distributed: source.clone(),
+                },
+            }
+            .serialize(serializer)
+        }
+    }
+}
+
+impl<'de> serde::Deserialize<'de> for BenchmarkCaseError {
+    fn deserialize<D: serde::Deserializer<'de>>(deserializer: D) -> Result<Self, D::Error> {
+        if deserializer.is_human_readable() {
+            match BenchmarkCaseErrorHumanReadable::deserialize(deserializer)? {
+                BenchmarkCaseErrorHumanReadable::Python(source) => Ok(Self::Python(source)),
+                BenchmarkCaseErrorHumanReadable::Analysis(source) => Ok(Self::Analysis(source)),
+                BenchmarkCaseErrorHumanReadable::Distributed(source) => {
+                    Ok(Self::Distributed(source))
+                },
+            }
+        } else {
+            match BenchmarkCaseErrorBinary::deserialize(deserializer)? {
+                BenchmarkCaseErrorBinary::Python { python } => Ok(Self::Python(python)),
+                BenchmarkCaseErrorBinary::Analysis { analysis } => Ok(Self::Analysis(analysis)),
+                BenchmarkCaseErrorBinary::Distributed { distributed } => {
+                    Ok(Self::Distributed(distributed))
+                },
+            }
+        }
+    }
+}
+
+#[derive(serde::Serialize, serde::Deserialize)]
+#[serde(rename = "BenchmarkCaseError")]
+#[serde(rename_all = "kebab-case")]
+enum BenchmarkCaseErrorHumanReadable {
+    Python(LocationError<PyErrString>),
+    Analysis(LocationError<StringifiedError>),
+    Distributed(LocationError<StringifiedError>),
+}
+
+#[derive(serde::Serialize, serde::Deserialize)]
+#[serde(rename = "BenchmarkCaseError")]
+enum BenchmarkCaseErrorBinary {
+    Python {
+        python: LocationError<PyErrString>,
+    },
+    Analysis {
+        analysis: LocationError<StringifiedError>,
+    },
+    Distributed {
+        distributed: LocationError<StringifiedError>,
+    },
+}
+
 #[derive(Debug, Clone, Error, serde::Serialize, serde::Deserialize)]
 #[serde(transparent)]
 #[error("{0}")]
 pub struct StringError(pub String);
 
 #[derive(Debug, Clone, serde::Serialize, serde::Deserialize)]
-#[serde(untagged)]
-pub enum StringifiedError {
-    String(String),
-    Error {
-        message: String,
-        source: StringError,
-    },
+pub struct StringifiedError {
+    message: String,
+    source: Option<StringError>,
 }
 
 impl StringifiedError {
     #[must_use]
-    pub fn from_string(message: String) -> Self {
-        Self::String(message)
+    pub const fn from_string(message: String) -> Self {
+        Self {
+            message,
+            source: None,
+        }
     }
 
     #[must_use]
     pub fn from_err<E: std::error::Error>(err: E) -> Self {
         let message = format!("{err}");
+        let source =
+            std::error::Error::source(&err).map(|source| StringError(format!("{source:#}")));
 
-        if let Some(source) = std::error::Error::source(&err) {
-            Self::Error {
-                message,
-                source: StringError(format!("{source:#}")),
-            }
-        } else {
-            Self::String(message)
-        }
+        Self { message, source }
     }
 }
 
 impl fmt::Display for StringifiedError {
     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
-        match self {
-            Self::String(message) | Self::Error { message, .. } => fmt.write_str(message),
-        }
+        fmt.write_str(&self.message)
     }
 }
 
 impl std::error::Error for StringifiedError {
     fn source(&self) -> Option<&(dyn std::error::Error + 'static)> {
-        match self {
-            Self::String(_) => None,
-            Self::Error { source, .. } => Some(source),
+        #[allow(clippy::option_if_let_else)]
+        match &self.source {
+            None => None,
+            Some(source) => Some(source),
         }
     }
 }
 
 #[derive(Debug, Clone, serde::Serialize, serde::Deserialize)]
 #[serde(rename = "PyErr")]
 #[serde(deny_unknown_fields)]
```

### Comparing `field-compression-benchmark-0.0.1/core/benchmark/src/goodness.rs` & `field-compression-benchmark-0.0.2/core/benchmark/src/goodness.rs`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 struct DerivativeStackItem<'a> {
     head: Option<&'a DataDerivative>,
     tail: &'a [DataDerivative],
     py_data_array: Py<PyAny>,
     py_data_array_compressed: Py<PyAny>,
 }
 
-pub(crate) fn compute_derivatives_goodness_measurements(
+pub fn compute_derivatives_goodness_measurements(
     derivatives: &SortedSet<NonEmpty<DataDerivative>>,
     py_data_array: Py<PyAny>,
     py_data_array_compressed: Py<PyAny>,
     measurements: &mut [GoodnessMeasurements],
     error_settings: &ErrorSettings,
     seed: u64,
 ) -> Result<(), BenchmarkSingleCaseError> {
@@ -113,15 +113,15 @@
             )
         })?;
     }
 
     Ok(())
 }
 
-pub(crate) fn compute_goodness_measurements<'py>(
+pub fn compute_goodness_measurements<'py>(
     py: Python<'py>,
     py_data_array: &'py PyAny,
     py_data_array_compressed: &'py PyAny,
     measurements: &mut GoodnessMeasurements,
     error_settings: &ErrorSettings,
     seed: u64,
 ) -> Result<(), BenchmarkSingleCaseError> {
```

### Comparing `field-compression-benchmark-0.0.1/core/benchmark/src/lib.rs` & `field-compression-benchmark-0.0.2/core/benchmark/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
-#![allow(clippy::module_name_repetitions)]
 #![allow(clippy::missing_errors_doc)] // FIXME
 
 use std::ops::ControlFlow;
 
 use nonempty::NonEmpty;
 use pyo3::{intern, prelude::*};
 use rand::SeedableRng;
```

### Comparing `field-compression-benchmark-0.0.1/core/benchmark/src/measuring.rs` & `field-compression-benchmark-0.0.2/core/benchmark/src/measuring.rs`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     #[must_use]
     pub fn new(
         num_measurements: usize,
         histogram_resample: usize,
         num_derivatives: usize,
         num_codecs: usize,
     ) -> Self {
-        Measurements {
+        Self {
             goodness: NonEmpty {
                 head: GoodnessMeasurements {
                     uniformity: Vec::with_capacity(1),
                     uniformity_rel: Vec::with_capacity(1),
                     correlation: Vec::with_capacity(1),
                     preserved_pca: Vec::with_capacity(1),
                     bit_information: Vec::with_capacity(1),
```

### Comparing `field-compression-benchmark-0.0.1/core/benchmark/src/performance.rs` & `field-compression-benchmark-0.0.2/core/benchmark/src/performance.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 use core_measure::{
     measurement::{Bytes, CompressionRatio, InstructionsPerByte, ThroughputPerSecond, WallTime},
     Measurable,
 };
 
 use crate::{error::BenchmarkSingleCaseError, measuring::Measurements};
 
-pub(crate) fn compress_and_perform_performance_measurements<'py>(
+pub fn compress_and_perform_performance_measurements<'py>(
     py: Python<'py>,
     compressor: &ConcreteCompressor,
     py_data_array: &'py PyAny,
     measurements: &mut Measurements,
 ) -> Result<&'py PyAny, BenchmarkSingleCaseError> {
     let py_compressor = compressor.build_py(py)?;
 
     let timing = WallTime::start()?;
 
     // Eagerly compute the compression ⇄ decompression
     let (py_data_array_compressed, measurement) =
-        DataArrayCompressor::compute_compress_decompress(py, py_data_array, py_compressor)?;
+        DataArrayCompressor::compute_compress_decompress(py, py_data_array, &py_compressor)?;
 
     let timing = WallTime::end(timing)?;
 
     let mut total_instructions = None;
 
     for (measurements, measurement) in measurements.per_codec.iter_mut().zip(measurement.iter()) {
         measurements.compression_ratios.push(CompressionRatio::new(
```

### Comparing `field-compression-benchmark-0.0.1/core/benchmark/src/report.rs` & `field-compression-benchmark-0.0.2/core/benchmark/src/report.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,18 @@
     pub results: VecMap<BenchmarkCaseId, BenchmarkCaseReport<'a>>,
     pub summary: BenchmarkSummary,
 }
 
 #[derive(Debug, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
 pub struct BenchmarkCaseReport<'a> {
+    #[serde(borrow)]
     pub dataset: Cow<'a, Path>,
     pub format: DatasetFormat,
+    #[serde(borrow)]
     pub variable: DataVariableSummary<'a>,
     #[serde(borrow)]
     pub compressor: ConcreteCompressorSummary<'a>,
     pub result: Result<BenchmarkCaseOutput, BenchmarkCaseError>,
 }
 
 #[derive(Debug, Default, serde::Serialize, serde::Deserialize)]
```

### Comparing `field-compression-benchmark-0.0.1/core/benchmark/src/reporter.rs` & `field-compression-benchmark-0.0.2/core/benchmark/src/reporter.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/core/benchmark/src/settings.rs` & `field-compression-benchmark-0.0.2/core/benchmark/src/settings.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 use core_dataset::dataset::DatasetSettings;
 
 const TEN: NonZeroUsize = NonZeroUsize::MIN.saturating_add(9);
 const HUNDRED: NonZeroUsize = NonZeroUsize::MIN.saturating_add(99);
 const THOUSAND: NonZeroUsize = NonZeroUsize::MIN.saturating_add(999);
 
-#[derive(Debug, Clone, Default, PartialEq, serde::Serialize, serde::Deserialize)]
+#[derive(Debug, Clone, Default, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
 #[serde(default)]
 pub struct BenchmarkSettings {
     pub measurements: MeasurementSettings,
     pub datasets: DatasetSettings,
 }
 
-#[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
+#[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
 #[serde(default)]
 pub struct MeasurementSettings {
     pub num_repeats: NonZeroUsize,
     pub bootstrap: BootstrapSettings,
     pub error: ErrorSettings,
 }
@@ -29,15 +29,15 @@
             num_repeats: TEN,
             bootstrap: BootstrapSettings::default(),
             error: ErrorSettings::default(),
         }
     }
 }
 
-#[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
+#[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
 #[serde(default)]
 pub struct BootstrapSettings {
     pub seed: u64,
     pub samples: Option<NonZeroUsize>,
 }
 
@@ -46,15 +46,15 @@
         Self {
             seed: 42,
             samples: Some(THOUSAND),
         }
     }
 }
 
-#[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
+#[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
 #[serde(default)]
 pub struct ErrorSettings {
     pub bins: NonZeroUsize,
     pub resamples: NonZeroUsize,
 }
```

### Comparing `field-compression-benchmark-0.0.1/core/compressor/Cargo.toml` & `field-compression-benchmark-0.0.2/core/compressor/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 core-error = { path = "../error", default-features = false }
 core-measure = { path = "../measure", default-features = false }
+evalexpr = { version = "11.3.0", default-features = false }
 nonempty = { version = "0.10", default-features = false, features = ["serialize"] }
 numpy = { version = "0.20", default-features = false }
 pyo3 = { version = "0.20", default-features = false, features = ["abi3"] }
 serde = { version = "1.0", default-features = false, features = ["derive"] }
 thiserror = { version = "1.0", default-features = false }
 toml = { version = "0.8", default-features = false, features = ["parse", "preserve_order"] }
 vecmap-rs = { version = "0.2", default-features = false, features = ["serde"] }
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/core/compressor/src/codec/config.rs` & `field-compression-benchmark-0.0.2/core/compressor/src/codec/config.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 use std::fmt;
 
 use pyo3::{
     exceptions::PyTypeError,
     intern,
     prelude::*,
-    types::{IntoPyDict, PyType},
+    types::{IntoPyDict, PyString, PyType},
 };
 use vecmap::{VecMap, VecSet};
 
-use crate::parameter::Parameter;
+use crate::parameter::{Parameter, ParameterEvalContext, ParameterSeed};
 
 use super::Codec;
 
-pub struct CodecSeed<'py> {
+pub struct CodecSeed<'a, 'py> {
     py: Python<'py>,
+    codecs: &'a mut VecMap<String, Codec>,
+    eval_context: &'a mut ParameterEvalContext,
 }
 
-impl<'py> CodecSeed<'py> {
-    pub fn new(py: Python<'py>) -> Self {
-        Self { py }
+impl<'a, 'py> CodecSeed<'a, 'py> {
+    pub fn new(
+        py: Python<'py>,
+        codecs: &'a mut VecMap<String, Codec>,
+        eval_context: &'a mut ParameterEvalContext,
+    ) -> Self {
+        Self {
+            py,
+            codecs,
+            eval_context,
+        }
     }
 }
 
-impl<'py, 'de> serde::de::DeserializeSeed<'de> for CodecSeed<'py> {
-    type Value = Codec;
+impl<'a, 'py, 'de> serde::de::DeserializeSeed<'de> for CodecSeed<'a, 'py> {
+    type Value = ();
 
     fn deserialize<D: serde::Deserializer<'de>>(
         self,
         deserializer: D,
     ) -> Result<Self::Value, D::Error> {
         serde::Deserializer::deserialize_struct(deserializer, "Codec", FIELDS, self)
     }
 }
 
-const FIELDS: &[&str] = &["import", "kind", "parameters"];
+const FIELDS: &[&str] = &["name", "import_path", "import", "kind", "parameters"];
 
 #[derive(Clone, Copy)]
 enum Field {
+    Name,
     Import,
     Kind,
     Parameters,
     Excessive,
 }
 
 impl<'de> serde::de::DeserializeSeed<'de> for Field {
@@ -59,50 +70,101 @@
 
     fn expecting(&self, formatter: &mut fmt::Formatter) -> fmt::Result {
         formatter.write_str("a codec config field identifier")
     }
 
     fn visit_str<E: serde::de::Error>(self, value: &str) -> Result<Self::Value, E> {
         match (self, value) {
-            (Self::Import, "import") | (Self::Kind, "kind") | (Self::Parameters, "parameters") => {
-                Ok(())
-            },
+            (Self::Name, "name")
+            | (Self::Import, "import_path" | "import")
+            | (Self::Kind, "kind")
+            | (Self::Parameters, "parameters") => Ok(()),
             _ => Err(serde::de::Error::unknown_field(
                 value,
                 match self {
-                    Self::Import => &["import"],
+                    Self::Name => &["name"],
+                    Self::Import => &["import_path", "import"],
                     Self::Kind => &["kind"],
                     Self::Parameters => &["parameters"],
                     Self::Excessive => &[],
                 },
             )),
         }
     }
 
     fn visit_bytes<E: serde::de::Error>(self, value: &[u8]) -> Result<Self::Value, E> {
         match (self, value) {
-            (Self::Import, b"import")
+            (Self::Name, b"name")
+            | (Self::Import, b"import_path" | b"import")
             | (Self::Kind, b"kind")
             | (Self::Parameters, b"parameters") => Ok(()),
             _ => {
                 let value = String::from_utf8_lossy(value);
                 Err(serde::de::Error::unknown_field(
                     &value,
                     match self {
-                        Self::Import => &["import"],
+                        Self::Name => &["name"],
+                        Self::Import => &["import_path", "import"],
                         Self::Kind => &["kind"],
                         Self::Parameters => &["parameters"],
                         Self::Excessive => &[],
                     },
                 ))
             },
         }
     }
 }
 
+struct CodecNameSeed<'a, 'py> {
+    py: Python<'py>,
+    codecs: &'a VecMap<String, Codec>,
+}
+
+impl<'a, 'py, 'de> serde::de::DeserializeSeed<'de> for CodecNameSeed<'a, 'py> {
+    type Value = String;
+
+    fn deserialize<D: serde::Deserializer<'de>>(
+        self,
+        deserializer: D,
+    ) -> Result<Self::Value, D::Error> {
+        deserializer.deserialize_str(self)
+    }
+}
+
+impl<'a, 'py, 'de> serde::de::Visitor<'de> for CodecNameSeed<'a, 'py> {
+    type Value = String;
+
+    fn expecting(&self, formatter: &mut fmt::Formatter) -> fmt::Result {
+        formatter.write_str("a codec name")
+    }
+
+    fn visit_str<E: serde::de::Error>(self, v: &str) -> Result<Self::Value, E> {
+        if self.codecs.contains_key(v) {
+            return Err(serde::de::Error::custom(format!(
+                "duplicate codec name `{v}`"
+            )));
+        }
+
+        let is_identifier: bool = (|| {
+            PyString::new(self.py, v)
+                .call_method0(intern!(self.py, "isidentifier"))?
+                .extract()
+        })()
+        .map_err(serde::de::Error::custom)?;
+
+        if !is_identifier {
+            return Err(serde::de::Error::custom(format!(
+                "invalid codec name `{v}`: not a valid identifier"
+            )));
+        }
+
+        Ok(String::from(v))
+    }
+}
+
 struct CodecImportSeed<'py> {
     py: Python<'py>,
 }
 
 impl<'py, 'de> serde::de::DeserializeSeed<'de> for CodecImportSeed<'py> {
     type Value = (String, VecSet<String>);
 
@@ -118,26 +180,26 @@
     type Value = (String, VecSet<String>);
 
     fn expecting(&self, formatter: &mut fmt::Formatter) -> fmt::Result {
         formatter.write_str("a codec import string")
     }
 
     fn visit_str<E: serde::de::Error>(self, v: &str) -> Result<Self::Value, E> {
-        fn visit_str_inner(py: Python, import: &str) -> Result<VecSet<String>, PyErr> {
+        fn visit_str_inner(py: Python, import_path: &str) -> Result<VecSet<String>, PyErr> {
             let mut locals = Vec::new();
-            for (pos, c) in import.char_indices() {
+            for (pos, c) in import_path.char_indices() {
                 if c == '.' {
-                    if let Some(module) = import.get(..pos) {
+                    if let Some(module) = import_path.get(..pos) {
                         locals.push((module, py.import(module)?));
                     }
                 }
             }
             let locals = locals.into_py_dict(py);
 
-            let ty: &PyType = py.eval(import, None, Some(locals))?.extract()?;
+            let ty: &PyType = py.eval(import_path, None, Some(locals))?.extract()?;
 
             if !ty.is_subclass(
                 py.import(intern!(py, "numcodecs.abc"))?
                     .getattr(intern!(py, "Codec"))?,
             )? {
                 return Err(PyTypeError::new_err(
                     "not an instance of `numcodecs.abc.Codec`",
@@ -162,15 +224,15 @@
             Ok(parameters) => Ok((String::from(v), parameters)),
             Err(err) => Err(serde::de::Error::custom(err)),
         }
     }
 }
 
 struct CodecParameterNameSeed<'a> {
-    import: &'a str,
+    import_path: &'a str,
     parameters: &'a VecSet<String>,
     parameters_seen: &'a mut VecSet<String>,
 }
 
 impl<'a, 'de> serde::de::DeserializeSeed<'de> for CodecParameterNameSeed<'a> {
     type Value = String;
 
@@ -189,32 +251,34 @@
         formatter.write_str("a parameter name")
     }
 
     fn visit_str<E: serde::de::Error>(self, v: &str) -> Result<Self::Value, E> {
         if !self.parameters.contains(v) {
             return Err(serde::de::Error::custom(format!(
                 "codec {} does not have a parameter named {v:?}",
-                self.import
+                self.import_path
             )));
         }
 
         if !self.parameters_seen.insert(String::from(v)) {
             return Err(serde::de::Error::custom(format!(
                 "duplicate parameter name {v:?}"
             )));
         }
 
         Ok(String::from(v))
     }
 }
 
 struct CodecParametersSeed<'a> {
-    import: &'a str,
+    name: &'a str,
+    import_path: &'a str,
     parameters: VecSet<String>,
     parameters_seen: VecSet<String>,
+    eval_context: &'a mut ParameterEvalContext,
 }
 
 impl<'a, 'de> serde::de::DeserializeSeed<'de> for CodecParametersSeed<'a> {
     type Value = VecMap<String, Parameter>;
 
     fn deserialize<D: serde::Deserializer<'de>>(
         self,
@@ -234,59 +298,94 @@
     fn visit_map<A: serde::de::MapAccess<'de>>(
         mut self,
         mut map: A,
     ) -> Result<Self::Value, A::Error> {
         let mut parameters = VecMap::with_capacity(map.size_hint().unwrap_or(0));
 
         while let Some(name) = map.next_key_seed(CodecParameterNameSeed {
-            import: self.import,
+            import_path: self.import_path,
             parameters: &self.parameters,
             parameters_seen: &mut self.parameters_seen,
         })? {
-            parameters.insert(name, map.next_value()?);
+            let parameter = map.next_value_seed(ParameterSeed::new(self.eval_context))?;
+
+            self.eval_context
+                .set_value(
+                    self.name,
+                    &name,
+                    &parameter
+                        .example(self.name, &name, self.eval_context)
+                        .map_err(serde::de::Error::custom)?,
+                )
+                .map_err(serde::de::Error::custom)?;
+
+            parameters.insert(name, parameter);
         }
 
         Ok(parameters)
     }
 }
 
-impl<'py, 'de> serde::de::Visitor<'de> for CodecSeed<'py> {
-    type Value = Codec;
+impl<'a, 'py, 'de> serde::de::Visitor<'de> for CodecSeed<'a, 'py> {
+    type Value = ();
 
     fn expecting(&self, formatter: &mut fmt::Formatter) -> fmt::Result {
         formatter.write_str("a codec config")
     }
 
     fn visit_map<A: serde::de::MapAccess<'de>>(self, mut map: A) -> Result<Self::Value, A::Error> {
+        let Some(()) = map.next_key_seed(Field::Name)? else {
+            return Err(serde::de::Error::custom(
+                "a codec must start with a `name` field",
+            ));
+        };
+
+        let name = map.next_value_seed(CodecNameSeed {
+            py: self.py,
+            codecs: self.codecs,
+        })?;
+
         let Some(()) = map.next_key_seed(Field::Import)? else {
             return Err(serde::de::Error::custom(
-                "a codec must start with an `import` field",
+                "a codec must continue with an `import` field",
             ));
         };
 
         let (import, parameters) = map.next_value_seed(CodecImportSeed { py: self.py })?;
 
         let Some(()) = map.next_key_seed(Field::Kind)? else {
-            return Err(serde::de::Error::missing_field("kind"));
+            return Err(serde::de::Error::custom(
+                "a codec must continue with a `kind` field",
+            ));
         };
 
         let kind = map.next_value()?;
 
         let Some(()) = map.next_key_seed(Field::Parameters)? else {
-            return Err(serde::de::Error::missing_field("parameters"));
+            return Err(serde::de::Error::custom(
+                "a codec must continue with a `parameters` field",
+            ));
         };
 
         let parameters = map.next_value_seed(CodecParametersSeed {
-            import: &import,
+            name: &name,
+            import_path: &import,
             parameters_seen: VecSet::with_capacity(parameters.len()),
             parameters,
+            eval_context: self.eval_context,
         })?;
 
         map.next_key_seed(Field::Excessive)?;
 
-        Ok(Codec {
-            import,
-            kind,
-            parameters,
-        })
+        self.codecs.insert(
+            name.clone(),
+            Codec {
+                name,
+                import_path: import,
+                kind,
+                parameters,
+            },
+        );
+
+        Ok(())
     }
 }
```

### Comparing `field-compression-benchmark-0.0.1/core/compressor/src/codec/mod.rs` & `field-compression-benchmark-0.0.2/core/compressor/src/codec/mod.rs`

 * *Files 25% similar despite different names*

```diff
@@ -6,40 +6,44 @@
 };
 use vecmap::VecMap;
 
 use core_error::LocationError;
 
 use crate::{
     numcodecs,
-    parameter::{ConcreteParameter, ConcreteParameterSummary, Parameter, ParameterIterator},
+    parameter::{
+        ConcreteParameter, ConcreteParameterSummary, Parameter, ParameterEvalContext,
+        ParameterEvalError, ParameterIterator,
+    },
 };
 
 mod config;
 pub(super) use config::CodecSeed;
 
 #[derive(Debug, Clone)]
 pub struct Codec {
-    import: String,
+    name: String,
+    import_path: String,
     kind: CodecKind,
     parameters: VecMap<String, Parameter>,
 }
 
 impl Codec {
     pub fn import_py<'py>(&self, py: Python<'py>) -> Result<&'py PyType, LocationError<PyErr>> {
         let mut locals = Vec::new();
-        for (pos, c) in self.import.char_indices() {
+        for (pos, c) in self.import_path.char_indices() {
             if c == '.' {
-                if let Some(module) = self.import.get(..pos) {
+                if let Some(module) = self.import_path.get(..pos) {
                     locals.push((module, py.import(module)?));
                 }
             }
         }
         let locals = locals.into_py_dict(py);
 
-        py.eval(&self.import, None, Some(locals))?
+        py.eval(&self.import_path, None, Some(locals))?
             .extract()
             .map_err(LocationError::new)
     }
 
     #[must_use]
     pub fn cyclic_iter_concrete(&self) -> ConcreteCodecIterator {
         let parameters = self
@@ -55,29 +59,34 @@
     }
 
     pub fn minimise(&mut self) {
         self.parameters.values_mut().for_each(Parameter::minimise);
     }
 
     #[must_use]
-    pub fn import(&self) -> &str {
-        &self.import
+    pub fn name(&self) -> &str {
+        &self.name
     }
 
     #[must_use]
-    pub fn kind(&self) -> CodecKind {
+    pub fn import_path(&self) -> &str {
+        &self.import_path
+    }
+
+    #[must_use]
+    pub const fn kind(&self) -> CodecKind {
         self.kind
     }
 }
 
 impl fmt::Display for Codec {
     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
-        let name = match self.import.rsplit_once('.') {
+        let name = match self.import_path.rsplit_once('.') {
             Some((_, name)) => name,
-            None => &*self.import,
+            None => &*self.import_path,
         };
 
         fmt.write_fmt(format_args!("{name}("))?;
 
         for (i, (name, value)) in self.parameters.iter().enumerate() {
             if i > 0 {
                 fmt.write_str(", ")?;
@@ -97,17 +106,17 @@
     SymbolicLossless,
     Lossy,
 }
 
 impl fmt::Display for CodecKind {
     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
         match self {
-            CodecKind::BinaryLossless => fmt.write_str("binary-lossless"),
-            CodecKind::SymbolicLossless => fmt.write_str("symbolic-lossless"),
-            CodecKind::Lossy => fmt.write_str("lossy"),
+            Self::BinaryLossless => fmt.write_str("binary-lossless"),
+            Self::SymbolicLossless => fmt.write_str("symbolic-lossless"),
+            Self::Lossy => fmt.write_str("lossy"),
         }
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct ConcreteCodec<'a> {
     codec: &'a Codec,
@@ -137,52 +146,52 @@
             }
         }
 
         numcodecs::Codec::from_config(py_codec, config).map_err(LocationError::new)
     }
 
     #[must_use]
-    pub fn import(&self) -> &str {
-        self.codec.import()
+    pub fn import_path(&self) -> &str {
+        self.codec.import_path()
     }
 
     #[must_use]
-    pub fn kind(&self) -> CodecKind {
+    pub const fn kind(&self) -> CodecKind {
         self.codec.kind()
     }
 
     pub fn parameters(&self) -> impl Iterator<Item = (&str, &ConcreteParameter<'a>)> {
         self.codec
             .parameters
             .iter()
             .zip(self.parameters.iter())
             .map(|((name, _), concrete)| (&**name, concrete))
     }
 
     #[must_use]
     pub fn summary(&self) -> ConcreteCodecSummary<'a> {
         ConcreteCodecSummary {
-            import: Cow::Borrowed(self.codec.import.as_str()),
+            import_path: Cow::Borrowed(self.codec.import_path.as_str()),
             kind: self.codec.kind,
             parameters: self
                 .codec
                 .parameters
                 .keys()
                 .map(|name| Cow::Borrowed(name.as_str()))
                 .zip(self.parameters.iter().map(ConcreteParameter::summary))
                 .collect(),
         }
     }
 }
 
 impl<'a> fmt::Display for ConcreteCodec<'a> {
     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
-        let name = match self.codec.import.rsplit_once('.') {
+        let name = match self.codec.import_path.rsplit_once('.') {
             Some((_, name)) => name,
-            None => &*self.codec.import,
+            None => &*self.codec.import_path,
         };
 
         fmt.write_fmt(format_args!("{name}("))?;
 
         for (i, (name, value)) in self
             .codec
             .parameters
@@ -202,62 +211,87 @@
 }
 
 #[derive(Debug, Clone, serde::Serialize, serde::Deserialize)]
 #[serde(rename = "Codec")]
 #[serde(deny_unknown_fields)]
 pub struct ConcreteCodecSummary<'a> {
     #[serde(borrow)]
-    import: Cow<'a, str>,
+    import_path: Cow<'a, str>,
     kind: CodecKind,
     #[serde(borrow)]
     parameters: VecMap<Cow<'a, str>, ConcreteParameterSummary<'a>>,
 }
 
 pub struct ConcreteCodecIterator<'a> {
     codec: &'a Codec,
     parameters: Vec<ParameterIterator<'a>>,
 }
 
 impl<'a> ConcreteCodecIterator<'a> {
-    #[allow(clippy::should_implement_trait)] // FIXME
-    pub fn next(&mut self) -> ControlFlow<ConcreteCodec<'a>, ConcreteCodec<'a>> {
+    pub fn next(
+        &mut self,
+        eval_context: &mut ParameterEvalContext,
+    ) -> Result<ControlFlow<ConcreteCodec<'a>, ConcreteCodec<'a>>, ParameterEvalError> {
         let mut all_done = true;
 
+        #[allow(clippy::needless_collect)]
+        // we must not short-circuit early to ensure further iteration is not broken
         let parameters = self
+            .codec
             .parameters
-            .iter_mut()
-            .map(|parameter| {
-                if all_done {
-                    match parameter.next() {
+            .keys()
+            .zip(self.parameters.iter_mut())
+            .map(|(name, param)| -> Result<_, ParameterEvalError> {
+                let param = if all_done {
+                    match param.next(self.codec.name(), name, eval_context)? {
                         ControlFlow::Break(value) => value,
                         ControlFlow::Continue(value) => {
                             all_done = false;
                             value
                         },
                     }
                 } else {
-                    parameter.get()
-                }
+                    param.get(self.codec.name(), name, eval_context)?
+                };
+
+                eval_context.set_value(self.codec.name(), name, &param)?;
+
+                Ok(param)
             })
-            .collect();
+            .collect::<Vec<_>>();
 
         let iter = ConcreteCodec {
             codec: self.codec,
-            parameters,
+            parameters: parameters.into_iter().collect::<Result<Vec<_>, _>>()?,
         };
 
         if all_done {
-            ControlFlow::Break(iter)
+            Ok(ControlFlow::Break(iter))
         } else {
-            ControlFlow::Continue(iter)
+            Ok(ControlFlow::Continue(iter))
         }
     }
 
-    pub fn get(&self) -> ConcreteCodec<'a> {
-        let parameters = self.parameters.iter().map(ParameterIterator::get).collect();
+    pub fn get(
+        &self,
+        eval_context: &mut ParameterEvalContext,
+    ) -> Result<ConcreteCodec<'a>, ParameterEvalError> {
+        let parameters = self
+            .codec
+            .parameters
+            .keys()
+            .zip(self.parameters.iter())
+            .map(|(name, param)| -> Result<_, ParameterEvalError> {
+                let param = ParameterIterator::get(param, self.codec.name(), name, eval_context)?;
+
+                eval_context.set_value(self.codec.name(), name, &param)?;
 
-        ConcreteCodec {
+                Ok(param)
+            })
+            .collect::<Result<Vec<_>, _>>()?;
+
+        Ok(ConcreteCodec {
             codec: self.codec,
             parameters,
-        }
+        })
     }
 }
```

### Comparing `field-compression-benchmark-0.0.1/core/compressor/src/compress.rs` & `field-compression-benchmark-0.0.2/core/compressor/src/compress.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+#![allow(clippy::redundant_pub_crate)]
+
 use std::time::Duration;
 
 use numpy::PyUntypedArray;
 use pyo3::{
     intern,
     prelude::*,
-    types::{IntoPyDict, PyBool, PyList, PyTuple},
+    types::{IntoPyDict, PyBool, PyTuple},
 };
 
 use core_error::LocationError;
 use core_measure::{measurement::WallTime, Measurable};
 
+use crate::numcodecs;
+
 pub enum DataArrayCompressor {}
 
 impl DataArrayCompressor {
     pub fn compute_compress_decompress<'py>(
         py: Python<'py>,
         da: &'py PyAny,
-        compressor: &'py PyList,
+        compressor: &[&numcodecs::Codec],
     ) -> Result<(&'py PyAny, Vec<CodecPerformanceMeasurement>), LocationError<PyErr>> {
         let xarray_map_blocks = py
             .import(intern!(py, "xarray"))?
             .getattr(intern!(py, "map_blocks"))?;
 
         let tracker = PyCell::new(
             py,
@@ -36,15 +40,15 @@
                     };
                     compressor.len()
                 ],
             },
         )?;
 
         let kwargs = [
-            (intern!(py, "codecs"), &**compressor),
+            (intern!(py, "codecs"), &**PyTuple::new(py, compressor)),
             (intern!(py, "tracker"), tracker),
         ]
         .into_py_dict(py);
 
         // The compression-decompression must run single-threaded since the tracker
         //  requires mutable borrows
         let context = py
@@ -81,14 +85,61 @@
             per_codec: Vec::new(),
         });
 
         Ok((decompressed, measurement))
     }
 }
 
+pub enum NumpyArrayCompressor {}
+
+impl NumpyArrayCompressor {
+    pub fn compress_decompress<'py>(
+        py: Python<'py>,
+        array: &'py PyUntypedArray,
+        compressor: Vec<&'py crate::numcodecs::Codec>,
+    ) -> Result<(&'py PyUntypedArray, Vec<CodecPerformanceMeasurement>), LocationError<PyErr>> {
+        let numpy = py.import(intern!(py, "numpy"))?;
+
+        // ensure that the uncompressed data is in a unique and contiguous array
+        let array: &PyUntypedArray = {
+            let contiguous: &PyUntypedArray = numpy
+                .getattr(intern!(py, "ascontiguousarray"))?
+                .call1((array,))?
+                .extract()?;
+            if contiguous.is(array) {
+                numpy
+                    .getattr(intern!(py, "copy"))?
+                    .call1((contiguous,))?
+                    .extract()?
+            } else {
+                array
+            }
+        };
+
+        let mut tracker = CompressorPerformanceTracker {
+            per_codec: vec![
+                CodecPerformanceMeasurement {
+                    encode_timing: Duration::ZERO,
+                    decode_timing: Duration::ZERO,
+                    encode_instructions: None,
+                    decode_instructions: None,
+                    encoded_bytes: 0,
+                    decoded_bytes: 0,
+                };
+                compressor.len()
+            ],
+        };
+
+        let decompressed =
+            compress_decompress_contiguous_numpy_array(py, array, compressor, &mut tracker)?;
+
+        Ok((decompressed, tracker.per_codec))
+    }
+}
+
 #[derive(Clone, serde::Serialize, serde::Deserialize)]
 pub struct CodecPerformanceMeasurement {
     pub encode_timing: Duration,
     pub decode_timing: Duration,
     pub encode_instructions: Option<u64>,
     pub decode_instructions: Option<u64>,
     pub encoded_bytes: usize,
@@ -136,16 +187,15 @@
             .getattr(intern!(py, "copy"))?
             .call1((array,))?
             .extract()?
     } else {
         array
     };
 
-    let decoded =
-        compress_decompress_data_array_single_chunk_continuous(py, array, codecs, tracker)?;
+    let decoded = compress_decompress_contiguous_numpy_array(py, array, codecs, tracker)?;
 
     da.call_method(
         intern!(py, "copy"),
         PyTuple::empty(py),
         Some(
             [
                 (intern!(py, "deep"), &**PyBool::new(py, false)),
@@ -153,19 +203,19 @@
             ]
             .into_py_dict(py),
         ),
     )?
     .call_method1(intern!(py, "chunk"), (new_chunks,))
 }
 
-fn compress_decompress_data_array_single_chunk_continuous<'py>(
+fn compress_decompress_contiguous_numpy_array<'py>(
     py: Python<'py>,
     array: &'py PyUntypedArray,
     codecs: Vec<&'py crate::numcodecs::Codec>,
-    tracker: &'py mut CompressorPerformanceTracker,
+    tracker: &mut CompressorPerformanceTracker,
 ) -> Result<&'py PyUntypedArray, PyErr> {
     // pre-obtain methods that are needed in the hot encode and decode loops
     let numpy = py.import(intern!(py, "numpy"))?;
     let ensure_contiguous_ndarray_like = py
         .import(intern!(py, "numcodecs"))?
         .getattr(intern!(py, "compat"))?
         .getattr(intern!(py, "ensure_contiguous_ndarray_like"))?;
```

### Comparing `field-compression-benchmark-0.0.1/core/compressor/src/compressor/config.rs` & `field-compression-benchmark-0.0.2/core/compressor/src/compressor/config.rs`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 use pyo3::prelude::*;
 use vecmap::VecMap;
 
 use crate::{
     codec::{Codec, CodecSeed},
     compressor::Compressor,
+    parameter::ParameterEvalContext,
 };
 
 pub struct CompressorSeed<'a, 'py> {
     py: Python<'py>,
     path: Option<PathBuf>,
     compressors: Option<&'a mut VecMap<String, Option<PathBuf>>>,
 }
@@ -116,36 +117,40 @@
 }
 
 struct CompressorCodecsSeed<'py> {
     py: Python<'py>,
 }
 
 impl<'py, 'de> serde::de::DeserializeSeed<'de> for CompressorCodecsSeed<'py> {
-    type Value = Vec<Codec>;
+    type Value = VecMap<String, Codec>;
 
     fn deserialize<D: serde::Deserializer<'de>>(
         self,
         deserializer: D,
     ) -> Result<Self::Value, D::Error> {
         deserializer.deserialize_seq(self)
     }
 }
 
 impl<'py, 'de> serde::de::Visitor<'de> for CompressorCodecsSeed<'py> {
-    type Value = Vec<Codec>;
+    type Value = VecMap<String, Codec>;
 
     fn expecting(&self, formatter: &mut fmt::Formatter) -> fmt::Result {
         formatter.write_str("a list of codecs")
     }
 
     fn visit_seq<A: serde::de::SeqAccess<'de>>(self, mut seq: A) -> Result<Self::Value, A::Error> {
-        let mut codecs = Vec::with_capacity(seq.size_hint().unwrap_or(0));
+        let mut codecs = VecMap::with_capacity(seq.size_hint().unwrap_or(0));
+        let mut eval_context = ParameterEvalContext::new().map_err(serde::de::Error::custom)?;
 
-        while let Some(codec) = seq.next_element_seed(CodecSeed::new(self.py))? {
-            codecs.push(codec);
+        #[allow(clippy::equatable_if_let)]
+        while let Some(()) =
+            seq.next_element_seed(CodecSeed::new(self.py, &mut codecs, &mut eval_context))?
+        {
+            // no-op
         }
 
         Ok(codecs)
     }
 }
 
 impl<'a, 'de> serde::de::Visitor<'de> for CompressorNameSeed<'a> {
```

### Comparing `field-compression-benchmark-0.0.1/core/compressor/src/compressor/mod.rs` & `field-compression-benchmark-0.0.2/core/compressor/src/compressor/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 use std::{
     borrow::Cow,
     fmt, fs,
     ops::ControlFlow,
     path::{Path, PathBuf},
 };
 
-use pyo3::{exceptions::PyTypeError, intern, prelude::*, types::PyList};
+use pyo3::{exceptions::PyTypeError, intern, prelude::*};
 use thiserror::Error;
 use vecmap::{VecMap, VecSet};
 
 use core_error::LocationError;
 
 mod config;
 
 use self::config::CompressorSeed;
-use crate::codec::{Codec, ConcreteCodec, ConcreteCodecIterator, ConcreteCodecSummary};
+use crate::{
+    codec::{Codec, ConcreteCodec, ConcreteCodecIterator, ConcreteCodecSummary},
+    numcodecs,
+    parameter::{ParameterEvalContext, ParameterEvalError},
+};
 
 #[derive(Debug, Clone)]
 pub struct Compressor {
     config_path: Option<PathBuf>,
     name: String,
-    codecs: Vec<Codec>,
+    codecs: VecMap<String, Codec>,
 }
 
 impl Compressor {
     pub fn from_deserialised_config<'py: 'de, 'de, D: serde::Deserializer<'de>>(
         py: Python<'py>,
         deserializer: D,
-    ) -> Result<Compressor, D::Error> {
+    ) -> Result<Self, D::Error> {
         serde::de::DeserializeSeed::deserialize(CompressorSeed::new(py, None, None), deserializer)
     }
 
     pub fn from_config_str(
         py: Python,
         config: &str,
-    ) -> Result<Compressor, LocationError<ParseCompressorError>> {
+    ) -> Result<Self, LocationError<ParseCompressorError>> {
         Self::from_deserialised_config(py, toml::Deserializer::new(config))
             .map_err(|err| ParseCompressorError::ParseConfig { source: err })
             .map_err(LocationError::new)
     }
 
     pub fn from_config_file(
         py: Python,
         config_file: &Path,
-    ) -> Result<Compressor, LocationError<ParseCompressorError>> {
+    ) -> Result<Self, LocationError<ParseCompressorError>> {
         let config =
             fs::read_to_string(config_file).map_err(|err| ParseCompressorError::ReadFile {
                 source: err,
                 file: config_file.to_path_buf(),
             })?;
 
         serde::de::DeserializeSeed::deserialize(
@@ -127,66 +131,67 @@
     }
 
     pub fn ensure_py_imports(&self, py: Python) -> Result<(), LocationError<PyErr>> {
         let numcodecs_codec = py
             .import(intern!(py, "numcodecs.abc"))?
             .getattr(intern!(py, "Codec"))?;
 
-        for codec in &self.codecs {
+        for codec in self.codecs.values() {
             let codec = codec.import_py(py)?;
 
             if !codec.is_subclass(numcodecs_codec)? {
                 return Err(
                     PyErr::new::<PyTypeError, _>("not a subclass of numcodecs.abc.Codec").into(),
                 );
             }
         }
 
         Ok(())
     }
 
-    pub fn iter_concrete(&self) -> ConcreteCompressorIterator {
+    pub fn iter_concrete(&self) -> Result<ConcreteCompressorIterator, ParameterEvalError> {
         let codecs = self
             .codecs
-            .iter()
+            .values()
             .map(Codec::cyclic_iter_concrete)
             .collect::<Vec<_>>();
 
-        ConcreteCompressorIterator {
+        Ok(ConcreteCompressorIterator {
             compressor: self,
             codecs,
             all_done: false,
-        }
+            eval_context: ParameterEvalContext::new()?,
+        })
     }
 
     #[must_use]
     pub fn name(&self) -> &str {
         &self.name
     }
 
     #[must_use]
     pub fn config_path(&self) -> Option<&Path> {
         self.config_path.as_deref()
     }
 
     #[must_use]
     pub fn codecs(&self) -> impl ExactSizeIterator<Item = &Codec> {
-        self.codecs.iter()
+        self.codecs.values()
     }
 
     pub fn minimise(&mut self) {
-        self.codecs.iter_mut().for_each(Codec::minimise);
+        self.codecs.values_mut().for_each(Codec::minimise);
     }
 }
 
 impl fmt::Display for Compressor {
     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
         fmt.write_fmt(format_args!("{}: raw ⇄ ", self.name))?;
 
-        for codec in &self.codecs {
+        for codec in self.codecs.values() {
             fmt.write_fmt(format_args!("{codec} ⇄ "))?;
         }
 
         fmt.write_str("compressed")
     }
 }
 
@@ -221,24 +226,22 @@
 #[derive(Debug, Clone)]
 pub struct ConcreteCompressor<'a> {
     compressor: &'a Compressor,
     codecs: Vec<ConcreteCodec<'a>>,
 }
 
 impl<'a> ConcreteCompressor<'a> {
-    pub fn build_py<'py>(&self, py: Python<'py>) -> Result<&'py PyList, LocationError<PyErr>> {
-        let py_codecs = PyList::empty(py);
-
-        for codec in &self.codecs {
-            py_codecs
-                .append(codec.build_py(py)?)
-                .map_err(LocationError::new)?;
-        }
-
-        Ok(py_codecs)
+    pub fn build_py<'py>(
+        &self,
+        py: Python<'py>,
+    ) -> Result<Vec<&'py numcodecs::Codec>, LocationError<PyErr>> {
+        self.codecs
+            .iter()
+            .map(|codec| codec.build_py(py))
+            .collect::<Result<Vec<_>, _>>()
     }
 
     #[must_use]
     pub fn name(&self) -> &str {
         self.compressor.name()
     }
 
@@ -282,47 +285,53 @@
     codecs: Vec<ConcreteCodecSummary<'a>>,
 }
 
 pub struct ConcreteCompressorIterator<'a> {
     compressor: &'a Compressor,
     codecs: Vec<ConcreteCodecIterator<'a>>,
     all_done: bool,
+    eval_context: ParameterEvalContext,
 }
 
 impl<'a> Iterator for ConcreteCompressorIterator<'a> {
-    type Item = ConcreteCompressor<'a>;
+    type Item = Result<ConcreteCompressor<'a>, ParameterEvalError>;
 
     fn next(&mut self) -> Option<Self::Item> {
         if self.all_done {
             return None;
         }
 
         self.all_done = true;
+        self.eval_context.reset();
 
+        #[allow(clippy::needless_collect)]
+        // we must not short-circuit early to ensure further iteration is not broken
         let codecs = self
             .codecs
             .iter_mut()
-            .map(|codec| {
+            .map(|codec| -> Result<_, ParameterEvalError> {
                 if self.all_done {
-                    match codec.next() {
-                        ControlFlow::Break(codec) => codec,
+                    match codec.next(&mut self.eval_context)? {
+                        ControlFlow::Break(codec) => Ok(codec),
                         ControlFlow::Continue(codec) => {
                             self.all_done = false;
-                            codec
+                            Ok(codec)
                         },
                     }
                 } else {
-                    codec.get()
+                    codec.get(&mut self.eval_context)
                 }
             })
-            .collect();
+            .collect::<Vec<_>>();
 
-        Some(ConcreteCompressor {
+        let codecs = codecs.into_iter().collect::<Result<Vec<_>, _>>();
+
+        Some(codecs.map(|codecs| ConcreteCompressor {
             compressor: self.compressor,
             codecs,
-        })
+        }))
     }
 }
 
 // Correctness: all_done guarantees that None is always returned after the first
 //              `None`
 impl<'a> std::iter::FusedIterator for ConcreteCompressorIterator<'a> {}
```

### Comparing `field-compression-benchmark-0.0.1/core/compressor/src/numcodecs.rs` & `field-compression-benchmark-0.0.2/core/compressor/src/numcodecs.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/core/compressor/src/parameter/config.rs` & `field-compression-benchmark-0.0.2/core/compressor/src/parameter/config.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 use std::fmt;
 
+use evalexpr::Node;
 use nonempty::NonEmpty;
 use vecmap::VecSet;
 
-use super::Parameter;
+use super::{Parameter, ParameterEvalContext, Type};
 
-impl<'de> serde::Deserialize<'de> for Parameter {
-    fn deserialize<D: serde::Deserializer<'de>>(deserializer: D) -> Result<Self, D::Error> {
-        serde::Deserializer::deserialize_struct(deserializer, "Parameter", FIELDS, Visitor)
+pub struct ParameterSeed<'a> {
+    eval_context: &'a ParameterEvalContext,
+}
+
+impl<'a> ParameterSeed<'a> {
+    pub const fn new(eval_context: &'a ParameterEvalContext) -> Self {
+        Self { eval_context }
     }
 }
 
-const FIELDS: &[&str] = &["type", "value", "values", "min", "max"];
+impl<'a, 'de> serde::de::DeserializeSeed<'de> for ParameterSeed<'a> {
+    type Value = Parameter;
+
+    fn deserialize<D: serde::Deserializer<'de>>(
+        self,
+        deserializer: D,
+    ) -> Result<Self::Value, D::Error> {
+        serde::Deserializer::deserialize_struct(deserializer, "Parameter", FIELDS, self)
+    }
+}
+
+const FIELDS: &[&str] = &["type", "value", "valueset", "min", "max", "expr"];
 
 struct TypeField;
 
 impl<'de> serde::Deserialize<'de> for TypeField {
     fn deserialize<D: serde::Deserializer<'de>>(deserializer: D) -> Result<Self, D::Error> {
         struct Visitor;
 
@@ -49,17 +65,18 @@
         serde::Deserializer::deserialize_identifier(deserializer, Visitor)
     }
 }
 
 #[derive(Clone, Copy)]
 enum Field {
     Value,
-    Values,
+    ValueSet,
     Min,
     Max,
+    Expr,
 }
 
 struct FieldSeed<const N: usize> {
     keys: &'static [&'static str; N],
     values: &'static [Field; N],
 }
 
@@ -154,52 +171,43 @@
         }
 
         let value = String::from_utf8_lossy(value);
         Err(serde::de::Error::unknown_field(&value, self.keys))
     }
 }
 
-#[derive(serde::Serialize, serde::Deserialize)]
-#[serde(rename_all = "lowercase")]
-enum Type {
-    Int,
-    Float,
-    Str,
-}
-
-struct Visitor;
-
-impl<'de> serde::de::Visitor<'de> for Visitor {
+impl<'a, 'de> serde::de::Visitor<'de> for ParameterSeed<'a> {
     type Value = Parameter;
 
     fn expecting(&self, formatter: &mut fmt::Formatter) -> fmt::Result {
         formatter.write_str("a codec parameter")
     }
 
+    #[allow(clippy::too_many_lines)] // FIXME
     fn visit_map<A: serde::de::MapAccess<'de>>(self, mut map: A) -> Result<Self::Value, A::Error> {
         let Some(TypeField) = map.next_key()? else {
             return Err(serde::de::Error::custom("expected field `type`"));
         };
         let r#type: Type = map.next_value()?;
 
         let parameter = match r#type {
             Type::Int => FieldSeed {
-                keys: &["value", "values", "min"],
-                values: &[Field::Value, Field::Values, Field::Min],
+                keys: &["value", "valueset", "min", "expr"],
+                values: &[Field::Value, Field::ValueSet, Field::Min, Field::Expr],
             }
             .with_deserialize_key(&mut map, |map, field| match field {
                 Field::Value => Ok(Some(Parameter::IntValue {
                     value: map.next_value()?,
                 })),
-                Field::Values => {
+                Field::ValueSet => {
                     let values: VecSet<i64> = map.next_value()?;
-                    match NonEmpty::collect(values.into_iter()) {
-                        Some(values) => Ok(Some(Parameter::IntSet { values })),
-                        None => Err(serde::de::Error::custom("empty int parameter values range")),
-                    }
+                    NonEmpty::collect(values.into_iter()).map_or_else(
+                        || Err(serde::de::Error::custom("empty int parameter value set")),
+                        |values| Ok(Some(Parameter::IntSet { values })),
+                    )
                 },
                 Field::Min => {
                     let range_min: i64 = map.next_value()?;
                     FieldSeed {
                         keys: &["max"],
                         values: &[Field::Max],
                     }
@@ -213,49 +221,68 @@
                     } else {
                         Err(serde::de::Error::custom(
                             "empty int parameter min..=max range",
                         ))
                     }
                 },
                 Field::Max => Ok(None),
+                Field::Expr => Ok(Some(Parameter::Expr {
+                    ty: Type::Int,
+                    expr: map.next_value_seed(ExprSeed {
+                        ty: Type::Int,
+                        context: self.eval_context,
+                    })?,
+                })),
             }),
             Type::Float => FieldSeed {
-                keys: &["value", "values"],
-                values: &[Field::Value, Field::Values],
+                keys: &["value", "valueset", "expr"],
+                values: &[Field::Value, Field::ValueSet, Field::Expr],
             }
             .with_deserialize_key(&mut map, |map, field| match field {
                 Field::Value => Ok(Some(Parameter::FloatValue {
                     value: map.next_value()?,
                 })),
-                Field::Values => {
+                Field::ValueSet => {
                     let values: VecSet<F64> = map.next_value()?;
-                    match NonEmpty::collect(values.into_iter().map(|f| f.0)) {
-                        Some(values) => Ok(Some(Parameter::FloatSet { values })),
-                        None => Err(serde::de::Error::custom(
-                            "empty float parameter values range",
-                        )),
-                    }
+                    NonEmpty::collect(values.into_iter().map(|f| f.0)).map_or_else(
+                        || Err(serde::de::Error::custom("empty float parameter value set")),
+                        |values| Ok(Some(Parameter::FloatSet { values })),
+                    )
                 },
+                Field::Expr => Ok(Some(Parameter::Expr {
+                    ty: Type::Float,
+                    expr: map.next_value_seed(ExprSeed {
+                        ty: Type::Float,
+                        context: self.eval_context,
+                    })?,
+                })),
                 _ => Ok(None),
             }),
             Type::Str => FieldSeed {
-                keys: &["value", "values"],
-                values: &[Field::Value, Field::Values],
+                keys: &["value", "valueset", "expr"],
+                values: &[Field::Value, Field::ValueSet, Field::Expr],
             }
             .with_deserialize_key(&mut map, |map, field| match field {
                 Field::Value => Ok(Some(Parameter::StrValue {
                     value: map.next_value()?,
                 })),
-                Field::Values => {
+                Field::ValueSet => {
                     let values: VecSet<String> = map.next_value()?;
-                    match NonEmpty::collect(values.into_iter()) {
-                        Some(values) => Ok(Some(Parameter::StrSet { values })),
-                        None => Err(serde::de::Error::custom("empty str parameter values range")),
-                    }
+                    NonEmpty::collect(values.into_iter()).map_or_else(
+                        || Err(serde::de::Error::custom("empty str parameter value set")),
+                        |values| Ok(Some(Parameter::StrSet { values })),
+                    )
                 },
+                Field::Expr => Ok(Some(Parameter::Expr {
+                    ty: Type::Str,
+                    expr: map.next_value_seed(ExprSeed {
+                        ty: Type::Str,
+                        context: self.eval_context,
+                    })?,
+                })),
                 _ => Ok(None),
             }),
         }?;
 
         map.next_key_seed(FieldSeed {
             keys: &[],
             values: &[],
@@ -275,7 +302,44 @@
             std::cmp::Ordering::Equal => true,
             std::cmp::Ordering::Less | std::cmp::Ordering::Greater => false,
         }
     }
 }
 
 impl Eq for F64 {}
+
+struct ExprSeed<'a> {
+    ty: Type,
+    context: &'a ParameterEvalContext,
+}
+
+impl<'a, 'de> serde::de::DeserializeSeed<'de> for ExprSeed<'a> {
+    type Value = Node;
+
+    fn deserialize<D: serde::Deserializer<'de>>(
+        self,
+        deserializer: D,
+    ) -> Result<Self::Value, D::Error> {
+        deserializer.deserialize_str(self)
+    }
+}
+
+impl<'a, 'de> serde::de::Visitor<'de> for ExprSeed<'a> {
+    type Value = Node;
+
+    fn expecting(&self, formatter: &mut fmt::Formatter) -> fmt::Result {
+        formatter.write_str("an expression string")
+    }
+
+    fn visit_str<E: serde::de::Error>(self, v: &str) -> Result<Self::Value, E> {
+        let expr = evalexpr::build_operator_tree(v).map_err(serde::de::Error::custom)?;
+
+        match self.ty {
+            Type::Int => expr.eval_int_with_context(self.context).map(|_| ()),
+            Type::Float => expr.eval_float_with_context(self.context).map(|_| ()),
+            Type::Str => expr.eval_string_with_context(self.context).map(|_| ()),
+        }
+        .map_err(serde::de::Error::custom)?;
+
+        Ok(expr)
+    }
+}
```

### Comparing `field-compression-benchmark-0.0.1/core/dataset/Cargo.toml` & `field-compression-benchmark-0.0.2/core/dataset/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,7 +11,10 @@
 nonempty = { version = "0.10", default-features = false, features = ["serialize"] }
 pyo3 = { version = "0.20", default-features = false, features = ["macros", "abi3"] }
 serde = { version = "1.0", default-features = false, features = ["derive"] }
 sorted-vec = { version = "0.8", default-features = false }
 thiserror = { version = "1.0", default-features = false }
 toml = { version = "0.8", default-features = false, features = ["parse", "preserve_order"] }
 vecmap-rs = { version = "0.2", default-features = false, features = ["serde"] }
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/core/dataset/src/dataset/config.rs` & `field-compression-benchmark-0.0.2/core/dataset/src/dataset/config.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     py: Python<'py>,
     config_path: Option<&'a Path>,
     unit_registry: &'py UnitRegistry,
     settings: &'a DatasetSettings,
 }
 
 impl<'a, 'py> DatasetSeed<'a, 'py> {
-    pub fn new(
+    pub const fn new(
         py: Python<'py>,
         config_path: Option<&'a Path>,
         unit_registry: &'py UnitRegistry,
         settings: &'a DatasetSettings,
     ) -> Self {
         Self {
             py,
@@ -138,14 +138,15 @@
         formatter.write_str("a sequence of variables")
     }
 
     fn visit_seq<A: serde::de::SeqAccess<'de>>(
         mut self,
         mut seq: A,
     ) -> Result<Self::Value, A::Error> {
+        #[allow(clippy::equatable_if_let)]
         while let Some(()) = seq.next_element_seed(DataVariableSeed::new(
             self.py,
             self.ds,
             &mut self.variables,
             &mut self.variables_seen,
         ))? {
             // no-op
```

### Comparing `field-compression-benchmark-0.0.1/core/dataset/src/dataset/mod.rs` & `field-compression-benchmark-0.0.2/core/dataset/src/dataset/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -31,38 +31,38 @@
 
 impl Dataset {
     pub fn from_deserialised_config<'a, 'py, 'de, D: serde::Deserializer<'de>>(
         py: Python<'py>,
         deserializer: D,
         unit_registry: &'py UnitRegistry,
         settings: &DatasetSettings,
-    ) -> Result<Dataset, D::Error> {
+    ) -> Result<Self, D::Error> {
         serde::de::DeserializeSeed::deserialize(
             DatasetSeed::new(py, None, unit_registry, settings),
             deserializer,
         )
     }
 
     pub fn from_config_str<'py>(
         py: Python<'py>,
         config: &str,
         unit_registry: &'py UnitRegistry,
         settings: &DatasetSettings,
-    ) -> Result<Dataset, LocationError<ParseDatasetError>> {
+    ) -> Result<Self, LocationError<ParseDatasetError>> {
         Self::from_deserialised_config(py, toml::Deserializer::new(config), unit_registry, settings)
             .map_err(|err| ParseDatasetError::ParseConfig { source: err })
             .map_err(LocationError::new)
     }
 
     pub fn from_config_file<'py>(
         py: Python<'py>,
         config_file: &Path,
         unit_registry: &'py UnitRegistry,
         settings: &DatasetSettings,
-    ) -> Result<Dataset, LocationError<ParseDatasetError>> {
+    ) -> Result<Self, LocationError<ParseDatasetError>> {
         let config =
             fs::read_to_string(config_file).map_err(|err| ParseDatasetError::ReadFile {
                 source: err,
                 file: config_file.to_path_buf(),
             })?;
 
         serde::de::DeserializeSeed::deserialize(
@@ -132,15 +132,15 @@
 
     #[must_use]
     pub fn path(&self) -> &Path {
         &self.path
     }
 
     #[must_use]
-    pub fn format(&self) -> DatasetFormat {
+    pub const fn format(&self) -> DatasetFormat {
         self.format
     }
 
     #[must_use]
     pub fn variables(&self) -> impl ExactSizeIterator<Item = &DataVariable> {
         self.variables.values()
     }
@@ -194,35 +194,35 @@
             keep
         });
     }
 }
 
 #[allow(clippy::upper_case_acronyms)]
 #[derive(Copy, Clone, Debug, PartialEq, Eq, Hash, serde::Serialize, serde::Deserialize)]
-#[serde(rename = "lowercase")]
+#[serde(rename_all = "lowercase")]
 pub enum DatasetFormat {
     #[serde(alias = "GRIB")]
     GRIB,
     #[serde(alias = "NetCDF4", alias = "NetCDF", alias = "netcdf")]
     NetCDF4,
     #[serde(alias = "Zarr")]
     Zarr,
 }
 
 impl fmt::Display for DatasetFormat {
     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
         match self {
-            DatasetFormat::GRIB => fmt.write_str("GRIB"),
-            DatasetFormat::NetCDF4 => fmt.write_str("NetCDF4"),
-            DatasetFormat::Zarr => fmt.write_str("Zarr"),
+            Self::GRIB => fmt.write_str("GRIB"),
+            Self::NetCDF4 => fmt.write_str("NetCDF4"),
+            Self::Zarr => fmt.write_str("Zarr"),
         }
     }
 }
 
-#[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
+#[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
 #[serde(default)]
 pub struct DatasetSettings {
     pub auto_chunk_size: Byte,
 }
 
 impl Default for DatasetSettings {
```

### Comparing `field-compression-benchmark-0.0.1/core/dataset/src/units.rs` & `field-compression-benchmark-0.0.2/core/dataset/src/units.rs`

 * *Files 0% similar despite different names*

```diff
@@ -97,20 +97,20 @@
 pub struct DataUnit {
     verbose: ParsedDataUnit,
     base: ParsedDataUnit,
 }
 
 impl DataUnit {
     #[must_use]
-    pub fn verbose(&self) -> &ParsedDataUnit {
+    pub const fn verbose(&self) -> &ParsedDataUnit {
         &self.verbose
     }
 
     #[must_use]
-    pub fn base(&self) -> &ParsedDataUnit {
+    pub const fn base(&self) -> &ParsedDataUnit {
         &self.base
     }
 
     #[must_use]
     pub fn summary(&self) -> DataUnitSummary {
         DataUnitSummary {
             verbose: self.verbose.summary(),
@@ -123,14 +123,15 @@
     fn hash<H: Hasher>(&self, state: &mut H) {
         // Note: we only hash verbose representation, since the base is derived from it
         self.verbose.hash(state);
     }
 }
 
 #[derive(Debug, Clone, serde::Serialize, serde::Deserialize)]
+#[serde(rename = "DataUnit")]
 #[serde(deny_unknown_fields)]
 pub struct DataUnitSummary<'a> {
     #[serde(borrow)]
     verbose: ParsedDataUnitSummary<'a>,
     #[serde(borrow)]
     base: ParsedDataUnitSummary<'a>,
 }
@@ -140,27 +141,27 @@
     magnitude: f64,
     units: VecMap<String, f64>,
     expression: Option<UnitExpression>,
 }
 
 impl ParsedDataUnit {
     #[must_use]
-    pub fn magnitude(&self) -> f64 {
+    pub const fn magnitude(&self) -> f64 {
         self.magnitude
     }
 
     #[must_use]
     pub fn units(&self) -> impl ExactSizeIterator<Item = (&str, f64)> {
         self.units
             .iter()
             .map(|(unit, exponent)| (&**unit, *exponent))
     }
 
     #[must_use]
-    pub fn expression(&self) -> Option<&UnitExpression> {
+    pub const fn expression(&self) -> Option<&UnitExpression> {
         self.expression.as_ref()
     }
 
     #[must_use]
     pub fn summary(&self) -> ParsedDataUnitSummary {
         ParsedDataUnitSummary {
             magnitude: self.magnitude,
```

### Comparing `field-compression-benchmark-0.0.1/core/dataset/src/variable/config.rs` & `field-compression-benchmark-0.0.2/core/dataset/src/variable/config.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/core/dataset/src/variable/derivative/config.rs` & `field-compression-benchmark-0.0.2/core/dataset/src/variable/derivative/config.rs`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 pub struct DataDerivativeFormulaSetSeed<'a> {
     variable: &'a str,
     dimensions: VecSet<&'a str>,
 }
 
 impl<'a> DataDerivativeFormulaSetSeed<'a> {
-    pub fn new(variable: &'a str, dimensions: VecSet<&'a str>) -> Self {
+    pub const fn new(variable: &'a str, dimensions: VecSet<&'a str>) -> Self {
         Self {
             variable,
             dimensions,
         }
     }
 }
 
@@ -241,15 +241,15 @@
         if self.integrated_dimensions.contains(v) {
             return Err(serde::de::Error::custom(format!(
                 "{v:?} has already been integrated over for variable {:?}",
                 self.variable
             )));
         }
 
-        if let Method::Integrate = self.method {
+        if matches!(self.method, Method::Integrate) {
             self.integrated_dimensions.insert(String::from(v));
         }
 
         Ok(String::from(v))
     }
 }
```

### Comparing `field-compression-benchmark-0.0.1/core/dataset/src/variable/dimension/config/mod.rs` & `field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/config/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/core/dataset/src/variable/dimension/config/slice.rs` & `field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/config/slice.rs`

 * *Files 5% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 pub struct PerVariableDataSlice<'a, 'py> {
     variable: &'a str,
     da: &'py PyAny,
 }
 
 impl<'a, 'py> PerVariableDataSlice<'a, 'py> {
     #[must_use]
-    pub fn new(variable: &'a str, da: &'py PyAny) -> Self {
+    pub const fn new(variable: &'a str, da: &'py PyAny) -> Self {
         Self { variable, da }
     }
 }
 
 pub struct DataSliceSeed<'b, 'a, 'py> {
     py: Python<'py>,
     dimension: &'a str,
     per_variable: &'b [PerVariableDataSlice<'a, 'py>],
 }
 
 impl<'b, 'a, 'py> DataSliceSeed<'b, 'a, 'py> {
     #[must_use]
-    pub fn new(
+    pub const fn new(
         py: Python<'py>,
         dimension: &'a str,
         per_variable: &'b [PerVariableDataSlice<'a, 'py>],
     ) -> Self {
         Self {
             py,
             dimension,
@@ -44,21 +44,21 @@
         self,
         deserializer: D,
     ) -> Result<Self::Value, D::Error> {
         serde::Deserializer::deserialize_struct(deserializer, "DataDimension", FIELDS, self)
     }
 }
 
-const FIELDS: &[&str] = &["type", "value", "index", "values", "reduce"];
+const FIELDS: &[&str] = &["type", "value", "index", "valueset", "reduce"];
 
 #[derive(Clone, Copy)]
 enum Field {
     Type,
     Index,
-    Values,
+    ValueSet,
 }
 
 impl<'de> serde::de::Deserialize<'de> for Field {
     fn deserialize<D: serde::Deserializer<'de>>(deserializer: D) -> Result<Self, D::Error> {
         serde::Deserializer::deserialize_identifier(deserializer, FieldVisitor)
     }
 }
@@ -72,32 +72,32 @@
         formatter.write_str("a data dimension field identifier")
     }
 
     fn visit_str<E: serde::de::Error>(self, value: &str) -> Result<Self::Value, E> {
         match value {
             "type" => Ok(Field::Type),
             "index" => Ok(Field::Index),
-            "values" => Ok(Field::Values),
+            "valueset" => Ok(Field::ValueSet),
             _ => Err(serde::de::Error::custom(format!(
                 "unexpected field `{value}`, a data dimension must start with either a `type`, \
-                 `index`, or `values` field"
+                 `index`, or `valueset` field"
             ))),
         }
     }
 
     fn visit_bytes<E: serde::de::Error>(self, value: &[u8]) -> Result<Self::Value, E> {
         match value {
             b"type" => Ok(Field::Type),
             b"index" => Ok(Field::Index),
-            b"values" => Ok(Field::Values),
+            b"valueset" => Ok(Field::ValueSet),
             _ => {
                 let value = String::from_utf8_lossy(value);
                 Err(serde::de::Error::custom(format!(
                     "unexpected field `{value}`, a data dimension must start with either a \
-                     `type`, `index`, or `values` field"
+                     `type`, `index`, or `valueset` field"
                 )))
             },
         }
     }
 }
 
 #[derive(Clone, Copy)]
@@ -168,15 +168,15 @@
 pub enum Type {
     Int,
     Float,
 }
 
 #[derive(Debug, serde::Serialize, serde::Deserialize)]
 #[serde(rename_all = "lowercase")]
-pub enum Values {
+pub enum ValueSet {
     All,
 }
 
 struct DataSliceValueSeed<'b, 'a, 'py, T: Copy + serde::de::DeserializeOwned + IntoPy<Py<PyAny>>> {
     py: Python<'py>,
     dimension: &'a str,
     ty: PhantomData<T>,
@@ -225,15 +225,15 @@
         formatter.write_str("a data dimension")
     }
 
     fn visit_map<A: serde::de::MapAccess<'de>>(self, mut map: A) -> Result<Self::Value, A::Error> {
         let Some(identifier) = map.next_key()? else {
             return Err(serde::de::Error::custom(
                 "missing field, a data dimension must start with either a `type`, `index`, or \
-                 `values` field",
+                 `valueset` field",
             ));
         };
 
         let slice = match identifier {
             Field::Type => {
                 let r#type = map.next_value()?;
 
@@ -267,16 +267,16 @@
                     py: self.py,
                     dimension: self.dimension,
                     ty: PhantomData::<isize>,
                     is_index: true,
                     per_variable: self.per_variable,
                 })?,
             },
-            Field::Values => {
-                let Values::All = map.next_value()?;
+            Field::ValueSet => {
+                let ValueSet::All = map.next_value()?;
 
                 let reduce = match map.next_key_seed(ExtraField::Reduce)? {
                     Some(()) => map.next_value()?,
                     None => false,
                 };
 
                 DataSlice::All { reduce }
```

### Comparing `field-compression-benchmark-0.0.1/core/dataset/src/variable/mod.rs` & `field-compression-benchmark-0.0.2/core/dataset/src/variable/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             {
                 let (name, size) = dimension?.extract()?;
                 dimensions.insert(name, DataDimension::with_size(size));
             }
 
             variables.insert(
                 name.clone(),
-                DataVariable {
+                Self {
                     name,
                     long_name,
                     units,
                     dtype,
                     dimensions,
                     derivatives: SortedSet::new(),
                 },
@@ -93,20 +93,20 @@
 
     #[must_use]
     pub fn long_name(&self) -> Option<&str> {
         self.long_name.as_deref()
     }
 
     #[must_use]
-    pub fn units(&self) -> Option<&DataUnit> {
+    pub const fn units(&self) -> Option<&DataUnit> {
         self.units.as_ref()
     }
 
     #[must_use]
-    pub fn dtype(&self) -> DataDType {
+    pub const fn dtype(&self) -> DataDType {
         self.dtype
     }
 
     pub fn dimensions(&self) -> impl Iterator<Item = (&str, &DataDimension)> {
         self.dimensions
             .iter()
             .map(|(name, dimension)| (name.as_str(), dimension))
@@ -130,15 +130,15 @@
                 .filter_map(DataDimension::iter_reductions)
                 .collect(),
             all_done: false,
         }
     }
 
     #[must_use]
-    pub fn derivatives(&self) -> &SortedSet<NonEmpty<DataDerivative>> {
+    pub const fn derivatives(&self) -> &SortedSet<NonEmpty<DataDerivative>> {
         &self.derivatives
     }
 
     pub fn minimise(&mut self, dimensions: bool, derivatives: bool) {
         if dimensions {
             self.dimensions
                 .values_mut()
```

### Comparing `field-compression-benchmark-0.0.1/core/error/src/lib.rs` & `field-compression-benchmark-0.0.2/core/error/src/lib.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 use std::{borrow::Cow, error::Error, fmt};
 
+use serde_name::{DeserializeNameAdapter, SerializeNameAdapter};
+
 #[derive(
     Debug, Clone, PartialEq, Eq, PartialOrd, Ord, Hash, serde::Serialize, serde::Deserialize,
 )]
 pub struct Location {
     file: Cow<'static, str>,
     line: u32,
     column: u32,
@@ -55,30 +57,30 @@
     pub fn from2<E2: Into<E>>(error: E2) -> Self {
         Self::new(error.into())
     }
 }
 
 impl<E: Error> LocationError<E> {
     #[must_use]
-    pub fn error(&self) -> &E {
+    pub const fn error(&self) -> &E {
         &self.inner.error
     }
 
     #[must_use]
     pub fn error_mut(&mut self) -> &mut E {
         &mut self.inner.error
     }
 
     #[must_use]
     pub fn into_error(self) -> E {
         self.inner.error
     }
 
     #[must_use]
-    pub fn location(&self) -> &Location {
+    pub const fn location(&self) -> &Location {
         &self.inner.location
     }
 
     #[must_use]
     pub fn map<F: Error>(self, map: impl FnOnce(E) -> F) -> LocationError<F> {
         LocationError {
             inner: Box::new(LocationErrorInner {
@@ -132,11 +134,31 @@
     fn source(&self) -> Option<&(dyn Error + 'static)> {
         self.inner.error.source()
     }
 }
 
 #[derive(Clone, PartialEq, Eq, PartialOrd, Ord, Hash, serde::Serialize, serde::Deserialize)]
 #[serde(rename = "LocationError")]
+#[serde(remote = "LocationErrorInner")]
 struct LocationErrorInner<E: Error> {
     error: E,
     location: Location,
 }
+
+// FIXME: don't generate overly specific names
+impl<E: Error + serde::Serialize> serde::Serialize for LocationErrorInner<E> {
+    fn serialize<S: serde::Serializer>(&self, serializer: S) -> Result<S::Ok, S::Error> {
+        Self::serialize(
+            self,
+            SerializeNameAdapter::new(serializer, std::any::type_name::<Self>()),
+        )
+    }
+}
+
+impl<'de, E: Error + serde::Deserialize<'de>> serde::Deserialize<'de> for LocationErrorInner<E> {
+    fn deserialize<D: serde::Deserializer<'de>>(deserializer: D) -> Result<Self, D::Error> {
+        Self::deserialize(DeserializeNameAdapter::new(
+            deserializer,
+            std::any::type_name::<Self>(),
+        ))
+    }
+}
```

### Comparing `field-compression-benchmark-0.0.1/core/goodness/Cargo.toml` & `field-compression-benchmark-0.0.2/core/goodness/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,7 +9,10 @@
 core-error = { path = "../error", default-features = false }
 core-measure = { path = "../measure", default-features = false }
 crunchy = { version = "0.2", default-features = false }
 numpy = { version = "0.20", default-features = false }
 puruspe = { version = "0.2", default-features = false }
 pyo3 = { version = "0.20", default-features = false, features = ["abi3"] }
 serde = { version = "1.0", default-features = false, features = ["derive"] }
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/core/goodness/src/bit_information.rs` & `field-compression-benchmark-0.0.2/core/goodness/src/bit_information.rs`

 * *Files 2% similar despite different names*

```diff
@@ -232,44 +232,45 @@
             }
         }
     }
 
     fn binom_free_binary_entropy(n: usize, confidence: f64) -> f64 {
         let p = Self::binom_confidence(n, confidence);
 
-        let binary_entropy = -(p * p.log2() + (1.0 - p) * (1.0 - p).log2());
+        let binary_entropy = -p.mul_add(p.log2(), (1.0 - p) * (1.0 - p).log2());
 
         1.0 - binary_entropy
     }
 
     fn binom_confidence(n: usize, confidence: f64) -> f64 {
         #[allow(clippy::cast_precision_loss)]
         let n = n as f64;
 
-        let p =
-            0.5 + Self::standard_normal_quantile(1.0 - (1.0 - confidence) * 0.5) / (n.sqrt() * 2.0);
+        let p = 0.5
+            + Self::standard_normal_quantile((1.0 - confidence).mul_add(-0.5, 1.0))
+                / (n.sqrt() * 2.0);
 
         // cap probability at 1 (only important for when n is small)
         p.min(1.0_f64)
     }
 
     fn standard_normal_quantile(p: f64) -> f64 {
-        std::f64::consts::SQRT_2 * puruspe::inverf(p * 2.0 - 1.0)
+        std::f64::consts::SQRT_2 * puruspe::inverf(p.mul_add(2.0, -1.0))
     }
 }
 
 #[derive(Copy, Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
 pub struct BitInformationGoodness {
     information_content_ratio: f64,
 }
 
 impl BitInformationGoodness {
     #[must_use]
-    pub fn new(information_content_ratio: f64) -> Self {
+    pub const fn new(information_content_ratio: f64) -> Self {
         Self {
             information_content_ratio,
         }
     }
 }
 
 impl Measurement for BitInformationGoodness {
@@ -386,14 +387,15 @@
             .zip(b.iter())
             .all(|(a, b)| (a - b).abs() <= f64::EPSILON);
 
         assert!(close, "{a:?} != {b:?}");
     }
 
     #[test]
+    #[allow(clippy::cognitive_complexity)]
     fn bit_information_u32() {
         assert_close(
             DataArrayBitInformation::bit_information_slice(&[0_u32, 0], false, 0.99),
             [0.0_f64; 32],
         );
 
         assert_close(
@@ -409,14 +411,15 @@
                 } }
                 bit_information
             },
         );
     }
 
     #[test]
+    #[allow(clippy::cognitive_complexity)]
     fn bit_information_u64() {
         assert_close(
             DataArrayBitInformation::bit_information_slice(&[0_u64, 0], false, 0.99),
             [0.0_f64; 64],
         );
 
         assert_close(
```

### Comparing `field-compression-benchmark-0.0.1/core/goodness/src/correlation.rs` & `field-compression-benchmark-0.0.2/core/goodness/src/correlation.rs`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 #[serde(deny_unknown_fields)]
 pub struct CompressionCorrelationGoodness {
     abs_correlation: f64,
 }
 
 impl CompressionCorrelationGoodness {
     #[must_use]
-    pub fn new(abs_correlation: f64) -> Self {
+    pub const fn new(abs_correlation: f64) -> Self {
         Self { abs_correlation }
     }
 }
 
 impl Measurement for CompressionCorrelationGoodness {
     type Error = Infallible;
```

### Comparing `field-compression-benchmark-0.0.1/core/goodness/src/error.rs` & `field-compression-benchmark-0.0.2/core/goodness/src/error.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/core/goodness/src/lib.rs` & `field-compression-benchmark-0.0.2/core/goodness/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
-#![allow(clippy::module_name_repetitions)]
 #![allow(clippy::missing_errors_doc)] // FIXME
 
 #[macro_use]
 extern crate crunchy;
 
 use std::{convert::Infallible, num::NonZeroUsize};
 
@@ -122,15 +112,14 @@
         percentiles: [f64; N],
     ) -> Result<[f64; N], LocationError<PyErr>> {
         self.approximate_quantiles_tuple(self.da.py(), &percentiles)?
             .extract()
             .map_err(LocationError::new)
     }
 
-    #[allow(unused)] // FIXME
     pub fn summarise(&self) -> Result<ConfidenceInterval<f64>, LocationError<PyErr>> {
         let [p2_5, p15_9, p50, p84_1, p97_5] =
             self.approximate_quantiles([0.025, 0.159, 0.5, 0.841, 0.975])?;
 
         Ok(ConfidenceInterval {
             p2_5,
             p15_9,
```

### Comparing `field-compression-benchmark-0.0.1/core/goodness/src/pca.rs` & `field-compression-benchmark-0.0.2/core/goodness/src/pca.rs`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 #[serde(deny_unknown_fields)]
 pub struct PreservedPCAGoodness {
     abs_correlation_sum_fraction: f64,
 }
 
 impl PreservedPCAGoodness {
     #[must_use]
-    pub fn new(abs_correlation_sum_fraction: f64) -> Self {
+    pub const fn new(abs_correlation_sum_fraction: f64) -> Self {
         Self {
             abs_correlation_sum_fraction,
         }
     }
 }
 
 impl Measurement for PreservedPCAGoodness {
```

### Comparing `field-compression-benchmark-0.0.1/core/goodness/src/uniformity.rs` & `field-compression-benchmark-0.0.2/core/goodness/src/uniformity.rs`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 #[serde(deny_unknown_fields)]
 pub struct CompressionUniformityGoodness {
     uniformity: f64,
 }
 
 impl CompressionUniformityGoodness {
     #[must_use]
-    pub fn new(uniformity: f64) -> Self {
+    pub const fn new(uniformity: f64) -> Self {
         Self { uniformity }
     }
 }
 
 impl Measurement for CompressionUniformityGoodness {
     type Error = Infallible;
```

### Comparing `field-compression-benchmark-0.0.1/core/measure/Cargo.toml` & `field-compression-benchmark-0.0.2/core/measure/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,8 +6,12 @@
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 core-error = { path = "../error", default-features = false }
 human_bytes = { version = "0.4", default-features = false, features = ["si-units"] }
 rand = { version = "0.8", default-features = false }
 serde = { version = "1.0", default-features = false, features = ["derive"] }
+serde-name = { version = "0.2", default-features = false }
 thiserror = { version = "1.0", default-features = false }
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/core/measure/src/lib.rs` & `field-compression-benchmark-0.0.2/core/measure/src/lib.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
-#![allow(clippy::module_name_repetitions)]
 #![allow(clippy::missing_errors_doc)] // FIXME
 
 use std::{error::Error, fmt};
 
 use core_error::LocationError;
 
 pub mod measurement;
```

### Comparing `field-compression-benchmark-0.0.1/core/measure/src/measurement.rs` & `field-compression-benchmark-0.0.2/core/measure/src/measurement.rs`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             Self {
                 throughput: (decoded_bytes as f64) / timing.as_secs_f64(),
             }
         }
     }
 
     #[must_use]
-    pub fn zero() -> Self {
+    pub const fn zero() -> Self {
         Self { throughput: 0.0 }
     }
 }
 
 impl Measurement for ThroughputPerSecond {
     type Error = Infallible;
 
@@ -178,15 +178,15 @@
         fmt.write_str(&human_bytes::human_bytes(self.bytes))
     }
 }
 
 impl From<usize> for Bytes {
     fn from(bytes: usize) -> Self {
         #[allow(clippy::cast_precision_loss)]
-        Bytes {
+        Self {
             bytes: bytes as f64,
         }
     }
 }
 
 #[derive(Copy, Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
@@ -204,15 +204,15 @@
             Self {
                 ratio: (decoded_bytes as f64) / (encoded_bytes as f64),
             }
         }
     }
 
     #[must_use]
-    pub fn unchanged() -> Self {
+    pub const fn unchanged() -> Self {
         Self { ratio: 1.0 }
     }
 }
 
 impl Measurement for CompressionRatio {
     type Error = Infallible;
 
@@ -245,29 +245,31 @@
     }
 
     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
         fmt.write_fmt(format_args!("{self}"))
     }
 }
 
-#[derive(Debug, Copy, Clone, PartialEq)]
+#[derive(Debug, Copy, Clone, PartialEq, Eq)]
 pub enum AnyMeasurement {}
 
 impl Measurement for AnyMeasurement {
     type Error = AnyError;
 
     fn to_f64(&self) -> f64 {
+        #[allow(clippy::uninhabited_references)] // FIXME
         match *self {}
     }
 
     fn try_from_f64(_v: f64) -> Result<Self, LocationError<Self::Error>> {
         Err(AnyError("cannot construct any measurement".into()).into())
     }
 
     fn fmt(&self, _fmt: &mut fmt::Formatter) -> fmt::Result {
+        #[allow(clippy::uninhabited_references)] // FIXME
         match *self {}
     }
 }
 
 #[derive(Debug, thiserror::Error)]
 #[error(transparent)]
 pub struct AnyError(Box<dyn 'static + std::error::Error>);
```

### Comparing `field-compression-benchmark-0.0.1/core/measure/src/stats.rs` & `field-compression-benchmark-0.0.2/core/measure/src/stats.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,47 @@
 use std::{fmt, num::NonZeroUsize};
 
 use rand::{distributions::Slice, Rng};
+use serde_name::{DeserializeNameAdapter, SerializeNameAdapter};
 use thiserror::Error;
 
 use core_error::LocationError;
 
 use crate::{
     measurement::{AnyError, AnyMeasurement},
     Measurement,
 };
 
 #[derive(Debug, Clone, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
+#[serde(remote = "BenchmarkStats")]
 pub struct BenchmarkStats<T: Measurement> {
     pub mean: ConfidenceInterval<T>,
     pub median: ConfidenceInterval<T>,
 }
 
+// FIXME: don't generate overly specific names
+impl<T: Measurement + serde::Serialize> serde::Serialize for BenchmarkStats<T> {
+    fn serialize<S: serde::Serializer>(&self, serializer: S) -> Result<S::Ok, S::Error> {
+        Self::serialize(
+            self,
+            SerializeNameAdapter::new(serializer, std::any::type_name::<Self>()),
+        )
+    }
+}
+
+impl<'de, T: Measurement + serde::Deserialize<'de>> serde::Deserialize<'de> for BenchmarkStats<T> {
+    fn deserialize<D: serde::Deserializer<'de>>(deserializer: D) -> Result<Self, D::Error> {
+        Self::deserialize(DeserializeNameAdapter::new(
+            deserializer,
+            std::any::type_name::<Self>(),
+        ))
+    }
+}
+
 impl<T: Measurement> BenchmarkStats<T> {
     pub fn try_from_bootstrap_analysis(
         samples: &[T],
         rng: &mut impl Rng,
         bootstrap_samples: Option<NonZeroUsize>,
     ) -> Result<Self, LocationError<AnalysisError<AnyMeasurement>>> {
         Self::try_from_bootstrap_analysis_explicit_error(samples, rng, bootstrap_samples)
@@ -120,25 +141,47 @@
 
         Ok(())
     }
 }
 
 #[derive(Debug, Clone, serde::Serialize, serde::Deserialize)]
 #[serde(deny_unknown_fields)]
+#[serde(remote = "ConfidenceInterval")]
 pub struct ConfidenceInterval<T: Measurement> {
     pub p2_5: T,
     pub p15_9: T,
     pub p50: T,
     pub p84_1: T,
     pub p97_5: T,
 }
 
+// FIXME: don't generate overly specific names
+impl<T: Measurement + serde::Serialize> serde::Serialize for ConfidenceInterval<T> {
+    fn serialize<S: serde::Serializer>(&self, serializer: S) -> Result<S::Ok, S::Error> {
+        Self::serialize(
+            self,
+            SerializeNameAdapter::new(serializer, std::any::type_name::<Self>()),
+        )
+    }
+}
+
+impl<'de, T: Measurement + serde::Deserialize<'de>> serde::Deserialize<'de>
+    for ConfidenceInterval<T>
+{
+    fn deserialize<D: serde::Deserializer<'de>>(deserializer: D) -> Result<Self, D::Error> {
+        Self::deserialize(DeserializeNameAdapter::new(
+            deserializer,
+            std::any::type_name::<Self>(),
+        ))
+    }
+}
+
 impl<T: Measurement> ConfidenceInterval<T> {
     #[must_use]
-    pub fn from_const(v: T) -> Self {
+    pub const fn from_const(v: T) -> Self {
         Self {
             p2_5: v,
             p15_9: v,
             p50: v,
             p84_1: v,
             p97_5: v,
         }
```

### Comparing `field-compression-benchmark-0.0.1/core/model/src/boundary/periodic.rs` & `field-compression-benchmark-0.0.2/core/model/src/boundary/periodic.rs`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
                 .map(|_| SliceInfoElem::from(..))
                 .collect::<Vec<_>>();
             let mut right_slice = shape
                 .iter()
                 .map(|_| SliceInfoElem::from(..))
                 .collect::<Vec<_>>();
 
+            #[allow(clippy::indexing_slicing, clippy::unwrap_used)] // FIXME
             for (i, len) in shape.iter().copied().enumerate() {
                 left_slice[i] = SliceInfoElem::from(0..N);
                 right_slice[i] = SliceInfoElem::from((len - 2 * N)..(len - N));
 
                 let left = SliceInfo::try_from(&left_slice[..]).unwrap();
                 let right = SliceInfo::try_from(&right_slice[..]).unwrap();
```

### Comparing `field-compression-benchmark-0.0.1/core/model/src/boundary/zero.rs` & `field-compression-benchmark-0.0.2/core/model/src/boundary/zero.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/core/model/src/model/linadv.rs` & `field-compression-benchmark-0.0.2/core/model/src/model/linadv.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,80 @@
-use ndarray::{Array, Array1, ArrayView, ArrayViewMut, Ix1, NdFloat};
+use ndarray::{s, Array, Array1, ArrayView, ArrayViewMut, Ix1, NdFloat};
 
 use crate::{model::Model, num::two};
 
 pub struct Linadv<F: NdFloat> {
     parameters: LinadvParameters<F>,
     h_m: Array1<F>,
 }
 
 impl<F: NdFloat> Linadv<F> {
     #[must_use]
-    pub const fn new(parameters: LinadvParameters<F>, h_m: Array1<F>) -> Self {
-        Self { parameters, h_m }
+    pub fn new(parameters: LinadvParameters<F>) -> Self {
+        Self {
+            parameters,
+            h_m: Array1::zeros((parameters.x_dim,)),
+        }
     }
 
     #[must_use]
     pub const fn parameters(&self) -> &LinadvParameters<F> {
         &self.parameters
     }
 }
 
 impl<F: NdFloat> Model for Linadv<F> {
     type Dimension = Ix1;
     type Dtype = F;
     type Ext = ();
     type State = Array<F, Ix1>;
 
+    fn variables(&self) -> impl Iterator<Item = &'static str> {
+        ["h_m"].into_iter()
+    }
+
     fn state(&self) -> ArrayView<Self::Dtype, Self::Dimension> {
         self.h_m.view()
     }
 
     fn state_mut(&mut self) -> ArrayViewMut<Self::Dtype, Self::Dimension> {
         self.h_m.view_mut()
     }
 
     fn tendencies_for_state(
         &self,
         state: ArrayView<Self::Dtype, Self::Dimension>,
         _ext: &mut Self::Ext,
     ) -> Array<Self::Dtype, Self::Dimension> {
-        let h_m = state;
+        let LinadvParameters {
+            x_dim: _,
+            dx_m,
+            U_const_m_s,
+        } = self.parameters;
 
-        let LinadvParameters { dx_m, U_const_m_s } = self.parameters;
-
-        let mut h_tend_m_s = Array1::<F>::zeros([h_m.len()]);
+        let h_m = state;
 
-        for ((h_tend_m_s_i, h_m_ip1), h_m_im1) in h_tend_m_s
-            .iter_mut()
-            .skip(1)
-            .zip(h_m.iter().skip(2).copied())
-            .zip(h_m.iter().copied())
-        {
-            *h_tend_m_s_i = -U_const_m_s * (h_m_ip1 - h_m_im1) / (dx_m * two());
-        }
+        // Calculate the initial tendency of the height variable
+        let mut h_tend_m_s = Array1::zeros(state.dim());
+        #[allow(clippy::reversed_empty_ranges)]
+        h_tend_m_s.slice_mut(s![1..-1]).assign(
+            &-((h_m.slice(s![2..]).to_owned() - h_m.slice(s![..-2])) * U_const_m_s
+                / (dx_m * two())),
+        );
 
         h_tend_m_s
     }
 
     fn with_state(&self, h_m: Array<Self::Dtype, Self::Dimension>) -> Self {
-        Self::new(self.parameters, h_m)
+        let mut model = Self::new(self.parameters);
+        model.h_m.view_mut().assign(&h_m);
+        model
     }
 }
 
 #[derive(Clone, Copy, serde::Serialize, serde::Deserialize)]
 #[allow(non_snake_case)]
 pub struct LinadvParameters<F: NdFloat> {
+    pub x_dim: usize,
     pub dx_m: F,
     pub U_const_m_s: F,
 }
```

### Comparing `field-compression-benchmark-0.0.1/core/model/src/model/lorenz_63.rs` & `field-compression-benchmark-0.0.2/core/model/src/model/lorenz_63.rs`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 pub struct Lorenz63<F: NdFloat> {
     parameters: Lorenz63Parameters<F>,
     state: [F; 3],
 }
 
 impl<F: NdFloat> Lorenz63<F> {
     #[must_use]
-    pub const fn new(parameters: Lorenz63Parameters<F>, state: [F; 3]) -> Self {
+    pub fn new(parameters: Lorenz63Parameters<F>) -> Self {
+        Self::new_with(parameters, [F::zero(); 3])
+    }
+
+    #[must_use]
+    pub const fn new_with(parameters: Lorenz63Parameters<F>, state: [F; 3]) -> Self {
         Self { parameters, state }
     }
 
     #[must_use]
     pub const fn parameters(&self) -> &Lorenz63Parameters<F> {
         &self.parameters
     }
@@ -21,43 +26,48 @@
 
 impl<F: NdFloat> Model for Lorenz63<F> {
     type Dimension = Ix1;
     type Dtype = F;
     type Ext = ();
     type State = Array<F, Ix1>;
 
+    fn variables(&self) -> impl Iterator<Item = &'static str> {
+        ["x123"].into_iter()
+    }
+
     fn state(&self) -> ArrayView<Self::Dtype, Self::Dimension> {
         ArrayView::from(&self.state)
     }
 
     fn state_mut(&mut self) -> ArrayViewMut<Self::Dtype, Self::Dimension> {
         ArrayViewMut::from(&mut self.state)
     }
 
     fn tendencies_for_state(
         &self,
         state: ArrayView<Self::Dtype, Self::Dimension>,
         _ext: &mut Self::Ext,
     ) -> Array<Self::Dtype, Self::Dimension> {
-        let mut new_state @ [x1, x2, x3] = [F::zero(); 3];
+        let mut new_state = [F::zero(); 3];
         ArrayViewMut::from(&mut new_state).assign(&state);
+        let [x1, x2, x3] = new_state;
 
         let Lorenz63Parameters { sigma, rho, beta } = self.parameters;
 
         array![
             sigma * (x2 - x1),
             x1 * (rho - x3) - x2,
             (x1 * x2) - (beta * x3),
         ]
     }
 
     fn with_state(&self, state: Array<Self::Dtype, Self::Dimension>) -> Self {
-        let mut new_state = [F::zero(); 3];
-        ArrayViewMut::from(&mut new_state).assign(&state);
-        Self::new(self.parameters, new_state)
+        let mut model = Self::new(self.parameters);
+        ArrayViewMut::from(&mut model.state).assign(&state);
+        model
     }
 }
 
 #[derive(Clone, Copy, serde::Serialize, serde::Deserialize)]
 pub struct Lorenz63Parameters<F: NdFloat> {
     pub sigma: F,
     pub rho: F,
```

### Comparing `field-compression-benchmark-0.0.1/core/model/src/model/lorenz_96.rs` & `field-compression-benchmark-0.0.2/core/model/src/model/lorenz_96.rs`

 * *Files 24% similar despite different names*

```diff
@@ -9,102 +9,164 @@
 pub struct Lorenz96<F: NdFloat, S: ForcingSampler<Dtype = F>> {
     parameters: Lorenz96Parameters<F, S>,
     state: Array1<F>,
 }
 
 impl<F: NdFloat, S: ForcingSampler<Dtype = F>> Lorenz96<F, S> {
     #[must_use]
-    pub const fn new(parameters: Lorenz96Parameters<F, S>, state: Array1<F>) -> Self {
-        // TODO: validate shape >= 4
-        Self { parameters, state }
+    pub fn new(parameters: Lorenz96Parameters<F, S>) -> Self {
+        let k = parameters.k;
+        Self {
+            parameters,
+            state: Array1::zeros((k.get(),)),
+        }
     }
 
     #[must_use]
     pub const fn parameters(&self) -> &Lorenz96Parameters<F, S> {
         &self.parameters
     }
 }
 
 impl<F: NdFloat, S: ForcingSampler<Dtype = F>> Model for Lorenz96<F, S> {
     type Dimension = Ix1;
     type Dtype = F;
     type Ext = S::Ext;
     type State = Array<F, Ix1>;
 
+    fn variables(&self) -> impl Iterator<Item = &'static str> {
+        ["X_k"].into_iter()
+    }
+
     fn state(&self) -> ArrayView<Self::Dtype, Self::Dimension> {
         self.state.view()
     }
 
     fn state_mut(&mut self) -> ArrayViewMut<Self::Dtype, Self::Dimension> {
         self.state.view_mut()
     }
 
     fn tendencies_for_state(
         &self,
         state: ArrayView<Self::Dtype, Self::Dimension>,
         ext: &mut Self::Ext,
     ) -> Array<Self::Dtype, Self::Dimension> {
-        let Lorenz96Parameters { forcing } = &self.parameters;
+        let Lorenz96Parameters { k: _, forcing } = &self.parameters;
 
-        let mut tendencies = state.to_owned();
+        let mut tendencies = Array1::zeros(state.dim());
 
         for (((x_k, &x_kp1), &x_km1), &x_km2) in tendencies
             .iter_mut()
             .zip(state.iter().cycle().skip(1))
-            .zip(
-                state.iter().cycle().skip(state.len() - 1), // FIXME
-            )
-            .zip(
-                state.iter().cycle().skip(state.len() - 2), // FIXME
-            )
+            .zip(state.iter().cycle().skip(state.len() - 1))
+            .zip(state.iter().cycle().skip(state.len() - 2))
         {
             *x_k = -x_km2 * x_km1 + x_km1 * x_kp1 - (*x_k) + forcing.sample(ext);
         }
 
         tendencies
     }
 
     fn with_state(&self, state: Array<Self::Dtype, Self::Dimension>) -> Self {
-        Self::new(self.parameters.clone(), state)
+        let mut model = Self::new(self.parameters.clone());
+        model.state.view_mut().assign(&state);
+        model
     }
 }
 
 #[derive(Clone, Copy, serde::Serialize, serde::Deserialize)]
 pub struct Lorenz96Parameters<F: NdFloat, S: ForcingSampler<Dtype = F>> {
+    pub k: K,
     pub forcing: S,
 }
 
+#[derive(
+    Clone, Copy, PartialEq, Eq, PartialOrd, Ord, Hash, serde::Serialize, serde::Deserialize,
+)]
+#[serde(try_from = "usize", into = "usize")]
+pub struct K(usize);
+
+impl K {
+    pub const MIN: Self = Self(4);
+
+    #[must_use]
+    pub const fn new(x: usize) -> Option<Self> {
+        if x >= 4 {
+            Some(Self(x))
+        } else {
+            None
+        }
+    }
+
+    #[must_use]
+    pub const fn get(&self) -> usize {
+        self.0
+    }
+}
+
+impl From<K> for usize {
+    fn from(value: K) -> Self {
+        value.get()
+    }
+}
+
+impl TryFrom<usize> for K {
+    type Error = &'static str;
+
+    fn try_from(value: usize) -> Result<Self, Self::Error> {
+        Self::new(value).ok_or("k must be >= 4")
+    }
+}
+
 pub trait ForcingSampler: Clone {
     type Dtype: NdFloat;
-    type Ext: ?Sized;
+    type Ext;
 
     fn sample(&self, ext: &mut Self::Ext) -> Self::Dtype;
 }
 
 #[derive(Clone, Copy, serde::Serialize, serde::Deserialize)]
 pub struct Const<F: NdFloat> {
     r#const: F,
 }
 
-#[derive(Clone, Copy, serde::Serialize, serde::Deserialize)]
-pub struct Distr<F: NdFloat, D: Distribution<F> + Clone> {
-    distr: D,
-    _marker: PhantomData<F>,
+impl<F: NdFloat> Const<F> {
+    #[must_use]
+    pub const fn new(r#const: F) -> Self {
+        Self { r#const }
+    }
 }
 
 impl<F: NdFloat> ForcingSampler for Const<F> {
     type Dtype = F;
     type Ext = ();
 
     fn sample(&self, _ext: &mut Self::Ext) -> Self::Dtype {
         self.r#const
     }
 }
 
+#[derive(Clone, Copy, serde::Serialize, serde::Deserialize)]
+pub struct Distr<F: NdFloat, D: Distribution<F> + Clone> {
+    distr: D,
+    #[serde(skip)]
+    _marker: PhantomData<F>,
+}
+
+impl<F: NdFloat, D: Distribution<F> + Clone> Distr<F, D> {
+    #[must_use]
+    pub const fn new(distr: D) -> Self {
+        Self {
+            distr,
+            _marker: PhantomData::<F>,
+        }
+    }
+}
+
 impl<F: NdFloat, D: Distribution<F> + Clone> ForcingSampler for Distr<F, D> {
     type Dtype = F;
-    type Ext = dyn RngCore;
+    type Ext = Box<dyn 'static + RngCore + Send + Sync>;
 
     fn sample(&self, ext: &mut Self::Ext) -> Self::Dtype {
-        self.distr.sample(ext)
+        self.distr.sample(&mut **ext)
     }
 }
```

### Comparing `field-compression-benchmark-0.0.1/core/model/src/model/mod.rs` & `field-compression-benchmark-0.0.2/core/model/src/model/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 use ndarray::{Array, ArrayView, ArrayViewMut, Dimension, NdFloat};
 
+pub mod any;
 pub mod linadv;
 pub mod lorenz_63;
 pub mod lorenz_96;
+pub mod onedsw;
+pub mod twodsw;
 
 pub trait Model {
     type Dtype: NdFloat;
     type Dimension: Dimension;
     type State: State<Dtype = Self::Dtype, Dimension = Self::Dimension>;
-    type Ext: ?Sized;
+    type Ext;
+
+    fn variables(&self) -> impl Iterator<Item = &'static str>;
 
     fn state(&self) -> <Self::State as State>::View<'_>;
     fn state_mut(&mut self) -> <Self::State as State>::ViewMut<'_>;
 
     #[must_use]
     fn tendencies(&self, ext: &mut Self::Ext) -> Self::State {
         self.tendencies_for_state(self.state(), ext)
```

### Comparing `field-compression-benchmark-0.0.1/core/model/src/timestep/euler_smoothing.rs` & `field-compression-benchmark-0.0.2/core/model/src/extrapolation/euler_smoothing.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 use crate::{
+    extrapolation::TimeExtrapolation,
     model::{Model, State, StateView, StateViewMut},
     num::half,
-    timestep::TimeStep,
 };
 
 pub struct EulerSmoothing;
 
-impl<L: ?Sized + Model> TimeStep<L> for EulerSmoothing {
+impl<L: ?Sized + Model> TimeExtrapolation<L> for EulerSmoothing {
     fn step(&mut self, model: &mut L, ext: &mut L::Ext, dt: L::Dtype) {
         // X_n
         let x_n = model.state().to_owned();
         // model.state = X_n
 
         // X_(n+1) = X_n + X'_n * dt
         let mut x_np1 = model.tendencies(ext);
```

### Comparing `field-compression-benchmark-0.0.1/core/model/src/timestep/leapfrog.rs` & `field-compression-benchmark-0.0.2/core/model/src/extrapolation/leapfrog.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 use crate::{
+    extrapolation::TimeExtrapolation,
     model::{Model, State, StateViewMut},
     num::two,
-    timestep::TimeStep,
 };
 
 pub struct LeapFrog<L: ?Sized + Model> {
     state_prev: L::State,
 }
 
 impl<L: ?Sized + Model> LeapFrog<L> {
     #[must_use]
     pub const fn new(state_prev: L::State) -> Self {
         Self { state_prev }
     }
 }
 
-impl<L: ?Sized + Model> TimeStep<L> for LeapFrog<L> {
+impl<L: ?Sized + Model> TimeExtrapolation<L> for LeapFrog<L> {
     fn step(&mut self, model: &mut L, ext: &mut L::Ext, dt: L::Dtype) {
         // model.state = X_n
         // self.state_prev = X_(n-1)
 
         // X_(n+1) = X_(n-1) + 2 * X'_n * dt
         let mut x_np1 = model.tendencies(ext);
         x_np1.mul_assign(dt * two());
```

### Comparing `field-compression-benchmark-0.0.1/core/model/src/timestep/runge_kutta.rs` & `field-compression-benchmark-0.0.2/core/model/src/extrapolation/runge_kutta.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 use crate::{
+    extrapolation::TimeExtrapolation,
     model::{Model, State, StateViewMut},
     num::{half, two},
-    timestep::TimeStep,
 };
 
-pub struct RungeKutta;
+pub struct RungeKutta4;
 
-impl<L: ?Sized + Model> TimeStep<L> for RungeKutta {
+impl<L: ?Sized + Model> TimeExtrapolation<L> for RungeKutta4 {
     fn step(&mut self, model: &mut L, ext: &mut L::Ext, dt: L::Dtype) {
         // model.state = X_n
 
         // k1 = X'(X_n)
         let k1 = model.tendencies(ext);
 
         // k2 = X'(X_n + k1 * dt/2)
```

### Comparing `field-compression-benchmark-0.0.1/fcbench/fcbench/codecs.py` & `field-compression-benchmark-0.0.2/fcbench/fcbench/codecs.py`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/fcbench/fcbench/plot.py` & `field-compression-benchmark-0.0.2/fcbench/fcbench/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 def _tokenize_compressor(compressor: dict) -> list[str]:
     tokens = [compressor["name"], ": "]
 
     for i, codec in enumerate(compressor["codecs"]):
         if i > 0:
             tokens.append(", ")
-        tokens.append(codec["import"].split(".")[-1])
+        tokens.append(codec["import_path"].split(".")[-1])
         tokens.append("(")
 
         for j, (parameter, value) in enumerate(codec["parameters"].items()):
             if j > 0:
                 tokens.append(", ")
             tokens.append(parameter)
             tokens.append("=")
```

### Comparing `field-compression-benchmark-0.0.1/fcbench/src/benchmark.rs` & `field-compression-benchmark-0.0.2/fcbench/src/benchmark.rs`

 * *Files 7% similar despite different names*

```diff
@@ -5,30 +5,48 @@
     intern,
     prelude::*,
     types::PyDict,
 };
 
 use crate::{
     compressor::ConcreteCompressor,
-    dataclass::{Dataclass, DataclassOut},
+    dataclass::{Dataclass, DataclassOut, DataclassRegistry},
     dataset::Dataset,
 };
 
 pub fn create_module(py: Python) -> Result<&PyModule, PyErr> {
     let module = PyModule::new(py, "benchmark")?;
 
     module.add_class::<BenchmarkCase>()?;
     module.add_class::<BenchmarkCaseId>()?;
     module.add_class::<BenchmarkCaseFilter>()?;
     module.add_function(wrap_pyfunction!(report, module)?)?;
     module.add_function(wrap_pyfunction!(settings, module)?)?;
 
+    let types = PyModule::new(py, "types")?;
+    dataclass_registry().export(py, types)?;
+    module.add_submodule(types)?;
+
     Ok(module)
 }
 
+fn dataclass_registry() -> DataclassRegistry {
+    let mut registry = DataclassRegistry::new();
+
+    registry.insert::<core_benchmark::settings::BenchmarkSettings>();
+    registry.insert::<core_benchmark::error::BenchmarkCaseError>();
+    registry.insert::<core_benchmark::report::BenchmarkCaseReport>();
+    registry.insert_with_sample(&core_benchmark::case::BenchmarkCaseId::from_uuid(
+        uuid::Uuid::nil(),
+    ));
+    registry.insert::<core_benchmark::report::BenchmarkReport>();
+
+    registry
+}
+
 #[pyclass(module = "fcbench.benchmark", frozen)]
 pub struct BenchmarkCase {
     dataset: Py<crate::dataset::Dataset>,
     variable: Py<crate::dataset::DataVariable>,
     compressor: Py<crate::compressor::ConcreteCompressor>,
 }
 
@@ -53,57 +71,55 @@
             dataset: dataset.into(),
             variable: Py::new(py, variable)?,
             compressor: compressor.into(),
         })
     }
 
     #[getter]
+    /// [SIGNATURE]: # "(self) -> BenchmarkCaseId"
     pub fn id(&self, py: Python) -> Result<BenchmarkCaseId, PyErr> {
         self.with_case(py, |case| Ok(BenchmarkCaseId { id: case.get_id() }))
     }
 
     #[getter]
+    /// [SIGNATURE]: # "(self) -> UUID"
     pub fn uuid<'py>(&self, py: Python<'py>) -> Result<&'py PyAny, PyErr> {
         self.with_case(py, |case| {
             let uuid = case.get_uuid();
 
             py.import(intern!(py, "uuid"))?
                 .getattr("UUID")?
                 .call1((format!("{uuid}"),))
         })
     }
 
     #[allow(clippy::needless_pass_by_value)]
-    pub fn benchmark<'py>(
+    /// [SIGNATURE]: # "(settings: types.BenchmarkSettings) -> types.BenchmarkCaseReport"
+    pub fn benchmark(
         &self,
-        py: Python<'py>,
+        py: Python,
         settings: Dataclass<core_benchmark::settings::BenchmarkSettings>,
-    ) -> Result<&'py PyDict, PyErr> {
+    ) -> Result<DataclassOut<core_benchmark::report::BenchmarkCaseReport>, PyErr> {
         let dataset: &core_dataset::dataset::Dataset = &self.dataset.try_borrow(py)?.dataset;
         let variable: &core_dataset::variable::DataVariable =
             &self.variable.try_borrow(py)?.variable;
         let compressor: &core_compressor::compressor::ConcreteCompressor =
             &self.compressor.try_borrow(py)?.concrete;
 
         match core_benchmark::run_benchmark_case(dataset, variable, compressor, &settings) {
-            Ok(result) => {
-                let result_py = pythonize::pythonize(
-                    py,
-                    &core_benchmark::report::BenchmarkCaseReport {
-                        dataset: Cow::Borrowed(dataset.path()),
-                        format: dataset.format(),
-                        variable: variable.summary(),
-                        compressor: compressor.summary(),
-                        result: Ok(result),
-                    },
-                )
-                .map_err(PyErr::from)?;
-
-                result_py.into_ref(py).extract()
-            },
+            Ok(result) => DataclassOut::new(
+                &core_benchmark::report::BenchmarkCaseReport {
+                    dataset: Cow::Borrowed(dataset.path()),
+                    format: dataset.format(),
+                    variable: variable.summary(),
+                    compressor: compressor.summary(),
+                    result: Ok(result),
+                },
+                py,
+            ),
             Err(err) => Err(PyErr::from(err)),
         }
     }
 }
 
 impl BenchmarkCase {
     fn with_case<Q>(
@@ -124,21 +140,21 @@
 pub struct BenchmarkCaseId {
     id: core_benchmark::case::BenchmarkCaseId,
 }
 
 #[pymethods]
 impl BenchmarkCaseId {
     #[staticmethod]
-    #[pyo3(signature = (uuid), text_signature = "(uuid: uuid.UUID)")]
+    /// [SIGNATURE]: # "(self, uuid: UUID) -> BenchmarkCaseId"
     pub fn from_uuid(py: Python, uuid: &PyAny) -> Result<Self, PyErr> {
-        let codec = py
+        let uuid_class = py
             .import(intern!(py, "uuid"))?
             .getattr(intern!(py, "UUID"))?;
 
-        if !uuid.is_instance(codec)? {
+        if !uuid.is_instance(uuid_class)? {
             return Err(PyErr::new::<PyTypeError, _>(
                 "uuid is not an instance of uuid.UUID",
             ));
         }
 
         let uuid: &str = uuid.str()?.extract()?;
         let uuid = uuid
@@ -147,14 +163,15 @@
 
         Ok(Self {
             id: core_benchmark::case::BenchmarkCaseId::from_uuid(uuid),
         })
     }
 
     #[getter]
+    /// [SIGNATURE]: # "(self) -> UUID"
     pub fn uuid<'py>(&self, py: Python<'py>) -> Result<&'py PyAny, PyErr> {
         let uuid = self.id.into_uuid();
 
         py.import(intern!(py, "uuid"))?
             .getattr("UUID")?
             .call1((format!("{uuid}"),))
     }
@@ -164,26 +181,27 @@
     fn extract(object: &'py PyAny) -> Result<Self, PyErr> {
         if let Ok(id) = object.downcast::<PyCell<Self>>() {
             let id: PyRef<Self> = PyCell::try_borrow(id)?;
             let id: &Self = &id;
             return Ok(Self { id: id.id });
         }
 
-        BenchmarkCaseId::from_uuid(object.py(), object)
+        Self::from_uuid(object.py(), object)
     }
 }
 
 #[pyclass(module = "fcbench.benchmark", frozen)]
 pub struct BenchmarkCaseFilter {
     filter: core_benchmark::case::BenchmarkCaseFilter,
 }
 
 #[pymethods]
 impl BenchmarkCaseFilter {
     #[new]
+    /// [SIGNATURE]: # "(ids: Set[Union[BenchmarkCaseId, UUID]]) -> BenchmarkCaseFilter"
     pub fn new(ids: HashSet<BenchmarkCaseId>) -> Self {
         Self {
             filter: core_benchmark::case::BenchmarkCaseFilter::new(
                 ids.into_iter().map(|id| id.id).collect(),
             ),
         }
     }
@@ -221,37 +239,41 @@
     #[allow(clippy::needless_pass_by_value)]
     pub fn __contains__(&self, id: BenchmarkCaseId) -> bool {
         self.filter.contains_case_id(&id.id)
     }
 
     #[must_use]
     #[allow(clippy::needless_pass_by_value)]
+    /// [SIGNATURE]: # "(self, dataset: Union[str, bytes, PathLike]) -> bool"
     pub fn contains_dataset(&self, dataset: PathBuf) -> bool {
         self.filter.contains_dataset(&dataset)
     }
 
     #[must_use]
+    /// [SIGNATURE]: # "(self, variable: str) -> bool"
     pub fn contains_variable(&self, variable: &str) -> bool {
         self.filter.contains_variable(variable)
     }
 
     #[must_use]
     #[allow(clippy::needless_pass_by_value)]
+    /// [SIGNATURE]: # "(self, compressor: Union[str, bytes, PathLike]) -> bool"
     pub fn contains_compressor(&self, compressor: PathBuf) -> bool {
         self.filter.contains_compressor(&compressor)
     }
 
     #[must_use]
     pub fn contains_codec_params(
         &self,
         codec_params: &crate::compressor::ConcreteCompressor,
     ) -> bool {
         self.filter.contains_codec_params(&codec_params.concrete)
     }
 
+    /// [SIGNATURE]: # "(self, case: BenchmarkCase) -> bool"
     pub fn contains_case(&self, py: Python, case: &BenchmarkCase) -> Result<bool, PyErr> {
         case.with_case(py, |case| Ok(self.filter.contains_case(&case)))
     }
 }
 
 #[pyclass(module = "fcbench.benchmark")]
 // not frozen as the iterator is mutated on iteration
@@ -283,32 +305,42 @@
 
         Ok(filter.filter.contains_case_id(&id.id))
     }
 }
 
 #[pyfunction]
 #[pyo3(signature = (**kwargs))]
+/// [SIGNATURE]: # "(**kwargs) -> types.BenchmarkSettings"
 fn settings(
     py: Python,
     kwargs: Option<&PyDict>,
 ) -> Result<DataclassOut<core_benchmark::settings::BenchmarkSettings>, PyErr> {
     DataclassOut::new(
         &*kwargs
-            .unwrap_or(PyDict::new(py))
+            .unwrap_or_else(|| PyDict::new(py))
             .extract::<Dataclass<_>>()?,
         py,
     )
 }
 
 #[pyfunction]
 #[pyo3(signature = (**kwargs))]
+/// [SIGNATURE]: # "(**kwargs) -> types.BenchmarkReport"
 fn report<'py>(
     py: Python<'py>,
     kwargs: Option<&'py PyDict>,
 ) -> Result<DataclassOut<core_benchmark::report::BenchmarkReport<'py>>, PyErr> {
     DataclassOut::new(
         &*kwargs
-            .unwrap_or(PyDict::new(py))
+            .unwrap_or_else(|| PyDict::new(py))
             .extract::<Dataclass<_>>()?,
         py,
     )
 }
+
+#[cfg(test)]
+mod tests {
+    #[test]
+    fn dataclass_registry() {
+        let _ = super::dataclass_registry();
+    }
+}
```

### Comparing `field-compression-benchmark-0.0.1/field_compression_benchmark.egg-info/PKG-INFO` & `field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: field-compression-benchmark
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data compression methods and benchmarks for Cli/Met datasets
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 Maintainer-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `field-compression-benchmark-0.0.1/field_compression_benchmark.egg-info/SOURCES.txt` & `field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 ./codecs/linear-quantize/src/lib.rs
 ./codecs/log/Cargo.toml
 ./codecs/log/src/lib.rs
 ./codecs/reinterpret/Cargo.toml
 ./codecs/reinterpret/src/lib.rs
 ./codecs/sz3/Cargo.toml
 ./codecs/sz3/src/lib.rs
+./codecs/uniform-noise/Cargo.toml
+./codecs/uniform-noise/src/lib.rs
 ./codecs/wit/world.wit
 ./codecs/zfp/Cargo.toml
 ./codecs/zfp/src/lib.rs
 ./codecs/zfp/src/zfp.rs
 ./codecs/zlib/Cargo.toml
 ./codecs/zlib/src/lib.rs
 ./codecs/zstd/Cargo.toml
@@ -105,23 +107,26 @@
 ./core/model/Cargo.toml
 ./core/model/src/lib.rs
 ./core/model/src/num.rs
 ./core/model/src/boundary/mod.rs
 ./core/model/src/boundary/noop.rs
 ./core/model/src/boundary/periodic.rs
 ./core/model/src/boundary/zero.rs
+./core/model/src/extrapolation/direct.rs
+./core/model/src/extrapolation/euler_smoothing.rs
+./core/model/src/extrapolation/leapfrog.rs
+./core/model/src/extrapolation/mod.rs
+./core/model/src/extrapolation/runge_kutta.rs
+./core/model/src/model/any.rs
 ./core/model/src/model/linadv.rs
 ./core/model/src/model/lorenz_63.rs
 ./core/model/src/model/lorenz_96.rs
 ./core/model/src/model/mod.rs
-./core/model/src/timestep/direct.rs
-./core/model/src/timestep/euler_smoothing.rs
-./core/model/src/timestep/leapfrog.rs
-./core/model/src/timestep/mod.rs
-./core/model/src/timestep/runge_kutta.rs
+./core/model/src/model/onedsw.rs
+./core/model/src/model/twodsw.rs
 ./data/codecs/wasmtime.toml
 ./fcbench/Cargo.toml
 ./fcbench/src/benchmark.rs
 ./fcbench/src/compressor.rs
 ./fcbench/src/dataclass.rs
 ./fcbench/src/dataset.rs
 ./fcbench/src/lib.rs
@@ -190,18 +195,22 @@
 ./wasi/wit/deps/sockets/network.wit
 ./wasi/wit/deps/sockets/tcp-create-socket.wit
 ./wasi/wit/deps/sockets/tcp.wit
 ./wasi/wit/deps/sockets/udp-create-socket.wit
 ./wasi/wit/deps/sockets/udp.wit
 ./wasi/wit/deps/sockets/world.wit
 fcbench/fcbench/__init__.py
-fcbench/fcbench/benchmark.py
 fcbench/fcbench/codecs.py
-fcbench/fcbench/compressor.py
-fcbench/fcbench/dataset.py
-fcbench/fcbench/model.py
 fcbench/fcbench/plot.py
+fcbench/fcbench/benchmark/__init__.py
+fcbench/fcbench/benchmark/types.py
+fcbench/fcbench/compressor/__init__.py
+fcbench/fcbench/compressor/types.py
+fcbench/fcbench/dataset/__init__.py
+fcbench/fcbench/dataset/types.py
+fcbench/fcbench/model/__init__.py
+fcbench/fcbench/model/types.py
 field_compression_benchmark.egg-info/PKG-INFO
 field_compression_benchmark.egg-info/SOURCES.txt
 field_compression_benchmark.egg-info/dependency_links.txt
 field_compression_benchmark.egg-info/requires.txt
 field_compression_benchmark.egg-info/top_level.txt
```

### Comparing `field-compression-benchmark-0.0.1/fork/Cargo.toml` & `field-compression-benchmark-0.0.2/codecs/sz3/Cargo.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
-name = "fork"
+name = "sz3-codec"
 version = "0.1.0"
 edition = "2021"
-authors = ["Juniper Tyree <juniper.tyree@helsinki.fi>"]
-homepage = "https://github.com/juntyr/field-compression-benchmarkt"
-repository = "https://github.com/juntyr/field-compression-benchmark"
-readme = "README.md"
-license = "MIT OR Apache-2.0"
-rust-version = "1.76"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
+[lib]
+crate-type = ["cdylib"]
+
 [dependencies]
-core-error = { path = "../core/error", default-features = false }
-ipc-channel = { version = "0.18", default-features = false }
-libc = { version = "0.2", default-features = false }
-log = { version = "0.4", default-features = false }
-serde = { version = "1.0", default-features = false, features = ["std"] }
-signal-hook = { version = "0.3", default-features = false, features = ["iterator"] }
-thiserror = { version = "1.0", default-features = false }
+codecs-core = { path = "../core", default-features = false }
+codecs-core-wasm = { path = "../core-wasm", default-features = false }
+postcard = { version = "1.0", default-features = false }
+serde = { version = "1.0", default-features = false, features = ["std", "derive"] }
+sz3 = { git = "https://github.com/juntyr/sz3-rs.git", rev = "475d6e0", version = "0.1", default-features = false }
+# sz3-sys/zstd-sys@2.0.10 breaks compilation with XXH_STATIC_ASSERT=0
+zstd-sys = { version = "=2.0.9", default-features = false }
+
+[lints]
+workspace = true
```

### Comparing `field-compression-benchmark-0.0.1/fork/src/fork.rs` & `field-compression-benchmark-0.0.2/fork/src/fork.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-use std::cmp::Ordering;
-
 use thiserror::Error;
 
 use core_error::LocationError;
 
 use crate::Reaper;
 
 #[derive(Debug, Error)]
@@ -16,68 +14,70 @@
 }
 
 pub struct ForkChild {
     _private: (),
 }
 
 pub struct ForkParent {
-    child_pid: i32,
+    child_pid: rustix::process::Pid,
     _private: (),
 }
 
 impl ForkParent {
-    /// Wait for the forked child process to terminate and return its exit code
-    /// on success.
+    /// Wait for the forked child process to terminate.
     ///
     /// # Errors
     /// Returns the [`std::io::Error`] if waiting on the child process failed.
-    pub fn wait_for_child(self) -> Result<i32, LocationError<std::io::Error>> {
+    pub fn wait_for_child(self) -> Result<(), LocationError<std::io::Error>> {
         loop {
-            let mut status = 0;
-
-            match unsafe { libc::waitpid(self.child_pid, &mut status, libc::WNOHANG) }.cmp(&0) {
-                Ordering::Less => return Err(std::io::Error::last_os_error().into()),
-                Ordering::Equal => continue,
-                Ordering::Greater => return Ok(libc::WEXITSTATUS(status)),
-            };
+            match rustix::process::waitpid(
+                Some(self.child_pid),
+                rustix::process::WaitOptions::NOHANG,
+            ) {
+                Err(err) => return Err(LocationError::from2(err)),
+                Ok(None) => continue,
+                Ok(Some(_)) => return Ok(()),
+            }
         }
     }
 
-    /// Try to wait for the forked child process to terminate and return its
-    /// exit code on success. If the child has not yet terminated, [`Self`]
-    /// is returned to try again.
+    /// Try to wait for the forked child process to terminate. If the child has
+    /// not yet terminated, [`Self`] is returned to try again.
     ///
     /// # Errors
     /// Returns the [`std::io::Error`] if waiting on the child process failed.
-    pub fn try_wait_for_child(self) -> Result<Result<i32, Self>, LocationError<std::io::Error>> {
-        let mut status = 0;
-
-        match unsafe { libc::waitpid(self.child_pid, &mut status, libc::WNOHANG) }.cmp(&0) {
-            Ordering::Less => Err(std::io::Error::last_os_error().into()),
-            Ordering::Equal => Ok(Err(self)),
-            Ordering::Greater => Ok(Ok(libc::WEXITSTATUS(status))),
+    pub fn try_wait_for_child(self) -> Result<Result<(), Self>, LocationError<std::io::Error>> {
+        match rustix::process::waitpid(Some(self.child_pid), rustix::process::WaitOptions::NOHANG) {
+            Err(err) => Err(LocationError::from2(err)),
+            Ok(None) => Ok(Err(self)),
+            Ok(Some(_)) => Ok(Ok(())),
         }
     }
 
-    pub(crate) fn child_pid(&self) -> i32 {
+    pub(crate) const fn child_pid(&self) -> rustix::process::Pid {
         self.child_pid
     }
 }
 
 impl Reaper {
     /// Forks the current process and returns on the child and the parent
     /// process. [`Fork`] indicates if the process is the child or parent
     /// on success.
     ///
     /// # Errors
     /// Returns the [`std::io::Error`] if forking child process failed.
     pub fn fork(&self) -> Result<Fork, LocationError<std::io::Error>> {
-        match unsafe { libc::fork() } {
-            -1 => Err(std::io::Error::last_os_error().into()),
-            0 => Ok(Fork::Child(ForkChild { _private: () })),
-            child_pid => Ok(Fork::Parent(ForkParent {
+        // FIXME
+        // see https://docs.rs/rustix/0.38.32/src/rustix/runtime.rs.html#232-317
+        #[allow(unsafe_code)]
+        let child_pid = unsafe { libc::fork() };
+
+        match rustix::process::Pid::from_raw(child_pid) {
+            None if child_pid == 0 => Ok(Fork::Child(ForkChild { _private: () })),
+            None => Err(std::io::Error::last_os_error().into()),
+            Some(child_pid) => Ok(Fork::Parent(ForkParent {
                 child_pid,
                 _private: (),
             })),
         }
     }
 }
```

### Comparing `field-compression-benchmark-0.0.1/fork/src/reaper/canary.rs` & `field-compression-benchmark-0.0.2/fork/src/reaper/canary.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,69 @@
-use std::cmp::Ordering;
-
 use signal_hook::iterator::Signals;
 use thiserror::Error;
 
 use core_error::LocationError;
 
 use super::{exit_with_report, handler::reaper_handler_setup};
 use crate::{Fork, Reaper};
 
 pub fn reaper_canary_setup<F: FnOnce(&Reaper) -> Q, Q>(
     inner: F,
 ) -> Result<Q, LocationError<CanarySetupError>> {
-    let canary_pid = unsafe { libc::getpid() };
+    let canary_pid = rustix::process::getpid();
 
     match Reaper::new().fork() {
         Err(err) => Err(CanarySetupError::CanaryForkError(err).into()),
         Ok(Fork::Child(_)) => match reaper_handler_setup(canary_pid, inner) {
             Ok(result) => Ok(result),
             Err(err) => exit_with_report(err),
         },
         Ok(Fork::Parent(parent)) => match reaper_canary(canary_pid, parent.child_pid()) {
             Ok(status) => std::process::exit(status),
             Err(err) => exit_with_report(err),
         },
     }
 }
 
-fn reaper_canary(canary_pid: i32, handler_pid: i32) -> Result<i32, LocationError<CanaryError>> {
+fn reaper_canary(
+    canary_pid: rustix::process::Pid,
+    handler_pid: rustix::process::Pid,
+) -> Result<i32, LocationError<CanaryError>> {
     let mut signals =
         Signals::new((1..32).filter(|signal| !signal_hook::consts::FORBIDDEN.contains(signal)))
             .map_err(CanaryError::SignalInstallation)?;
 
     let status = loop {
-        let mut status = 0;
-
-        match unsafe { libc::waitpid(handler_pid, &mut status, libc::WNOHANG) }.cmp(&0) {
-            Ordering::Less => {
-                return Err(CanaryError::HandlerWait(std::io::Error::last_os_error()).into());
-            },
-            Ordering::Equal => (),
-            Ordering::Greater => break libc::WEXITSTATUS(status),
+        match rustix::process::waitpid(Some(handler_pid), rustix::process::WaitOptions::NOHANG) {
+            Err(err) => return Err(CanaryError::HandlerWait(err.into()).into()),
+            Ok(None) => (),
+            #[allow(clippy::cast_possible_wrap)] // FIXME
+            Ok(Some(status)) => break libc::WEXITSTATUS(status.as_raw() as i32),
         };
 
         for signal in signals.wait() {
-            log::debug!(
-                "The CANARY {} has received the signal {}.",
-                canary_pid,
-                signal
-            );
+            let Some(signal) = rustix::process::Signal::from_raw(signal) else {
+                return Err(CanaryError::UnknownSignal(signal).into());
+            };
+
+            log::debug!("The CANARY {canary_pid:?} has received the signal {signal:?}.");
 
-            if signal != libc::SIGCHLD {
+            if signal != rustix::process::Signal::Child {
                 log::debug!(
-                    "The CANARY {} will send the signal {} to the HANDLER {}.",
-                    handler_pid,
-                    signal,
-                    handler_pid
+                    "The CANARY {handler_pid:?} will send the signal {signal:?} to the HANDLER \
+                     {handler_pid:?}."
                 );
 
                 // Error is ignored as the handler may have already terminated
-                unsafe { libc::kill(handler_pid, signal) };
+                let _ = rustix::process::kill_process(handler_pid, signal);
             }
         }
     };
 
-    log::debug!(
-        "The CANARY {} will exit with status {}.",
-        canary_pid,
-        status
-    );
+    log::debug!("The CANARY {canary_pid:?} will exit with status {status}.");
 
     Ok(status)
 }
 
 #[derive(Debug, Error)]
 pub enum CanarySetupError {
     #[error("failed to fork the main process into a canary and a handler")]
@@ -80,8 +72,10 @@
 
 #[derive(Debug, Error)]
 enum CanaryError {
     #[error("failed to install the signal handler in the canary")]
     SignalInstallation(#[source] std::io::Error),
     #[error("failed to wait for the handler to terminate")]
     HandlerWait(#[source] std::io::Error),
+    #[error("failed to forward unknown signal {0} to the handler")]
+    UnknownSignal(i32),
 }
```

### Comparing `field-compression-benchmark-0.0.1/fork/src/reaper/mod.rs` & `field-compression-benchmark-0.0.2/fork/src/reaper/mod.rs`

 * *Files 23% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 mod worker;
 
 use canary::reaper_canary_setup;
 
 pub struct Reaper(());
 
 impl Reaper {
-    fn new() -> Self {
+    const fn new() -> Self {
         Self(())
     }
 
     /// Initialise the current (main) process to clean up any child processes
     /// it spawns. If setting up the reaper fails, the process is terminated.
-    pub fn with_subprocess_reaper<F: FnOnce(&Reaper) -> Q, Q>(
+    pub fn with_subprocess_reaper<F: FnOnce(&Self) -> Q, Q>(
         token: private::ReaperToken,
         inner: F,
     ) -> Q {
         #[allow(clippy::drop_non_drop)]
         std::mem::drop(token);
 
         match reaper_canary_setup(inner) {
```

### Comparing `field-compression-benchmark-0.0.1/fork/src/reaper/worker.rs` & `field-compression-benchmark-0.0.2/fork/src/reaper/worker.rs`

 * *Files 24% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 use core_error::LocationError;
 
 use crate::Reaper;
 
 pub fn reaper_worker<F: FnOnce(&Reaper) -> Q, Q>(
     inner: F,
 ) -> Result<Q, LocationError<WorkerSetupError>> {
-    let worker_pid = unsafe { libc::getpid() };
+    let worker_pid = rustix::process::getpid();
 
-    if unsafe { libc::setsid() } == -1 {
-        return Err(WorkerSetupError::ProcessGroupSetup(std::io::Error::last_os_error()).into());
+    if let Err(err) = rustix::process::setsid() {
+        return Err(WorkerSetupError::ProcessGroupSetup(err.into()).into());
     }
 
-    log::debug!("The WORKER {} will now start to execute.", worker_pid,);
+    log::debug!("The WORKER {worker_pid:?} will now start to execute.");
 
     let result = inner(&Reaper::new());
 
-    log::debug!("The WORKER {} has finished executing.", worker_pid,);
+    log::debug!("The WORKER {worker_pid:?} has finished executing.");
 
     Ok(result)
 }
 
 #[derive(Debug, Error)]
 pub enum WorkerSetupError {
     #[error("failed to create a new process group for the worker")]
```

### Comparing `field-compression-benchmark-0.0.1/fork/src/work.rs` & `field-compression-benchmark-0.0.2/fork/src/work.rs`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     fn clean_up_graveyard(&mut self) {
         let mut index = 0;
 
         while index < self.graveyard.len() {
             let fork = self.graveyard.swap_remove(index);
 
             match fork.try_wait_for_child() {
-                Ok(Ok(_)) => (),
+                Ok(Ok(())) => (),
                 Ok(Err(fork)) => self.graveyard.push(fork),
                 Err(err) => log::warn!("worker process could not be awaited: {err}"),
             }
 
             index += 1;
         }
     }
@@ -212,15 +212,15 @@
 
                             any_update = true;
 
                             // Try to wait for the worker process to terminate
                             // Since we already have the result, non-critical wait errors
                             //  are only logged, not passed on further
                             match worker.try_wait_for_child() {
-                                Ok(Ok(_)) => (),
+                                Ok(Ok(())) => (),
                                 Ok(Err(worker)) => self.graveyard.push(worker),
                                 Err(err) => {
                                     log::warn!("worker process could not be awaited: {err}");
                                 },
                             };
 
                             self.max_processes += 1;
```

### Comparing `field-compression-benchmark-0.0.1/pyproject.toml` & `field-compression-benchmark-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel", "setuptools-rust"]
 
 [project]
 name = "field-compression-benchmark"
-version = "0.0.1"
+version = "0.0.2"
 requires-python = ">=3.10"
 description = "Data compression methods and benchmarks for Cli/Met datasets"
 license = { file = "LICENSE-APACHE" }
 authors = [
     { name = "Juniper Tyree", email = "juniper.tyree@helsinki.fi" }
 ]
 maintainers = [
@@ -23,14 +23,15 @@
     "dask == 2024.2.1",
     "matplotlib == 3.4.3",
     "netcdf4 == 1.6.5",
     "numcodecs == 0.12.1",
     "numpy == 1.26.4",
     "pint == 0.23",
     "proplot == 0.9.7",
+    "result == 0.16.1",
     "xarray == 2023.12.0",
     "xeofs == 2.3.1",
     "xhistogram == 0.3.2",
     "zarr == 2.17.0",
 ]
 
 [project.readme]
@@ -47,15 +48,15 @@
 [[tool.setuptools-rust.ext-modules]]
 target = "fcbench._fcbench"
 path = "fcbench/Cargo.toml"
 binding = "PyO3"
 
 [tool.poetry]
 name = "field-compression-benchmark"
-version = "0.0.1"
+version = "0.0.2"
 description = "field-compression-benchmark Python environment"
 authors = ["Juniper Tyree <juniper.tyree@helsinki.fi>"]
 package-mode = false
 
 [tool.poetry.dependencies]
 python = "~3.11"
 cfgrib = "0.9.10.4"
```

### Comparing `field-compression-benchmark-0.0.1/setup.py` & `field-compression-benchmark-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/src/args.rs` & `field-compression-benchmark-0.0.2/src/args.rs`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     /// Colour and pretty-format console messages
     pub color: Option<ColorChoice>,
 }
 
 pub enum Command {
     /// Execute the benchmarking suite
     Bench(BenchArgs),
+    /// Launch the embedded Python REPL
+    Python(PythonArgs),
 }
 
 pub struct BenchArgs {
     /// Include the following WASM codec files
     pub codecs: VecSet<PathBuf>,
     /// Include the following compressor config files
     pub compressors: VecSet<PathBuf>,
@@ -65,49 +67,58 @@
     /// Distribute the benchmark across several processes, or use the available
     /// parallelism
     pub num_processes: Option<NonZeroUsize>,
     /// Select the detail of the progress updates as benchmark cases complete
     pub progress: Option<Progress>,
 }
 
+pub struct PythonArgs {
+    /// Program read from script file
+    pub file: Option<PathBuf>,
+    /// Arguments passed to the program in sys.argv[1:]
+    pub arg: Vec<String>,
+}
+
 impl Cli {
     pub fn parse() -> Result<Self, LocationError<io::Error>> {
         let CliImpl {
             command,
             log,
             quiet,
             color,
         } = CliImpl::parse();
 
         let command = match command {
-            CommandImpl::Bench(BenchArgsImpl {
-                codecs,
-                excluded_codecs,
-                compressors,
-                excluded_compressors,
-                datasets,
-                excluded_datasets,
-                cases,
-                minimal,
-                dry_run,
-                num_repeats,
-                bootstrap_seed,
-                bootstrap_samples,
-                error_bins,
-                error_resamples,
-                dataset_auto_chunk_size,
-                output,
-                resume,
-                keep_going,
-                num_processes,
-                progress,
-                _no_dry_run,
-                _no_resume,
-                _no_keep_going,
-            }) => {
+            CommandImpl::Bench(args) => {
+                let BenchArgsImpl {
+                    codecs,
+                    excluded_codecs,
+                    compressors,
+                    excluded_compressors,
+                    datasets,
+                    excluded_datasets,
+                    cases,
+                    minimal,
+                    dry_run,
+                    num_repeats,
+                    bootstrap_seed,
+                    bootstrap_samples,
+                    error_bins,
+                    error_resamples,
+                    dataset_auto_chunk_size,
+                    output,
+                    resume,
+                    keep_going,
+                    num_processes,
+                    progress,
+                    _no_dry_run,
+                    _no_resume,
+                    _no_keep_going,
+                } = *args;
+
                 let args = BenchArgs {
                     codecs: CliImpl::expand_exclude_config_files(
                         &codecs,
                         &excluded_codecs,
                         "wasm",
                     )?,
                     compressors: CliImpl::expand_exclude_config_files(
@@ -134,14 +145,19 @@
                     keep_going,
                     num_processes,
                     progress,
                 };
 
                 Command::Bench(args)
             },
+            CommandImpl::Python(args) => {
+                let PythonArgsImpl { file, arg } = *args;
+
+                Command::Python(PythonArgs { file, arg })
+            },
         };
 
         Ok(Self {
             command,
             log,
             quiet,
             color,
@@ -182,15 +198,17 @@
     #[arg(short, long, value_enum)]
     color: Option<ColorChoice>,
 }
 
 #[derive(Subcommand)]
 enum CommandImpl {
     /// Execute the benchmarking suite
-    Bench(BenchArgsImpl),
+    Bench(Box<BenchArgsImpl>),
+    /// Launch the embedded Python REPL
+    Python(Box<PythonArgsImpl>),
 }
 
 #[allow(clippy::struct_excessive_bools)]
 #[derive(Args)]
 struct BenchArgsImpl {
     /// Include the following WASM codec files or directories
     #[arg(long = "codec", num_args(0..), default_value = Path::new("data").join("codecs").into_os_string())]
@@ -287,14 +305,24 @@
     _no_resume: bool,
 
     /// Stop with the first benchmark case failure (default)
     #[arg(long = "no-keep-going")]
     _no_keep_going: bool,
 }
 
+#[derive(Args)]
+#[clap(trailing_var_arg = true)]
+struct PythonArgsImpl {
+    /// Program read from script file
+    file: Option<PathBuf>,
+    /// Arguments passed to the program in sys.argv[1:]
+    #[clap(num_args(0..), allow_hyphen_values=true)]
+    arg: Vec<String>,
+}
+
 impl CliImpl {
     fn expand_exclude_config_files(
         includes: &[PathBuf],
         excludes: &[PathBuf],
         extension: &str,
     ) -> Result<VecSet<PathBuf>, LocationError<io::Error>> {
         let mut expanded = VecSet::with_capacity(includes.len());
@@ -336,32 +364,32 @@
     pub variable_dimensions: bool,
     pub variable_derivatives: bool,
 }
 
 impl From<Option<Vec<MinimalFlag>>> for Minimal {
     fn from(flags: Option<Vec<MinimalFlag>>) -> Self {
         let Some(flags) = flags else {
-            return Minimal {
+            return Self {
                 codec_parameters: false,
                 dataset_variables: false,
                 variable_dimensions: false,
                 variable_derivatives: false,
             };
         };
 
         if flags.is_empty() || flags.contains(&MinimalFlag::All) {
-            return Minimal {
+            return Self {
                 codec_parameters: true,
                 dataset_variables: true,
                 variable_dimensions: true,
                 variable_derivatives: true,
             };
         }
 
-        Minimal {
+        Self {
             codec_parameters: flags.contains(&MinimalFlag::CodecParameters),
             dataset_variables: flags.contains(&MinimalFlag::DatasetVariables),
             variable_dimensions: flags.contains(&MinimalFlag::VariableDimensions),
             variable_derivatives: flags.contains(&MinimalFlag::VariableDerivatives),
         }
     }
 }
@@ -384,20 +412,20 @@
     Debug,
     Trace,
 }
 
 impl From<LogLevelFilter> for LevelFilter {
     fn from(filter: LogLevelFilter) -> Self {
         match filter {
-            LogLevelFilter::Off => LevelFilter::Off,
-            LogLevelFilter::Error => LevelFilter::Error,
-            LogLevelFilter::Warn => LevelFilter::Warn,
-            LogLevelFilter::Info => LevelFilter::Info,
-            LogLevelFilter::Debug => LevelFilter::Debug,
-            LogLevelFilter::Trace => LevelFilter::Trace,
+            LogLevelFilter::Off => Self::Off,
+            LogLevelFilter::Error => Self::Error,
+            LogLevelFilter::Warn => Self::Warn,
+            LogLevelFilter::Info => Self::Info,
+            LogLevelFilter::Debug => Self::Debug,
+            LogLevelFilter::Trace => Self::Trace,
         }
     }
 }
 
 #[derive(Clone, Debug, ValueEnum)]
 pub enum Progress {
     Off,
```

### Comparing `field-compression-benchmark-0.0.1/src/benchmarking/mod.rs` & `field-compression-benchmark-0.0.2/src/benchmarking/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/src/benchmarking/prepare.rs` & `field-compression-benchmark-0.0.2/src/benchmarking/prepare.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 use std::{iter::FusedIterator, path::PathBuf};
 
 use pyo3::{intern, prelude::*};
 use thiserror::Error;
 use vecmap::{VecMap, VecSet};
 
 use core_benchmark::case::BenchmarkCaseFilter;
-use core_compressor::compressor::{Compressor, ParseCompressorError};
+use core_compressor::{
+    compressor::{Compressor, ParseCompressorError},
+    parameter::ParameterEvalError,
+};
 use core_dataset::{
     dataset::{Dataset, DatasetSettings, ParseDatasetError},
     units::{UnitExpression, UnitRegistry},
     variable::{derivative::DataDerivative, dimension::DataSlice},
 };
 use core_error::LocationError;
 
@@ -25,15 +28,15 @@
     pub fn prepare(
         py: Python,
         mut compressors: VecSet<PathBuf>,
         mut datasets: VecSet<PathBuf>,
         minimal: &Minimal,
         case_filter: Option<&BenchmarkCaseFilter>,
         dataset_settings: &DatasetSettings,
-    ) -> Result<Benchmark, LocationError<BenchmarkPrepareError>> {
+    ) -> Result<Self, LocationError<BenchmarkPrepareError>> {
         println!("- Loading the SI unit registry");
 
         let unit_registry =
             UnitRegistry::try_new(py).map_err(BenchmarkPrepareError::UnitRegistry)?;
 
         println!("- Parsing the compressor configuration files");
 
@@ -145,15 +148,15 @@
                     println!("      - {variable}");
                 }
             }
         }
 
         println!();
 
-        Ok(Benchmark {
+        Ok(Self {
             compressors,
             datasets,
         })
     }
 
     pub fn prepare_python(py: Python) -> Result<(), LocationError<PyErr>> {
         let py_version: &str = py.import("sys")?.getattr("version")?.extract()?;
@@ -193,23 +196,34 @@
         self.datasets.values()
     }
 
     pub fn pre_check_concrete_compressors(
         &self,
         py: Python,
         case_filter: Option<&BenchmarkCaseFilter>,
-    ) -> Result<usize, LocationError<PyErr>> {
+    ) -> Result<usize, BenchmarkPrepareError> {
         let mut num_compressors = 0;
 
         for compressor in self.compressors() {
-            for concrete in compressor.iter_concrete() {
+            for concrete in compressor
+                .iter_concrete()
+                .map_err(LocationError::from)
+                .map_err(BenchmarkPrepareError::PrecheckCompressorParameter)?
+            {
+                let concrete = concrete
+                    .map_err(LocationError::from)
+                    .map_err(BenchmarkPrepareError::PrecheckCompressorParameter)?;
+
                 if case_filter.as_ref().map_or(true, |case_filter| {
                     case_filter.contains_codec_params(&concrete)
                 }) {
-                    concrete.build_py(py)?;
+                    concrete
+                        .build_py(py)
+                        .map_err(LocationError::from)
+                        .map_err(BenchmarkPrepareError::PrecheckCompressorPython)?;
                     num_compressors += 1;
                 }
             }
         }
 
         Ok(num_compressors)
     }
@@ -221,8 +235,12 @@
     Dataset(#[source] LocationError<ParseDatasetError>),
     #[error("failed to load a compressor")]
     Compressor(#[source] LocationError<ParseCompressorError>),
     #[error("failed to import a codec")]
     CodecImport(#[source] LocationError<PyErr>),
     #[error("failed to load the unit registry")]
     UnitRegistry(#[source] LocationError<PyErr>),
+    #[error("failed to precheck a compressor")]
+    PrecheckCompressorPython(#[source] LocationError<PyErr>),
+    #[error("failed to precheck a compressor")]
+    PrecheckCompressorParameter(#[source] LocationError<ParameterEvalError>),
 }
```

### Comparing `field-compression-benchmark-0.0.1/src/benchmarking/report.rs` & `field-compression-benchmark-0.0.2/src/benchmarking/report.rs`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 pub struct ProgressReporter {
     success: usize,
     failure: usize,
 }
 
 impl ProgressReporter {
     #[must_use]
-    pub fn new() -> Self {
+    pub const fn new() -> Self {
         Self {
             success: 0,
             failure: 0,
         }
     }
 
     fn report_case(&self, summary: &'static str, case: &BenchmarkCase) {
@@ -285,18 +285,15 @@
                 // Try again with closing brackets in case the benchmark
                 //  terminated unexpectedly
                 json_report.push(b'}');
                 json_report.push(b',');
                 serde_json::to_writer(&mut json_report, &BenchmarkSummary::default())
                     .map_err(io::Error::from)?;
                 json_report.push(b'}');
-                match serde_json::from_slice(&json_report) {
-                    Ok(partial_report) => Ok(partial_report),
-                    Err(_) => Err(io::Error::from(err)),
-                }
+                serde_json::from_slice(&json_report).map_err(|_| io::Error::from(err))
             },
         }?;
 
         // NOTE: since arguments are already resolved at this point,
         //        they need to be passed explicitly
         if settings != &partial_report.settings {
             return Err(io::Error::new(
@@ -319,15 +316,15 @@
             .filter_map(|(id, result)| {
                 match result.result {
                     Ok(_) => {
                         pre_success += 1;
                         Some(*id)
                     },
                     // We give distributed failures another chance
-                    Err(BenchmarkCaseError::Distributed(_)) => None,
+                    Err(BenchmarkCaseError::Distributed { .. }) => None,
                     // We give keyboard interrupt failures another chance
                     Err(BenchmarkCaseError::Python(ref err))
                         if matches!(
                             err.error(), PyErrString { r#type, .. } if r#type == "KeyboardInterrupt"
                         ) =>
                     {
                         None
```

### Comparing `field-compression-benchmark-0.0.1/src/fcpy.rs` & `field-compression-benchmark-0.0.2/src/fcpy.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/src/main.rs` & `field-compression-benchmark-0.0.2/src/main.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
-#![allow(clippy::module_name_repetitions)]
-
 use std::{
-    borrow::Cow, collections::HashSet, iter::FusedIterator, num::NonZeroUsize, path::PathBuf,
+    borrow::Cow,
+    collections::HashSet,
+    iter::FusedIterator,
+    num::NonZeroUsize,
+    path::{Path, PathBuf},
     sync::Mutex,
 };
 
+use args::PythonArgs;
 use byte_unit::{Byte, Unit, UnitType};
 use clap::ColorChoice;
 use log::LevelFilter;
 use pretty_env_logger::env_logger::WriteStyle;
-use pyo3::prelude::*;
+use pyo3::{
+    exceptions::{PyFileNotFoundError, PySystemExit},
+    prelude::*,
+    types::PyList,
+};
 use thiserror::Error;
 use vecmap::VecSet;
 
 use core_benchmark::{
     case::{BenchmarkCase, BenchmarkCaseFilter, BenchmarkCaseId},
     report::BenchmarkReport,
     settings::{BenchmarkSettings, BootstrapSettings, ErrorSettings, MeasurementSettings},
@@ -49,24 +47,31 @@
     let Cli {
         command,
         log,
         quiet,
         color,
     } = Cli::parse().map_err(BenchmarkSuiteError::CliArgs)?;
 
-    let Command::Bench(args) = command;
+    // create a Python runtime
+    pyo3::prepare_freethreaded_python();
+
+    let args = match command {
+        Command::Bench(args) => args,
+        Command::Python(PythonArgs { file: None, arg: _ }) => return python_repl(),
+        Command::Python(PythonArgs {
+            file: Some(file),
+            arg,
+        }) => return python_exec(&file, arg),
+    };
 
     setup_log_and_color(log.map(LevelFilter::from), quiet, color)?;
 
     let token = try_get_reaper_token(&fork::REAPER_TOKEN).map_err(BenchmarkSuiteError::Reaper)?;
 
     Reaper::with_subprocess_reaper(token, |reaper| {
-        // create a Python runtime
-        pyo3::prepare_freethreaded_python();
-
         Python::with_gil(Benchmark::prepare_python)
             .map_err(BenchmarkSuiteError::PythonDependencies)?;
 
         let settings = prepare_benchmark_settings(
             args.num_repeats,
             args.bootstrap_seed,
             args.bootstrap_samples,
@@ -99,15 +104,16 @@
             )
         })
         .map_err(BenchmarkSuiteError::PrepareBenchmark)?;
 
         let num_compressors = Python::with_gil(|py| {
             benchmark.pre_check_concrete_compressors(py, case_filter.as_ref())
         })
-        .map_err(BenchmarkSuiteError::PrecheckCompressor)?;
+        .map_err(LocationError::from)
+        .map_err(BenchmarkSuiteError::PrepareBenchmark)?;
 
         let benchmark_cases = generate_benchmark_cases(&benchmark, &case_filter);
 
         if args.dry_run {
             let benchmark_case_ids: HashSet<BenchmarkCaseId> =
                 benchmark_cases.map(|case| case.get_id()).collect();
 
@@ -167,15 +173,80 @@
             );
         }
 
         Ok(())
     })
 }
 
+fn python_repl() -> Result<(), LocationError<BenchmarkSuiteError>> {
+    Python::with_gil(|py| -> Result<(), LocationError<PyErr>> {
+        let sys = py.import("sys")?;
+        let sys_version: &str = sys.getattr("version")?.extract()?;
+        let sys_platform: &str = sys.getattr("platform")?.extract()?;
+
+        let banner = format!(
+            "Python {sys_version} on {sys_platform}\nType \"help\", \"copyright\", \"credits\" or \
+             \"license\" for more information."
+        );
+
+        let Err(err) = py
+            .import("code")?
+            .getattr("interact")?
+            .call1((banner,))
+            .map_err(LocationError::new)
+        else {
+            return Ok(());
+        };
+
+        if !err.error().is_instance_of::<PySystemExit>(py) {
+            return Err(err);
+        }
+
+        let code = err.error().value(py).getattr("code")?;
+
+        if code.is_none() {
+            return Ok(());
+        }
+
+        if let Ok(code) = code.extract() {
+            std::process::exit(code);
+        }
+
+        err.error().print(py);
+        std::process::exit(1);
+    })
+    .map_err(|err| LocationError::new(BenchmarkSuiteError::Repl(err)))
+}
+
+fn python_exec(
+    file: &Path,
+    mut args: Vec<String>,
+) -> Result<(), LocationError<BenchmarkSuiteError>> {
+    Python::with_gil(|py| -> Result<(), LocationError<PyErr>> {
+        let code = std::fs::read_to_string(file).map_err(|err| {
+            PyFileNotFoundError::new_err(format!("can't open file {file:?}: {err}"))
+        })?;
+
+        let file_str = file.display().to_string();
+
+        args.insert(0, file_str.clone());
+        let args = PyList::new(py, args);
+
+        let sys = py.import("sys")?;
+        sys.setattr("argv", args)?;
+
+        let _module = PyModule::from_code(py, &code, &file_str, "__main__")?;
+
+        Ok(())
+    })
+    .map_err(|err| LocationError::new(BenchmarkSuiteError::Repl(err)))
+}
+
 fn try_get_reaper_token<T>(token: &Mutex<Option<T>>) -> Result<T, LocationError<ReaperError>> {
+    #[allow(clippy::significant_drop_in_scrutinee)]
     match token.lock().map(|mut guarded_token| guarded_token.take()) {
         Ok(Some(token)) => Ok(token),
         Ok(None) => Err(ReaperError::AlreadyInitialised.into()),
         Err(_) => Err(ReaperError::PoisonedToken.into()),
     }
 }
 
@@ -235,33 +306,46 @@
 
 fn generate_benchmark_cases<'a>(
     benchmark: &'a Benchmark,
     case_filter: &'a Option<BenchmarkCaseFilter>,
 ) -> impl FusedIterator<Item = BenchmarkCase<'a>> + 'a {
     benchmark.datasets().flat_map(|dataset| {
         dataset.variables().flat_map(|variable| {
-            benchmark.compressors().flat_map(|compressor| {
-                compressor
-                    .iter_concrete()
-                    .filter(|codec_params| {
-                        case_filter.as_ref().map_or(true, |case_filter| {
-                            case_filter.contains_codec_params(codec_params)
+            benchmark
+                .compressors()
+                // we already pre-checked all configs,
+                //  so we can silently skip errors here
+                .filter_map(|compressor| compressor.iter_concrete().ok())
+                .flat_map(|compressors| {
+                    compressors
+                        .filter_map(|codec_params| {
+                            match codec_params {
+                                Ok(codec_params)
+                                    if case_filter.as_ref().map_or(true, |case_filter| {
+                                        case_filter.contains_codec_params(&codec_params)
+                                    }) =>
+                                {
+                                    Some(codec_params)
+                                },
+                                // we already pre-checked all configs,
+                                //  so we can silently skip errors here
+                                Ok(_) | Err(_) => None,
+                            }
+                        })
+                        .map(|concrete| BenchmarkCase {
+                            dataset,
+                            variable,
+                            compressor: Cow::Owned(concrete),
+                        })
+                        .filter(|case| {
+                            case_filter
+                                .as_ref()
+                                .map_or(true, |case_filter| case_filter.contains_case(case))
                         })
-                    })
-                    .map(|concrete| BenchmarkCase {
-                        dataset,
-                        variable,
-                        compressor: Cow::Owned(concrete),
-                    })
-                    .filter(|case| {
-                        case_filter
-                            .as_ref()
-                            .map_or(true, |case_filter| case_filter.contains_case(case))
-                    })
-            })
+                })
         })
     })
 }
 
 struct ReporterSettings {
     num_processes: NonZeroUsize,
     quiet: bool,
@@ -416,26 +500,26 @@
     Ok(())
 }
 
 #[derive(Debug, Error)]
 pub enum BenchmarkSuiteError {
     #[error("failed to parse the command line arguments")]
     CliArgs(#[source] LocationError<std::io::Error>),
+    #[error("failed to run the Python REPL")]
+    Repl(#[source] LocationError<PyErr>),
     #[error("failed to initialise the subprocess reaper")]
     Reaper(#[source] LocationError<ReaperError>),
     #[error("failed to load the Python dependencies")]
     PythonDependencies(#[source] LocationError<PyErr>),
     #[error("failed to initialise the benchmark settings")]
     BenchmarkSettings(#[source] LocationError<getrandom::Error>),
     #[error("failed to load the WASM codecs into fcpy")]
     FcpyCodecs(#[source] LocationError<PyErr>),
     #[error("failed to prepare the benchmark")]
     PrepareBenchmark(#[source] LocationError<BenchmarkPrepareError>),
-    #[error("failed to precheck a compressor")]
-    PrecheckCompressor(#[source] LocationError<PyErr>),
     #[error(transparent)]
     CaseIdFile(CaseIdFileError),
     #[error("failed to determine the available CPU parallelism")]
     Parallelism(#[source] std::io::Error),
     #[error(transparent)]
     JsonReporter(JsonReporterError),
     #[error("failed to initialise the logger")]
```

### Comparing `field-compression-benchmark-0.0.1/wasi/build/build.rs` & `field-compression-benchmark-0.0.2/wasi/build/build.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-#![deny(clippy::pedantic)]
-#![deny(clippy::unwrap_used)]
-#![deny(clippy::expect_used)]
-#![deny(clippy::indexing_slicing)]
-#![deny(clippy::panic)]
-#![deny(clippy::todo)]
-#![deny(clippy::unimplemented)]
-#![deny(clippy::unreachable)]
-#![deny(unsafe_code)]
-
 use std::{
     fs,
     io::{self, Write},
     path::{Path, PathBuf},
     process::Command,
 };
 
@@ -80,15 +70,15 @@
             .map(|(component_name, const_name)| format!("({component_name:?}, {const_name})"))
             .collect::<Vec<_>>()
             .join(", "),
     )?;
 
     components.flush()?;
 
-    println!("cargo:rustc-env=COMPONENTS={}", components_path.display());
+    println!("cargo::rustc-env=COMPONENTS={}", components_path.display());
 
     Ok(())
 }
 
 fn configure_cargo_cmd() -> io::Result<Command> {
     let cargo =
         PathBuf::from(std::env::var_os("CARGO").ok_or_else(|| {
@@ -162,15 +152,15 @@
         return Err(io::Error::new(
             io::ErrorKind::InvalidData,
             "invalid deps file format",
         ));
     };
 
     for dep in deps.split_whitespace() {
-        println!("cargo:rerun-if-changed={dep}");
+        println!("cargo::rerun-if-changed={dep}");
     }
 
     Ok(())
 }
 
 fn create_new_component(wasm: &Path) -> io::Result<PathBuf> {
     let wasm_component = wasm.with_extension("component.wasm");
```

### Comparing `field-compression-benchmark-0.0.1/wasi/cli/src/stdio.rs` & `field-compression-benchmark-0.0.2/wasi/cli/src/stdio.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/cli/src/terminal.rs` & `field-compression-benchmark-0.0.2/wasi/cli/src/terminal.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/clocks/src/lib.rs` & `field-compression-benchmark-0.0.2/wasi/clocks/src/lib.rs`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,20 @@
     wit_bindgen::generate!({
         path: "../wit",
         world: "virtual-wasi-clocks",
     });
 }
 
 pub enum VirtClock {}
-crate::bindings::export!(VirtClock with_types_in bindings);
+
+#[allow(unsafe_code)]
+mod export {
+    use crate::VirtClock;
+    crate::bindings::export!(VirtClock with_types_in crate::bindings);
+}
 
 static CLOCK_NS: AtomicU64 = AtomicU64::new(0);
 
 impl WasiClocksMonotonicClock for VirtClock {
     fn now() -> Instant {
         CLOCK_NS.load(Ordering::SeqCst)
     }
@@ -41,18 +46,19 @@
         CLOCK_NS.fetch_add(when, Ordering::SeqCst);
         ready_pollable()
     }
 }
 
 impl WasiClocksWallClock for VirtClock {
     fn now() -> Datetime {
-        const NANOSECONDS: u32 = 1000000000;
+        const NANOSECONDS: u32 = 1_000_000_000;
 
         let now_ns = CLOCK_NS.load(Ordering::SeqCst);
 
+        #[allow(clippy::cast_possible_truncation)]
         let nanoseconds = (now_ns % u64::from(NANOSECONDS)) as u32;
         let seconds = now_ns / u64::from(NANOSECONDS);
 
         Datetime {
             seconds,
             nanoseconds,
         }
```

### Comparing `field-compression-benchmark-0.0.1/wasi/filesystem/src/lib.rs` & `field-compression-benchmark-0.0.2/wasi/filesystem/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,20 @@
     wit_bindgen::generate!({
         path: "../wit",
         world: "virtual-wasi-filesystem",
     });
 }
 
 pub enum VirtFilesystem {}
-crate::bindings::export!(VirtFilesystem with_types_in bindings);
+
+#[allow(unsafe_code)]
+mod export {
+    use crate::VirtFilesystem;
+    crate::bindings::export!(VirtFilesystem with_types_in crate::bindings);
+}
 
 pub enum VirtDescriptor {}
 pub enum VirtDirectoryEntryStream {}
 
 impl WasiFilesystemPreopens for VirtFilesystem {
     fn get_directories() -> Vec<(Descriptor, String)> {
         Vec::new()
@@ -41,14 +46,15 @@
     type DirectoryEntryStream = VirtDirectoryEntryStream;
 
     fn filesystem_error_code(_err: &Error) -> Option<ErrorCode> {
         None
     }
 }
 
+#[allow(clippy::uninhabited_references)] // FIXME
 impl GuestDescriptor for VirtDescriptor {
     fn read_via_stream(&self, _offset: Filesize) -> Result<InputStream, ErrorCode> {
         match *self {}
     }
 
     fn write_via_stream(&self, _offset: Filesize) -> Result<OutputStream, ErrorCode> {
         match *self {}
@@ -187,12 +193,13 @@
         _path_flags: PathFlags,
         _path: String,
     ) -> Result<MetadataHashValue, ErrorCode> {
         match *self {}
     }
 }
 
+#[allow(clippy::uninhabited_references)] // FIXME
 impl GuestDirectoryEntryStream for VirtDirectoryEntryStream {
     fn read_directory_entry(&self) -> Result<Option<DirectoryEntry>, ErrorCode> {
         match *self {}
     }
 }
```

### Comparing `field-compression-benchmark-0.0.1/wasi/io/src/lib.rs` & `field-compression-benchmark-0.0.2/wasi/io/src/lib.rs`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,20 @@
     wit_bindgen::generate!({
         path: "../wit",
         world: "virtual-wasi-io",
     });
 }
 
 pub enum VirtIO {}
-crate::bindings::export!(VirtIO with_types_in bindings);
+
+#[allow(unsafe_code)]
+mod export {
+    use crate::VirtIO;
+    crate::bindings::export!(VirtIO with_types_in crate::bindings);
+}
 
 impl WasiVirtNullIO for VirtIO {
     fn ready_pollable() -> Pollable {
         poll::VirtPollable::ready()
     }
 
     fn closed_input() -> InputStream {
```

### Comparing `field-compression-benchmark-0.0.1/wasi/io/src/poll.rs` & `field-compression-benchmark-0.0.2/wasi/io/src/poll.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/io/src/streams.rs` & `field-compression-benchmark-0.0.2/wasi/io/src/streams.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/random/src/lib.rs` & `field-compression-benchmark-0.0.2/wasi/random/src/lib.rs`

 * *Files 17% similar despite different names*

```diff
@@ -16,45 +16,52 @@
     wit_bindgen::generate!({
         path: "../wit",
         world: "virtual-wasi-random",
     });
 }
 
 pub enum VirtRandom {}
-crate::bindings::export!(VirtRandom with_types_in bindings);
+
+#[allow(unsafe_code)]
+mod export {
+    use crate::VirtRandom;
+    crate::bindings::export!(VirtRandom with_types_in crate::bindings);
+}
 
 fn rng() -> MutexGuard<'static, Pcg64> {
     static RNG: OnceLock<Mutex<Pcg64>> = OnceLock::new();
 
     #[cold]
     #[inline(never)]
     fn init_rng() -> &'static Mutex<Pcg64> {
         RNG.get_or_init(|| {
-            const PCG64_DEFAULT_STREAM: u128 = 0xa02bdbf7bb3c0a7ac28fa16a64abf96;
+            const PCG64_DEFAULT_STREAM: u128 = 0x0a02_bdbf_7bb3_c0a7_ac28_fa16_a64a_bf96;
 
             // let (state_lo, state_hi) = insecure_seed_host();
             // let state = u128::from(state_lo) | (u128::from(state_hi) << 64);
-            let state = 0xcafef00dd15ea5e5;
+            let state = 0xcafe_f00d_d15e_a5e5;
 
             Mutex::new(Pcg64::new(state, PCG64_DEFAULT_STREAM))
         })
     }
 
+    #[allow(clippy::unwrap_used)]
     RNG.get().unwrap_or_else(|| init_rng()).lock().unwrap()
 }
 
 impl WasiRandomInsecureSeed for VirtRandom {
     fn insecure_seed() -> (u64, u64) {
         let mut rng = rng();
         (rng.next_u64(), rng.next_u64())
     }
 }
 
 impl WasiRandomInsecure for VirtRandom {
     fn get_insecure_random_bytes(len: u64) -> Vec<u8> {
+        #[allow(clippy::unwrap_used)] // FIXME
         let mut buffer = vec![0; usize::try_from(len).unwrap()];
         rng().fill_bytes(&mut buffer);
         buffer
     }
 
     fn get_insecure_random_u64() -> u64 {
         rng().next_u64()
```

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/cli/environment.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/cli/environment.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/cli/terminal.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/cli/terminal.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/clocks/monotonic-clock.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/clocks/monotonic-clock.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/clocks/wall-clock.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/clocks/wall-clock.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/filesystem/types.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/filesystem/types.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/http/handler.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/http/handler.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/http/proxy.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/http/proxy.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/http/types.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/http/types.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/io/error.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/io/error.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/io/poll.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/io/poll.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/io/streams.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/io/streams.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/random/insecure-seed.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/random/insecure-seed.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/random/insecure.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/random/insecure.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/random/random.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/random/random.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/ip-name-lookup.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/ip-name-lookup.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/network.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/network.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/tcp-create-socket.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/tcp-create-socket.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/tcp.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/tcp.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/udp-create-socket.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/udp-create-socket.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/deps/sockets/udp.wit` & `field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/udp.wit`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.1/wasi/wit/world.wit` & `field-compression-benchmark-0.0.2/wasi/wit/world.wit`

 * *Files identical despite different names*

