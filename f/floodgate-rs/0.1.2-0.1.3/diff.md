# Comparing `tmp/floodgate_rs-0.1.2.tar.gz` & `tmp/floodgate_rs-0.1.3.tar.gz`

## Comparing `floodgate_rs-0.1.2.tar` & `floodgate_rs-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 floodgate_rs-0.1.2/Cargo.toml
--rw-r--r--   0     1001      123     2009 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/.github/workflows/release.yml
--rw-r--r--   0     1001      123      685 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/.gitignore
--rw-r--r--   0     1001      123     1068 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/LICENSE
--rw-r--r--   0     1001      123      516 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/README.md
--rw-r--r--   0     1001      123      186 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/floodgate/__init__.py
--rw-r--r--   0     1001      123    11914 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/floodgate/floodgate.pyi
--rw-r--r--   0     1001      123        0 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/floodgate/py.typed
--rw-r--r--   0     1001      123     1094 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/pyproject.toml
--rw-r--r--   0     1001      123     2323 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/src/dynamic_mapping.rs
--rw-r--r--   0     1001      123     1837 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/src/fixed_mapping.rs
--rw-r--r--   0     1001      123     1235 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/src/jumping_window.rs
--rw-r--r--   0     1001      123      374 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/src/lib.rs
--rw-r--r--   0     1001      123      755 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/src/traits.rs
--rw-r--r--   0     1001      123    15606 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 floodgate_rs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 floodgate_rs-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      123     2009 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      685 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/.gitignore
+-rw-r--r--   0     1001      123     1068 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/LICENSE
+-rw-r--r--   0     1001      123      516 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/README.md
+-rw-r--r--   0     1001      123      186 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/floodgate/__init__.py
+-rw-r--r--   0     1001      123    11914 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/floodgate/floodgate.pyi
+-rw-r--r--   0     1001      123        0 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/floodgate/py.typed
+-rw-r--r--   0     1001      123     1094 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/pyproject.toml
+-rw-r--r--   0     1001      123     2323 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/src/dynamic_mapping.rs
+-rw-r--r--   0     1001      123     1837 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/src/fixed_mapping.rs
+-rw-r--r--   0     1001      123     1235 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/src/jumping_window.rs
+-rw-r--r--   0     1001      123      374 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      123      857 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/src/traits.rs
+-rw-r--r--   0     1001      123    13694 2023-07-21 21:50:00.000000 floodgate_rs-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 floodgate_rs-0.1.3/PKG-INFO
```

### Comparing `floodgate_rs-0.1.2/.github/workflows/release.yml` & `floodgate_rs-0.1.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.2/.gitignore` & `floodgate_rs-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.2/LICENSE` & `floodgate_rs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.2/README.md` & `floodgate_rs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.2/floodgate/floodgate.pyi` & `floodgate_rs-0.1.3/floodgate/floodgate.pyi`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.2/pyproject.toml` & `floodgate_rs-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "floodgate-rs"
-version = "0.1.2"
+version = "0.1.3"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 description = "Python bindings for, a ratelimiting library written in Rust."
```

### Comparing `floodgate_rs-0.1.2/src/dynamic_mapping.rs` & `floodgate_rs-0.1.3/src/dynamic_mapping.rs`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.2/src/fixed_mapping.rs` & `floodgate_rs-0.1.3/src/fixed_mapping.rs`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.2/src/jumping_window.rs` & `floodgate_rs-0.1.3/src/jumping_window.rs`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.2/src/traits.rs` & `floodgate_rs-0.1.3/src/traits.rs`

 * *Files 13% similar despite different names*

```diff
@@ -7,21 +7,27 @@
     fn as_duration(&self) -> Duration;
 }
 
 impl ToDuration for PyDelta {
     fn as_duration(&self) -> Duration {
         let days = self.get_days() as u64;
         let seconds = self.get_seconds() as u64;
-        let mircros = self.get_microseconds() as u64;
-        Duration::from_micros((days * 86400 + seconds) * 1000000 + mircros)
+        let micros = self.get_microseconds() as u64;
+        Duration::from_secs(days * 86400 + seconds) + Duration::from_micros(micros)
     }
 }
 
 pub trait ToPydelta {
     fn as_pydelta<'py>(&self, py: Python<'py>) -> PyResult<&'py PyDelta>;
 }
 
 impl ToPydelta for Duration {
     fn as_pydelta<'py>(&self, py: Python<'py>) -> PyResult<&'py PyDelta> {
-        PyDelta::new(py, 0, 0, self.as_micros() as i32, false)
+        PyDelta::new(
+            py,
+            0,
+            self.as_secs() as i32,
+            self.subsec_micros() as i32,
+            false,
+        )
     }
 }
```

