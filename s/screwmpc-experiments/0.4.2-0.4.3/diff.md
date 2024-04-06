# Comparing `tmp/screwmpc_experiments-0.4.2.tar.gz` & `tmp/screwmpc_experiments-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Mar 15 17:01:56 2024, max compression
+gzip compressed data, last modified: Sat Apr  6 14:46:00 2024, max compression
```

## Comparing `screwmpc_experiments-0.4.2.tar` & `screwmpc_experiments-0.4.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      380 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/.copier-answers.yml
--rw-r--r--   0        0        0      125 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/.gitattributes
--rw-r--r--   0        0        0     2314 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/.readthedocs.yaml
--rw-r--r--   0        0        0     2768 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/noxfile.py
--rw-r--r--   0        0        0     2405 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      344 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1014 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1554 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      855 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/docs/conf.py
--rw-r--r--   0        0        0      207 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/docs/index.md
--rw-r--r--   0        0        0      425 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/docs/api/screwmpc_experiments.experiments.rst
--rw-r--r--   0        0        0      407 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/docs/api/screwmpc_experiments.launchers.rst
--rw-r--r--   0        0        0      278 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/docs/api/screwmpc_experiments.rst
--rw-r--r--   0        0        0      225 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/__init__.py
--rw-r--r--   0        0        0      411 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/_version.py
--rw-r--r--   0        0        0      118 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/_version.pyi
--rw-r--r--   0        0        0        0 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/py.typed
--rw-r--r--   0        0        0     1319 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/assets/pivoting.xml
--rw-r--r--   0        0        0     1001 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/assets/random.xml
--rw-r--r--   0        0        0        0 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/experiments/__init__.py
--rw-r--r--   0        0        0     4716 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/experiments/common.py
--rw-r--r--   0        0        0    23926 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/experiments/screwmpc.py
--rw-r--r--   0        0        0      577 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/launchers/__init__.py
--rw-r--r--   0        0        0     1476 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/launchers/pivoting.py
--rw-r--r--   0        0        0     2737 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/launchers/random.py
--rw-r--r--   0        0        0     8921 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/src/screwmpc_experiments/launchers/trigger_grasp.py
--rw-r--r--   0        0        0      197 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/tests/test_package.py
--rw-r--r--   0        0        0     2218 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/.gitignore
--rw-r--r--   0        0        0    11342 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/LICENSE
--rw-r--r--   0        0        0     1432 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/README.md
--rw-r--r--   0        0        0     4124 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    16145 2024-03-15 17:01:56.000000 screwmpc_experiments-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      380 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/.copier-answers.yml
+-rw-r--r--   0        0        0      125 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/.gitattributes
+-rw-r--r--   0        0        0     2314 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/.readthedocs.yaml
+-rw-r--r--   0        0        0     2768 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/noxfile.py
+-rw-r--r--   0        0        0     2405 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      344 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1014 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1554 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      855 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/docs/conf.py
+-rw-r--r--   0        0        0      207 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/docs/index.md
+-rw-r--r--   0        0        0      425 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/docs/api/screwmpc_experiments.experiments.rst
+-rw-r--r--   0        0        0      407 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/docs/api/screwmpc_experiments.launchers.rst
+-rw-r--r--   0        0        0      278 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/docs/api/screwmpc_experiments.rst
+-rw-r--r--   0        0        0      225 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/_version.py
+-rw-r--r--   0        0        0      118 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/_version.pyi
+-rw-r--r--   0        0        0        0 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/py.typed
+-rw-r--r--   0        0        0     1331 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/assets/pivoting.xml
+-rw-r--r--   0        0        0     1001 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/assets/random.xml
+-rw-r--r--   0        0        0        0 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/experiments/__init__.py
+-rw-r--r--   0        0        0     5651 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/experiments/common.py
+-rw-r--r--   0        0        0    27239 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/experiments/screwmpc.py
+-rw-r--r--   0        0        0      577 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/launchers/__init__.py
+-rw-r--r--   0        0        0     1431 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/launchers/pivoting.py
+-rw-r--r--   0        0        0     2697 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/launchers/random.py
+-rw-r--r--   0        0        0     8921 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/src/screwmpc_experiments/launchers/trigger_grasp.py
+-rw-r--r--   0        0        0      197 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/tests/test_package.py
+-rw-r--r--   0        0        0     2218 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/.gitignore
+-rw-r--r--   0        0        0    11342 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1432 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/README.md
+-rw-r--r--   0        0        0     4124 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    16145 2024-04-06 14:46:00.000000 screwmpc_experiments-0.4.3/PKG-INFO
```

### Comparing `screwmpc_experiments-0.4.2/.pre-commit-config.yaml` & `screwmpc_experiments-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `screwmpc_experiments-0.4.2/noxfile.py` & `screwmpc_experiments-0.4.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `screwmpc_experiments-0.4.2/.github/CONTRIBUTING.md` & `screwmpc_experiments-0.4.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `screwmpc_experiments-0.4.2/.github/matchers/pylint.json` & `screwmpc_experiments-0.4.3/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `screwmpc_experiments-0.4.2/.github/workflows/cd.yml` & `screwmpc_experiments-0.4.3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `screwmpc_experiments-0.4.2/.github/workflows/ci.yml` & `screwmpc_experiments-0.4.3/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -58,10 +58,10 @@
 
       - name: Test package
         run: >-
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
           --durations=20
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.1.1
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `screwmpc_experiments-0.4.2/docs/conf.py` & `screwmpc_experiments-0.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `screwmpc_experiments-0.4.2/src/screwmpc_experiments/assets/pivoting.xml` & `screwmpc_experiments-0.4.3/src/screwmpc_experiments/assets/random.xml`

 * *Files 12% similar despite different names*

