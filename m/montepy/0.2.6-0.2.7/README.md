# Comparing `tmp/montepy-0.2.6.tar.gz` & `tmp/montepy-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "montepy-0.2.6.tar", last modified: Mon Apr 15 21:59:32 2024, max compression
+gzip compressed data, was "montepy-0.2.7.tar", last modified: Thu May 30 18:12:54 2024, max compression
```

## Comparing `montepy-0.2.6.tar` & `montepy-0.2.7.tar`

### file list

```diff
@@ -1,240 +1,249 @@
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:32.125330 montepy-0.2.6/
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.239627 montepy-0.2.6/.github/
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.297110 montepy-0.2.6/.github/ISSUE_TEMPLATE/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2491 2024-04-15 21:58:30.000000 montepy-0.2.6/.github/ISSUE_TEMPLATE/bug_report.md
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      773 2024-04-15 21:58:30.000000 montepy-0.2.6/.github/ISSUE_TEMPLATE/feature_request.md
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      668 2024-04-15 21:58:30.000000 montepy-0.2.6/.github/pull_request_template.md
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.348112 montepy-0.2.6/.github/workflows/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4475 2024-04-15 21:58:30.000000 montepy-0.2.6/.github/workflows/deploy.yml
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3484 2024-04-15 21:58:30.000000 montepy-0.2.6/.github/workflows/main.yml
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      142 2024-04-15 21:58:30.000000 montepy-0.2.6/.gitignore
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-10 03:00:18.000000 montepy-0.2.6/AUTHORS
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1086 2024-01-10 02:47:53.000000 montepy-0.2.6/LICENSE
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1742 2024-01-10 02:47:34.000000 montepy-0.2.6/NOTICE.txt
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6597 2024-04-15 21:59:32.114337 montepy-0.2.6/PKG-INFO
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3317 2024-04-15 21:58:30.000000 montepy-0.2.6/README.md
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.415146 montepy-0.2.6/demo/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3932 2024-01-12 01:37:19.000000 montepy-0.2.6/demo/Pin_cell.ipynb
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      620 2024-01-12 01:37:19.000000 montepy-0.2.6/demo/pin_cell.imcnp
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.477595 montepy-0.2.6/doc/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      638 2024-01-10 03:00:18.000000 montepy-0.2.6/doc/Makefile
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      799 2024-01-10 03:00:18.000000 montepy-0.2.6/doc/make.bat
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.942703 montepy-0.2.6/doc/source/
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.981225 montepy-0.2.6/doc/source/_static/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-01-10 03:00:18.000000 montepy-0.2.6/doc/source/_static/placeholder
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:25.023227 montepy-0.2.6/doc/source/_templates/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-01-10 03:00:18.000000 montepy-0.2.6/doc/source/_templates/placeholder
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1026 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/_test_for_missing_docs.py
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:27.447191 montepy-0.2.6/doc/source/api/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       67 2024-04-15 21:58:25.000000 montepy-0.2.6/doc/source/api/modules.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      125 2024-04-15 21:58:25.000000 montepy-0.2.6/doc/source/api/montepy.cell.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      128 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.cells.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.constants.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      365 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.cell_modifier.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      248 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.data_input.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      186 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.data_parser.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.element.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      163 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.fill.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      181 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.importance.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.isotope.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.lattice.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      192 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.lattice_input.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      175 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.material.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      207 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.material_component.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      163 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.mode.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      816 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      166 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.tally.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      199 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.tally_multiplier.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      207 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.thermal_scattering.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      178 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.transform.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      195 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.universe_input.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      169 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.volume.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      131 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.errors.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      169 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.geometry_operators.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      186 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.block_type.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      189 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.cell_parser.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      189 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.data_parser.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      242 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.input_file.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      192 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.input_reader.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      215 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.input_syntax_reader.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      186 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.mcnp_input.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      189 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.parser_base.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      189 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.read_parser.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      753 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      181 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.shortcuts.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      198 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.surface_parser.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      244 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.syntax_node.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      192 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.tally_parser.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      198 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.thermal_parser.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.tokens.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.materials.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      208 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.mcnp_object.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      151 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.mcnp_problem.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      177 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.numbered_mcnp_object.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      195 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.numbered_object_collection.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      137 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.particle.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      663 2024-04-15 21:58:25.000000 montepy-0.2.6/doc/source/api/montepy.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      169 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surface_collection.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.axis_plane.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      192 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.cylinder_on_axis.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      195 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.cylinder_par_axis.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      181 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.general_plane.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.half_space.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      461 2024-04-15 21:58:25.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      161 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.surface.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      187 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.surface_builder.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      178 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.surface_type.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      143 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.transforms.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      137 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.universe.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.universes.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.utilities.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2275 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/conf.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    42074 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/developing.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3373 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/faq.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      861 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/index.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    98645 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/monty.svg
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      362 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/publications.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    28253 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/starting.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2141 2024-01-10 03:00:18.000000 montepy-0.2.6/doc/source/tricks.rst
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4057 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/utilities.rst
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:27.468191 montepy-0.2.6/graphics/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    98645 2024-01-12 01:37:20.000000 montepy-0.2.6/graphics/monty.svg
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:28.097539 montepy-0.2.6/montepy/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1383 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/__init__.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1784 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/__main__.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1182 2024-01-10 03:00:19.000000 montepy-0.2.6/montepy/_cell_data_control.py
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:28.267306 montepy-0.2.6/montepy/_scripts/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/_scripts/__init__.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2566 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/_scripts/change_to_ascii.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      411 2024-04-15 21:59:20.000000 montepy-0.2.6/montepy/_version.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    24162 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/cell.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6872 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/cells.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1818 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/constants.py
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:29.134337 montepy-0.2.6/montepy/data_inputs/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      256 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/__init__.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    10340 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/cell_modifier.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    10150 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/data_input.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1271 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/data_parser.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7752 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/element.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    19502 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/data_inputs/fill.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    15591 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/importance.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5753 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/isotope.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      400 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/lattice.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4238 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/lattice_input.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7849 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/data_inputs/material.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1956 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/material_component.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5451 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/mode.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      466 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/tally.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      449 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/tally_multiplier.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4438 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/thermal_scattering.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     8779 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/transform.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7412 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/universe_input.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6873 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/volume.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5935 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/errors.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      558 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/geometry_operators.py
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:29.705772 montepy-0.2.6/montepy/input_parser/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      358 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/__init__.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      478 2024-01-10 03:00:19.000000 montepy-0.2.6/montepy/input_parser/block_type.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6467 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/input_parser/cell_parser.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5014 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/data_parser.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4148 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/input_parser/input_file.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1321 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/input_parser/input_reader.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7611 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/input_parser/input_syntax_reader.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    12817 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/mcnp_input.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    14577 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/parser_base.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1341 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/read_parser.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      632 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/shortcuts.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1839 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/surface_parser.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    65199 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/input_parser/syntax_node.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2192 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/tally_parser.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1124 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/thermal_parser.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    11112 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/tokens.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      551 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/materials.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    15206 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/mcnp_object.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    17607 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/mcnp_problem.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      571 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/numbered_mcnp_object.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    14849 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/numbered_object_collection.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1245 2024-01-10 03:00:19.000000 montepy-0.2.6/montepy/particle.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1791 2024-01-10 03:00:19.000000 montepy-0.2.6/montepy/surface_collection.py
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:30.107340 montepy-0.2.6/montepy/surfaces/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      360 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/__init__.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2364 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/axis_plane.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2454 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/cylinder_on_axis.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4234 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/cylinder_par_axis.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      981 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/general_plane.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    22387 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/half_space.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    11238 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/surface.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1288 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/surface_builder.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2549 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/surface_type.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      451 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/transforms.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3169 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/universe.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      421 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/universes.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5136 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/utilities.py
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:32.100331 montepy-0.2.6/montepy.egg-info/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6597 2024-04-15 21:59:20.000000 montepy-0.2.6/montepy.egg-info/PKG-INFO
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7513 2024-04-15 21:59:24.000000 montepy-0.2.6/montepy.egg-info/SOURCES.txt
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)        1 2024-04-15 21:59:20.000000 montepy-0.2.6/montepy.egg-info/dependency_links.txt
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       74 2024-04-15 21:59:20.000000 montepy-0.2.6/montepy.egg-info/entry_points.txt
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      236 2024-04-15 21:59:20.000000 montepy-0.2.6/montepy.egg-info/requires.txt
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)        8 2024-04-15 21:59:20.000000 montepy-0.2.6/montepy.egg-info/top_level.txt
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2303 2024-04-15 21:58:30.000000 montepy-0.2.6/pyproject.toml
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       38 2024-04-15 21:59:32.126331 montepy-0.2.6/setup.cfg
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:30.891354 montepy-0.2.6/tests/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/__init__.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      841 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/constants.py
-drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:32.070547 montepy-0.2.6/tests/inputs/
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      912 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/inputs/bad_encoding.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      293 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/breaking_comments.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      626 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/number_conflict_pin_cell.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      887 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/inputs/test.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       87 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/testRead.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       63 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/testReadRec1.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       29 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/testReadRec2.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)        7 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/testReadRec3.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)        8 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/testReadTarget.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       56 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/testVerticalMode.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       34 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_bad_syntax.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       79 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_broken_cell_surf_link.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       77 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_broken_complement.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       76 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_broken_mat_link.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       41 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_broken_surf_link.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       57 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_broken_transform_link.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      641 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_complement_edge.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      835 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_dos.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      125 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_excess_mt.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       77 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_extra_data_imp.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       51 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_extra_data_param.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       88 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_extra_params.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      766 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_imp_redundant.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      765 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_importance.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       84 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_interp_edge.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      957 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_long_lines.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       95 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_missing_mat_for_mt.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      355 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_redundant_surf.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)       62 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_surfaces.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      853 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_tab.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      937 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_universe.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      768 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_universe_data.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      782 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_vol_redundant.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      881 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/inputs/unicode.imcnp
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5775 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_cell_problem.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    12053 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_data_inputs.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7255 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/test_edge_cases.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    17864 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/test_geometry.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7097 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_importance.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2249 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_input_file.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    43268 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/test_integration.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1071 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_interface.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1379 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_main.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    14900 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_material.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      816 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_mcnp_problem.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3579 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_mode.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    10482 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/test_numbered_collection.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3356 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/test_scripts.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      561 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_source_def.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    11668 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_surfaces.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    57902 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_syntax_parsing.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1266 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_tally.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    10797 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_transform.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)    14670 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_universe.py
--rwxrwxrwx   0 mgale     (1000) mgale     (1000)      748 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/test_utilities.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:54.453007 montepy-0.2.7/
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:42.082267 montepy-0.2.7/.github/
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:42.198265 montepy-0.2.7/.github/ISSUE_TEMPLATE/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2491 2024-04-15 21:58:30.000000 montepy-0.2.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      773 2024-04-15 21:58:30.000000 montepy-0.2.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      668 2024-04-15 21:58:30.000000 montepy-0.2.7/.github/pull_request_template.md
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:42.405788 montepy-0.2.7/.github/workflows/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5207 2024-05-30 18:11:44.000000 montepy-0.2.7/.github/workflows/deploy.yml
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4627 2024-05-30 18:11:44.000000 montepy-0.2.7/.github/workflows/main.yml
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      142 2024-04-15 21:58:30.000000 montepy-0.2.7/.gitignore
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-10 03:00:18.000000 montepy-0.2.7/AUTHORS
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4860 2024-05-30 18:11:44.000000 montepy-0.2.7/CHANGELOG.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1597 2024-05-30 18:11:44.000000 montepy-0.2.7/CONTRIBUTING.md
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1086 2024-01-10 02:47:53.000000 montepy-0.2.7/LICENSE
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       30 2024-05-30 18:11:44.000000 montepy-0.2.7/MANIFEST.in
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1742 2024-01-10 02:47:34.000000 montepy-0.2.7/NOTICE.txt
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6597 2024-05-30 18:12:54.438478 montepy-0.2.7/PKG-INFO
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3317 2024-04-15 21:58:30.000000 montepy-0.2.7/README.md
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:42.515914 montepy-0.2.7/demo/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3932 2024-01-12 01:37:19.000000 montepy-0.2.7/demo/Pin_cell.ipynb
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      620 2024-01-12 01:37:19.000000 montepy-0.2.7/demo/pin_cell.imcnp
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:42.624412 montepy-0.2.7/doc/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      638 2024-01-10 03:00:18.000000 montepy-0.2.7/doc/Makefile
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      799 2024-01-10 03:00:18.000000 montepy-0.2.7/doc/make.bat
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:43.552897 montepy-0.2.7/doc/source/
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:43.594896 montepy-0.2.7/doc/source/_static/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-01-10 03:00:18.000000 montepy-0.2.7/doc/source/_static/placeholder
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:43.672437 montepy-0.2.7/doc/source/_templates/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-01-10 03:00:18.000000 montepy-0.2.7/doc/source/_templates/placeholder
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1103 2024-05-30 18:11:44.000000 montepy-0.2.7/doc/source/_test_for_missing_docs.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:48.555669 montepy-0.2.7/doc/source/api/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      577 2024-05-30 18:11:44.000000 montepy-0.2.7/doc/source/api/modules.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      129 2024-05-30 18:11:44.000000 montepy-0.2.7/doc/source/api/montepy.cell.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      128 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.cells.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.constants.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      365 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.cell_modifier.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      248 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.data_input.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      186 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.data_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.element.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      163 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.fill.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      181 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.importance.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.isotope.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.lattice.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      192 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.lattice_input.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      175 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.material.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      207 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.material_component.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      163 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.mode.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      794 2024-05-30 18:11:44.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      166 2024-04-15 21:58:30.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.tally.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      199 2024-04-15 21:58:30.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.tally_multiplier.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      207 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.thermal_scattering.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      178 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.transform.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      195 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.universe_input.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      169 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.data_inputs.volume.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      131 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.errors.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      169 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.geometry_operators.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      186 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.block_type.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      189 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.cell_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      189 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.data_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      242 2024-04-15 21:58:30.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.input_file.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      192 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.input_reader.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      215 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.input_syntax_reader.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      186 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.mcnp_input.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      189 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.parser_base.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      189 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.read_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      730 2024-05-30 18:11:44.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      181 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.shortcuts.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      198 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.surface_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      244 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.syntax_node.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      192 2024-04-15 21:58:30.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.tally_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      198 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.thermal_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.input_parser.tokens.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.materials.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      208 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.mcnp_object.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      151 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.mcnp_problem.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      177 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.numbered_mcnp_object.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      195 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.numbered_object_collection.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      137 2024-01-12 01:37:19.000000 montepy-0.2.7/doc/source/api/montepy.particle.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      169 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.surface_collection.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.surfaces.axis_plane.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      192 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.surfaces.cylinder_on_axis.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      195 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.surfaces.cylinder_par_axis.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      181 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.surfaces.general_plane.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.surfaces.half_space.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      439 2024-05-30 18:11:44.000000 montepy-0.2.7/doc/source/api/montepy.surfaces.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      161 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.surfaces.surface.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      187 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.surfaces.surface_builder.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      178 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.surfaces.surface_type.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      143 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.transforms.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      137 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.universe.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.universes.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/api/montepy.utilities.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4860 2024-05-30 18:11:44.000000 montepy-0.2.7/doc/source/changelog.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2275 2024-04-15 21:58:30.000000 montepy-0.2.7/doc/source/conf.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      121 2024-05-30 18:11:44.000000 montepy-0.2.7/doc/source/dev_tree.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    40676 2024-05-30 18:11:44.000000 montepy-0.2.7/doc/source/developing.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3373 2024-04-15 21:58:30.000000 montepy-0.2.7/doc/source/faq.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1185 2024-05-30 18:11:44.000000 montepy-0.2.7/doc/source/index.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    98645 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/monty.svg
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      362 2024-04-15 21:58:30.000000 montepy-0.2.7/doc/source/publications.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4538 2024-05-30 18:11:44.000000 montepy-0.2.7/doc/source/scope.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    28253 2024-01-12 01:37:20.000000 montepy-0.2.7/doc/source/starting.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2141 2024-01-10 03:00:18.000000 montepy-0.2.7/doc/source/tricks.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      147 2024-05-30 18:11:45.000000 montepy-0.2.7/doc/source/users.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4057 2024-04-15 21:58:30.000000 montepy-0.2.7/doc/source/utilities.rst
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:48.587664 montepy-0.2.7/graphics/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    98645 2024-01-12 01:37:20.000000 montepy-0.2.7/graphics/monty.svg
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:49.500776 montepy-0.2.7/montepy/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1398 2024-05-30 18:11:45.000000 montepy-0.2.7/montepy/__init__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1784 2024-04-15 21:58:30.000000 montepy-0.2.7/montepy/__main__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1182 2024-01-10 03:00:19.000000 montepy-0.2.7/montepy/_cell_data_control.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:49.730621 montepy-0.2.7/montepy/_scripts/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:58:30.000000 montepy-0.2.7/montepy/_scripts/__init__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2566 2024-04-15 21:58:30.000000 montepy-0.2.7/montepy/_scripts/change_to_ascii.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      411 2024-05-30 18:12:33.000000 montepy-0.2.7/montepy/_version.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    24162 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/cell.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6872 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/cells.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1818 2024-04-15 21:58:30.000000 montepy-0.2.7/montepy/constants.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:50.711430 montepy-0.2.7/montepy/data_inputs/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      256 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/__init__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    10340 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/cell_modifier.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    10150 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/data_input.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1271 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/data_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7752 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/element.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    19502 2024-04-15 21:58:30.000000 montepy-0.2.7/montepy/data_inputs/fill.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    15591 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/importance.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5770 2024-05-30 18:11:45.000000 montepy-0.2.7/montepy/data_inputs/isotope.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      400 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/lattice.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4238 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/lattice_input.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     8809 2024-05-30 18:11:45.000000 montepy-0.2.7/montepy/data_inputs/material.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1956 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/material_component.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5451 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/mode.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      466 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/tally.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      449 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/tally_multiplier.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4438 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/thermal_scattering.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     8779 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/transform.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7412 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/universe_input.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6873 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/data_inputs/volume.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5935 2024-04-15 21:58:30.000000 montepy-0.2.7/montepy/errors.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      558 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/geometry_operators.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:51.531745 montepy-0.2.7/montepy/input_parser/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      388 2024-05-30 18:11:45.000000 montepy-0.2.7/montepy/input_parser/__init__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      478 2024-01-10 03:00:19.000000 montepy-0.2.7/montepy/input_parser/block_type.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6467 2024-04-15 21:58:30.000000 montepy-0.2.7/montepy/input_parser/cell_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5014 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/input_parser/data_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4148 2024-04-15 21:58:30.000000 montepy-0.2.7/montepy/input_parser/input_file.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1321 2024-04-15 21:58:30.000000 montepy-0.2.7/montepy/input_parser/input_reader.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7223 2024-05-30 18:11:45.000000 montepy-0.2.7/montepy/input_parser/input_syntax_reader.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      978 2024-05-30 18:11:45.000000 montepy-0.2.7/montepy/input_parser/material_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    13233 2024-05-30 18:11:45.000000 montepy-0.2.7/montepy/input_parser/mcnp_input.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    14600 2024-05-30 18:11:45.000000 montepy-0.2.7/montepy/input_parser/parser_base.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1341 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/input_parser/read_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      632 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/input_parser/shortcuts.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1839 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/input_parser/surface_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    65199 2024-04-15 21:58:30.000000 montepy-0.2.7/montepy/input_parser/syntax_node.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2192 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/input_parser/tally_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1124 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/input_parser/thermal_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    11112 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/input_parser/tokens.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      551 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/materials.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    15206 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/mcnp_object.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    17607 2024-04-15 21:58:30.000000 montepy-0.2.7/montepy/mcnp_problem.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      571 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/numbered_mcnp_object.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    14849 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/numbered_object_collection.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1245 2024-01-10 03:00:19.000000 montepy-0.2.7/montepy/particle.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1791 2024-01-10 03:00:19.000000 montepy-0.2.7/montepy/surface_collection.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:51.955785 montepy-0.2.7/montepy/surfaces/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      360 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/surfaces/__init__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2364 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/surfaces/axis_plane.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2454 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/surfaces/cylinder_on_axis.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4234 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/surfaces/cylinder_par_axis.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      981 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/surfaces/general_plane.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    22387 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/surfaces/half_space.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    11238 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/surfaces/surface.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1288 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/surfaces/surface_builder.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2549 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/surfaces/surface_type.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      451 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/transforms.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3169 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/universe.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      421 2024-01-12 01:37:20.000000 montepy-0.2.7/montepy/universes.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5743 2024-05-30 18:11:45.000000 montepy-0.2.7/montepy/utilities.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:54.415464 montepy-0.2.7/montepy.egg-info/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6597 2024-05-30 18:12:33.000000 montepy-0.2.7/montepy.egg-info/PKG-INFO
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7720 2024-05-30 18:12:41.000000 montepy-0.2.7/montepy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        1 2024-05-30 18:12:33.000000 montepy-0.2.7/montepy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       74 2024-05-30 18:12:33.000000 montepy-0.2.7/montepy.egg-info/entry_points.txt
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      236 2024-05-30 18:12:33.000000 montepy-0.2.7/montepy.egg-info/requires.txt
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        8 2024-05-30 18:12:33.000000 montepy-0.2.7/montepy.egg-info/top_level.txt
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2281 2024-05-30 18:11:45.000000 montepy-0.2.7/pyproject.toml
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       38 2024-05-30 18:12:54.456012 montepy-0.2.7/setup.cfg
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:52.805826 montepy-0.2.7/tests/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/__init__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      864 2024-05-30 18:11:45.000000 montepy-0.2.7/tests/constants.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-05-30 18:12:54.365467 montepy-0.2.7/tests/inputs/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      912 2024-04-15 21:58:30.000000 montepy-0.2.7/tests/inputs/bad_encoding.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      293 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/inputs/breaking_comments.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        9 2024-05-30 18:11:45.000000 montepy-0.2.7/tests/inputs/file2read.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      626 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/inputs/number_conflict_pin_cell.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       83 2024-05-30 18:11:45.000000 montepy-0.2.7/tests/inputs/readEdgeCase.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      887 2024-04-15 21:58:30.000000 montepy-0.2.7/tests/inputs/test.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       87 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/inputs/testRead.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       63 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/testReadRec1.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       29 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/testReadRec2.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        7 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/testReadRec3.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        8 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/inputs/testReadTarget.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       56 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/testVerticalMode.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       34 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/inputs/test_bad_syntax.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       79 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_broken_cell_surf_link.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       77 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_broken_complement.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       76 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_broken_mat_link.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       41 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_broken_surf_link.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       57 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_broken_transform_link.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      641 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_complement_edge.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      835 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_dos.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      125 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/inputs/test_excess_mt.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       77 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/inputs/test_extra_data_imp.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       51 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/inputs/test_extra_data_param.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       88 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/inputs/test_extra_params.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      766 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_imp_redundant.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      765 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_importance.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       84 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_interp_edge.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      957 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_long_lines.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       95 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/inputs/test_missing_mat_for_mt.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      355 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_redundant_surf.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       62 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_surfaces.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      853 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/inputs/test_tab.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      937 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/inputs/test_universe.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      768 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_universe_data.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      782 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/inputs/test_vol_redundant.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      881 2024-04-15 21:58:30.000000 montepy-0.2.7/tests/inputs/unicode.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5775 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_cell_problem.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    12053 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_data_inputs.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7399 2024-05-30 18:11:45.000000 montepy-0.2.7/tests/test_edge_cases.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    17864 2024-04-15 21:58:30.000000 montepy-0.2.7/tests/test_geometry.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7097 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_importance.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2249 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_input_file.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    43268 2024-04-15 21:58:30.000000 montepy-0.2.7/tests/test_integration.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1071 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_interface.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1379 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_main.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    15540 2024-05-30 18:11:45.000000 montepy-0.2.7/tests/test_material.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      816 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_mcnp_problem.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3579 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_mode.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    10482 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/test_numbered_collection.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3356 2024-04-15 21:58:30.000000 montepy-0.2.7/tests/test_scripts.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      561 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_source_def.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    11668 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_surfaces.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    58043 2024-05-30 18:11:45.000000 montepy-0.2.7/tests/test_syntax_parsing.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1266 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_tally.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    10797 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_transform.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    14670 2024-01-12 01:37:20.000000 montepy-0.2.7/tests/test_universe.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      748 2024-01-10 03:00:19.000000 montepy-0.2.7/tests/test_utilities.py
```

### Comparing `montepy-0.2.6/.github/ISSUE_TEMPLATE/bug_report.md` & `montepy-0.2.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/.github/ISSUE_TEMPLATE/feature_request.md` & `montepy-0.2.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/.github/pull_request_template.md` & `montepy-0.2.7/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/.github/workflows/deploy.yml` & `montepy-0.2.7/.github/workflows/deploy.yml`

 * *Files 12% similar despite different names*

```diff
@@ -7,31 +7,34 @@
 
 jobs:
   last-minute-test:
     runs-on: ubuntu-latest    
     steps:
       - uses: actions/checkout@v4
       - name: set up python  3.8
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with: 
           python-version: 3.8
       - run: pip install . montepy[develop]
       - run: python -m pytest
       
   build-pages:
