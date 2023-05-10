# Comparing `tmp/VirxERLU_RLib-1.1.0.tar.gz` & `tmp/VirxERLU_RLib-1.1.1.tar.gz`

## Comparing `VirxERLU_RLib-1.1.0.tar` & `VirxERLU_RLib-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 VirxERLU_RLib-1.1.0/Cargo.toml
--rw-r--r--   0     1001      123     3406 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/README.md
--rw-r--r--   0     1001      123      597 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/pyproject.toml
--rw-r--r--   0     1001      123     8400 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/src/air.rs
--rw-r--r--   0     1001      123    11814 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/src/analyzer.rs
--rw-r--r--   0     1001      123    18566 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/src/car.rs
--rw-r--r--   0     1001      123     2956 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/src/constants.rs
--rw-r--r--   0     1001      123     7688 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/src/ground.rs
--rw-r--r--   0     1001      123    19211 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/src/lib.rs
--rw-r--r--   0     1001      123    10661 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/src/pytypes.rs
--rw-r--r--   0     1001      123     8609 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/src/shot.rs
--rw-r--r--   0     1001      123     6345 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/src/utils.rs
--rw-r--r--   0     1001      123     4764 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/virx_erlu_rlib.pyi
--rw-r--r--   0     1001      123    12715 2023-03-10 14:07:49.000000 VirxERLU_RLib-1.1.0/Cargo.lock
--rw-r--r--   0        0        0     4211 1970-01-01 00:00:00.000000 VirxERLU_RLib-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 VirxERLU_RLib-1.1.1/Cargo.toml
+-rw-r--r--   0     1001      123     3406 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/README.md
+-rw-r--r--   0     1001      123      597 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/pyproject.toml
+-rw-r--r--   0     1001      123     8401 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/air.rs
+-rw-r--r--   0     1001      123    11816 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/analyzer.rs
+-rw-r--r--   0     1001      123    18567 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/car.rs
+-rw-r--r--   0     1001      123     2956 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/constants.rs
+-rw-r--r--   0     1001      123     7690 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/ground.rs
+-rw-r--r--   0     1001      123    19062 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/lib.rs
+-rw-r--r--   0     1001      123    10689 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/pytypes.rs
+-rw-r--r--   0     1001      123     8610 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/shot.rs
+-rw-r--r--   0     1001      123     6345 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/utils.rs
+-rw-r--r--   0     1001      123     4764 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/virx_erlu_rlib.pyi
+-rw-r--r--   0     1001      123    12715 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/Cargo.lock
+-rw-r--r--   0        0        0     4211 1970-01-01 00:00:00.000000 VirxERLU_RLib-1.1.1/PKG-INFO
```

### Comparing `VirxERLU_RLib-1.1.0/Cargo.toml` & `VirxERLU_RLib-1.1.1/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "virx_erlu_rlib"
-version = "1.1.0"
+version = "1.1.1"
 edition = "2021"
 authors = ["VirxEC <virx@virxcase.dev>"]
 readme = "README.md"
 description = "Rust modules for VirxERLU"
 homepage = "https://github.com/VirxEC/VirxERLU-RLib"
 license = "MIT"
 include = ["/src", "pyproject.toml", "virx_erlu_rlib.pyi", "/README.md"]
@@ -15,24 +15,24 @@
 
 [lib]
 name = "virx_erlu_rlib"
 crate-type = ["cdylib"]
 path = "src/lib.rs"
 
 [dependencies]
-dubins_paths = { version = "1.4.4", features = ["fast-math"] }
+dubins_paths = { version = "1.6.0", features = ["glam"] }
 combo_vec = "0.5.1"
 
 [dependencies.rl_ball_sym]
 version = "3.0.0"
 default-features = false
 features = ["stable-compression", "standard", "dropshot", "hoops", "throwback"]
 
 [dependencies.glam]
-version = "0.23.0"
+version = "0.24.0"
 features = ["fast-math"]
 
 [dependencies.pyo3]
 version = "0.18.1"
 features = ["extension-module", "abi3-py37"]
 
 [dev-dependencies]