#### Comparing `screwmpc_experiments-0.4.2/src/screwmpc_experiments/assets/pivoting.xml` & `screwmpc_experiments-0.4.3/src/screwmpc_experiments/assets/random.xml`

```diff
@@ -15,15 +15,9 @@
   </visual>
   <default>
     <geom solimp="0.9 0.95 0.001 0.5 2" solref="0.005 1" condim="6"/>
   </default>
   <worldbody>
     <geom name="floor" type="plane" size="2 2 2" conaffinity="1" material="grid"/>
     <light directional="true" diffuse=".7 .7 .7" pos="1 .1 2" dir="0 -.1 -2" specular=".3 .3 .3" castshadow="true"/>
-    <body>
-      <geom type="box" name="table_top" pos=".3 0 0.17" size=".2 .5 0.01"/>
-      <!-- surface at 0.17m + 0.01m = 0.18m-->
-      <geom type="box" name="table_column_a" pos=".3 .3 0.085 " size=".15 .15 0.085"/>
-      <geom type="box" name="table_column_b" pos=".3 -.3 0.085 " size=".15 .15 0.085"/>
-    </body>
   </worldbody>
 </mujoco>
```

### Comparing `screwmpc_experiments-0.4.2/src/screwmpc_experiments/assets/random.xml` & `screwmpc_experiments-0.4.3/src/screwmpc_experiments/assets/pivoting.xml`

 * *Files 18% similar despite different names*

#### Comparing `screwmpc_experiments-0.4.2/src/screwmpc_experiments/assets/random.xml` & `screwmpc_experiments-0.4.3/src/screwmpc_experiments/assets/pivoting.xml`

```diff
@@ -15,9 +15,15 @@
   </visual>
   <default>
     <geom solimp="0.9 0.95 0.001 0.5 2" solref="0.005 1" condim="6"/>
   </default>
   <worldbody>
     <geom name="floor" type="plane" size="2 2 2" conaffinity="1" material="grid"/>
     <light directional="true" diffuse=".7 .7 .7" pos="1 .1 2" dir="0 -.1 -2" specular=".3 .3 .3" castshadow="true"/>
+    <body>
+      <geom type="box" name="table_top" pos=".3 0 0.16" size=".2 .5 0.02" solref="0.2 1"/>
+      <!-- surface at 0.16m + 0.02m = 0.18m -->
+      <geom type="box" name="table_column_a" pos=".3 .3 0.07 " size=".15 .15 0.07"/>
+      <geom type="box" name="table_column_b" pos=".3 -.3 0.07 " size=".15 .15 0.07"/>
+    </body>
   </worldbody>
 </mujoco>
```

