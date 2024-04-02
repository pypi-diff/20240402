# Comparing `tmp/laser_learning_environment-0.2.0.tar.gz` & `tmp/laser_learning_environment-0.2.2.tar.gz`

## Comparing `laser_learning_environment-0.2.0.tar` & `laser_learning_environment-0.2.2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 laser_learning_environment-0.2.0/Cargo.toml
--rw-r--r--   0     1001      127     4752 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      715 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/.gitignore
--rw-r--r--   0     1001      127     4581 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/build.rs
--rw-r--r--   0     1001      127     1923 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/docs/3x1.png
--rw-r--r--   0     1001      127    46239 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/docs/lvl6-annotated.png
--rw-r--r--   0     1001      127      207 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/docs/tutorials/boards/board
--rw-r--r--   0     1001      127       60 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/docs/tutorials/boards/empty
--rw-r--r--   0     1001      127       18 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/docs/tutorials/boards/gems
--rw-r--r--   0     1001      127        8 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/docs/tutorials/boards/linear
--rw-r--r--   0     1001      127       17 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/docs/tutorials/boards/linear2
--rw-r--r--   0     1001      127       55 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/docs/tutorials/boards/tatl
--rw-r--r--   0     1001      127       51 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/docs/tutorials/boards/two_agents
--rw-r--r--   0     1001      127       60 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/docs/tutorials/boards/walls
--rw-r--r--   0     1001      127   239686 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/docs/tutorials/lle_env_introduction.ipynb
--rw-r--r--   0     1001      127   470085 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/docs/tutorials/world_introduction.ipynb
--rw-r--r--   0     1001      127   103640 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/poetry.lock
--rw-r--r--   0     1001      127      381 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/allowlist.txt
--rw-r--r--   0     1001      127      277 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/examples/create.py
--rw-r--r--   0     1001      127      718 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/__init__.py
--rw-r--r--   0     1001      127      753 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/action.pyi
--rw-r--r--   0     1001      127      425 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/agent.pyi
--rw-r--r--   0     1001      127      344 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/direction.pyi
--rw-r--r--   0     1001      127     7648 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/env.py
--rw-r--r--   0     1001      127      317 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/event.pyi
--rw-r--r--   0     1001      127      165 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/exceptions.pyi
--rw-r--r--   0     1001      127      611 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/lle.py
--rw-r--r--   0     1001      127    10481 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/observations.py
--rw-r--r--   0     1001      127        0 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/py.typed
--rw-r--r--   0     1001      127     1095 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/tile.pyi
--rw-r--r--   0     1001      127      243 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/types.py
--rw-r--r--   0     1001      127     4301 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/lle/world.pyi
--rw-r--r--   0     1001      127     1613 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/test.py
--rw-r--r--   0     1001      127        0 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/tests/__init__.py
--rw-r--r--   0     1001      127      496 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/tests/test_actions.py
--rw-r--r--   0     1001      127      297 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/tests/test_direction.py
--rw-r--r--   0     1001      127    10615 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/tests/test_env.py
--rw-r--r--   0     1001      127      721 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/tests/test_level_generator.py
--rw-r--r--   0     1001      127     7842 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/tests/test_observations.py
--rw-r--r--   0     1001      127     1368 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/tests/test_serialization.py
--rw-r--r--   0     1001      127     8393 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/python/tests/test_world.py
--rw-r--r--   0     1001      127     3922 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/readme.md
--rw-r--r--   0     1001      127      323 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/levels/lvl1
--rw-r--r--   0     1001      127      335 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/levels/lvl2
--rw-r--r--   0     1001      127      371 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/levels/lvl3
--rw-r--r--   0     1001      127      373 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/levels/lvl4
--rw-r--r--   0     1001      127      415 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/levels/lvl5
--rw-r--r--   0     1001      127      463 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/levels/lvl6
--rw-r--r--   0     1001      127      652 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/agents/blue.png
--rw-r--r--   0     1001      127      652 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/agents/green.png
--rw-r--r--   0     1001      127      650 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/agents/red.png
--rw-r--r--   0     1001      127      653 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/agents/yellow.png
--rw-r--r--   0     1001      127      609 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/convert.py
--rw-r--r--   0     1001      127      874 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/gem.png
--rw-r--r--   0     1001      127      262 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/east/blue.png
--rw-r--r--   0     1001      127      263 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/east/green.png
--rw-r--r--   0     1001      127      264 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/east/red.png
--rw-r--r--   0     1001      127      289 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/east/yellow.png
--rw-r--r--   0     1001      127      264 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/north/blue.png
--rw-r--r--   0     1001      127      265 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/north/green.png
--rw-r--r--   0     1001      127      265 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/north/red.png
--rw-r--r--   0     1001      127      286 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/north/yellow.png
--rw-r--r--   0     1001      127      261 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/south/blue.png
--rw-r--r--   0     1001      127      261 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/south/green.png
--rw-r--r--   0     1001      127      261 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/south/red.png
--rw-r--r--   0     1001      127      282 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/south/yellow.png
--rw-r--r--   0     1001      127      266 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/west/blue.png
--rw-r--r--   0     1001      127      266 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/west/green.png
--rw-r--r--   0     1001      127      265 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/west/red.png
--rw-r--r--   0     1001      127      292 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/laser_sources/west/yellow.png
--rw-r--r--   0     1001      127     1039 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/lasers/horizontal/blue.png
--rw-r--r--   0     1001      127     1055 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/lasers/horizontal/green.png
--rw-r--r--   0     1001      127     1096 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/lasers/horizontal/red.png
--rw-r--r--   0     1001      127     1161 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/lasers/horizontal/yellow.png
--rw-r--r--   0     1001      127     1830 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/lasers/vertical/blue.png
--rw-r--r--   0     1001      127     1987 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/lasers/vertical/green.png
--rw-r--r--   0     1001      127     1803 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/lasers/vertical/red.png
--rw-r--r--   0     1001      127     1739 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/lasers/vertical/yellow.png
--rw-r--r--   0     1001      127     7261 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/resources/sprites/void.png
--rw-r--r--   0     1001      127     2413 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/action.rs
--rw-r--r--   0     1001      127      944 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/agent.rs
--rw-r--r--   0     1001      127     1130 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/bindings/mod.rs
--rw-r--r--   0     1001      127     2630 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/bindings/pyaction.rs
--rw-r--r--   0     1001      127      498 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/bindings/pyagent.rs
--rw-r--r--   0     1001      127     1306 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/bindings/pydirection.rs
--rw-r--r--   0     1001      127     1411 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/bindings/pyevent.rs
--rw-r--r--   0     1001      127     4120 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/bindings/pyexceptions.rs
--rw-r--r--   0     1001      127     2901 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/bindings/pytile.rs
--rw-r--r--   0     1001      127     8604 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/bindings/pyworld.rs
--rw-r--r--   0     1001      127     2460 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/bindings/pyworld_state.rs
--rw-r--r--   0     1001      127      916 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/errors.rs
--rw-r--r--   0     1001      127      194 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/event.rs
--rw-r--r--   0     1001      127      702 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/levels.rs
--rw-r--r--   0     1001      127      238 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/mod.rs
--rw-r--r--   0     1001      127      869 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/parsing/errors.rs
--rw-r--r--   0     1001      127       76 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/parsing/mod.rs
--rw-r--r--   0     1001      127     6089 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/parsing/parser.rs
--rw-r--r--   0     1001      127      735 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/tiles/direction.rs
--rw-r--r--   0     1001      127     1182 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/tiles/gem.rs
--rw-r--r--   0     1001      127     3866 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/tiles/laser.rs
--rw-r--r--   0     1001      127     2015 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/tiles/laser_source.rs
--rw-r--r--   0     1001      127      240 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/tiles/mod.rs
--rw-r--r--   0     1001      127     1749 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/tiles/start_exit.rs
--rw-r--r--   0     1001      127     3048 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/tiles/tile.rs
--rw-r--r--   0     1001      127    13901 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/world.rs
--rw-r--r--   0     1001      127      470 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/core/world_state.rs
--rw-r--r--   0     1001      127      447 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/lib.rs
--rw-r--r--   0     1001      127      316 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/rendering/mod.rs
--rw-r--r--   0     1001      127     7539 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/rendering/renderer.rs
--rw-r--r--   0     1001      127     2049 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/rendering/sprites.rs
--rw-r--r--   0     1001      127      220 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/rendering/tile_visitor.rs
--rw-r--r--   0     1001      127    13187 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/unit_tests/test_core.rs
--rw-r--r--   0     1001      127     1281 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/unit_tests/test_done_strategy.rs
--rw-r--r--   0     1001      127      367 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/unit_tests/test_renderer.rs
--rw-r--r--   0     1001      127        0 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/unit_tests/test_reward.rs
--rw-r--r--   0     1001      127     2619 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/unit_tests/test_tile.rs
--rw-r--r--   0     1001      127      678 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/src/utils/mod.rs
--rw-r--r--   0     1001      127    10803 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/tests/world_integration_tests.rs
--rw-r--r--   0     1001      127    32522 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/Cargo.lock
--rw-r--r--   0     1001      127     1195 2024-03-28 19:13:52.000000 laser_learning_environment-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4244 1970-01-01 00:00:00.000000 laser_learning_environment-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 laser_learning_environment-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      127     4752 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      739 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/.gitignore
+-rw-r--r--   0     1001      127     4581 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/build.rs
+-rw-r--r--   0     1001      127     1923 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/docs/3x1.png
+-rw-r--r--   0     1001      127    46239 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/docs/lvl6-annotated.png
+-rw-r--r--   0     1001      127      207 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/docs/tutorials/boards/board
+-rw-r--r--   0     1001      127       60 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/docs/tutorials/boards/empty
+-rw-r--r--   0     1001      127       18 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/docs/tutorials/boards/gems
+-rw-r--r--   0     1001      127        8 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/docs/tutorials/boards/linear
+-rw-r--r--   0     1001      127       17 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/docs/tutorials/boards/linear2
+-rw-r--r--   0     1001      127       55 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/docs/tutorials/boards/tatl
+-rw-r--r--   0     1001      127       51 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/docs/tutorials/boards/two_agents
+-rw-r--r--   0     1001      127       60 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/docs/tutorials/boards/walls
+-rw-r--r--   0     1001      127   239686 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/docs/tutorials/lle_env_introduction.ipynb
+-rw-r--r--   0     1001      127   470085 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/docs/tutorials/world_introduction.ipynb
+-rw-r--r--   0     1001      127      294 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/allowlist.txt
+-rw-r--r--   0     1001      127      277 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/examples/create.py
+-rw-r--r--   0     1001      127      742 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/__init__.py
+-rw-r--r--   0     1001      127      753 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/action.pyi
+-rw-r--r--   0     1001      127      425 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/agent.pyi
+-rw-r--r--   0     1001      127      341 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/direction.pyi
+-rw-r--r--   0     1001      127     7607 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/env.py
+-rw-r--r--   0     1001      127      317 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/event.pyi
+-rw-r--r--   0     1001      127      165 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/exceptions.pyi
+-rw-r--r--   0     1001      127      612 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/lle.py
+-rw-r--r--   0     1001      127    10521 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/observations.py
+-rw-r--r--   0     1001      127        0 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/py.typed
+-rw-r--r--   0     1001      127     1656 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/tile.pyi
+-rw-r--r--   0     1001      127      396 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/types.py
+-rw-r--r--   0     1001      127     5398 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/lle/world.pyi
+-rw-r--r--   0     1001      127     1613 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/test.py
+-rw-r--r--   0     1001      127        0 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/tests/__init__.py
+-rw-r--r--   0     1001      127      496 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/tests/test_actions.py
+-rw-r--r--   0     1001      127      297 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/tests/test_direction.py
+-rw-r--r--   0     1001      127    10615 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/tests/test_env.py
+-rw-r--r--   0     1001      127      721 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/tests/test_level_generator.py
+-rw-r--r--   0     1001      127     7852 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/tests/test_observations.py
+-rw-r--r--   0     1001      127     1292 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/tests/test_serialization.py
+-rw-r--r--   0     1001      127     9887 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/python/tests/test_world.py
+-rw-r--r--   0     1001      127     3922 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/readme.md
+-rw-r--r--   0     1001      127      323 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/levels/lvl1
+-rw-r--r--   0     1001      127      335 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/levels/lvl2
+-rw-r--r--   0     1001      127      371 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/levels/lvl3
+-rw-r--r--   0     1001      127      373 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/levels/lvl4
+-rw-r--r--   0     1001      127      415 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/levels/lvl5
+-rw-r--r--   0     1001      127      463 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/levels/lvl6
+-rw-r--r--   0     1001      127      652 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/agents/blue.png
+-rw-r--r--   0     1001      127      652 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/agents/green.png
+-rw-r--r--   0     1001      127      650 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/agents/red.png
+-rw-r--r--   0     1001      127      653 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/agents/yellow.png
+-rw-r--r--   0     1001      127      609 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/convert.py
+-rw-r--r--   0     1001      127      874 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/gem.png
+-rw-r--r--   0     1001      127      262 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/east/blue.png
+-rw-r--r--   0     1001      127      263 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/east/green.png
+-rw-r--r--   0     1001      127      264 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/east/red.png
+-rw-r--r--   0     1001      127      289 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/east/yellow.png
+-rw-r--r--   0     1001      127      264 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/north/blue.png
+-rw-r--r--   0     1001      127      265 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/north/green.png
+-rw-r--r--   0     1001      127      265 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/north/red.png
+-rw-r--r--   0     1001      127      286 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/north/yellow.png
+-rw-r--r--   0     1001      127      261 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/south/blue.png
+-rw-r--r--   0     1001      127      261 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/south/green.png
+-rw-r--r--   0     1001      127      261 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/south/red.png
+-rw-r--r--   0     1001      127      282 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/south/yellow.png
+-rw-r--r--   0     1001      127      266 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/west/blue.png
+-rw-r--r--   0     1001      127      266 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/west/green.png
+-rw-r--r--   0     1001      127      265 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/west/red.png
+-rw-r--r--   0     1001      127      292 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/laser_sources/west/yellow.png
+-rw-r--r--   0     1001      127     1039 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/lasers/horizontal/blue.png
+-rw-r--r--   0     1001      127     1055 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/lasers/horizontal/green.png
+-rw-r--r--   0     1001      127     1096 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/lasers/horizontal/red.png
+-rw-r--r--   0     1001      127     1161 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/lasers/horizontal/yellow.png
+-rw-r--r--   0     1001      127     1830 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/lasers/vertical/blue.png
+-rw-r--r--   0     1001      127     1987 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/lasers/vertical/green.png
+-rw-r--r--   0     1001      127     1803 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/lasers/vertical/red.png
+-rw-r--r--   0     1001      127     1739 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/lasers/vertical/yellow.png
+-rw-r--r--   0     1001      127     7261 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/resources/sprites/void.png
+-rw-r--r--   0     1001      127     2413 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/action.rs
+-rw-r--r--   0     1001      127      944 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/agent.rs
+-rw-r--r--   0     1001      127     1188 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/bindings/mod.rs
+-rw-r--r--   0     1001      127     2630 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/bindings/pyaction.rs
+-rw-r--r--   0     1001      127      498 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/bindings/pyagent.rs
+-rw-r--r--   0     1001      127     1432 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/bindings/pydirection.rs
+-rw-r--r--   0     1001      127     1401 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/bindings/pyevent.rs
+-rw-r--r--   0     1001      127     4120 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/bindings/pyexceptions.rs
+-rw-r--r--   0     1001      127     3233 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/bindings/pytile.rs
+-rw-r--r--   0     1001      127     9777 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/bindings/pyworld.rs
+-rw-r--r--   0     1001      127     2471 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/bindings/pyworld_state.rs
+-rw-r--r--   0     1001      127      916 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/errors.rs
+-rw-r--r--   0     1001      127      194 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/event.rs
+-rw-r--r--   0     1001      127      702 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/levels.rs
+-rw-r--r--   0     1001      127      238 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/mod.rs
+-rw-r--r--   0     1001      127      869 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/parsing/errors.rs
+-rw-r--r--   0     1001      127       76 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/parsing/mod.rs
+-rw-r--r--   0     1001      127     6141 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/parsing/parser.rs
+-rw-r--r--   0     1001      127      735 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/tiles/direction.rs
+-rw-r--r--   0     1001      127     1182 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/tiles/gem.rs
+-rw-r--r--   0     1001      127     4563 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/tiles/laser.rs
+-rw-r--r--   0     1001      127     2624 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/tiles/laser_source.rs
+-rw-r--r--   0     1001      127      251 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/tiles/mod.rs
+-rw-r--r--   0     1001      127     1749 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/tiles/start_exit.rs
+-rw-r--r--   0     1001      127     3048 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/tiles/tile.rs
+-rw-r--r--   0     1001      127    13901 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/world.rs
+-rw-r--r--   0     1001      127      470 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/core/world_state.rs
+-rw-r--r--   0     1001      127      447 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      127      316 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/rendering/mod.rs
+-rw-r--r--   0     1001      127     7539 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/rendering/renderer.rs
+-rw-r--r--   0     1001      127     2049 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/rendering/sprites.rs
+-rw-r--r--   0     1001      127      220 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/rendering/tile_visitor.rs
+-rw-r--r--   0     1001      127    13187 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/unit_tests/test_core.rs
+-rw-r--r--   0     1001      127     1281 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/unit_tests/test_done_strategy.rs
+-rw-r--r--   0     1001      127      367 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/unit_tests/test_renderer.rs
+-rw-r--r--   0     1001      127        0 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/unit_tests/test_reward.rs
+-rw-r--r--   0     1001      127     2622 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/unit_tests/test_tile.rs
+-rw-r--r--   0     1001      127      678 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/src/utils/mod.rs
+-rw-r--r--   0     1001      127       58 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/stubcheck.sh
+-rw-r--r--   0     1001      127    12052 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/tests/world_integration_tests.rs
+-rw-r--r--   0     1001      127    32522 2024-04-02 09:23:53.000000 laser_learning_environment-0.2.2/Cargo.lock
+-rw-r--r--   0     1001      127     1156 2024-04-02 09:23:44.000000 laser_learning_environment-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4244 1970-01-01 00:00:00.000000 laser_learning_environment-0.2.2/PKG-INFO
```

### Comparing `laser_learning_environment-0.2.0/.github/workflows/CI.yml` & `laser_learning_environment-0.2.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/.gitignore` & `laser_learning_environment-0.2.2/.gitignore`

 * *Files 26% similar despite different names*

```diff
@@ -69,8 +69,11 @@
 .vscode/
 
 # Pyenv
 .python-version
 
 .mypy_cache
 .env