```

### Comparing `VirxERLU_RLib-1.1.0/README.md` & `VirxERLU_RLib-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `VirxERLU_RLib-1.1.0/pyproject.toml` & `VirxERLU_RLib-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `VirxERLU_RLib-1.1.0/src/air.rs` & `VirxERLU_RLib-1.1.1/src/air.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 use std::f32::consts::PI;
 
+use dubins_paths::{NoPathError, Result as DubinsResult};
+use glam::Vec3A;
+
 use crate::{
     car::Car,
     constants::*,
     pytypes::{BasicShotInfo, ShotType},
     BoostAmount, Mutators,
 };
-use dubins_paths::{NoPathError, Result as DubinsResult};
-use glam::Vec3A;
 
 #[inline]
 fn angle_3d(a: Vec3A, b: Vec3A) -> f32 {
     a.dot(b).clamp(-1., 1.).acos()
 }
 
 #[derive(Debug)]
```

### Comparing `VirxERLU_RLib-1.1.0/src/analyzer.rs` & `VirxERLU_RLib-1.1.1/src/analyzer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+use std::f32::consts::PI;
+
+use dubins_paths::{mod2pi, DubinsPath, NoPathError, PathType, PosRot, Result as DubinsResult};
+use glam::Vec3A;
+use rl_ball_sym::simulation::ball::Ball;
+
 use crate::{
     air::{aerial_shot_is_viable, AerialTargetInfo},
     car::Car,
     ground::{angle_2d, get_turn_exit_tanget, shortest_path_in_validate, GroundTargetInfo},
     pytypes::ShotType,
     utils::flatten,
     Mutators,
 };
-use dubins_paths::{mod2pi, DubinsPath, NoPathError, PathType, PosRot, Result as DubinsResult};
-use glam::Vec3A;
-use rl_ball_sym::simulation::ball::Ball;
-use std::f32::consts::PI;
 
 #[derive(Clone, Copy, Debug, PartialEq, Eq)]
 enum Shot {
     Ground,
     Jump,
     DoubleJump,
     Aerial,
```

### Comparing `VirxERLU_RLib-1.1.0/src/car.rs` & `VirxERLU_RLib-1.1.1/src/car.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+use dubins_paths::DubinsPath;
+use glam::Vec3A;
+
 use crate::{
     constants::*,
     pytypes::{GameCar, Hitbox},
     utils::{flatten, minimum_non_negative, vertex_quadratic_solve_for_x},
     BoostAmount, Mutators,
 };
-use dubins_paths::DubinsPath;
-use glam::Vec3A;
 
 pub fn throttle_acceleration(forward_velocity: f32) -> f32 {
     let x = forward_velocity.abs();
 
     if x >= MAX_SPEED_NO_BOOST {
         return 0.;
     }
```

### Comparing `VirxERLU_RLib-1.1.0/src/constants.rs` & `VirxERLU_RLib-1.1.1/src/constants.rs`

 * *Files identical despite different names*

### Comparing `VirxERLU_RLib-1.1.0/src/ground.rs` & `VirxERLU_RLib-1.1.1/src/ground.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+use std::f32::{consts::E, INFINITY};
+
+use dubins_paths::{DubinsPath, Intermediate, NoPathError, PathType, PosRot, Result as DubinsResult};
+use glam::Vec3A;
+
 use crate::{
     car::{throttle_acceleration, Car, FieldRect},
     constants::*,
     pytypes::{BasicShotInfo, ShotType},
     utils::*,
     BoostAmount, Mutators,
 };
-use dubins_paths::{DubinsPath, Intermediate, NoPathError, PathType, PosRot, Result as DubinsResult};
-use glam::Vec3A;
-use std::f32::{consts::E, INFINITY};
 
 /// <https://stackoverflow.com/a/49987361/10930209>
 fn get_turn_exit_tangets(target: Vec3A, circle_center: Vec3A, radius: f32) -> (Vec3A, Vec3A) {
     let circle_center_to_target = target - circle_center;
     let b = circle_center_to_target.length();
     let th = (radius / b).acos();
     let d = circle_center_to_target.y.atan2(circle_center_to_target.x);
```

### Comparing `VirxERLU_RLib-1.1.0/src/lib.rs` & `VirxERLU_RLib-1.1.1/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 mod car;
 mod constants;
 mod ground;
 mod pytypes;
 mod shot;
 mod utils;
 
-use analyzer::*;
-use car::{turn_radius, Car};
+use std::sync::RwLock;
+
 use combo_vec::{rearr, ReArr};
-use constants::*;
 use glam::Vec3A;
 use pyo3::prelude::*;
-use pytypes::*;
 use rl_ball_sym::simulation::{
     ball::{Ball, Predictions},
     game::Game,
 };
+
+use analyzer::*;
+use car::{turn_radius, Car};
+use constants::*;
+use pytypes::*;
 use shot::{AirBasedShot, GroundBasedShot, Options, Shot, Target};
-use std::sync::RwLock;
 use utils::*;
 
 static CARS: RwLock<ReArr<Car, 8>> = RwLock::new(rearr![]);
 static BALL_STRUCT: RwLock<Predictions> = RwLock::new(Predictions::new());
 static GRAVITY: RwLock<Vec3A> = RwLock::new(Vec3A::ZERO);
 static GAME_TIME: RwLock<f32> = RwLock::new(0.);
 static GAME: RwLock<Option<Game>> = RwLock::new(None);
@@ -140,36 +142,33 @@
                 _ => BOOST_ACCEL,
             },
         })
     }
 }
 
 #[pyfunction]