### Comparing `screwmpc_experiments-0.4.2/src/screwmpc_experiments/experiments/common.py` & `screwmpc_experiments-0.4.3/src/screwmpc_experiments/experiments/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,46 +16,64 @@
 from panda_py import constants
 
 from . import screwmpc
 
 
 def create_environment(
     xml_path: pathlib.Path, args: argparse.Namespace
-) -> tuple[environment.PandaEnvironment, params.RobotParams]:
+) -> tuple[environment.PandaEnvironment, params.RobotParams, screwmpc.ScrewMPCAgent]:
     """Creates the basic environment for the experiments."""
+    agent = create_agent(args)
+
     if not args.move_to_start and args.robot_ip is not None:
         q = panda_py.Panda(args.robot_ip).q
     else:
         q = constants.JOINT_POSITION_START
+        # q = np.array([-0.13083284218478622, -0.6435437375202514, -1.2014952440764255, -1.3871403382451892, 0.2967545260853238, 1.124549853383633, 2.329884358906789])
     robot_params = params.RobotParams(
         robot_ip=args.robot_ip,
         joint_positions=q,
         actuation=arm_constants.Actuation.JOINT_VELOCITY,
         enforce_realtime=args.realtime_priority,
     )
-    goal = screwmpc.Goal()
+    goal = screwmpc.Goal(color=(0, 1, 0, 0.3))
     arena = composer.Arena(xml_path=xml_path)
     arena.attach(goal)
+    intermediate = []
+    blend = np.linspace(0, 1, 10)
+
+    if args.visualize_sclerp:
+        for i in range(10):
+            intermediate.append(screwmpc.Goal(color=(1 - blend[i], blend[i], 0, 0.3)))
+            arena.attach(intermediate[-1])
 
-    panda_env = environment.PandaEnvironment(robot_params, arena, control_timestep=0.02)
+    panda_env = environment.PandaEnvironment(
+        robot_params, arena, control_timestep=0.02, physics_timestep=0.001
+    )
 
     # Add extra sensors for flange and goal reference sites
     # to make them observable to the agent and preprocessors.
     flange_sensor = site_sensor.SiteSensor(
         panda_env.robots["panda"].arm.mjcf_model.find("site", "real_aligned_tcp"),
         "flange",
     )
     goal_sensor = site_sensor.SiteSensor(
         goal.mjcf_model.find("site", "panda_hand/wrist_site"), "goal"
     )
 
     panda_env.add_extra_sensors([flange_sensor, goal_sensor])
-    panda_env.add_extra_effectors([screwmpc.SceneEffector(goal)])
+    panda_env.add_extra_effectors([screwmpc.SceneEffector(goal, intermediate)])
     panda_env.add_timestep_preprocessors(
         [
+            # observation_transforms.AddObservation(
+            #     "u_state", agent.get_u_state_observation
+            # ),
+            # observation_transforms.AddObservation(
+            #     "mpc_state", agent.get_mpc_state_observation
+            # ),
             observation_transforms.AddObservation(
                 "manipulability",
                 screwmpc.manipulability,
                 specs.Array((1,), dtype=np.float32),
             ),
             rewards.ComputeReward(screwmpc.goal_reward),
             observation_transforms.RetainObservations(
@@ -67,15 +85,15 @@
                     "panda_tcp_quat",
                     "panda_force",
                     "panda_torque",
                 ]
             ),
         ]
     )
-    return panda_env, robot_params
+    return panda_env, robot_params, agent
 
 
 def create_argparser() -> argparse.ArgumentParser:
     """Create argument parser with common arguments for all experiments."""
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
@@ -119,24 +137,28 @@
         default=2.0,
     )
     parser.add_argument(
         "--move-to-start",
         action="store_true",
         help="move the robot into the start position in the beginning",
     )
+    parser.add_argument(
+        "--visualize-sclerp",
+        action="store_true",
+        help="visualize sclerp poses",
+    )
     return parser
 
 
 def create_agent(
-    env: subtask_env.SubTaskEnvironment,
     args: argparse.Namespace,
 ) -> screwmpc.ScrewMPCAgent:
     """Creates a screwmpc.ScrewMPCAgent from a moma subtask environment and arguments."""
     return screwmpc.ScrewMPCAgent(
-        env.action_spec(),
+        specs.BoundedArray((86,), np.float64, -np.inf, np.inf),
         args.goal_tolerance,
         args.sclerp,
         args.manipulability,
         args.output,
         grasp_time=args.grasp_time,
     )