-.ruff_cache
+.ruff_cache
+
+Cargo.lock
+poetry.lock
```

### Comparing `laser_learning_environment-0.2.0/build.rs` & `laser_learning_environment-0.2.2/build.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/docs/3x1.png` & `laser_learning_environment-0.2.2/docs/3x1.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/docs/lvl6-annotated.png` & `laser_learning_environment-0.2.2/docs/lvl6-annotated.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/docs/tutorials/lle_env_introduction.ipynb` & `laser_learning_environment-0.2.2/docs/tutorials/lle_env_introduction.ipynb`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/docs/tutorials/world_introduction.ipynb` & `laser_learning_environment-0.2.2/docs/tutorials/world_introduction.ipynb`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/python/lle/__init__.py` & `laser_learning_environment-0.2.2/python/lle/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,23 +8,24 @@
     "LaserSource",
     "Direction",
     "LLE",
     "World",
     "ObservationType",
     "Position",
     "AgentId",
+    "LaserId",
     "WorldEvent",
     "EventType",
     "InvalidActionError",
     "InvalidLevelError",
     "InvalidWorldStateError",
     "ParsingError",
 ]
 
-from .types import Position, AgentId
+from .types import Position, AgentId, LaserId
 
 from .lle import (
     __version__,
     Action,
     World,
     WorldEvent,
     EventType,
```

### Comparing `laser_learning_environment-0.2.0/python/lle/action.pyi` & `laser_learning_environment-0.2.2/python/lle/action.pyi`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/python/lle/env.py` & `laser_learning_environment-0.2.2/python/lle/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Literal, ClassVar, Sequence
+from typing import Any, Literal, ClassVar
 from typing_extensions import override
 from dataclasses import dataclass
 from serde import serde
 import cv2
 import numpy as np
 
 from lle import World, Action, EventType, WorldState, WorldEvent
@@ -71,23 +71,23 @@
             case other:
                 raise ValueError(f"State type {other} does not support `unit_state_size`.")
 
     def get_observation(self):
         return Observation(self.observation_generator.observe(), self.available_actions(), self.get_state())
 
     @override
-    def available_actions(self) -> np.ndarray[np.int32, Any]:
-        available_actions = np.zeros((self.n_agents, self.n_actions), dtype=np.int64)
+    def available_actions(self):
+        available_actions = np.zeros((self.n_agents, self.n_actions), dtype=np.float32)
         for agent, actions in enumerate(self.world.available_actions()):
             for action in actions:
                 available_actions[agent, action.value] = 1
         return available_actions
 
     @override
-    def step(self, actions: Sequence[int] | np.ndarray[np.int32, Any]):
+    def step(self, actions: list[int] | np.ndarray[np.int32, Any]):
         assert not self.done, "Can not play when the game is done !"
         events = self.world.step([Action(a) for a in actions])
 
         for event in events:
             match event.event_type:
                 case EventType.AGENT_DIED:
                     self.done = True
```

### Comparing `laser_learning_environment-0.2.0/python/lle/lle.py` & `laser_learning_environment-0.2.2/python/lle/lle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from .action import Action
 from .world import World, WorldState
 from .agent import Agent
-from .tile import Gem, Laser, LaserSource, Tile
+from .tile import Gem, Laser, LaserSource
 from .direction import Direction
 from .event import WorldEvent, EventType
 from .exceptions import InvalidActionError, InvalidLevelError, InvalidWorldStateError, ParsingError
 
 
 __version__: str
 
 __all__ = [
+    "__version__",
     "Action",
     "World",
     "WorldState",
     "Agent",
     "Gem",
     "Laser",
     "LaserSource",
-    "Tile",
     "Direction",
     "WorldEvent",
     "EventType",
     "InvalidActionError",
     "InvalidLevelError",
     "InvalidWorldStateError",
     "ParsingError",
```

### Comparing `laser_learning_environment-0.2.0/python/lle/observations.py` & `laser_learning_environment-0.2.2/python/lle/observations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import Any
 from abc import ABC, abstractmethod
-from enum import IntEnum, auto
+from enum import IntEnum
 import numpy as np
 import cv2
 from lle import World, AgentId, Position
 
 
 class ObservationType(IntEnum):
     """The different observation types for the World"""
 
-    RELATIVE_POSITIONS = auto()
-    STATE = auto()
-    RGB_IMAGE = auto()
-    LAYERED = auto()
-    FLATTENED = auto()
-    PARTIAL_3x3 = auto()
-    PARTIAL_5x5 = auto()
-    PARTIAL_7x7 = auto()
-    LAYERED_PADDED = auto()
-    LAYERED_PADDED_1AGENT = auto()
-    LAYERED_PADDED_2AGENTS = auto()
-    LAYERED_PADDED_3AGENTS = auto()
+    RELATIVE_POSITIONS = 0
+    STATE = 1
+    RGB_IMAGE = 2
+    LAYERED = 3
+    FLATTENED = 4
+    PARTIAL_3x3 = 5
+    PARTIAL_5x5 = 6
+    PARTIAL_7x7 = 7
+    LAYERED_PADDED = 8
+    LAYERED_PADDED_1AGENT = 9
+    LAYERED_PADDED_2AGENTS = 10
+    LAYERED_PADDED_3AGENTS = 11
 
     @staticmethod
     def from_str(s: str) -> "ObservationType":
         """Convert a string to an ObservationType"""
         s = s.upper()
         for enum in ObservationType:
             if enum.name == s:
@@ -89,15 +89,15 @@
         super().__init__(world)
         self.n_gems = world.n_gems
         self.dimensions = np.array([world.height, world.width])
 
     def observe(self):
         positions = np.tile((self._world.agents_positions / self.dimensions).flatten(), (self._world.n_agents, 1))
         gems_collected = np.tile(
-            np.array([not gem.is_collected for _, gem in self._world.gems], dtype=np.float32), (self._world.n_agents, 1)
+            np.array([not gem.is_collected for gem in self._world.gems.values()], dtype=np.float32), (self._world.n_agents, 1)
         )
         return np.concatenate([positions, gems_collected], axis=1).astype(np.float32)
 
     @property
     def obs_type(self) -> ObservationType:
         return ObservationType.STATE
 
@@ -167,29 +167,29 @@
         obs = np.zeros(self._shape, dtype=np.float32)
         for i, j in self._world.exit_pos:
             obs[self.EXIT, i, j] = 1.0
 
         for i, j in self._world.wall_pos:
             obs[self.WALL, i, j] = 1.0
 
-        for (i, j), source in self._world.laser_sources:
+        for (i, j), source in self._world.laser_sources.items():
             obs[self.LASER_0 + source.agent_id, i, j] = -1.0
             obs[self.WALL, i, j] = 1.0
 
         for i, j in self._world.void_pos:
             obs[self.VOID, i, j] = 1.0
 
         return obs
 
     def observe(self):
         obs = np.copy(self.static_obs)
         for (i, j), laser in self._world.lasers:
             if laser.is_on:
                 obs[self.LASER_0 + laser.agent_id, i, j] = 1.0
-        for (i, j), gem in self._world.gems:
+        for (i, j), gem in self._world.gems.items():
             if not gem.is_collected:
                 obs[self.GEM, i, j] = 1.0
         for i, (y, x) in enumerate(self._world.agents_positions):
             obs[self.A0 + i, y, x] = 1.0
         return np.tile(obs, (self.n_agents, 1, 1, 1))
 
     @property
@@ -237,15 +237,16 @@
 
 
 class PartialGenerator(ObservationGenerator):
     def __init__(self, world: World, square_size: int):
         super().__init__(world)
         assert square_size % 2 == 1, "Can only use odd numbers for the square size"
         self.size = square_size
-        self._shape = (world.n_agents * 2 + 3, self.size, self.size)
+        # Each agent, each laser, walls, gems, exits
+        self._shape = (world.n_agents + world.n_agents + 3, self.size, self.size)
         self._center = self.size // 2
         self.WALL = world.n_agents
         self.LASER_0 = self.WALL + 1
         self.GEM = self.LASER_0 + world.n_agents
         self.EXIT = self.GEM + 1
 
     @property
@@ -267,25 +268,25 @@
     def observe(self) -> np.ndarray[np.float32, Any]:
         obs = np.zeros((self._world.n_agents, *self._shape), dtype=np.float32)
         for a, agent_pos in enumerate(self._world.agents_positions):
             # Agents positions
             for a2, other_pos in enumerate(self._world.agents_positions):
                 self.encode_layer(obs[a, a2], agent_pos, [other_pos])
             # Gems
-            self.encode_layer(obs[a, self.GEM], agent_pos, [gem_pos for gem_pos, gem in self._world.gems if not gem.is_collected])
+            self.encode_layer(obs[a, self.GEM], agent_pos, [gem_pos for gem_pos, gem in self._world.gems.items() if not gem.is_collected])
             # Exits
             self.encode_layer(obs[a, self.EXIT], agent_pos, [exit_pos for exit_pos in self._world.exit_pos])
             # Walls
             self.encode_layer(obs[a, self.WALL], agent_pos, [wall_pos for wall_pos in self._world.wall_pos])
             # Lasers
             laser_positions = self._get_lasers_positions()
             for agent_id, positions in laser_positions.items():
                 self.encode_layer(obs[a, self.LASER_0 + agent_id], agent_pos, positions)
             # Laser sources
-            for pos, source in self._world.laser_sources:
+            for pos, source in self._world.laser_sources.items():
                 self.encode_layer(obs[a, self.LASER_0 + source.agent_id], agent_pos, [pos], fill_value=-1.0)
         return obs
 
     def _get_lasers_positions(self) -> dict[AgentId, list[Position]]:
         laser_positions = dict[AgentId, list[Position]]()
         for laser_pos, laser in self._world.lasers:
             if laser.is_on:
```

### Comparing `laser_learning_environment-0.2.0/python/lle/world.pyi` & `laser_learning_environment-0.2.2/python/lle/world.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Tuple, List, Any, final
 import numpy as np
 
 from .event import WorldEvent
 from .action import Action
 from .agent import Agent
 from .tile import Gem, LaserSource, Laser
-from .types import Position
+from .types import Position, AgentId
 
 @final
 class WorldState:
     def __init__(self, agents_positions: List[Position], gems_collected: List[bool]):
         """Construct a WorldState from the (i, j) position of each agent and the collection status of each gem."""
     @property
     def agents_positions(self) -> List[Position]:
@@ -31,26 +31,38 @@
     """The width (in number of tiles) of the gridworld."""
     height: int
     """The height (in number of tiles) of the gridworld."""
     image_dimensions: Tuple[int, int]
     """The dimensions (in pixels) of the image redered (width, height)"""
     n_gems: int
     """The total number of gems in the world."""
-    gems: List[Tuple[Position, Gem]]
-    """The list of gems in the world"""
+    gems: dict[Position, Gem]
+    """
+    The list of gems in the world
+    
+    Note: Accessing this attribute is costly because it creates the mapping on the fly every time.
+    """
     exit_pos: List[Position]
     """The (i, j) position of each exit tile."""
     wall_pos: List[Position]
     """The (i, j) position of every wall tile."""
     void_pos: List[Position]
     """The (i, j) position of every void tile."""
-    laser_sources: List[Tuple[Position, LaserSource]]
-    """The (i, j) position of every laser source."""
+    laser_sources: dict[Position, LaserSource]
+    """
+    A mapping from positions to laser sources.
+    
+    Note: Accessing this attribute is costly because it creates the mapping on the fly every time.
+    """
     lasers: List[Tuple[Position, Laser]]
-    """The (i, j) position of every laser."""
+    """
+    The (i, j) position of every laser
+
+    Note: Accessing this attribute is costly because it creates the list on the fly for every call.
+    """
     agents_positions: List[Position]
     """The current (i, j) position of each agent"""
     world_string: str
     """The string upon which the world has been constructed."""
 
     def __init__(self, world_str: str):
         """Constructs a World from a string.
@@ -94,14 +106,37 @@
     def set_state(self, state: WorldState) -> list[WorldEvent]:
         """
         Force the world to a given state.
 
         - Returns the list of events that occurred while agents entered their state.
         - Raises a `InvalidWorldStateError` if the state is invalid.
         """
+    def disable_laser_source(self, source: LaserSource):
+        """
+        Disable a laser source (deactivate all the beam from this source).
+
+        Raise a `ValueError` if a source with the same `LaserId` is not found.
+        """
+
+    def enable_laser_source(self, source: LaserSource):
+        """
+        Enable a laser source.
+
+        Raise a `ValueError` if a source with the same `LaserId` is not found.
+        """
+
+    def set_laser_colour(self, source: LaserSource, new_colour: AgentId):
+        """
+        Change the colour of a laser source (and of all corresponding laser tiles).
+
+        Raise a `ValueError` if
+            - a source with the same `LaserId` is not found
+            - the `new_colour` does not belong to an agent
+        """
+
     @staticmethod
     def from_file(filename: str) -> "World":
         """
         Parse the content of `filename` to create a World.
 
         Raise a `FileNotFoundError` if the file does not exist.
         """
```

### Comparing `laser_learning_environment-0.2.0/python/test.py` & `laser_learning_environment-0.2.2/python/test.py`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/python/tests/test_env.py` & `laser_learning_environment-0.2.2/python/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/python/tests/test_level_generator.py` & `laser_learning_environment-0.2.2/python/tests/test_level_generator.py`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/python/tests/test_observations.py` & `laser_learning_environment-0.2.2/python/tests/test_observations.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,22 +87,22 @@
     WALL_LAYER = world.n_agents
     VOID_LAYER = world.n_agents * 2 + 1
     GEM_LAYER = VOID_LAYER + 1
     EXIT_LAYER = -1
 
     for i, j in world.wall_pos:
         assert np.all(layers[:, WALL_LAYER, i, j] == 1)
-    for (i, j), _ in world.gems:
+    for i, j in world.gems.keys():
         assert np.all(layers[:, GEM_LAYER, i, j] == 1)
     for i, j in world.exit_pos:
         assert np.all(layers[:, EXIT_LAYER, i, j] == 1)
     for (i, j), laser in world.lasers:
         if laser.is_on:
             assert np.all(layers[:, LASER_0_LAYER + laser.agent_id, i, j] == 1)
-    for (i, j), source in world.laser_sources:
+    for (i, j), source in world.laser_sources.items():
         assert np.all(layers[:, LASER_0_LAYER + source.agent_id, i, j] == -1)
     assert np.all(layers[:, VOID_LAYER] == 0)
 
 
 def test_observe_layered_void():
     world = World(
         """
```

### Comparing `laser_learning_environment-0.2.0/python/tests/test_serialization.py` & `laser_learning_environment-0.2.2/python/tests/test_serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,16 @@
 import pickle
 import random
 
 
 def test_pickle_world_state():
     for i in range(50):
         s = WorldState(
-            gems_collected=[
-                random.choice([True, False]) for _ in range(random.randint(0, 10))
-            ],
-            agents_positions=[
-                (random.randint(0, 50), random.randint(0, 90))
-                for _ in range(random.randint(0, 10))
-            ],
+            gems_collected=[random.choice([True, False]) for _ in range(random.randint(0, 10))],
+            agents_positions=[(random.randint(0, 50), random.randint(0, 90)) for _ in range(random.randint(0, 10))],
         )
         serialised = pickle.dumps(s)
         deserialised = pickle.loads(serialised)
         assert s == deserialised
 
 
 def test_pickle_world():
```

### Comparing `laser_learning_environment-0.2.0/python/tests/test_world.py` & `laser_learning_environment-0.2.2/python/tests/test_world.py`

 * *Files 14% similar despite different names*

```diff
@@ -325,25 +325,86 @@
 def test_get_standard_level():
     for i in range(1, 7):
         World.level(i)
         World.from_file(f"lvl{i}")
         World.from_file(f"level{i}")
 
 
+def test_laser_tile_state():
+    world = World("L0E S0 . X")
+    world.reset()
+    for _, laser in world.lasers:
+        assert laser.is_off
+
+    world.step([Action.EAST])
+    for pos, laser in world.lasers:
+        match pos:
+            case (0, 1):
+                assert laser.is_on
+            case _:
+                assert laser.is_off
+
+
+def test_disable_deadly_laser_source_and_walk_into_it():
+    world = World(
+        """
+        L0E . . X
+        S0 S1 . X
+        """
+    )
+    world.reset()
+    source = world.laser_sources[0, 0]
+    world.disable_laser_source(source)
+    events = world.step([Action.STAY, Action.NORTH])
+    assert len(events) == 0
+    assert all(a.is_alive for a in world.agents)
+
+
 def test_change_laser_colour():
     world = World(
         """
-        X L0S .
-        .  .  S1
-        X  .  S0"""
+        L0E . .  .  X
+        L1E . S1 S0 X
+        """
     )
     world.reset()
-    world.step([Action.STAY, Action.WEST])
-    assert world.agents[1].is_dead, "Agent 1 should be dead"
+    lasers = dict(world.lasers)
+    sources = dict(world.laser_sources)
+    assert lasers[0, 1].agent_id == 0
+    assert lasers[1, 1].agent_id == 1
+    top_source = sources[0, 0]
+
+    NEW_COLOUR = 1
+    world.set_laser_colour(top_source, NEW_COLOUR)
+    world.reset()
+
+    # Check that all the laser tiles have changed their colour
+    for (i, _), laser in world.lasers:
+        if i == 0:
+            assert laser.agent_id == NEW_COLOUR
+    events = world.step([Action.NORTH, Action.NORTH])
+    assert len(events) == 0
+    assert all(a.is_alive for a in world.agents)
+
+
+def test_change_laser_colour_to_negative_colour():
+    world = World("L0E S0 . X")
+    world.reset()
+    source = world.laser_sources[0, 0]
+
+    try:
+        world.set_laser_colour(source, -1)
+        raise Exception("Negative colours are not allowed")
+    except ValueError:
+        pass
 
+
+def test_change_laser_colour_to_invalid_colour():
+    world = World("L0E S0 . X")
     world.reset()
-    _, source = world.laser_sources[0]
-    source.set_agent_id(1)
-    world.step([Action.STAY, Action.WEST])
-    assert world.agents[1].is_alive, "Agent 1 should be alive"
-    world.step([Action.WEST, Action.WEST])
-    assert world.agents[0].is_dead, "Agent 0 should be dead in the laser"
+    source = world.laser_sources[0, 0]
+
+    try:
+        world.set_laser_colour(source, 2)
+        raise Exception("This should not be allowed because there is only one agent in the world")
+    except ValueError:
+        pass
```

### Comparing `laser_learning_environment-0.2.0/readme.md` & `laser_learning_environment-0.2.2/readme.md`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/agents/blue.png` & `laser_learning_environment-0.2.2/resources/sprites/agents/blue.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/agents/green.png` & `laser_learning_environment-0.2.2/resources/sprites/agents/green.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/agents/red.png` & `laser_learning_environment-0.2.2/resources/sprites/agents/red.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/agents/yellow.png` & `laser_learning_environment-0.2.2/resources/sprites/agents/yellow.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/convert.py` & `laser_learning_environment-0.2.2/resources/sprites/convert.py`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/gem.png` & `laser_learning_environment-0.2.2/resources/sprites/gem.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/lasers/horizontal/blue.png` & `laser_learning_environment-0.2.2/resources/sprites/lasers/horizontal/blue.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/lasers/horizontal/green.png` & `laser_learning_environment-0.2.2/resources/sprites/lasers/horizontal/green.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/lasers/horizontal/red.png` & `laser_learning_environment-0.2.2/resources/sprites/lasers/horizontal/red.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/lasers/horizontal/yellow.png` & `laser_learning_environment-0.2.2/resources/sprites/lasers/horizontal/yellow.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/lasers/vertical/blue.png` & `laser_learning_environment-0.2.2/resources/sprites/lasers/vertical/blue.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/lasers/vertical/green.png` & `laser_learning_environment-0.2.2/resources/sprites/lasers/vertical/green.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/lasers/vertical/red.png` & `laser_learning_environment-0.2.2/resources/sprites/lasers/vertical/red.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/lasers/vertical/yellow.png` & `laser_learning_environment-0.2.2/resources/sprites/lasers/vertical/yellow.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/resources/sprites/void.png` & `laser_learning_environment-0.2.2/resources/sprites/void.png`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/action.rs` & `laser_learning_environment-0.2.2/src/action.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/agent.rs` & `laser_learning_environment-0.2.2/src/agent.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/bindings/mod.rs` & `laser_learning_environment-0.2.2/src/bindings/mod.rs`

 * *Files 11% similar despite different names*

```diff
@@ -8,34 +8,37 @@
 mod pytile;
 mod pyworld;
 mod pyworld_state;
 
 // pub use pyworld::PyWorld;
 
 #[pymodule]
-pub fn lle(py: Python, m: &PyModule) -> PyResult<()> {
+pub fn lle(py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<pyevent::PyEventType>()?;
     m.add_class::<pyevent::PyWorldEvent>()?;
     m.add_class::<pyworld::PyWorld>()?;
     m.add_class::<pyworld_state::PyWorldState>()?;
     m.add_class::<pyaction::PyAction>()?;
     m.add_class::<pyagent::PyAgent>()?;
     m.add_class::<pydirection::PyDirection>()?;
     m.add_class::<pytile::PyGem>()?;
     m.add_class::<pytile::PyLaser>()?;
     m.add_class::<pytile::PyLaserSource>()?;
     m.add(
         "InvalidWorldStateError",
-        py.get_type::<pyexceptions::InvalidWorldStateError>(),
+        py.get_type_bound::<pyexceptions::InvalidWorldStateError>(),
     )?;
     m.add(
         "InvalidActionError",
-        py.get_type::<pyexceptions::InvalidActionError>(),
+        py.get_type_bound::<pyexceptions::InvalidActionError>(),
+    )?;
+    m.add(
+        "ParsingError",
+        py.get_type_bound::<pyexceptions::ParsingError>(),
     )?;
-    m.add("ParsingError", py.get_type::<pyexceptions::ParsingError>())?;
     m.add(
         "InvalidLevelError",
-        py.get_type::<pyexceptions::InvalidLevelError>(),
+        py.get_type_bound::<pyexceptions::InvalidLevelError>(),
     )?;
     m.add("__version__", crate::VERSION)?;
     Ok(())
 }
```

### Comparing `laser_learning_environment-0.2.0/src/bindings/pyaction.rs` & `laser_learning_environment-0.2.2/src/bindings/pyaction.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/bindings/pydirection.rs` & `laser_learning_environment-0.2.2/src/bindings/pydirection.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 use crate::tiles::Direction;
 use pyo3::{prelude::*, pyclass::CompareOp};
 
 #[pyclass(name = "Direction")]
-#[derive(Clone)]
+#[derive(Clone, Debug)]
 pub struct PyDirection {
     direction: Direction,
 }
 
 impl PyDirection {
     pub fn new(direction: Direction) -> Self {
         Self { direction }
     }
 }
 
+impl From<Direction> for PyDirection {
+    fn from(direction: Direction) -> Self {
+        Self { direction }
+    }
+}
+
 #[pymethods]
 impl PyDirection {
     #[classattr]
     const NORTH: Self = Self {
         direction: Direction::North,
     };
     #[classattr]
```

### Comparing `laser_learning_environment-0.2.0/src/bindings/pyevent.rs` & `laser_learning_environment-0.2.2/src/bindings/pyevent.rs`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     #[pyo3(name = "AGENT_DIED")]
     AgentDied,
 }
 
 #[derive(Clone)]
 #[pyclass(name = "WorldEvent", module = "lle")]
 pub struct PyWorldEvent {
-    #[pyo3(get, set)]
+    #[pyo3(get)]
     event_type: PyEventType,
     // pos: Position,
-    #[pyo3(get, set)]
+    #[pyo3(get)]
     agent_id: AgentId,
 }
 
 impl PyWorldEvent {
     pub fn new(event_type: PyEventType, agent_id: AgentId) -> Self {
         Self {
             event_type,
```

### Comparing `laser_learning_environment-0.2.0/src/bindings/pyexceptions.rs` & `laser_learning_environment-0.2.2/src/bindings/pyexceptions.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/bindings/pytile.rs` & `laser_learning_environment-0.2.2/src/bindings/pytile.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 use pyo3::prelude::*;
 
 use crate::{
     agent::AgentId,
-    tiles::{LaserSource, Tile},
+    tiles::{Laser, LaserId, LaserSource},
+    Tile,
 };
 
 use super::pydirection::PyDirection;
 
 #[pyclass(name = "Gem")]
 pub struct PyGem {
-    #[pyo3(get, set)]
+    #[pyo3(get)]
     agent: Option<AgentId>,
-    #[pyo3(get, set)]
+    #[pyo3(get)]
     is_collected: bool,
 }
 
 impl PyGem {
     pub fn new(agent: Option<AgentId>, is_collected: bool) -> Self {
         PyGem {
             agent,
@@ -37,113 +38,122 @@
     pub fn __repr__(&self) -> String {
         self.__str__()
     }
 }
 
 #[pyclass(name = "Laser")]
 pub struct PyLaser {
-    #[pyo3(get, set)]
+    #[pyo3(get)]
     is_on: bool,
-    #[pyo3(get, set)]
+    #[pyo3(get)]
+    is_enabled: bool,
+    #[pyo3(get)]
     direction: PyDirection,
-    #[pyo3(get, set)]
+    #[pyo3(get)]
     agent_id: AgentId,
-    #[pyo3(get, set)]
+    #[pyo3(get)]
     agent: Option<AgentId>,
-}
-
-impl PyLaser {
-    pub fn new(
-        is_on: bool,
-        direction: PyDirection,
-        agent_id: AgentId,
-        agent: Option<AgentId>,
-    ) -> Self {
-        PyLaser {
-            is_on,
-            direction,
-            agent,
-            agent_id,
-        }
-    }
+    #[pyo3(get)]
+    laser_id: LaserId,
 }
 
 #[pymethods]
 impl PyLaser {
     #[getter]
     pub fn is_off(&self) -> bool {
         !self.is_on
     }
 
+    #[getter]
+    pub fn is_disabled(&self) -> bool {
+        !self.is_enabled
+    }
+
     pub fn __str__(&self) -> String {
         let agent = match self.agent {
             Some(agent) => agent.to_string(),
             None => String::from("None"),
         };
 
         format!(
-            "Laser(is_on={}, direction={}, agent_id={}, agent={agent})",
+            "Laser(laser_id={}, is_on={}, direction={}, agent_id={}, agent={agent})",
+            self.laser_id,
             self.is_on,
             self.direction.name(),
             self.agent_id
         )
     }
 
     pub fn __repr__(&self) -> String {
         self.__str__()
     }
 }
 
+// Implement from and into
+impl From<&Laser> for PyLaser {
+    fn from(laser: &Laser) -> Self {
+        PyLaser {
+            is_enabled: laser.is_enabled(),
+            agent: laser.agent(),
+            is_on: laser.is_on(),
+            direction: laser.direction().into(),
+            agent_id: laser.agent_id(),
+            laser_id: laser.laser_id(),
+        }
+    }
+}
+
 #[pyclass(name = "LaserSource")]
+#[derive(Debug)]
 pub struct PyLaserSource {
-    source: LaserSource,
+    direction: PyDirection,
+    agent_id: AgentId,
+    laser_id: LaserId,
+    is_enabled: bool,
 }
 
-unsafe impl Send for PyLaserSource {}
-
-impl PyLaserSource {
-    pub fn new(source: LaserSource) -> Self {
-        PyLaserSource { source }
+impl From<&LaserSource> for PyLaserSource {
+    fn from(source: &LaserSource) -> Self {
+        PyLaserSource {
+            direction: source.direction().into(),
+            agent_id: source.agent_id(),
+            laser_id: source.laser_id(),
+            is_enabled: source.is_enabled(),
+        }
     }
 }
 
 #[pymethods]
 impl PyLaserSource {
     #[getter]
-    fn direction(&self) -> PyDirection {
-        PyDirection::new(self.source.direction())
+    pub fn is_enabled(&self) -> bool {
+        self.is_enabled
     }
 
     #[getter]
-    fn agent_id(&self) -> AgentId {
-        self.source.agent_id()
+    pub fn is_disabled(&self) -> bool {
+        !self.is_enabled
     }
 
     #[getter]
-    fn agent(&self) -> Option<AgentId> {
-        self.source.agent()
+    pub fn direction(&self) -> PyDirection {
+        self.direction.clone()
     }
 
-    fn set_agent_id(&self, agent_id: AgentId) {
-        self.source.set_agent_id(agent_id);
-    }
-
-    fn turn_on(&self) {
-        self.source.turn_on();
+    #[getter]
+    pub fn agent_id(&self) -> AgentId {
+        self.agent_id
     }
 
-    fn turn_off(&self) {
-        self.source.turn_off();
+    #[getter]
+    pub fn laser_id(&self) -> LaserId {
+        self.laser_id
     }
 
     pub fn __str__(&self) -> String {
-        format!(
-            "LaserSource(direction={}, agent_id={})",
-            self.direction().name(),
-            self.source.agent_id(),
-        )
+        format!("{:?}", self)
     }
 
     pub fn __repr__(&self) -> String {
         self.__str__()
     }
 }
```

### Comparing `laser_learning_environment-0.2.0/src/bindings/pyworld.rs` & `laser_learning_environment-0.2.2/src/bindings/pyworld.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-use numpy::PyArray1;
-use pyo3::{prelude::*, types::PyDict};
+use std::collections::HashMap;
 
-use crate::{Position, Renderer, Tile, World, WorldEvent, WorldState};
+use numpy::{PyArray1, PyArrayMethods};
+use pyo3::{exceptions::PyValueError, prelude::*, types::PyDict};
+
+use crate::{AgentId, Position, Renderer, Tile, World, WorldState};
 
 use super::{
     pyaction::PyAction,
     pyagent::PyAgent,
-    pydirection::PyDirection,
-    pyevent::{PyEventType, PyWorldEvent},
+    pyevent::PyWorldEvent,
     pyexceptions::{parse_error_to_exception, runtime_error_to_pyexception},
     pytile::{PyGem, PyLaser, PyLaserSource},
     pyworld_state::PyWorldState,
 };
 
 #[pyclass(name = "World", module = "lle")]
 pub struct PyWorld {
@@ -107,74 +108,103 @@
     /// The positions of the wall tiles.
     fn wall_pos(&self) -> Vec<Position> {
         self.world.walls().copied().collect()
     }
 
     #[getter]
     /// The gems with their respective position.
-    fn gems(&self) -> Vec<(Position, PyGem)> {
+    fn gems(&self) -> HashMap<Position, PyGem> {
         self.world
             .gems()
             .map(|(pos, gem)| (*pos, PyGem::new(gem.agent(), gem.is_collected())))
             .collect()
     }
 
     #[getter]
     /// The lasers with their respective position.
     fn lasers(&self) -> Vec<(Position, PyLaser)> {
         self.world
             .lasers()
-            .map(|(pos, laser)| {
-                (
-                    *pos,
-                    PyLaser::new(
-                        laser.is_on(),
-                        PyDirection::new(laser.direction()),
-                        laser.agent_id(),
-                        laser.agent(),
-                    ),
-                )
-            })
+            .map(|(pos, laser)| (*pos, PyLaser::from(laser)))
             .collect()
     }
 
     #[getter]
     /// The laser sources with their respective position.
-    fn laser_sources(&self) -> Vec<(Position, PyLaserSource)> {
+    fn laser_sources(&self) -> HashMap<Position, PyLaserSource> {
         self.world
             .laser_sources()
-            .map(|(pos, laser_source)| (*pos, PyLaserSource::new(laser_source.clone())))
+            .map(|(pos, laser_source)| (*pos, PyLaserSource::from(laser_source)))
             .collect()
     }
 
+    fn disable_laser_source(&self, laser_source: &PyLaserSource) -> PyResult<()> {
+        let id = laser_source.laser_id();
+        if let Some((_, source)) = self.world.laser_sources().find(|(_, l)| l.laser_id() == id) {
+            source.disable();
+            return Ok(());
+        }
+        return Err(PyValueError::new_err(format!(
+            "Laser source with laser_id {id} not found"
+        )));
+    }
+
+    fn enable_laser_source(&self, laser_source: &PyLaserSource) -> PyResult<()> {
+        let id = laser_source.laser_id();
+        if let Some((_, source)) = self.world.laser_sources().find(|(_, l)| l.laser_id() == id) {
+            source.enable();
+            return Ok(());
+        }
+        Err(PyValueError::new_err(format!(
+            "Laser source with laser_id {id} not found"
+        )))
+    }
+
+    fn set_laser_colour(&self, laser_source: &PyLaserSource, new_colour: i32) -> PyResult<()> {
+        let new_colour = match AgentId::try_from(new_colour) {
+            Ok(r) => r,
+            Err(_) => {
+                return Err(PyValueError::new_err(format!(
+                    "New colour {new_colour} must be >= 0"
+                )))
+            }
+        };
+        if laser_source.agent_id() == new_colour {
+            return Ok(());
+        }
+        if new_colour > self.world.n_agents() {
+            let n_agents = self.world.n_agents();
+            return Err(PyValueError::new_err(format!(
+                "New colour {new_colour} does not belong to an existing agent !\nThere are {n_agents} agents in the world, provide a value bewteen 0 and {} included.",
+                n_agents -1
+            )));
+        }
+        let id = laser_source.laser_id();
+        if let Some((_, source)) = self.world.laser_sources().find(|(_, l)| l.laser_id() == id) {
+            source.set_agent_id(new_colour);
+            return Ok(());
+        }
+        Err(PyValueError::new_err(format!(
+            "Laser source with laser_id {id} not found"
+        )))
+    }
+
     #[getter]
     /// The positions of the exit tiles.
     fn exit_pos(&self) -> Vec<Position> {
         self.world.exits().map(|(pos, _)| pos).copied().collect()
     }
 
     /// Perform a step in the world and returns the events that happened during that transition.
     pub fn step(&mut self, actions: Vec<PyAction>) -> PyResult<Vec<PyWorldEvent>> {
         let actions: Vec<_> = actions.into_iter().map(|a| a.action).collect();
         match self.world.step(&actions) {
             Ok(events) => {
-                let events: Vec<PyWorldEvent> = events
-                    .iter()
-                    .map(|e| match e {
-                        WorldEvent::AgentExit { agent_id } => {
-                            PyWorldEvent::new(PyEventType::AgentExit, *agent_id)
-                        }
-                        WorldEvent::GemCollected { agent_id } => {
-                            PyWorldEvent::new(PyEventType::GemCollected, *agent_id)
-                        }
-                        WorldEvent::AgentDied { agent_id } => {
-                            PyWorldEvent::new(PyEventType::AgentDied, *agent_id)
-                        }
-                    })
-                    .collect();
+                let events: Vec<PyWorldEvent> =
+                    events.iter().map(|e| PyWorldEvent::from(e)).collect();
                 Ok(events)
             }
             Err(e) => Err(runtime_error_to_pyexception(e)),
         }
     }
 
     /// Reset the world to its original state.
@@ -204,15 +234,15 @@
 
     /// Renders the world as an image and returns it in a numpy array.
     fn get_image(&self, py: Python) -> PyResult<PyObject> {
         let dims = self.image_dimensions();
         let dims = (dims.1 as usize, dims.0 as usize, 3);
         let img = self.renderer.update(&self.world);
         let buffer = img.into_raw();
-        let res = PyArray1::from_vec(py, buffer)
+        let res = PyArray1::from_vec_bound(py, buffer)
             .reshape(dims)
             .unwrap_or_else(|_| panic!("Could not reshape the image to {dims:?}"));
         Ok(res.into_py(py))
     }
 
     /// Force the world to a specific state
     fn set_state(&mut self, state: PyWorldState) -> PyResult<Vec<PyWorldEvent>> {
@@ -224,15 +254,15 @@
 
     /// Return the current state of the world (that can be set with `world.set_state`)
     fn get_state(&self) -> PyWorldState {
         let state = self.world.get_state();
         PyWorldState::new(state.agents_positions, state.gems_collected)
     }
 
-    pub fn __deepcopy__(&self, _memo: &PyDict) -> Self {
+    pub fn __deepcopy__(&self, _memo: &Bound<PyDict>) -> Self {
         self.clone()
     }
 
     /// This method is called to instantiate the object before deserialisation.
     /// It required "default arguments" to be provided to the __new__ method
     /// before replacing them by the actual values in __setstate__.
     pub fn __getnewargs__(&self) -> PyResult<(String,)> {
```

### Comparing `laser_learning_environment-0.2.0/src/bindings/pyworld_state.rs` & `laser_learning_environment-0.2.2/src/bindings/pyworld_state.rs`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     pub fn new(agents_positions: Vec<Position>, gems_collected: Vec<bool>) -> Self {
         Self {
             agents_positions,
             gems_collected,
         }
     }
 
-    fn __deepcopy__(&self, _memo: &PyDict) -> Self {
+    fn __deepcopy__(&self, _memo: &Bound<'_, PyDict>) -> Self {
         self.clone()
     }
 
     fn __getstate__(&self) -> PyResult<(Vec<bool>, Vec<Position>)> {
         Ok((self.gems_collected.clone(), self.agents_positions.clone()))
     }
```

### Comparing `laser_learning_environment-0.2.0/src/core/errors.rs` & `laser_learning_environment-0.2.2/src/core/errors.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/core/levels.rs` & `laser_learning_environment-0.2.2/src/core/levels.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/core/parsing/errors.rs` & `laser_learning_environment-0.2.2/src/core/parsing/errors.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/core/parsing/parser.rs` & `laser_learning_environment-0.2.2/src/core/parsing/parser.rs`

 * *Files 4% similar despite different names*

```diff
@@ -133,14 +133,15 @@
     grid: &mut Vec<Vec<Rc<dyn Tile>>>,
     laser_sources: &[(Position, Rc<LaserSource>)],
 ) -> Vec<(Position, Rc<Laser>)> {
     let mut lasers = vec![];
     let width = grid[0].len() as i32;
     let height: i32 = grid.len() as i32;
     for (pos, source) in laser_sources.iter() {
+        let laser_id = source.laser_id();
         let dir = source.direction();
         let delta = dir.delta();
         let (mut i, mut j) = (pos.0 as i32, pos.1 as i32);
         let mut beam = vec![];
         let mut beam_pos = vec![];
 
         (i, j) = ((i + delta.0), (j + delta.1));
@@ -154,15 +155,15 @@
             beam_pos.push(pos);
             (i, j) = ((i + delta.0), (j + delta.1));
         }
 
         for (i, pos) in beam_pos.iter().enumerate() {
             let beam = LaserBeam::new(beam[i..].to_vec());
             let wrapped = grid[pos.0].remove(pos.1);
-            let laser = Rc::new(Laser::new(source.agent_id(), dir, wrapped, beam));
+            let laser = Rc::new(Laser::new(laser_id, source.agent_id(), dir, wrapped, beam));
             lasers.push((*pos, laser.clone()));
             source.add_laser_tile(laser.clone());
             grid[pos.0].insert(pos.1, laser);
         }
     }
     lasers
 }
```

### Comparing `laser_learning_environment-0.2.0/src/core/tiles/direction.rs` & `laser_learning_environment-0.2.2/src/core/tiles/direction.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/core/tiles/gem.rs` & `laser_learning_environment-0.2.2/src/core/tiles/gem.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/core/tiles/laser.rs` & `laser_learning_environment-0.2.2/src/core/tiles/laser.rs`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 use crate::{
     agent::{Agent, AgentId},
     rendering::{TileVisitor, VisitorData},
     WorldEvent,
 };
 
-use super::Tile;
+use super::{laser_source::LaserId, Tile};
 
 #[derive(Clone, Copy, Debug, PartialEq)]
 pub enum Direction {
     North,
     East,
     South,
     West,
@@ -76,35 +76,44 @@
         for cell in &self.beam {
             cell.set(false);
         }
     }
 }
 
 pub struct Laser {
+    laser_id: LaserId,
     direction: Direction,
     agent_id: Cell<AgentId>,
     beam: LaserBeam,
     wrapped: Rc<dyn Tile>,
+    disabled: Cell<bool>,
 }
 
 impl Laser {
     pub fn new(
+        laser_id: LaserId,
         agent_id: AgentId,
         direction: Direction,
         wrapped: Rc<dyn Tile>,
         beam: LaserBeam,
     ) -> Self {
         Self {
+            laser_id,
             agent_id: Cell::new(agent_id),
             direction,
             wrapped,
             beam,
+            disabled: Cell::new(false),
         }
     }
 
+    pub fn laser_id(&self) -> LaserId {
+        self.laser_id
+    }
+
     pub fn agent_id(&self) -> AgentId {
         self.agent_id.get()
     }
 
     pub fn set_agent_id(&self, agent_id: AgentId) {
         self.agent_id.set(agent_id);
     }
@@ -117,19 +126,40 @@
         self.beam.is_on()
     }
 
     pub fn is_off(&self) -> bool {
         self.beam.is_off()
     }
 
+    pub fn is_enabled(&self) -> bool {
+        !self.disabled.get()
+    }
+
+    pub fn is_disabled(&self) -> bool {
+        self.disabled.get()
+    }
+
     pub fn direction(&self) -> Direction {
         self.direction
     }
 
+    pub fn disable(&self) {
+        self.disabled.set(true);
+        self.turn_off();
+    }
+
+    pub fn enable(&self) {
+        self.disabled.set(false);
+        self.turn_on();
+    }
+
     pub fn turn_on(&self) {
+        if self.disabled.get() {
+            return;
+        }
         self.beam.turn_on();
     }
 
     pub fn turn_off(&self) {
         self.beam.turn_off();
     }
 }
@@ -138,14 +168,17 @@
     fn reset(&self) {
         self.turn_on();
         self.wrapped.reset();
     }
 
     fn pre_enter(&self, agent: &Agent) -> Result<(), String> {
         let res = self.wrapped.pre_enter(agent);
+        if self.disabled.get() {
+            return res;
+        }
         if agent.is_alive() && agent.id() == self.agent_id.get() {
             self.turn_off();
         }
         res
     }
 
     fn enter(&self, agent: &mut Agent) -> Option<WorldEvent> {
```

### Comparing `laser_learning_environment-0.2.0/src/core/tiles/laser_source.rs` & `laser_learning_environment-0.2.2/src/core/tiles/tile.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,137 @@
-use std::{
-    cell::{Cell, RefCell},
-    rc::Rc,
-};
-
 use crate::{
     agent::{Agent, AgentId},
     rendering::{TileVisitor, VisitorData},
     WorldEvent,
 };
+use core::panic;
+use std::cell::Cell;
 
-use super::{Direction, Laser, Tile, Wall};
-
-#[derive(Clone)]
-pub struct LaserSource {
-    wall: Wall,
-    laser_tiles: RefCell<Vec<Rc<Laser>>>,
-    direction: Direction,
-    agent_id: Cell<AgentId>,
-}
-
-impl LaserSource {
-    pub fn new(direction: Direction, agent_id: AgentId) -> Self {
-        Self {
-            wall: Wall {},
-            direction,
-            agent_id: Cell::new(agent_id),
-            laser_tiles: RefCell::new(vec![]),
+pub trait Tile {
+    fn pre_enter(&self, _agent: &Agent) -> Result<(), String> {
+        if !self.is_waklable() {
+            return Err("Cannot walk on this tile".to_string());
         }
+        Ok(())
     }
-
-    pub fn agent_id(&self) -> AgentId {
-        self.agent_id.get()
+    fn reset(&self);
+    fn enter(&self, agent: &mut Agent) -> Option<WorldEvent>;
+    fn leave(&self) -> AgentId;
+    fn agent(&self) -> Option<AgentId>;
+    fn is_waklable(&self) -> bool {
+        true
+    }
+    fn is_occupied(&self) -> bool {
+        self.agent().is_some()
     }
+    /// Visitor pattern to render the tile
+    fn accept(&self, visitor: &dyn TileVisitor, data: &mut VisitorData);
+}
+
+#[derive(Default)]
+pub struct Floor {
+    agent: Cell<Option<AgentId>>,
+}
 
-    pub fn direction(&self) -> Direction {
-        self.direction
+impl Tile for Floor {
+    fn reset(&self) {
+        self.agent.set(None);
     }
 
-    pub fn turn_on(&self) {
-        self.laser_tiles.borrow_mut().iter().for_each(|laser| {
-            laser.turn_on();
-        });
+    fn enter(&self, agent: &mut Agent) -> Option<WorldEvent> {
+        self.agent.set(Some(agent.id()));
+        None
     }
 
-    pub fn turn_off(&self) {
-        self.laser_tiles.borrow_mut().iter().for_each(|laser| {
-            laser.turn_off();
-        });
+    fn leave(&self) -> AgentId {
+        self.agent.take().expect("Can not call leave() because there is no agent on this tile.\nMaybe you forgot to perform a world.reset()?")
     }
 
-    pub fn add_laser_tile(&self, laser_tile: Rc<Laser>) {
-        self.laser_tiles.borrow_mut().push(laser_tile);
+    fn agent(&self) -> Option<AgentId> {
+        self.agent.get()
     }
 
-    pub fn set_agent_id(&self, agent_id: AgentId) {
-        self.agent_id.set(agent_id);
-        self.laser_tiles.borrow_mut().iter().for_each(|laser| {
-            laser.set_agent_id(agent_id);
-        });
+    fn accept(&self, _visitor: &dyn TileVisitor, _data: &mut VisitorData) {
+        // Nothing to do
     }
 }
 
-impl Tile for LaserSource {
-    fn pre_enter(&self, agent: &Agent) -> Result<(), String> {
-        self.wall.pre_enter(agent)
-    }
+#[derive(Default, Clone)]
+pub struct Wall {}
 
-    fn reset(&self) {
-        self.wall.reset();
+impl Tile for Wall {
+    fn pre_enter(&self, _agent: &Agent) -> Result<(), String> {
+        Err("Cannot pre-enter a wall".into())
     }
 
-    fn enter(&self, agent: &mut Agent) -> Option<WorldEvent> {
-        self.wall.enter(agent)
+    fn reset(&self) {}
+
+    fn enter(&self, _agent: &mut Agent) -> Option<WorldEvent> {
+        panic!("Cannot enter a wall")
     }
 
     fn leave(&self) -> AgentId {
-        self.wall.leave()
+        panic!("Cannot leave a wall")
+    }
+
+    fn is_occupied(&self) -> bool {
+        true
     }
 
     fn agent(&self) -> Option<AgentId> {
-        self.wall.agent()
+        None
     }
 
     fn is_waklable(&self) -> bool {
         false
     }
 
     fn accept(&self, _visitor: &dyn TileVisitor, _data: &mut VisitorData) {
         // Nothing to do here as it is statically rendered
     }
 }
+
+#[derive(Default)]
+pub struct Void {
+    agent: Cell<Option<AgentId>>,
+}
+
+impl Tile for Void {
+    fn agent(&self) -> Option<AgentId> {
+        self.agent.get()
+    }
+
+    fn enter(&self, agent: &mut Agent) -> Option<WorldEvent> {
+        self.agent.set(Some(agent.id()));
+        if agent.is_alive() {
+            agent.die();
+            return Some(WorldEvent::AgentDied {
+                agent_id: agent.id(),
+            });
+        }
+        None
+    }
+
+    fn leave(&self) -> AgentId {
+        panic!("Cannot leave a void: the game should be over !")
+    }
+
+    fn is_occupied(&self) -> bool {
+        self.agent.get().is_some()
+    }
+
+    fn is_waklable(&self) -> bool {
+        true
+    }
+
+    fn reset(&self) {
+        self.agent.set(None);
+    }
+
+    fn accept(&self, _visitor: &dyn TileVisitor, _data: &mut VisitorData) {
+        // Nothing to do
+    }
+}
+
+#[cfg(test)]
+#[path = "../../unit_tests/test_tile.rs"]
+mod tests;
```

### Comparing `laser_learning_environment-0.2.0/src/core/tiles/start_exit.rs` & `laser_learning_environment-0.2.2/src/core/tiles/start_exit.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/core/tiles/tile.rs` & `laser_learning_environment-0.2.2/src/core/tiles/laser_source.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,137 +1,116 @@
+use std::{
+    cell::{Cell, RefCell},
+    rc::Rc,
+    sync::Mutex,
+};
+
 use crate::{
     agent::{Agent, AgentId},
     rendering::{TileVisitor, VisitorData},
     WorldEvent,
 };
-use core::panic;
-use std::cell::Cell;
 
-pub trait Tile {
-    fn pre_enter(&self, _agent: &Agent) -> Result<(), String> {
-        if !self.is_waklable() {
-            return Err("Cannot walk on this tile".to_string());
-        }
-        Ok(())
-    }
-    fn reset(&self);
-    fn enter(&self, agent: &mut Agent) -> Option<WorldEvent>;
-    fn leave(&self) -> AgentId;
-    fn agent(&self) -> Option<AgentId>;
-    fn is_waklable(&self) -> bool {
-        true
-    }
-    fn is_occupied(&self) -> bool {
-        self.agent().is_some()
-    }
-    /// Visitor pattern to render the tile
-    fn accept(&self, visitor: &dyn TileVisitor, data: &mut VisitorData);
-}
+pub type LaserId = usize;
+use super::{Direction, Laser, Tile, Wall};
 
-#[derive(Default)]
-pub struct Floor {
-    agent: Cell<Option<AgentId>>,
-}
+const NUM_LASERS: Mutex<LaserId> = Mutex::new(0);
 
-impl Tile for Floor {
-    fn reset(&self) {
-        self.agent.set(None);
-    }
-
-    fn enter(&self, agent: &mut Agent) -> Option<WorldEvent> {
-        self.agent.set(Some(agent.id()));
-        None
-    }
-
-    fn leave(&self) -> AgentId {
-        self.agent.take().expect("Can not call leave() because there is no agent on this tile.\nMaybe you forgot to perform a world.reset()?")
-    }
-
-    fn agent(&self) -> Option<AgentId> {
-        self.agent.get()
+#[derive(Clone)]
+pub struct LaserSource {
+    enabled: Cell<bool>,
+    laser_id: LaserId,
+    wall: Wall,
+    laser_tiles: RefCell<Vec<Rc<Laser>>>,
+    direction: Direction,
+    agent_id: Cell<AgentId>,
+}
+
+impl LaserSource {
+    pub fn new(direction: Direction, agent_id: AgentId) -> Self {
+        // Increment the number of lasers and get the new id
+        let binding = NUM_LASERS;
+        let mut num_lasers = binding.lock().unwrap();
+        let laser_id = *num_lasers;
+        *num_lasers += 1;
+
+        Self {
+            enabled: Cell::new(true),
+            laser_id,
+            wall: Wall {},
+            direction,
+            agent_id: Cell::new(agent_id),
+            laser_tiles: RefCell::new(vec![]),
+        }
     }
 
-    fn accept(&self, _visitor: &dyn TileVisitor, _data: &mut VisitorData) {
-        // Nothing to do
+    pub fn is_enabled(&self) -> bool {
+        self.enabled.get()
     }
-}
-
-#[derive(Default, Clone)]
-pub struct Wall {}
 
-impl Tile for Wall {
-    fn pre_enter(&self, _agent: &Agent) -> Result<(), String> {
-        Err("Cannot pre-enter a wall".into())
+    pub fn agent_id(&self) -> AgentId {
+        self.agent_id.get()
     }
 
-    fn reset(&self) {}
-
-    fn enter(&self, _agent: &mut Agent) -> Option<WorldEvent> {
-        panic!("Cannot enter a wall")
+    pub fn direction(&self) -> Direction {
+        self.direction
     }
 
-    fn leave(&self) -> AgentId {
-        panic!("Cannot leave a wall")
+    pub fn laser_id(&self) -> LaserId {
+        self.laser_id
     }
 
-    fn is_occupied(&self) -> bool {
-        true
+    pub fn enable(&self) {
+        self.enabled.set(true);
+        self.laser_tiles.borrow().iter().for_each(|laser| {
+            laser.enable();
+        });
     }
 
-    fn agent(&self) -> Option<AgentId> {
-        None
+    pub fn disable(&self) {
+        self.enabled.set(false);
+        self.laser_tiles.borrow().iter().for_each(|laser| {
+            laser.disable();
+        });
     }
 
-    fn is_waklable(&self) -> bool {
-        false
+    pub fn add_laser_tile(&self, laser_tile: Rc<Laser>) {
+        self.laser_tiles.borrow_mut().push(laser_tile);
     }
 
-    fn accept(&self, _visitor: &dyn TileVisitor, _data: &mut VisitorData) {
-        // Nothing to do here as it is statically rendered
+    pub fn set_agent_id(&self, agent_id: AgentId) {
+        self.agent_id.set(agent_id);
+        self.laser_tiles.borrow_mut().iter().for_each(|laser| {
+            laser.set_agent_id(agent_id);
+        });
     }
 }
 
-#[derive(Default)]
-pub struct Void {
-    agent: Cell<Option<AgentId>>,
-}
+impl Tile for LaserSource {
+    fn pre_enter(&self, agent: &Agent) -> Result<(), String> {
+        self.wall.pre_enter(agent)
+    }
 
-impl Tile for Void {
-    fn agent(&self) -> Option<AgentId> {
-        self.agent.get()
+    fn reset(&self) {
+        self.wall.reset();
     }
 
     fn enter(&self, agent: &mut Agent) -> Option<WorldEvent> {
-        self.agent.set(Some(agent.id()));
-        if agent.is_alive() {
-            agent.die();
-            return Some(WorldEvent::AgentDied {
-                agent_id: agent.id(),
-            });
-        }
-        None
+        self.wall.enter(agent)
     }
 
     fn leave(&self) -> AgentId {
-        panic!("Cannot leave a void: the game should be over !")
+        self.wall.leave()
     }
 
-    fn is_occupied(&self) -> bool {
-        self.agent.get().is_some()
+    fn agent(&self) -> Option<AgentId> {
+        self.wall.agent()
     }
 
     fn is_waklable(&self) -> bool {
-        true
-    }
-
-    fn reset(&self) {
-        self.agent.set(None);
+        false
     }
 
     fn accept(&self, _visitor: &dyn TileVisitor, _data: &mut VisitorData) {
-        // Nothing to do
+        // Nothing to do here as it is statically rendered
     }
 }
-
-#[cfg(test)]
-#[path = "../../unit_tests/test_tile.rs"]
-mod tests;
```

### Comparing `laser_learning_environment-0.2.0/src/core/world.rs` & `laser_learning_environment-0.2.2/src/core/world.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/rendering/renderer.rs` & `laser_learning_environment-0.2.2/src/rendering/renderer.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/rendering/sprites.rs` & `laser_learning_environment-0.2.2/src/rendering/sprites.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/unit_tests/test_core.rs` & `laser_learning_environment-0.2.2/src/unit_tests/test_core.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/unit_tests/test_done_strategy.rs` & `laser_learning_environment-0.2.2/src/unit_tests/test_done_strategy.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/src/unit_tests/test_tile.rs` & `laser_learning_environment-0.2.2/src/unit_tests/test_tile.rs`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 };
 
 fn make_laser(agent_id: AgentId, length: usize) -> Laser {
     let wrapped = Rc::new(Floor::default());
     let mut beam = Vec::with_capacity(4);
     (0..length).for_each(|_| beam.push(Rc::new(Cell::new(true))));
     let beam = LaserBeam::new(beam);
-    Laser::new(agent_id, crate::tiles::Direction::East, wrapped, beam)
+    Laser::new(0, agent_id, crate::tiles::Direction::East, wrapped, beam)
 }
 
 #[test]
 fn test_start() {
     let mut agent = Agent::new(0);
     let start = Start::new(agent.id());
     assert_eq!(start.agent_id(), 0);
```

### Comparing `laser_learning_environment-0.2.0/src/utils/mod.rs` & `laser_learning_environment-0.2.2/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `laser_learning_environment-0.2.0/tests/world_integration_tests.rs` & `laser_learning_environment-0.2.2/tests/world_integration_tests.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use lle::{Action, ParseError, RuntimeWorldError, World, WorldEvent, WorldState};
+use lle::{tiles::Laser, Action, ParseError, RuntimeWorldError, World, WorldEvent, WorldState};
 
 #[test]
 fn test_available_actions() {
     let mut w = World::try_from(
         "
     S0 . G
     L0E X .
@@ -359,24 +359,67 @@
             assert_eq!(*agent_id, 0);
         }
         other => panic!("Expected AgentDied, got {:?}", other),
     }
 }
 
 #[test]
-fn turn_off_laser_source() {
+fn disable_laser_source() {
     let mut w = World::try_from(
         "
         S0 .   G  X
         .  .  L0W .
         .  S1  .  X 
         .  .   .  .",
     )
     .unwrap();
     w.reset();
     assert!(w.lasers().all(|(_, l)| l.is_on()));
     let (_, source) = w.laser_sources().next().unwrap();
-    source.turn_off();
+    source.disable();
     assert!(w.lasers().all(|(_, l)| l.is_off()));
-    source.turn_on();
+    source.enable();
     assert!(w.lasers().all(|(_, l)| l.is_on()));
 }
+
+/// We check that disabling a laser source will turn off the lasers it is connected to,
+/// even when an agent walks into the beam and then walks back away.
+#[test]
+fn disable_laser_source_and_block_with_agent() {
+    let mut w = World::try_from("L0E . S0 X").unwrap();
+    w.reset();
+
+    fn get_laser_at(w: &World, pos: (usize, usize)) -> &Laser {
+        w.lasers()
+            .filter(|(p, _)| **p == pos)
+            .map(|(_, l)| l)
+            .collect::<Vec<_>>()
+            .first()
+            .unwrap()
+    }
+    let laser = get_laser_at(&w, (0, 1));
+    assert!(laser.is_on());
+    w.laser_sources().next().unwrap().1.disable();
+    assert!(laser.is_off());
+    w.step(&[Action::West]).unwrap();
+    let laser = get_laser_at(&w, (0, 2));
+    assert!(laser.is_off());
+    w.step(&[Action::East]).unwrap();
+    let laser = get_laser_at(&w, (0, 1));
+    assert!(laser.is_off());
+}
+
+#[test]
+fn test_laser_id() {
+    let mut w = World::try_from(
+        "
+        S0 .   G  X
+        .  .  L0W .
+        .  S1  .  X 
+        .  .   .  .",
+    )
+    .unwrap();
+    w.reset();
+    let (_, source) = w.laser_sources().next().unwrap();
+    assert_eq!(source.laser_id(), 0);
+    assert!(w.lasers().all(|(_, l)| l.laser_id() == 0));
+}
```

### Comparing `laser_learning_environment-0.2.0/Cargo.lock` & `laser_learning_environment-0.2.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -289,17 +289,17 @@
 name = "heck"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
 
 [[package]]
 name = "image"
-version = "0.25.0"
+version = "0.25.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9b4f005360d32e9325029b38ba47ebd7a56f3316df09249368939562d518645"
+checksum = "fd54d660e773627692c524beaad361aca785a4f9f5730ce91f42aabe5bce3d11"
 dependencies = [
  "bytemuck",
  "byteorder",
  "color_quant",
  "exr",
  "gif",
  "image-webp",
@@ -408,15 +408,15 @@
  "arbitrary",
  "cc",
  "once_cell",
 ]
 
 [[package]]
 name = "lle"
-version = "0.2.0"
+version = "0.2.2"
 dependencies = [
  "image",
  "itertools",
  "lazy_static",
  "numpy",
  "pyo3",
  "toml",
@@ -592,17 +592,17 @@
 checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef41cbb417ea83b30525259e30ccef6af39b31c240bda578889494c5392d331"
+checksum = "ec170733ca37175f5d75a5bea5911d6ff45d2cd52849ce98b685394e4f2f37f4"
 dependencies = [
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
@@ -701,17 +701,17 @@
 dependencies = [
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -719,49 +719,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
@@ -983,17 +983,17 @@
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
  "lock_api",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.55"
+version = "2.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
+checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `laser_learning_environment-0.2.0/pyproject.toml` & `laser_learning_environment-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -17,27 +17,25 @@
 python-source = "python"
 
 [tool.poetry]
 authors = ["Yannick Molinghen <yannick.molinghen@ulb.be>"]
 description = "Laser Learning Environment (LLE) for Multi-Agent Reinforcement Learning"
 name = "lle"
 readme = "readme.md"
-version = "0.2.0"
+version = "0.2.2"
 
 [tool.poetry.dependencies]
 numpy = "^1.25.0"
 opencv-python = "^4.8.1.78"
 pyserde = "^0.12.3"
 python = ">=3.10,<3.13"
 
 [tool.poetry.dependencies.rlenv]
-# Git with tag "v1.0.0"
 branch = "main"
 git = "https://github.com/yamoling/rlenv.git"
-tag = "v1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.26.0"
 maturin = "^1.1.0"
 mypy = "^1.5.1"
 pytest = "^7.4.0"
 pytest-xdist = "^3.4.0"
```

### Comparing `laser_learning_environment-0.2.0/PKG-INFO` & `laser_learning_environment-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: laser-learning-environment
-Version: 0.2.0
+Version: 0.2.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Summary: A fast Multi-Agent Reinforcement Learning Environment
 Requires-Python: >=3.10, <4.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Laser Learning Environment (LLE)
```

