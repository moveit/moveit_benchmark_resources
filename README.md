MoveIt Benchmark Resources
==========================

This repository includes various resources needed for MoveIt benchmarking.
Main purpose is to separate out large files like scene databases tracked with Git-LFS.

## Databases
The databases are created with [yaml_to_warehouse](https://github.com/mamoll/yaml_to_warehouse) based on Roboflex YAML files provided by the
author of [MotionBenchMaker](https://github.com/KavrakiLab/motion_bench_maker?tab=readme-ov-file#simple-usage) (see [full_dataset](https://rice.box.com/s/7uwuzor40vys1xx0xec4e8mxa8fkdtnn)).

- `panda_kitchen_test_db.sqlite`: Contains a scene `kitchen_panda_scene_sensed1` with multiple planning queries
- `panda_benchmarks.sqlite`: Contains different scenes with a motion planning query for each scene for a panda arm.
- `ur_benchmarks.sqlite`: Contains different scenes with a motion planning query for each scene for a ur5 arm.

Scene names (0001 - 0010) in `panda_benchmarks.sqlite` (ROBOT is `panda`) and `ur_benchmarks.sqlite` (ROBOT_NAME is `ur5`):
- `bookshelf_small_ROBOT/scene0001.yaml`
- `bookshelf_small_ROBOT/scene_sensed0001.yaml`
- `bookshelf_tall_ROBOT/scene0001.yaml`
- `bookshelf_tall_ROBOT/scene_sensed0001.yaml`
- `bookshelf_thin_ROBOT/scene0001.yaml`
- `bookshelf_thin_ROBOT/scene_sensed0001.yaml`
- `cage_ROBOT/scene0001.yaml`
- `cage_ROBOT/scene_sensed0001.yaml`
- `kitchen_ROBOT/scene0001.yaml`
- `kitchen_ROBOT/scene_sensed0001.yaml`
- `table_bars_ROBOT/scene0001.yaml`
- `table_bars_ROBOT/scene_sensed0001.yaml`
- `table_pick_ROBOT/scene0001.yaml`
- `table_pick_ROBOT/scene_sensed0001.yaml`
- `table_under_pick_ROBOT/scene0001.yaml`
- `table_under_pick_ROBOT/scene_sensed0001.yaml`

## Notes

Please install [git lfs](https://git-lfs.com/) by running `git lfs install` if you plan to use the sqlite test databases.