```

### Comparing `screwmpc_experiments-0.4.2/src/screwmpc_experiments/experiments/screwmpc.py` & `screwmpc_experiments-0.4.3/src/screwmpc_experiments/experiments/screwmpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 
 import csv
 import logging
 import pathlib
 import threading
 import time
 import typing
+from collections import deque
 from xmlrpc import server
 
 import dm_env
 import dm_robotics.panda
 import dqrobotics
+import mujoco
 import numpy as np
 import panda_py
 import roboticstoolbox as rtb
 import spatialmath
 from dm_control import mjcf
+from dm_control.viewer import application, renderer, user_input
 from dm_env import specs
 from dm_robotics.agentflow import spec_utils
 from dm_robotics.agentflow.preprocessors import timestep_preprocessor
 from dm_robotics.geometry import pose_distribution
 from dm_robotics.moma import effector, prop, subtask_env
 from dm_robotics.panda import utils
 from dm_robotics.transformations import transformations as tr
@@ -95,14 +98,15 @@
         use_mp: bool = False,
         output_file: str = "obs.csv",
         grasp_time: float = 2.0,
     ) -> None:
         self._spec = spec
         self._goal_tolerance = goal_tolerance
         self._waypoints: list[tuple[np.ndarray, np.ndarray, int]] = []
+        self._intermediate: list[tuple[np.ndarray, np.ndarray, int]] | None = None
         self._goal: dqrobotics.DQ | None = None
         self._x_goal: tuple[np.ndarray, np.ndarray, float] | None = None
         self._obs: list[dict[str, np.ndarray]] = []
         self._output_file = output_file
         self._finished = False
         self._dead_time = 0.0
         self._grasp_time = grasp_time
@@ -122,41 +126,85 @@
         if self._goal is not None:
             # set joint velocities to mpc output
             action[:7] = self.motion_generator.step(
                 timestep.observation["panda_joint_pos"], self._goal
             )
         if self._x_goal is not None:
             # set goal object pose
-            action[-8:] = np.r_[self._x_goal[0], self._x_goal[1], self._x_goal[2]]
+            action[8:16] = np.r_[self._x_goal[0], self._x_goal[1], self._x_goal[2]]
             action[7] = self._x_goal[2]
+
+            if self._intermediate is not None:
+                for i in range(10):
+                    action[i * 7 + 16 : i * 7 + 16 + 7] = np.r_[
+                        self._intermediate[i][0], self._intermediate[i][1].vec
+                    ]
+
+            # joint_positions = panda_py.fk(timestep.observation["panda_joint_pos"])
+            # start = spatialmath.SE3(joint_positions)
+            # start *= T_F_EE.inv()
+
+            # intermediate = dqutil.interpolate_waypoints(
+            #     [
+            #         (start.t, spatialmath.UnitQuaternion(start)),
+            #         (self._x_goal[0], spatialmath.UnitQuaternion(self._x_goal[1])),
+            #     ],
+            #     10,
+            # )[1:-1]
+
+            # for i in range(10):
+            #     action[i * 7 + 16 : i * 7 + 16 + 7] = np.r_[
+            #         intermediate[i][0], intermediate[i][1].vec
+            #     ]
         if self.at_goal(timestep):
             logger.info("Goal reached.")
             self._goal = None
+            self.motion_generator.reset()
         if not self._finished:
             self._obs.append(timestep.observation)
         if (
             not self._finished
             and self._goal is None
             and self._dead_time < timestep.observation["time"][0]
         ):
             try:
                 x_goal = self._waypoints.pop(0)
                 self._goal = pose_to_dq(x_goal)
+
                 if (
                     self._x_goal is not None
                     and np.all(x_goal[0] == self._x_goal[0])
                     and np.all(x_goal[1] == self._x_goal[1])
                     and x_goal[2] != self._x_goal[2]
                 ):
                     logger.info("Grasping")
                     self._dead_time = timestep.observation["time"][0] + self._grasp_time
                 else:
                     logger.info("Tracking new goal: %s", self._goal)