+    needs: [last-minute-test, build-packages]
     environment:
       name: github-pages
     runs-on: ubuntu-latest
     steps:
       - name: Configure git
         env:
            TOKEN: ${{ secrets.ACCESS_TOKEN }}
         run: git config --global url."https://${TOKEN}:x-oauth-basic@github.com/".insteadOf "https://github.com/"
       - uses: actions/checkout@v4
-      - uses: actions/setup-python@v4
+        with: 
+          ref: main
+      - uses: actions/setup-python@v5
         with:
           python-version: 3.8
       - run: pip install --user . montepy[doc]
       - run: cd doc && make html
       - uses: actions/configure-pages@v4
       - uses: actions/upload-pages-artifact@v3
         with: 
@@ -49,21 +52,36 @@
       GH_TOKEN: ${{ github.token }}
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
           fetch-tags: true
       - name: set up python  3.8
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with: 
           python-version: 3.8
       - run: pip install . montepy[build]
+      - uses: mathieudutour/github-tag-action@v6.2
+        name: Get next version number (dry)
+        id: version_num
+        with: 
+          dry_run: True
+          github_token: ${{ secrets.GITHUB_TOKEN }}
+      - name: Update changelog version 
+        run: |
+          sed -i "s/#Next Version#/${{steps.version_num.outputs.new_version}}/w changes" doc/source/changelog.rst
+          [[ -s changes ]] || exit 1
+      - name: Commit new changelog
+        uses: actions4git/add-commit-push@v1.0.0
+        with: 
+          add-pathspec: doc/source
+          commit-message: Update Changelog version to ${{steps.version_num.outputs.new_version}}
       - name: GitHub Actions Create Tag
         id: tag_version