### Comparing `floodgate_rs-0.1.2/Cargo.lock` & `floodgate_rs-0.1.3/Cargo.lock`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
@@ -21,110 +27,56 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.11.1"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "572f695136211188308f16ad2ca5c851a712c464060ae6974944458eb83880ba"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "cc"
-version = "1.0.77"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e9f73505338f7d905b19d18738976aae232eb46b8efc15554ffc56deb5d9ebe4"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.23"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b0a3d9ed01224b22057780a37bb8c5dbfe1be8ba48678e7bf57ec4b385411f"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
  "js-sys",
- "num-integer",
  "num-traits",
  "time",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
-name = "codespan-reporting"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
-
-[[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
-
-[[package]]
-name = "cxx"
-version = "1.0.83"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdf07d07d6531bfcdbe9b8b739b104610c6508dcc4d63b410585faf338241daf"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.83"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2eb5b96ecdc99f72657332953d4d9c50135af1bac34277801cc3937906ebd39"
-dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
- "proc-macro2",
- "quote",
- "scratch",
- "syn",
-]
-
-[[package]]
-name = "cxxbridge-flags"
-version = "1.0.83"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac040a39517fd1674e0f32177648334b0f4074625b5588a64519804ba0553b12"
-
-[[package]]
-name = "cxxbridge-macro"
-version = "1.0.83"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1362b0ddcfc4eb0a1f57b68bd77dd99f0e826958a96abd0ae9bd092e114ffed6"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "dashmap"
-version = "5.4.0"
+version = "5.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
+checksum = "6943ae99c34386c84a470c499d3414f66502a41340aa895406e0d2e4a207b91d"
 dependencies = [
  "cfg-if",
  "hashbrown",
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
@@ -144,153 +96,130 @@
 checksum = "3fa228340d1d0a74e0bbc4f38e91b41f46041fe0d54abd713d505a802cd6fda2"
 dependencies = [
  "dashmap",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.12.3"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.53"
+version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64c122667b287044802d6ce17ee2ddf13207ed924c712de9a66a5814d5b64765"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "winapi",
+ "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.7"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adab1eaa3408fb7f0c777a73e7465fd5656136fc93b670eb6df3c88c2c1344e3"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "js-sys"
-version = "0.3.60"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49409df3e3bf0856b916e2ceaca09ee28e6871cf7d9ce97a692cacfdb2a25a47"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.138"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db6d7e329c562c5dfab7a46a2afabc8b987ab9a4834c9d1ca04dc54c1546cef8"
-
-[[package]]
-name = "link-cplusplus"
-version = "1.0.7"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9272ab7b96c9046fbc5bc56c06c117cb639fe2d509df0c421cad82d2915cf369"
-dependencies = [
- "cc",
-]
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "memoffset"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
-
-[[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.16.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f0b0d4bf799edbc74508c1e8bf170ff5f41238e5f8225603ca7caaae2b7860"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.5"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff9f3fef3968a3ec5945535ed654cb38ff72d7495a25619e2247fb15a2ed9ba"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.47"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ea3d908b0e36316caf9e9e2c4625cdde190a7e6f440d794667ed17a1855e725"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.17.3"
@@ -334,178 +263,168 @@
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.21"
+version = "1.0.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
+checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
-
-[[package]]
-name = "scratch"
-version = "1.0.2"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c8132065adcfd6e02db789d9285a0deb2f3fcb04002865ab67d5fb103533898"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
-version = "1.0.105"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60b9b43d45702de4c839cb9b51d9f529c5dd26a4aff255b42b1ebc03e88ee908"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "target-lexicon"
-version = "0.12.5"
+name = "syn"
+version = "2.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
 
 [[package]]
-name = "termcolor"
-version = "1.1.3"
+name = "target-lexicon"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
-dependencies = [
- "winapi-util",
-]
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "time"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
 dependencies = [
  "libc",
  "wasi",
  "winapi",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.5"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ceab39d59e4c9499d4e5a8ee0e2735b891bb7308ac83dfb4e80cad195c9f6f3"
-
-[[package]]
-name = "unicode-width"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ee9362deb4a96cef4d437d1ad49cffc9b9e92d202b6995674e928ce684f112"
+checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "wasi"
 version = "0.10.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaf9f5aceeec8be17c128b2e93e031fb8a4d469bb9c4ae2d7dc1888b26887268"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.27",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "052be0f94026e6cbc75cdefc9bae13fd6052cdcaf532fa6c45e7ae33a1e6c810"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.27",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -516,77 +435,77 @@
 [[package]]
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
-name = "winapi-util"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
-dependencies = [
- "winapi",
-]
-
-[[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `floodgate_rs-0.1.2/PKG-INFO` & `floodgate_rs-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floodgate-rs
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python bindings for, a ratelimiting library written in Rust.
 Keywords: cooldown,ratelimit,rate limit,rust,pyo3
 License: MIT
```