+
+                    joint_positions = panda_py.fk(
+                        timestep.observation["panda_joint_pos"]
+                    )
+                    start = spatialmath.SE3(joint_positions)
+                    start *= T_F_EE.inv()
+
+                    self._intermediate = dqutil.interpolate_waypoints(
+                        [
+                            (start.t, spatialmath.UnitQuaternion(start)),
+                            (
+                                x_goal[0],
+                                spatialmath.UnitQuaternion(x_goal[1]),
+                            ),
+                        ],
+                        10,
+                    )[1:-1]
+
                 self._x_goal = x_goal
-                action[-8:] = np.r_[self._x_goal[0], self._x_goal[1], self._x_goal[2]]
+                action[8:16] = np.r_[self._x_goal[0], self._x_goal[1], self._x_goal[2]]
+
             except IndexError:
                 self._finished = True
                 self._dead_time = 0
                 logger.info("Saving observations to %s", self._output_file)
                 save_obs(self._obs, self._output_file)
         return action
 
@@ -188,14 +236,28 @@
         """
         if waypoints is None:
             return
         self._waypoints.extend(waypoints)
         logger.info("Added %d new waypoints to buffer", len(waypoints))
         self._finished = False
 
+    def get_u_state_observation(
+        self, timestep: timestep_preprocessor.PreprocessorTimestep
+    ) -> np.ndarray:
+        """Retrieves the motion generator's internal `u` state observation."""
+        del timestep
+        return self.motion_generator.u_state
+
+    def get_mpc_state_observation(
+        self, timestep: timestep_preprocessor.PreprocessorTimestep
+    ) -> np.ndarray:
+        """Retrieves the motion generator's internal `mpc` state observation."""
+        del timestep
+        return self.motion_generator.mpc_state
+
 
 class RPCInterface:
     """Remote procedure call interface to interact with the simulation."""
 
     def __init__(
         self,
         agent: ScrewMPCAgent,
@@ -372,87 +434,99 @@
         self._thread.join()
         self._collision_env.close()
 
 
 class Goal(prop.Prop):  # type: ignore[misc]
     """Intangible prop representing the goal pose."""
 
-    def _build(self) -> None:  # pylint: disable=arguments-differ
+    def _build(self, color: tuple[float, float, float, float] = (1, 0, 0, 0.3)) -> None:  # pylint: disable=arguments-differ
         xml_path = (
             pathlib.Path(pathlib.Path(dm_robotics.panda.__file__).parent)
             / "assets"
             / "panda"
             / "panda_hand.xml"
         )
         mjcf_root = mjcf.from_path(xml_path)
         for geom in mjcf_root.find_all("geom"):
-            geom.rgba = (1, 0, 0, 0.3)
+            geom.rgba = color
             geom.conaffinity = 0
             geom.contype = 0
         rotated_root = mjcf.RootElement()
         rotated_root.worldbody.add("body", name="rotated_root").add(
             "site", euler=[0, 0, -0.7854]
         ).attach(mjcf_root)
         super()._build("goal", rotated_root, "rotated_root")
 
 
 class SceneEffector(effector.Effector):  # type: ignore[misc]
     """
     Effector used to update the state of the scene.
     """
 
-    def __init__(self, goal: Goal) -> None:
+    def __init__(self, goal: Goal, intermediate: list[Goal]) -> None:
         self._goal = goal
+        self._intermediate = intermediate
         self._actuator = goal.mjcf_model.find(
             "actuator", "panda_hand/panda_hand_actuator"
         )
+        self._intermediate_actuator = []
+        for i in self._intermediate:
+            self._intermediate_actuator.append(
+                i.mjcf_model.find("actuator", "panda_hand/panda_hand_actuator")
+            )
         self._spec = None
 
     def close(self) -> None:
         pass
 
     def initialize_episode(
         self, physics: mjcf.Physics, random_state: np.random.RandomState
     ) -> None:
         pass
 
     def action_spec(self, physics: mjcf.Physics) -> specs.BoundedArray:
         del physics
         if self._spec is None:
             self._spec = specs.BoundedArray(
-                (8,),
+                (78,),
                 np.float32,
-                np.full((8,), -10, dtype=np.float32),
-                np.full((8,), 10, dtype=np.float32),
+                np.full((78,), -10, dtype=np.float32),
+                np.full((78,), 10, dtype=np.float32),
                 "\t".join(
                     [
                         f"{self.prefix}_{n}"
                         for n in [
                             "goal_x",
                             "goal_y",
                             "goal_z",
                             "goal_qw",
                             "goal_qx",
                             "goal_qy",
                             "goal_qz",
                             "goal_grasp",
                         ]
+                        + [f"intermediate_{i}" for i in range(70)]
                     ]
                 ),
             )
         return self._spec
 
     @property
     def prefix(self) -> str:
         return "scene"
 
     def set_control(self, physics: mjcf.Physics, command: np.ndarray) -> None:
         pos = command[:3]
-        self._goal.set_pose(physics, pos, command[3:-1])
-        physics.bind(self._actuator).ctrl = command[-1]
+        self._goal.set_pose(physics, pos, command[3:7])
+        physics.bind(self._actuator).ctrl = command[7]
+
+        for i, __ in enumerate(self._intermediate):
+            subcommand = command[(i + 1) * 7 + 1 : (i + 1) * 7 + 8]
+            self._intermediate[i].set_pose(physics, subcommand[:3], subcommand[3:7])
+            physics.bind(self._intermediate_actuator).ctrl = command[7]
 
 
 def goal_reward(observation: spec_utils.ObservationValue) -> float:
     """Computes a reward based on distance between end-effector and goal."""
     pos_distance = np.linalg.norm(observation["goal_pos"] - observation["flange_pos"])
     rot_dist = tr.quat_dist(observation["goal_quat"], observation["flange_quat"])
     return float(-pos_distance - rot_dist / np.pi)
@@ -493,62 +567,61 @@
                     else:
                         new_row[key] = value[0]
                 else:
                     new_row[key] = value.item()  # Convert 0-d array to scalar
             writer.writerow(new_row)
 
 
+class ScrewMPCActionPlot(utils.ActionPlot):  # type: ignore[misc]
+    """A plotting component for :py:class:`dm_control.viewer.application.Application`
+    that plots the agent's actions in a screwmpc experiment.
+    """
+
+    def _init_buffer(self) -> None:
+        self.maxlines = 8
+        for _1 in range(self.maxlines):
+            self.y.append(deque(maxlen=self.maxlen))
+        self.reset_data()
+
+    def render(self, context: mujoco.MjrContext, viewport: renderer.Viewport) -> None:
+        if self._rt._time_step is None or self._rt.last_action is None:  # pylint: disable=protected-access
+            return
+        for i, a in enumerate(self._rt.last_action):
+            if i > 7:
+                break
+            self.fig.linepnt[i] = self.maxlen
+            self.y[i].append(a)
+            self.fig.linedata[i][: self.maxlen * 2] = np.array(
+                [self.x, self.y[i]]
+            ).T.reshape((-1,))
+        pos = mujoco.MjrRect(300 + 5, viewport.height - 200 - 5, 300, 200)  # pylint: disable=no-member
+        mujoco.mjr_figure(pos, self.fig, context.ptr)  # pylint: disable=no-member
+
+
 class ScrewMPCApp(utils.ApplicationWithPlot):  # type: ignore[misc]
     """Extends the GUI application with RPC functionality."""
 
     def __init__(
         self,
         title: str = "ScrewMPC Experiment",
         width: int = 1024,
         height: int = 768,
-        box: prop.Block = None,
     ):
         super().__init__(title, width, height)
         self._viewer.render_settings.toggle_rendering_flag(0)
         self._viewer.render_settings.toggle_rendering_flag(2)
-        self._box = box
-        self.server = server.SimpleXMLRPCServer(
-            ("0.0.0.0", 9001), allow_none=True, logRequests=False
-        )
-        self.server.register_function(self.reload_box, "reload_box")
-        self._thread = threading.Thread(target=self.server.serve_forever)
-        self._thread.start()
 
-    def reload_box(
-        self,
-        pose: tuple[np.ndarray, np.ndarray] | None = None,
-        size: np.ndarray | None = None,
-    ) -> None:
-        """Reload the bounding box object with new size and pose."""
-        if self._box is None or pose is None or size is None:
-            return
-        self._box.mjcf_model.find("geom", "body").size[:] = size
-        self._box.mjcf_model.find("geom", "body").pos[:] = pose[0]
-        self._box.mjcf_model.find("geom", "body").quat[:] = pose[1]
-        logger.info("Updating bounding box object")
-        self._restart_runtime()
-
-    def launch(
-        self,
-        environment_loader: subtask_env.SubTaskEnvironment,
-        policy: typing.Callable[[dm_env.TimeStep], np.ndarray] | None = None,
-    ) -> None:
-        super().launch(environment_loader, policy)
-        self.shutdown()
-
-    def shutdown(self) -> None:
-        """Shut down the server and close any open connections."""
-        self.server.shutdown()
-        self.server.socket.close()
-        self._thread.join()
+    def _perform_deferred_reload(self, params: application.ReloadParams) -> None:
+        application.Application._perform_deferred_reload(self, params)  # pylint: disable=protected-access
+        cmp = utils.ObservationPlot(self._runtime)
+        self._renderer.components += cmp
+        self._renderer.components += ScrewMPCActionPlot(self._runtime)
+        self._renderer.components += utils.RewardPlot(self._runtime)
+        self._input_map.bind(cmp.next_obs, user_input.KEY_F4)
+        self._input_map.bind(cmp.prev_obs, user_input.KEY_F3)
 
 
 class Box(prop.Prop):  # type: ignore[misc]
     """The bounding box object."""
 
     def _build(  # pylint:disable=arguments-renamed
         self,
@@ -575,32 +648,32 @@
     box = prop_root.add(
         "geom",
         name="body",
         type="box",
         pos=pos,
         quat=quat,
         size=size,
-        mass=0.10,
+        mass=0.01,
         solref=solref,
         solimp=solimp,
-        condim=4,
+        condim=1,
         rgba=color,
     )
     del box
     return mjcf_root
 
 
 def compute_trajectory(
     motion_generator: pandamg.PandaScrewMotionGenerator,
     q_init: np.ndarray,
     x_d: dqrobotics.DQ,
     dt: float = 0.001,
     linear_threshold: float = 0.05,
     angular_threshold: float = 5,
-    max_steps: int = 100,
+    max_steps: int = 1000,
 ) -> tuple[list[np.ndarray], bool]:
     """Offline computation of trajectory from `q_init` to `x_d`."""
     q_robot: np.ndarray = q_init.copy()
     joint_angles: list[np.ndarray] = [q_init]
     step: int = 0
     done: bool = False
     goal_pose = dqutil.dq_to_pose(x_d)
```

### Comparing `screwmpc_experiments-0.4.2/src/screwmpc_experiments/launchers/__init__.py` & `screwmpc_experiments-0.4.3/src/screwmpc_experiments/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `screwmpc_experiments-0.4.2/src/screwmpc_experiments/launchers/pivoting.py` & `screwmpc_experiments-0.4.3/src/screwmpc_experiments/launchers/pivoting.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,26 @@
 def main() -> None:
     """
     Main function of this experiment.
     Run from the terminal by executing `screwmpc-pivoting`.
     """
     args = common.create_argparser().parse_args()
     xml_path = pathlib.Path(__file__).parent / ".." / "assets" / "pivoting.xml"
-    panda_env, __ = common.create_environment(xml_path, args)
+    panda_env, __, agent = common.create_environment(xml_path, args)
     args.robot_ip = None
-    collision_env, __ = common.create_environment(xml_path, args)
+    collision_env, __, __ = common.create_environment(xml_path, args)
     collision_env.add_props([screwmpc.Box(pos=[0.3, 0, 0.3])])
 
     box = screwmpc.Box(pos=[0.3, 0, 0.3])
     panda_env.add_props([box])
 
     with panda_env.build_task_environment() as env:
-        agent = common.create_agent(env, args)
         # Run the environment and agent either in headless mode or inside the GUI.
         if not args.no_gui:
-            app = screwmpc.ScrewMPCApp("Screw MPC Pivoting Experiment", box=box)
+            app = screwmpc.ScrewMPCApp("Screw MPC Pivoting Experiment")
             rpc = screwmpc.RPCInterface(
                 agent, env, collision_env.build_task_environment(), gui=app
             )
             app.launch(env, policy=agent.step)
         else:
             rpc = screwmpc.RPCInterface(
                 agent, env, collision_env.build_task_environment()
```

### Comparing `screwmpc_experiments-0.4.2/src/screwmpc_experiments/launchers/random.py` & `screwmpc_experiments-0.4.3/src/screwmpc_experiments/launchers/random.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         help="rotation delta for random poses (default: 45 45 45)",
     )
     parser.add_argument(
         "-n", type=int, help="number of random poses (default: 10)", default=10
     )
     xml_path = pathlib.Path(__file__).parent / ".." / "assets" / "random.xml"
     args = parser.parse_args()
-    panda_env, robot_params = common.create_environment(xml_path, args)
+    panda_env, robot_params, agent = common.create_environment(xml_path, args)
 
     with panda_env.build_task_environment() as env:
         rng = np.random.RandomState(seed=args.seed)  # pylint: disable=no-member
 
         # Generate 10 random poses within these bounds centered around the starting pose
         # given as x, y, z (linear) and X, Y, Z (angular, euler angles)
         dp = args.position_delta
@@ -72,15 +72,14 @@
                 0 + dr[1],
                 0.25 * np.pi + dr[2],
             ]
         )
         poses = screwmpc.generate_random_poses(
             args.n, robot_params.joint_positions, min_pose_bounds, max_pose_bounds, rng
         )