-fn set_mutator_settings(py: Python, mutators: PyObject) -> PyResult<()> {
-    *MUTATORS.write().unwrap() = Mutators::try_from(mutators.as_ref(py))?;
+fn set_mutator_settings(mutators: &PyAny) -> PyResult<()> {
+    *MUTATORS.write().unwrap() = Mutators::try_from(mutators)?;
 
     Ok(())
 }
 
 #[pyfunction]
-fn tick(py: Python, packet: PyObject, prediction_time: Option<f32>) -> PyResult<()> {
+fn tick(packet: GamePacket, prediction_time: Option<f32>) -> PyResult<()> {
     TARGETS.write().unwrap().iter_mut().for_each(|target| {
         if matches!(target, Some(t) if !t.is_confirmed()) {
             *target = None;
         }
     });
 
     let mut game_guard = GAME.write().unwrap();
     let game = game_guard.as_mut().ok_or_else(|| PyErr::new::<NoGamePyErr, _>(NO_GAME_ERR))?;
 
     let mut ball = *BALL.read().unwrap();
 
-    let py_packet = packet.as_ref(py);
-    let packet = py_packet.extract::<GamePacket>()?;
-
     // Get general game information
     *GAME_TIME.write().unwrap() = packet.game_info.seconds_elapsed;
     game.gravity.z = packet.game_info.world_gravity_z;
     *GRAVITY.write().unwrap() = game.gravity;
 
     // Get information about the ball
     ball.update(
@@ -194,16 +193,16 @@
     let mut cars = CARS.write().unwrap();
 
     if cars.len() != packet.num_cars {
         const NEW_CAR: Car = Car::new();
         cars.resize(packet.num_cars, NEW_CAR);
     }
 
-    for (car, pycar) in cars.iter_mut().zip(py_packet.getattr("game_cars")?.iter()?) {
-        car.update(pycar?.extract()?, packet.game_info.seconds_elapsed);
+    for (car, pycar) in cars.iter_mut().zip(packet.game_cars.into_iter()) {
+        car.update(pycar, packet.game_info.seconds_elapsed);
     }
 
     Ok(())
 }
 
 #[pyfunction]
 fn get_slice(slice_time: f32) -> BallSlice {
```

### Comparing `VirxERLU_RLib-1.1.0/src/pytypes.rs` & `VirxERLU_RLib-1.1.1/src/pytypes.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+use glam::Vec3A;
+use pyo3::{pyclass, pymethods, FromPyObject};
+use rl_ball_sym::simulation::ball::Ball;
+
 use crate::{
     car::Car,
     constants::*,
     shot::{AirBasedShot, GroundBasedShot},
     utils::{flatten, get_tuple_from_vec3},
 };
-use glam::Vec3A;
-use pyo3::{pyclass, pymethods, FromPyObject};
-use rl_ball_sym::simulation::ball::Ball;
 
 #[derive(Clone, Copy, Debug, Default, FromPyObject)]
 pub struct Hitbox {
     pub length: f32,
     pub width: f32,
     pub height: f32,
 }
@@ -122,18 +123,19 @@
     pub boost: u8,
     pub jumped: bool,
     pub double_jumped: bool,
     pub is_demolished: bool,
     pub has_wheel_contact: bool,
 }
 
-#[derive(Clone, Copy, Debug, Default, FromPyObject)]
+#[derive(Clone, Debug, Default, FromPyObject)]
 pub struct GamePacket {
     pub game_info: GameInfo,
     pub game_ball: GameBall,
+    pub game_cars: Vec<GameCar>,
     pub num_cars: usize,
 }
 
 #[pyclass(frozen)]
 #[derive(Clone, Copy, Debug, PartialEq, Eq, Default)]
 pub enum ShotType {
     #[default]
```

### Comparing `VirxERLU_RLib-1.1.0/src/shot.rs` & `VirxERLU_RLib-1.1.1/src/shot.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+use dubins_paths::{DubinsPath, PosRot};
+use glam::Vec3A;
+use rl_ball_sym::simulation::ball::Ball;
+
 use crate::{
     air::{AerialJumpType, AerialTargetInfo},
     ground::GroundTargetInfo,
     pytypes::{ShotType, TargetOptions},
     utils::{get_samples_from_line, get_samples_from_path},
 };
-use dubins_paths::{DubinsPath, PosRot};
-use glam::Vec3A;
-use rl_ball_sym::simulation::ball::Ball;
 
 #[inline]
 const fn posrot_to_xy_tuple(posrot: &PosRot) -> (f32, f32) {
     let [x, y, _] = posrot.pos.to_array();
     (x, y)
 }
```

### Comparing `VirxERLU_RLib-1.1.0/src/utils.rs` & `VirxERLU_RLib-1.1.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `VirxERLU_RLib-1.1.0/virx_erlu_rlib.pyi` & `VirxERLU_RLib-1.1.1/virx_erlu_rlib.pyi`

 * *Files identical despite different names*

### Comparing `VirxERLU_RLib-1.1.0/Cargo.lock` & `VirxERLU_RLib-1.1.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -45,37 +45,37 @@
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "dubins_paths"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92c8960f5bd481ff20d4bd0125e0c8a9da6db5b74a85b0f038585319b662f572"
+checksum = "e24be98085e8b9dd5282d1b2d79ba5a41a69de8f19dcadca10ef7e81e584a84f"
 dependencies = [
  "glam",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "glam"
-version = "0.23.0"
+version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e4afd9ad95555081e109fe1d21f2a30c691b5f0919c67dfa690a2e1eb6bd51c"
+checksum = "ad83ab008a4fa3b31dfa713dd41b5a9bdea1e94e4cf1e2fc274ffbd49b0271d3"
 
 [[package]]
 name = "include-flate"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c2e11569346406931d20276cc460215ee2826e7cad43aa986999cb244dd7adb0"
 dependencies = [
@@ -117,17 +117,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libflate"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97822bf791bd4d5b403713886a5fbe8bf49520fe78e323b0dc480ca1a03e50b0"
 dependencies = [
@@ -203,86 +203,86 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radsort"
 version = "0.1.0"
@@ -326,17 +326,17 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rl_ball_sym"
-version = "3.0.0"
+version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25e5d69284d35ead07efc94858a851b225717f9c75b7a122ae06f0ac2a299f5d"
+checksum = "a742f7f8f7b1b7d3f1a75bdc6ed151d86cd83cb35dbc201314d7bbaf3cc4be65"
 dependencies = [
  "byteorder",
  "combo_vec",
  "glam",
  "include-flate",
  "radsort",
 ]
@@ -368,17 +368,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
@@ -386,15 +386,15 @@
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "virx_erlu_rlib"
-version = "1.1.0"
+version = "1.1.1"
 dependencies = [
  "combo_vec",
  "dubins_paths",
  "glam",
  "pyo3",
  "rand",
  "rl_ball_sym",
@@ -413,61 +413,61 @@
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
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
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
```

### Comparing `VirxERLU_RLib-1.1.0/PKG-INFO` & `VirxERLU_RLib-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VirxERLU-RLib
-Version: 1.1.0
+Version: 1.1.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