-        uses: mathieudutour/github-tag-action@v6.1
+        uses: mathieudutour/github-tag-action@v6.2
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
        # ensure tags are up to date
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
           fetch-tags: true
@@ -81,15 +99,15 @@
           name: Release ${{ steps.tag_version.outputs.new_tag }}
           body: ${{ steps.tag_version.outputs.changelog }}
           draft: true
       - run: >-
           gh release upload
           '${{ steps.tag_version.outputs.new_tag }}' dist/**
           --repo '${{ github.repository }}'
-      - uses: actions/upload-artifact@v4
+      - uses: actions/upload-artifact@v4.3.1
         with: 
            name: build
            path: |
                dist/*.tar.gz 
                dist/*.whl
 
   deploy-pages:
```

### Comparing `montepy-0.2.6/LICENSE` & `montepy-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/NOTICE.txt` & `montepy-0.2.7/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/PKG-INFO` & `montepy-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: montepy
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library for reading, editing, and writing MCNP input files
 Author: Brenna Carbno
 Author-email: Micah Gale <micah.gale@inl.gov>, Travis Labossiere-Hickman <Travis.LabossiereHickman@inl.gov>
 Maintainer-email: Micah Gale <micah.gale@inl.gov>
 License: MIT License
         
         Copyright (c) 2024 Battelle Energy Alliance, LLC
```

### Comparing `montepy-0.2.6/README.md` & `montepy-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/demo/Pin_cell.ipynb` & `montepy-0.2.7/demo/Pin_cell.ipynb`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/demo/pin_cell.imcnp` & `montepy-0.2.7/demo/pin_cell.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/doc/Makefile` & `montepy-0.2.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/doc/make.bat` & `montepy-0.2.7/doc/make.bat`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/doc/source/_test_for_missing_docs.py` & `montepy-0.2.7/doc/source/_test_for_missing_docs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import glob
 import os
 import sys
 import warnings
 
-ignored = {"__pycache__", "_version.py", "__main__.py", "_cell_data_control.py"}
+ignored = {"__pycache__", "_scripts", "_version.py", "__main__.py", "_cell_data_control.py"}
 
 base = os.path.join("..", "..")
 
 
 def crawl_path(rel_path):
     missing = False
     for f in os.listdir(os.path.join(base, rel_path)):
         f_name = os.path.join(rel_path, f)
         if f in ignored:
             continue
+        if f_name == "montepy/__init__.py":
+            continue
         if os.path.isdir(os.path.join(base, f_name)):
             crawl_path(f_name)
         elif os.path.isfile(os.path.join(base, f_name)) and ".py" in f:
             if f == "__init__.py":
                 path = f_name.replace("/", ".").replace(".__init__.py", ".rst")
             else:
                 path = f_name.replace("/", ".").replace(".py", ".rst")
```

### Comparing `montepy-0.2.6/doc/source/api/montepy.data_inputs.rst` & `montepy-0.2.7/doc/source/api/montepy.data_inputs.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 
 .. automodule:: montepy.data_inputs
    :members:
    :undoc-members:
    :show-inheritance:
 
-Submodules
-----------
 
 .. toctree::
    :maxdepth: 4
 
    montepy.data_inputs.cell_modifier
    montepy.data_inputs.data_input
    montepy.data_inputs.data_parser
```

### Comparing `montepy-0.2.6/doc/source/api/montepy.input_parser.rst` & `montepy-0.2.7/doc/source/api/montepy.input_parser.rst`

 * *Files 18% similar despite different names*

```diff
@@ -3,19 +3,16 @@
 
 
 .. automodule:: montepy.input_parser
    :members:
    :undoc-members:
    :show-inheritance:
 
-Submodules
-----------
-
 .. toctree::
-   :maxdepth: 4
+   :maxdepth: 2
 
    montepy.input_parser.block_type
    montepy.input_parser.cell_parser
    montepy.input_parser.data_parser
    montepy.input_parser.input_file
    montepy.input_parser.input_reader
    montepy.input_parser.input_syntax_reader
```

### Comparing `montepy-0.2.6/doc/source/conf.py` & `montepy-0.2.7/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/doc/source/developing.rst` & `montepy-0.2.7/doc/source/developing.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
    Instead MontePy refers to "inputs", and "files" or "problems". 
 
 Contributing
 ------------
 
 Here is a getting started guide to contributing. 
 If you have any questions Micah and Travis are available to give input and answer your questions.
+Before contributing you should review the :ref:`scope` and design philosophy.
 
 Setting up and Typical Development Workflow
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 #. Clone the repository.
 
 #. Install the required packages. 
@@ -150,35 +151,14 @@
 surfaces
 ^^^^^^^^
 This package contains all surface classes.
 All classes need to be children of :class:`~montepy.surfaces.surface.Surface`.
 When possible new surface classes should combine similar planes.
 For example :class:`~montepy.surfaces.axis_plane.AxisPlane` covers ``PX``, ``PY``, and ``PZ``.
 
-Design Philosophy
------------------
-#. **Do Not Repeat Yourself (DRY)**
-#. Use abstraction and inheritance smartly.
-#. Use ``_private`` fields mostly. Use ``__private`` for very private things that should never be touched.
-#. Use ``@property`` getters, and if needed setters. Setters must verify and clean user inputs. For the most part use :func:`~montepy.utilities.make_prop_val_node`, and :func:`~montepy.utilities.make_prop_pointer`.
-#. Fail early and politely. If there's something that might be bad: the user should get a helpful error as
-   soon as the error is apparent. 
-#. Test. test. test. The goal is to achieve 100% test coverage. Unit test first, then do integration testing. A new feature merge request will ideally have around a dozen new test cases.
-#. Do it right the first time. 
-#. Document all functions.
-#. Expect everything to mutate at any time.
-#. Avoid relative imports when possible. Use top level ones instead: e.g., ``import montepy.cell.Cell``.
-#. Defer to vanilla python, and only use the standard library. Currently the only dependencies are `numpy <https://numpy.org/>`_ and `sly <https://github.com/dabeaz/sly>`_. 
-   There must be good justification for breaking from this convention and complicating things for the user.
-
-Style Guide
------------
-#. Use ``black`` to autoformat all code.
-#. Spaces for indentation, tabs for alignment. Use spaces to build python syntax (4 spaces per level), and tabs for aligning text inside of docstrings.
-
 
 Introduction to SLY and Syntax Trees
 ------------------------------------
 
 In MontePy 0.2.0 the core of MontePy was radically changed. 
 A *real* syntax parser was actually used that actually does things like work with a Lexer, and an L-R table.
 This parsing engine is `SLY (Sly Lex-Yacc) <https://sly.readthedocs.io/en/latest/>`_.
```

### Comparing `montepy-0.2.6/doc/source/faq.rst` & `montepy-0.2.7/doc/source/faq.rst`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/doc/source/index.rst` & `montepy-0.2.7/doc/source/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 .. MontePy documentation master file, created by
    sphinx-quickstart on Thu Apr 21 15:29:53 2022.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
-Welcome to MontePy's documentation!
-===================================
+MontePy: a Python library for MCNP input files.
+===============================================
 
-.. toctree::
-   :maxdepth: 1
-   :caption: Contents:
+MontePy is a Python library for reading, editing, and writing MCNP input files.
+MontePy provides an object-oriented interface for MCNP input files. 
+This allows for easy automation of many different tasks for working with MCNP input files.
 
-   starting
+Installing
+----------
 
-   utilities
+MontePy can be installed with pip:
 
-   tricks
+.. code-block:: shell
 
-   faq
+   pip install montepy
 
-   developing
 
-   api/modules
+.. toctree::
+   :maxdepth: 2
+   :caption: Table of Contents:
 
-   publications
+   api/modules
+   users
+   dev_tree
 
 See Also
 ========
 
 * `MontePy github Repository <https://github.com/idaholab/montepy>`_ 
 * `MCNP 6.2 User Manual <https://mcnp.lanl.gov/pdf_files/TechReport_2017_LANL_LA-UR-17-29981_WernerArmstrongEtAl.pdf>`_
 * `MCNP 6.3 User Manual <https://mcnp.lanl.gov/pdf_files/TechReport_2022_LANL_LA-UR-22-30006Rev.1_KuleszaAdamsEtAl.pdf>`_
```

### Comparing `montepy-0.2.6/doc/source/monty.svg` & `montepy-0.2.7/doc/source/monty.svg`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/doc/source/starting.rst` & `montepy-0.2.7/doc/source/starting.rst`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/doc/source/tricks.rst` & `montepy-0.2.7/doc/source/tricks.rst`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/doc/source/utilities.rst` & `montepy-0.2.7/doc/source/utilities.rst`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/graphics/monty.svg` & `montepy-0.2.7/graphics/monty.svg`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/__init__.py` & `montepy-0.2.7/montepy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     __version__ = _version.version
 except ImportError:
     try:
         from setuptools_scm import get_version
 
         __version__ = get_version()
-    except ImportError:
+    except (ImportError, LookupError):
         __version__ = "Undefined"
 
 
 # enable deprecated warnings for users
 if not sys.warnoptions:
     import os, warnings
```

### Comparing `montepy-0.2.6/montepy/__main__.py` & `montepy-0.2.7/montepy/__main__.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/_cell_data_control.py` & `montepy-0.2.7/montepy/_cell_data_control.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/_scripts/change_to_ascii.py` & `montepy-0.2.7/montepy/_scripts/change_to_ascii.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/cell.py` & `montepy-0.2.7/montepy/cell.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/cells.py` & `montepy-0.2.7/montepy/cells.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/constants.py` & `montepy-0.2.7/montepy/constants.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/cell_modifier.py` & `montepy-0.2.7/montepy/data_inputs/cell_modifier.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/data_input.py` & `montepy-0.2.7/montepy/data_inputs/data_input.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/data_parser.py` & `montepy-0.2.7/montepy/data_inputs/data_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/element.py` & `montepy-0.2.7/montepy/data_inputs/element.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/fill.py` & `montepy-0.2.7/montepy/data_inputs/fill.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/importance.py` & `montepy-0.2.7/montepy/data_inputs/importance.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/isotope.py` & `montepy-0.2.7/montepy/data_inputs/isotope.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,28 +16,30 @@
     _BOUNDING_CURVE = [(17, 52), (35, 101), (54, 150), (76, 203), (96, 251), (118, 296)]
     """
     Points on bounding curve for determining if "valid" isotope
     """
 
     def __init__(self, ZAID="", node=None):
         if node is not None and isinstance(node, ValueNode):
+            if node.type == float:
+                node = ValueNode(node.token, str, node.padding)
             self._tree = node
             ZAID = node.value
-        if "." in ZAID:
-            parts = ZAID.split(".")
-            try:
-                assert len(parts) == 2
-                int(parts[0])
-            except (AssertionError, ValueError) as e:
-                raise ValueError(f"ZAID: {ZAID} could not be parsed as a valid isotope")
-            self._ZAID = parts[0]
-            self.__parse_zaid()
+        parts = ZAID.split(".")
+        try:
+            assert len(parts) <= 2
+            int(parts[0])
+        except (AssertionError, ValueError) as e:
+            raise ValueError(f"ZAID: {ZAID} could not be parsed as a valid isotope")
+        self._ZAID = parts[0]
+        self.__parse_zaid()
+        if len(parts) == 2:
             self._library = parts[1]
         else:
-            raise ValueError(f"ZAID: {ZAID} could not be parsed as a valid isotope")
+            self._library = ""
 
     def __parse_zaid(self):
         """
         Parses the ZAID fully including metastable isomers.
 
         See Table 3-32 of LA-UR-17-29881
```

### Comparing `montepy-0.2.6/montepy/data_inputs/lattice_input.py` & `montepy-0.2.7/montepy/data_inputs/lattice_input.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/material.py` & `montepy-0.2.7/montepy/data_inputs/material.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright 2024, Battelle Energy Alliance, LLC All Rights Reserved.
 import copy
 from montepy.data_inputs import data_input, thermal_scattering
 from montepy.data_inputs.isotope import Isotope
 from montepy.data_inputs.material_component import MaterialComponent
+from montepy.input_parser import syntax_node
+from montepy.input_parser.material_parser import MaterialParser
 from montepy import mcnp_object
 from montepy.numbered_mcnp_object import Numbered_MCNP_Object
 from montepy.errors import *
 from montepy.utilities import *
 import itertools
 import re
 
@@ -22,26 +24,45 @@
     """
     A class to represent an MCNP material.
 
     :param input: the input card that contains the data
     :type input: Input
     """
 
+    _parser = MaterialParser()
+
     def __init__(self, input=None):
         self._material_components = {}
         self._thermal_scattering = None
         self._number = self._generate_default_node(int, -1)
         super().__init__(input)
         if input:
             num = self._input_number
             self._old_number = copy.deepcopy(num)
             self._number = num
             set_atom_frac = False
             isotope_fractions = self._tree["data"]
-            for isotope_node, fraction in isotope_fractions:
+            if isinstance(isotope_fractions, syntax_node.ListNode):
+                # in python 3.12 this can be replaced with itertools.batched
+                def batch_gen():
+                    it = iter(isotope_fractions)
+                    while batch := tuple(itertools.islice(it, 2)):
+                        yield batch
+
+                iterator = batch_gen()
+            elif isinstance(isotope_fractions, syntax_node.IsotopesNode):
+                iterator = iter(isotope_fractions)
+            else:  # pragma: no cover
+                # this is a fall through error, that should never be raised,
+                # but is here just in case
+                raise MalformedInputError(
+                    input,
+                    f"Material definitions for material: {self.number} is not valid.",
+                )
+            for isotope_node, fraction in iterator:
                 isotope = Isotope(node=isotope_node)
                 fraction.is_negatable_float = True
                 if not set_atom_frac:
                     set_atom_frac = True
                     if not fraction.is_negative:
                         self._is_atom_fraction = True
                     else:
```

### Comparing `montepy-0.2.6/montepy/data_inputs/material_component.py` & `montepy-0.2.7/montepy/data_inputs/material_component.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/mode.py` & `montepy-0.2.7/montepy/data_inputs/mode.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/thermal_scattering.py` & `montepy-0.2.7/montepy/data_inputs/thermal_scattering.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/transform.py` & `montepy-0.2.7/montepy/data_inputs/transform.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/universe_input.py` & `montepy-0.2.7/montepy/data_inputs/universe_input.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/data_inputs/volume.py` & `montepy-0.2.7/montepy/data_inputs/volume.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/errors.py` & `montepy-0.2.7/montepy/errors.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/geometry_operators.py` & `montepy-0.2.7/montepy/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/input_parser/cell_parser.py` & `montepy-0.2.7/montepy/input_parser/cell_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/input_parser/data_parser.py` & `montepy-0.2.7/montepy/input_parser/data_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/input_parser/input_file.py` & `montepy-0.2.7/montepy/input_parser/input_file.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/input_parser/input_reader.py` & `montepy-0.2.7/montepy/input_parser/input_reader.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/input_parser/input_syntax_reader.py` & `montepy-0.2.7/montepy/input_parser/input_syntax_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import itertools
 import io
 from montepy.constants import *
 from montepy.errors import *
 from montepy.input_parser.input_file import MCNP_InputFile
 from montepy.input_parser.mcnp_input import Input, Message, ReadInput, Title
 from montepy.input_parser.read_parser import ReadParser
+from montepy.utilities import is_comment
 import os
 import warnings
 
 reading_queue = []
 
 
 def read_input_syntax(input_file, mcnp_version=DEFAULT_VERSION, replace=True):
@@ -84,28 +85,14 @@
                 is_in_message_block = False
         # title always follows complete message, or is first
         else:
             yield Title([line], line)
             break
 
 
-def is_comment(line):
-    """"""
-    upper_start = line[0 : BLANK_SPACE_CONTINUE + 1].upper()
-    non_blank_comment = upper_start and line.lstrip().upper().startswith("C ")
-    if non_blank_comment:
-        return True
-    blank_comment = (
-        "C\n" == upper_start.lstrip()
-        or "C\r\n" == upper_start.lstrip()
-        or ("C" == upper_start and "\n" not in line)
-    )
-    return blank_comment or non_blank_comment
-
-
 def read_data(fh, mcnp_version, block_type=None, recursion=False):
     """
     Reads the bulk of an MCNP file for all of the MCNP data.
 
     This is a generator function that will yield multiple :class:`MCNP_Input` instances.
 
     .. warning::
```

### Comparing `montepy-0.2.6/montepy/input_parser/mcnp_input.py` & `montepy-0.2.7/montepy/input_parser/mcnp_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,24 +291,36 @@
     :type lineno: int
     """
 
     _parser = ReadParser()
 
     def __init__(self, input_lines, block_type, input_file=None, lineno=None):
         super().__init__(input_lines, block_type, input_file, lineno)
+        if not self.is_read_input(input_lines):
+            raise ValueError("Not a valid Read Input")
         parse_result = self._parser.parse(self.tokenize(), self)
-        first_word = input_lines[0].split()[0].lower()
         if not parse_result:
-            if first_word != "read":
-                raise ValueError("Not a valid Read Input")
-            else:
-                raise ParsingError(self, "", self._parser.log.clear_queue())
+            raise ParsingError(self, "", self._parser.log.clear_queue())
         self._tree = parse_result
         self._parameters = self._tree["parameters"]
 
+    @staticmethod
+    def is_read_input(input_lines):
+        first_non_comment = ""
+        for line in input_lines:
+            if not is_comment(line):
+                first_non_comment = line
+                break
+        words = first_non_comment.split()
+        if len(words) > 0:
+            first_word = words[0].lower()
+            return first_word == "read"
+        # this is a fall through catch that only happens for a blank input
+        return False  # pragma: no cover
+
     @property
     def file_name(self):
         """
         The relative path to the filename specified in this read input.
 
         :rtype: str
         """
```

### Comparing `montepy-0.2.6/montepy/input_parser/parser_base.py` & `montepy-0.2.7/montepy/input_parser/parser_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,14 +370,15 @@
         "KEYWORD",
         "LOG_INTERPOLATE",
         "NULL",
         "REPEAT",
         "SURFACE_TYPE",
         "THERMAL_LAW",
         "ZAID",
+        "NUMBER_WORD",
     )
     def file_atom(self, p):
         return p[0]
 
     @_("file_name", "file_name padding")
     def file_phrase(self, p):
         """
```

### Comparing `montepy-0.2.6/montepy/input_parser/read_parser.py` & `montepy-0.2.7/montepy/input_parser/read_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/input_parser/shortcuts.py` & `montepy-0.2.7/montepy/input_parser/shortcuts.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/input_parser/surface_parser.py` & `montepy-0.2.7/montepy/input_parser/surface_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/input_parser/syntax_node.py` & `montepy-0.2.7/montepy/input_parser/syntax_node.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/input_parser/tally_parser.py` & `montepy-0.2.7/montepy/input_parser/tally_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/input_parser/thermal_parser.py` & `montepy-0.2.7/montepy/input_parser/thermal_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/input_parser/tokens.py` & `montepy-0.2.7/montepy/input_parser/tokens.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/materials.py` & `montepy-0.2.7/montepy/materials.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/mcnp_object.py` & `montepy-0.2.7/montepy/mcnp_object.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/mcnp_problem.py` & `montepy-0.2.7/montepy/mcnp_problem.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/numbered_mcnp_object.py` & `montepy-0.2.7/montepy/numbered_mcnp_object.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/numbered_object_collection.py` & `montepy-0.2.7/montepy/numbered_object_collection.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/particle.py` & `montepy-0.2.7/montepy/particle.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/surface_collection.py` & `montepy-0.2.7/montepy/surface_collection.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/surfaces/axis_plane.py` & `montepy-0.2.7/montepy/surfaces/axis_plane.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/surfaces/cylinder_on_axis.py` & `montepy-0.2.7/montepy/surfaces/cylinder_on_axis.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/surfaces/cylinder_par_axis.py` & `montepy-0.2.7/montepy/surfaces/cylinder_par_axis.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/surfaces/general_plane.py` & `montepy-0.2.7/montepy/surfaces/general_plane.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/surfaces/half_space.py` & `montepy-0.2.7/montepy/surfaces/half_space.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/surfaces/surface.py` & `montepy-0.2.7/montepy/surfaces/surface.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/surfaces/surface_builder.py` & `montepy-0.2.7/montepy/surfaces/surface_builder.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/surfaces/surface_type.py` & `montepy-0.2.7/montepy/surfaces/surface_type.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/universe.py` & `montepy-0.2.7/montepy/universe.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/montepy/utilities.py` & `montepy-0.2.7/montepy/utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright 2024, Battelle Energy Alliance, LLC All Rights Reserved.
+from montepy.constants import BLANK_SPACE_CONTINUE
 import functools
 import re
 
 """
 A package for helper universal utility functions
 """
 
@@ -27,14 +28,33 @@
         update_number = re.sub(r"(\d)([-+])", r"\1E\2", number_string)
         try:
             return float(update_number)
         except ValueError:
             raise ValueError(f"Value Not parsable as float: {number_string}") from e
 
 
+def is_comment(line):
+    """
+    Determines if the line is a ``C comment`` style comment.
+
+    :param line: the line to analyze
+    :type line: str
+    :returns: True if the line is a comment
+    :rtype: bool
+    """
+    upper_start = line[0 : BLANK_SPACE_CONTINUE + 1].upper()
+    non_blank_comment = upper_start and line.lstrip().upper().startswith("C ")
+    if non_blank_comment:
+        return True
+    blank_comment = ("C" == upper_start.strip() and "\n" in line) or (
+        "C" == upper_start and "\n" not in line
+    )
+    return blank_comment
+
+
 def make_prop_val_node(
     hidden_param, types=None, base_type=None, validator=None, deletable=False
 ):
     """
     A decorator function for making a property from a ValueNode.
 
     This decorator is meant to handle all boiler plate. It will get and
```

### Comparing `montepy-0.2.6/montepy.egg-info/PKG-INFO` & `montepy-0.2.7/montepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: montepy
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library for reading, editing, and writing MCNP input files
 Author: Brenna Carbno
 Author-email: Micah Gale <micah.gale@inl.gov>, Travis Labossiere-Hickman <Travis.LabossiereHickman@inl.gov>
 Maintainer-email: Micah Gale <micah.gale@inl.gov>
 License: MIT License
         
         Copyright (c) 2024 Battelle Energy Alliance, LLC
```

### Comparing `montepy-0.2.6/montepy.egg-info/SOURCES.txt` & `montepy-0.2.7/montepy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 .gitignore
 AUTHORS
+CHANGELOG.rst
+CONTRIBUTING.md
 LICENSE
+MANIFEST.in
 NOTICE.txt
 README.md
 pyproject.toml
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/deploy.yml
 .github/workflows/main.yml
 demo/Pin_cell.ipynb
 demo/pin_cell.imcnp
 doc/Makefile
 doc/make.bat
 doc/source/_test_for_missing_docs.py
+doc/source/changelog.rst
 doc/source/conf.py
+doc/source/dev_tree.rst
 doc/source/developing.rst
 doc/source/faq.rst
 doc/source/index.rst
 doc/source/monty.svg
 doc/source/publications.rst
+doc/source/scope.rst
 doc/source/starting.rst
 doc/source/tricks.rst
+doc/source/users.rst
 doc/source/utilities.rst
 doc/source/_static/placeholder
 doc/source/_templates/placeholder
 doc/source/api/modules.rst
 doc/source/api/montepy.cell.rst
 doc/source/api/montepy.cells.rst
 doc/source/api/montepy.constants.rst
@@ -68,15 +75,14 @@
 doc/source/api/montepy.input_parser.tokens.rst
 doc/source/api/montepy.materials.rst
 doc/source/api/montepy.mcnp_object.rst
 doc/source/api/montepy.mcnp_problem.rst
 doc/source/api/montepy.numbered_mcnp_object.rst
 doc/source/api/montepy.numbered_object_collection.rst
 doc/source/api/montepy.particle.rst
-doc/source/api/montepy.rst
 doc/source/api/montepy.surface_collection.rst
 doc/source/api/montepy.surfaces.axis_plane.rst
 doc/source/api/montepy.surfaces.cylinder_on_axis.rst
 doc/source/api/montepy.surfaces.cylinder_par_axis.rst
 doc/source/api/montepy.surfaces.general_plane.rst
 doc/source/api/montepy.surfaces.half_space.rst
 doc/source/api/montepy.surfaces.rst
@@ -138,14 +144,15 @@
 montepy/input_parser/__init__.py
 montepy/input_parser/block_type.py
 montepy/input_parser/cell_parser.py
 montepy/input_parser/data_parser.py
 montepy/input_parser/input_file.py
 montepy/input_parser/input_reader.py
 montepy/input_parser/input_syntax_reader.py
+montepy/input_parser/material_parser.py
 montepy/input_parser/mcnp_input.py
 montepy/input_parser/parser_base.py
 montepy/input_parser/read_parser.py
 montepy/input_parser/shortcuts.py
 montepy/input_parser/surface_parser.py
 montepy/input_parser/syntax_node.py
 montepy/input_parser/tally_parser.py
@@ -181,15 +188,17 @@
 tests/test_syntax_parsing.py
 tests/test_tally.py
 tests/test_transform.py
 tests/test_universe.py
 tests/test_utilities.py
 tests/inputs/bad_encoding.imcnp
 tests/inputs/breaking_comments.imcnp
+tests/inputs/file2read.imcnp
 tests/inputs/number_conflict_pin_cell.imcnp
+tests/inputs/readEdgeCase.imcnp
 tests/inputs/test.imcnp
 tests/inputs/testRead.imcnp
 tests/inputs/testReadRec1.imcnp
 tests/inputs/testReadRec2.imcnp
 tests/inputs/testReadRec3.imcnp
 tests/inputs/testReadTarget.imcnp
 tests/inputs/testVerticalMode.imcnp
```

### Comparing `montepy-0.2.6/pyproject.toml` & `montepy-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 [tool.setuptools_scm]
 version_file = "montepy/_version.py"
 
 [tool.setuptools.packages.find]
 include = ["montepy*"]
 
 [tool.coverage.run]
-omit = ["montepy/_version.py","tests/*"]
+omit = ["tests/*"]
 
 [tool.coverage.report]
 precision = 2
 show_missing = true
 fail_under = 90.0
 exclude_also = [
 	"\\s+@abstractmethod\\s*",
```

### Comparing `montepy-0.2.6/tests/constants.py` & `montepy-0.2.7/tests/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,13 +19,14 @@
 IGNORE_FILES = {
     "testReadRec1.imcnp",
     "testReadRec2.imcnp",
     "testReadRec3.imcnp",
     "testReadTarget.imcnp",
     "bad_encoding.imcnp",
     "unicode.imcnp",
+    "file2read.imcnp",
 }
 
 BAD_ENCODING_FILES = {
     "bad_encoding.imcnp",
     "unicode.imcnp",
 }
```

### Comparing `montepy-0.2.6/tests/inputs/bad_encoding.imcnp` & `montepy-0.2.7/tests/inputs/bad_encoding.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/inputs/number_conflict_pin_cell.imcnp` & `montepy-0.2.7/tests/inputs/number_conflict_pin_cell.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/inputs/test.imcnp` & `montepy-0.2.7/tests/inputs/test.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/inputs/test_complement_edge.imcnp` & `montepy-0.2.7/tests/inputs/test_complement_edge.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/inputs/test_dos.imcnp` & `montepy-0.2.7/tests/inputs/test_dos.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/inputs/test_imp_redundant.imcnp` & `montepy-0.2.7/tests/inputs/test_imp_redundant.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/inputs/test_importance.imcnp` & `montepy-0.2.7/tests/inputs/test_importance.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/inputs/test_long_lines.imcnp` & `montepy-0.2.7/tests/inputs/test_long_lines.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/inputs/test_tab.imcnp` & `montepy-0.2.7/tests/inputs/test_tab.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/inputs/test_universe.imcnp` & `montepy-0.2.7/tests/inputs/test_universe.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/inputs/test_universe_data.imcnp` & `montepy-0.2.7/tests/inputs/test_universe_data.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/inputs/test_vol_redundant.imcnp` & `montepy-0.2.7/tests/inputs/test_vol_redundant.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/inputs/unicode.imcnp` & `montepy-0.2.7/tests/inputs/unicode.imcnp`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_cell_problem.py` & `montepy-0.2.7/tests/test_cell_problem.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_data_inputs.py` & `montepy-0.2.7/tests/test_data_inputs.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_edge_cases.py` & `montepy-0.2.7/tests/test_edge_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,7 +173,12 @@
         input = montepy.input_parser.mcnp_input.Input(
             in_strs, montepy.input_parser.block_type.BlockType.CELL
         )
         cell = montepy.Cell(input)
         # this step caused an error for #163
         cell.comments
         cell._tree.format()
+
+    def test_bad_read(self):
+        problem = montepy.read_input(
+            os.path.join("tests", "inputs", "readEdgeCase.imcnp")
+        )
```

### Comparing `montepy-0.2.6/tests/test_geometry.py` & `montepy-0.2.7/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_importance.py` & `montepy-0.2.7/tests/test_importance.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_input_file.py` & `montepy-0.2.7/tests/test_input_file.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_integration.py` & `montepy-0.2.7/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_interface.py` & `montepy-0.2.7/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_main.py` & `montepy-0.2.7/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_material.py` & `montepy-0.2.7/tests/test_material.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,30 @@
         material = Material(input_card)
         self.assertEqual(material.number, 20)
         self.assertEqual(material.old_number, 20)
         self.assertTrue(material.is_atom_fraction)
         for component in material.material_components:
             self.assertEqual(material.material_components[component].fraction, 0.5)
 
+        # test implicit library with syntax tree errors
+        in_str = """m1 1001 0.33
+    8016 0.666667"""
+        input_card = Input(in_str.split("\n"), BlockType.DATA)
+        material = Material(input_card)
+        # test implicit library
+        in_str = "M20 1001 0.5 2001 0.5 8016.710nc 0.5"
+        input_card = Input([in_str], BlockType.DATA)
+        material = Material(input_card)
+        self.assertEqual(material.number, 20)
+        self.assertEqual(material.old_number, 20)
+        self.assertTrue(material.is_atom_fraction)
+        for component in material.material_components:
+            self.assertEqual(material.material_components[component].fraction, 0.5)
+
+        # test weight fraction
         in_str = "M20 1001.80c -0.5 8016.80c -0.5"
         input_card = Input([in_str], BlockType.DATA)
         material = Material(input_card)
         self.assertFalse(material.is_atom_fraction)
         for component in material.material_components:
             self.assertEqual(material.material_components[component].fraction, 0.5)
 
@@ -160,16 +176,14 @@
         self.assertEqual(isotope.A, 1)
         self.assertEqual(isotope.element.Z, 1)
         self.assertEqual(isotope.library, "80c")
         with self.assertRaises(ValueError):
             Isotope("1001.80c.5")
         with self.assertRaises(ValueError):
             Isotope("hi.80c")
-        with self.assertRaises(ValueError):
-            Isotope("1001")
 
     def test_isotope_metastable_init(self):
         isotope = Isotope("13426.02c")
         self.assertEqual(isotope.ZAID, "13426")
         self.assertEqual(isotope.Z, 13)
         self.assertEqual(isotope.A, 26)
         self.assertTrue(isotope.is_metastable)
```

### Comparing `montepy-0.2.6/tests/test_mcnp_problem.py` & `montepy-0.2.7/tests/test_mcnp_problem.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_mode.py` & `montepy-0.2.7/tests/test_mode.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_numbered_collection.py` & `montepy-0.2.7/tests/test_numbered_collection.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_scripts.py` & `montepy-0.2.7/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_source_def.py` & `montepy-0.2.7/tests/test_source_def.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_surfaces.py` & `montepy-0.2.7/tests/test_surfaces.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_syntax_parsing.py` & `montepy-0.2.7/tests/test_syntax_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1097,14 +1097,18 @@
         self.assertEqual(token.value, "c")
 
     def testReadCardConfusions(self):
         for file in {"A1_cells", "I1_cells"}:
             input = ReadInput([f"Read FILE={file}"], BlockType.CELL)
             self.assertEqual(input.file_name, file)
 
+    def testReadCardBadSyntax(self):
+        with self.assertRaises(ParsingError):
+            card = ReadInput(["Read 1"], BlockType.CELL)
+
     def testTitleFinder(self):
         test_title = "Richard Stallman writes GNU"
         test_string = f"""{test_title}
 1 0 -1
 """
         for tester, validator in [
             (test_string, test_title),
```

### Comparing `montepy-0.2.6/tests/test_tally.py` & `montepy-0.2.7/tests/test_tally.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_transform.py` & `montepy-0.2.7/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_universe.py` & `montepy-0.2.7/tests/test_universe.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.6/tests/test_utilities.py` & `montepy-0.2.7/tests/test_utilities.py`

 * *Files identical despite different names*