-        agent = common.create_agent(env, args)
         agent.add_waypoints(poses)
 
         # Run the environment and agent either in headless mode or inside the GUI.
         if not args.no_gui:
             app = screwmpc.ScrewMPCApp(title="ScrewMPC Random Experiment")
             app.launch(env, policy=agent.step)
         else:
```

### Comparing `screwmpc_experiments-0.4.2/src/screwmpc_experiments/launchers/trigger_grasp.py` & `screwmpc_experiments-0.4.3/src/screwmpc_experiments/launchers/trigger_grasp.py`

 * *Files identical despite different names*

### Comparing `screwmpc_experiments-0.4.2/.gitignore` & `screwmpc_experiments-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `screwmpc_experiments-0.4.2/LICENSE` & `screwmpc_experiments-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `screwmpc_experiments-0.4.2/README.md` & `screwmpc_experiments-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `screwmpc_experiments-0.4.2/pyproject.toml` & `screwmpc_experiments-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   "Programming Language :: Python :: 3.10",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
   "dm-robotics-panda >= 0.4.7",
-  "screwmpcpy >= 0.4.1",
+  "screwmpcpy >= 0.5.0",
 ]
 
 [project.scripts]
 screwmpc-random = "screwmpc_experiments.launchers.random:main"
 screwmpc-pivoting = "screwmpc_experiments.launchers.pivoting:main"
 screwmpc-trigger-grasp = "screwmpc_experiments.launchers.trigger_grasp:main"
```

### Comparing `screwmpc_experiments-0.4.2/PKG-INFO` & `screwmpc_experiments-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: screwmpc-experiments
-Version: 0.4.2
+Version: 0.4.3
 Summary: Experiments based on screwmpc.
 Project-URL: Homepage, https://github.com/JeanElsner/screwmpc-experiments
 Project-URL: Bug Tracker, https://github.com/JeanElsner/screwmpc-experiments/issues
 Project-URL: Discussions, https://github.com/JeanElsner/screwmpc-experiments/discussions
 Project-URL: Changelog, https://github.com/JeanElsner/screwmpc-experiments/releases
 Author-email: Jean Elsner <jean.elsner@tum.de>
 License: 
@@ -221,15 +221,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: <3.11,>=3.8
 Requires-Dist: dm-robotics-panda>=0.4.7
-Requires-Dist: screwmpcpy>=0.4.1
+Requires-Dist: screwmpcpy>=0.5.0
 Provides-Extra: dev
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo>=2023.08.17; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
```

