# Comparing `tmp/vessel_manoeuvring_models-0.0.6.tar.gz` & `tmp/vessel_manoeuvring_models-0.0.7.tar.gz`

## Comparing `vessel_manoeuvring_models-0.0.6.tar` & `vessel_manoeuvring_models-0.0.7.tar`

### file list

```diff
@@ -1,273 +1,290 @@
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/Makefile
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/requirements.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/requirements_build.txt
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/test_environment.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tox.ini
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/binder/apt.txt
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/binder/environment.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/binder/postBuild
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/data/external/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/data/interim/.gitkeep
--rw-r--r--   0        0        0    41828 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/data/interim/run_selection.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/data/processed/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/data/raw/.gitkeep
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/Makefile
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/commands.rst
--rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/conf.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/getting-started.rst
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/index.rst
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/make.bat
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/00.01_intro.md
--rw-r--r--   0        0        0    15206 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/00.02_intro_example.ipynb
--rw-r--r--   0        0        0    42000 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/01.01_manoeuvring_simulation.ipynb
--rw-r--r--   0        0        0    34911 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/02.01_manoeuvring_PIT.ipynb
--rw-r--r--   0        0        0    22082 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/10.03_OLS_covariance.ipynb
--rw-r--r--   0        0        0    29754 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/10.04_bias_variance.ipynb
--rw-r--r--   0        0        0    20341 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/15.39_KF_nomoto.ipynb
--rw-r--r--   0        0        0    19838 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/15.40_EKF_nomoto.ipynb
--rw-r--r--   0        0        0    18606 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/30.01_maximum_likelihood.ipynb
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/_config.yml
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/_toc.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/bibligraphy.md
--rw-r--r--   0        0        0    34134 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/book.mplstyle
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/chapter.ipynb
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/example_1.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/imports.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/kalman_filters.md
--rw-r--r--   0        0        0   469672 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/logo.png
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/markdown.md
--rw-r--r--   0        0        0   238911 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/references.bib
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/requirements.txt
--rw-r--r--   0        0        0    22325 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/01.1_seaman_matematical_model.ipynb
--rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/02.1_seaman_sway_hull_equation.ipynb
--rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/03.1_seaman_yaw_hull_equation.ipynb
--rw-r--r--   0        0        0    17435 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/04.1_seaman_rudder_equation.ipynb
--rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/04.2_seaman_rudder_equation_modified_drag.ipynb
--rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/05.1_seaman_surge_hull_equation.ipynb
--rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/06.1_seaman_roll_hull_equation.ipynb
--rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/10_seaman_rigid_body.ipynb
--rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/11_manoeuvring_simulation.ipynb
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/X_function.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/Y_function.py
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/__init__.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/bis_system.py
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/cd.png
--rw-r--r--   0        0        0   130907 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/coordinateSystem.png
--rw-r--r--   0        0        0    30237 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/coordinate_system.png
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/curve_fit.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/generate_input.py
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/notebooks_to_html.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/regression.py
--rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/regression_old.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/roll_hull_equations.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/roll_hull_lambda_functions.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/rudder_equations.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/rudder_lambda_functions.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/run_real_seaman.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/save_lambda_functions.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/seaman_symbol.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/seaman_symbols.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/substitute_dynamic_symbols.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/surge_hull_equations.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/surge_hull_lambda_functions.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/sway_hull_equations.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/sway_hull_lambda_functions.py
--rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/test_ship.ship
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/total_equations.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/total_lambda_functions.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/yaw_hull_equations.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/yaw_hull_lambda_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/models/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/.gitkeep
--rw-r--r--   0        0        0   332654 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/01.00_MDL_select_runs.ipynb
--rw-r--r--   0        0        0    27865 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/02.00_MDL_load_runs.ipynb
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/03.00_test_overview.ipynb
--rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.01_PIT_nomoto.ipynb
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.02_PIT_linear_VMM.ipynb
--rw-r--r--   0        0        0     9376 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.02_PIT_nomotos.ipynb
--rw-r--r--   0        0        0    19255 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.02_PIT_nonlinear_VMM.ipynb
--rw-r--r--   0        0        0    31214 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.03_PIT_VCT_linear_VMM.ipynb
--rw-r--r--   0        0        0    32154 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.03_PIT_VCT_nonlinear_VMM.ipynb
--rw-r--r--   0        0        0    34957 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.03_PIT_linear_VMM.ipynb
--rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/05.01_acceleration_Kalman.ipynb
--rw-r--r--   0        0        0   274069 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/05.02_transform_to_ship.ipynb
--rw-r--r--   0        0        0   879206 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/05.03_cutting.ipynb
--rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/05.semiempirical_rudder_wpcc.ipynb
--rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/06.01_linear_VMM.ipynb
--rw-r--r--   0        0        0    23562 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/06.01_linear_simplified_VMM.ipynb
--rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/06.02_linear_VMM_wPCC_brix.ipynb
--rw-r--r--   0        0        0  1165028 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/07.03_PIT_static_forces_nonlinear.ipynb
--rw-r--r--   0        0        0    37675 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/07_01_static_forces_from_model_test.ipynb
--rw-r--r--   0        0        0  1176968 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/07_02_static_forces_from_spirals.ipynb
--rw-r--r--   0        0        0    48697 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/07_05_static_forces_from_model_test-many.ipynb
--rw-r--r--   0        0        0    49041 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/08_01_PIT_summary.ipynb
--rw-r--r--   0        0        0    44439 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/08_02_PIT_nonlinear_summary.ipynb
--rw-r--r--   0        0        0    24616 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/09_01_PIT_tongton.ipynb
--rw-r--r--   0        0        0    23537 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/09_02_PIT_tongton_SI.ipynb
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/10.01_EOM_air.ipynb
--rw-r--r--   0        0        0    19914 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/10.02_kalman_PIT_sensitivity.ipynb
--rw-r--r--   0        0        0    33006 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/10.03_lowpass_PIT.ipynb
--rw-r--r--   0        0        0    30697 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/11.01_regression_revisited.ipynb
--rw-r--r--   0        0        0    25508 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.01_regression_simulated_data.ipynb
--rw-r--r--   0        0        0    25899 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.02_regression_simulated_data_nonlinear_EOM.ipynb
--rw-r--r--   0        0        0    37550 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.03_regression_simulated_data_mariner.ipynb
--rw-r--r--   0        0        0    24478 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.04_regression_too_little_simulated_data.ipynb
--rw-r--r--   0        0        0    28072 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.05.5_regression_simulated_data_simple_nonlinear_BDF.ipynb
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.05_regression_simulated_data_acc_thrust.ipynb
--rw-r--r--   0        0        0    27714 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.05_regression_simulated_data_simple_nonlinear.ipynb
--rw-r--r--   0        0        0    24448 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.06.5_regression_simulated_data_BDF_numerical_gradient.ipynb
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.06_regression_simulated_data_numerical_gradient.ipynb
--rw-r--r--   0        0        0    27318 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.07_regression_simulated_data_better_numerical_gradient.ipynb
--rw-r--r--   0        0        0    22934 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.08_regression_simulated_data_gausian_noise.ipynb
--rw-r--r--   0        0        0    24594 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.08_regression_simulated_more_data_gausian_noise.ipynb
--rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/13.01_solve_ivp.ipynb
--rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/14.01_EM_algorithm.ipynb
--rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/14.01_hidden_states.ipynb
--rw-r--r--   0        0        0    23581 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/14.02_hidden_states_gradient_regression.ipynb
--rw-r--r--   0        0        0    24046 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/14.03_hidden_states_gradient_regression_linear.ipynb
--rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.01_kalman_filter_unvariate.ipynb
--rw-r--r--   0        0        0    21616 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.10_kalman_filter_multivariate.ipynb
--rw-r--r--   0        0        0    31286 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.11_kalman_filter_linear_manoeuvring.ipynb
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.20_EM-algorithm.ipynb
--rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.30_KF_fossen.ipynb
--rw-r--r--   0        0        0    12804 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.31_EKF_fossen.ipynb
--rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.39_KF_nomoto.ipynb
--rw-r--r--   0        0        0    15487 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.40_EKF_nomoto.ipynb
--rw-r--r--   0        0        0    18938 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.41_EKF_PIT_nomoto.ipynb
--rw-r--r--   0        0        0    21033 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.42_EKF_EM_nomoto.ipynb
--rw-r--r--   0        0        0    19373 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.42_EKF_PIT_2_nomoto.ipynb
--rw-r--r--   0        0        0    17287 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.44_KF_EM_RTS_nomoto.ipynb
--rw-r--r--   0        0        0   299798 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.45_KF_EM_RTS_nomoto.ipynb
--rw-r--r--   0        0        0    14125 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.46_EKF_Abkowitz.ipynb
--rw-r--r--   0        0        0    45662 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.47_EKF_3DOF.ipynb
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.47_EKF_3DOF.py
--rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.48_EK_smoother_3DOF.ipynb
--rw-r--r--   0        0        0    29295 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.49_EK_smoother_3DOF_thrust.ipynb
--rw-r--r--   0        0        0    15522 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.50_KF_EM_RTS_nomoto.ipynb
--rw-r--r--   0        0        0    21888 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.51_EK_inverse_dynamics.ipynb
--rw-r--r--   0        0        0    10993 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.52_inverse_static.ipynb
--rw-r--r--   0        0        0    17497 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/16.01_PIT_VCT_revisited_linear.ipynb
--rw-r--r--   0        0        0    19792 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/16.02_PIT_VCT_revisited_nonlinear.ipynb
--rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/16.03_model_simulate.ipynb
--rw-r--r--   0        0        0    25951 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/17.01_RTS_manoeuvring_PIT.ipynb
--rw-r--r--   0        0        0    19422 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/21.01_parameter_drift.ipynb
--rw-r--r--   0        0        0    17265 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/21.02_parameter_drift.ipynb
--rw-r--r--   0        0        0    23816 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/21.03_parameter_drift.ipynb
--rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/21.04_perfect_captive.ipynb
--rw-r--r--   0        0        0    13073 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/21.05_perfect_captive_truncated.ipynb
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/22.01_scaling_VCT_captive.ipynb
--rw-r--r--   0        0        0   334166 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/30.01_joke.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/__init__.py
--rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/ai_research.png
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/example_ship2.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/imports.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/logbook.ipynb
--rw-r--r--   0        0        0    33486 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/matplotlibrc
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/research.ipynb
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/model_simulate/01.01_run_simulations.py
--rw-r--r--   0        0        0    10404 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/model_simulate/02.01_analyze_runs.ipynb
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/model_simulate/templates/16.03_model_simulate.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/references/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/reports/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/reports/figures/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/.gitkeep
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_EKF_PIT_Nomot.py
--rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_KF_Nomoto.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_extended_kalman_filter.py
--rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_extended_kalman_vmm.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_force_regression.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_kalman_filter.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_linear_vmm.py
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_model_simulator.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_parameter_denominator.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_prime_system.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_rts_smoother.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_vmm_simple_nonliear.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/__init__.py
--rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/bias_variance_tradeoff.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/equations.py
--rw-r--r--   0        0        0    12310 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/extended_kalman_filter.py
--rw-r--r--   0        0        0    21131 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/extended_kalman_vmm.py
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/feature_selection.py
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/kalman_filter.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/linear_vmm_equations.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/linear_vmm_simplified_equations.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/logger.py
--rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/mlflow_utils.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/nonlinear_abkowitz_vmm_equations.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/nonlinear_martin_vmm_equations.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/nonlinear_vmm_equations.py
--rw-r--r--   0        0        0    12924 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/notebook_to_latex.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/parameter_helpers.py
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/parameters.py
--rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/prime_system.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/substitute_dynamic_symbols.py
--rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/symbols.py
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/system_equations.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/to_mlflow.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/twin_simulations.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/vct_scaling.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/vmm_equations_VCT.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/__init__.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/case_0.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/case_1.py
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/kalman_filter.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/lowpass_filter.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/make_dataset.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/mdl.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/wpcc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/features/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/features/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/features/build_features.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/.gitkeep
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/MMG_hull.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/MMG_propeller.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/MMG_rudder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/__init__.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/brix_coefficients.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/captive_variation.py
--rw-r--r--   0        0        0     9394 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/diff_eq_to_matrix.py
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/force_from_motion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/linear_nomoto.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/linear_vmm.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/nonlinear_martin_vmm.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/nonlinear_vmm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/predict_model.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/propeller.py
--rw-r--r--   0        0        0    22054 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/regression.py
--rw-r--r--   0        0        0    12128 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/result.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/train_model.py
--rw-r--r--   0        0        0    29108 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_MMG.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_VCT.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_abkowitz.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_abkowitz_expanded.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_abkowitz_no_thrust.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_air.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_gsi.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_linear.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_mariner.py
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_martin.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_martin_linear.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_martin_simple.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_nonlinear_EOM.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_perturbed.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_simple.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_simple_nonlinear.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vessels/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vessels/mariner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/__init__.py
--rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/book_format.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/equation.py
--rw-r--r--   0        0        0    12833 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/plot.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/regression.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/visualize.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/LICENSE
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/README.md
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/Makefile
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/requirements.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/requirements_build.txt
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/test_environment.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tox.ini
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/binder/apt.txt
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/binder/environment.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/binder/postBuild
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/data/external/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/data/interim/.gitkeep
+-rw-r--r--   0        0        0    41828 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/data/interim/run_selection.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/data/processed/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/data/raw/.gitkeep
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/Makefile
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/commands.rst
+-rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/conf.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/getting-started.rst
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/index.rst
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/make.bat
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/00.01_intro.md
+-rw-r--r--   0        0        0    15206 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/00.02_intro_example.ipynb
+-rw-r--r--   0        0        0    42000 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/01.01_manoeuvring_simulation.ipynb
+-rw-r--r--   0        0        0    34911 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/02.01_manoeuvring_PIT.ipynb
+-rw-r--r--   0        0        0    22082 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/10.03_OLS_covariance.ipynb
+-rw-r--r--   0        0        0    29754 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/10.04_bias_variance.ipynb
+-rw-r--r--   0        0        0    20341 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/15.39_KF_nomoto.ipynb
+-rw-r--r--   0        0        0    19838 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/15.40_EKF_nomoto.ipynb
+-rw-r--r--   0        0        0    18606 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/30.01_maximum_likelihood.ipynb
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/_config.yml
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/_toc.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/bibligraphy.md
+-rw-r--r--   0        0        0    34134 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/book.mplstyle
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/chapter.ipynb
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/example_1.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/imports.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/kalman_filters.md
+-rw-r--r--   0        0        0   469672 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/logo.png
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/markdown.md
+-rw-r--r--   0        0        0   238911 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/references.bib
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/book/requirements.txt
+-rw-r--r--   0        0        0    22325 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/01.1_seaman_matematical_model.ipynb
+-rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/02.1_seaman_sway_hull_equation.ipynb
+-rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/03.1_seaman_yaw_hull_equation.ipynb
+-rw-r--r--   0        0        0    17435 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/04.1_seaman_rudder_equation.ipynb
+-rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/04.2_seaman_rudder_equation_modified_drag.ipynb
+-rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/05.1_seaman_surge_hull_equation.ipynb
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/06.1_seaman_roll_hull_equation.ipynb
+-rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/10_seaman_rigid_body.ipynb
+-rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/11_manoeuvring_simulation.ipynb
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/X_function.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/Y_function.py
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/__init__.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/bis_system.py
+-rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/cd.png
+-rw-r--r--   0        0        0   130907 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/coordinateSystem.png
+-rw-r--r--   0        0        0    30237 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/coordinate_system.png
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/curve_fit.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/generate_input.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/notebooks_to_html.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/regression.py
+-rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/regression_old.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/roll_hull_equations.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/roll_hull_lambda_functions.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/rudder_equations.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/rudder_lambda_functions.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/run_real_seaman.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/save_lambda_functions.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/seaman_symbol.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/seaman_symbols.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/substitute_dynamic_symbols.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/surge_hull_equations.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/surge_hull_lambda_functions.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/sway_hull_equations.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/sway_hull_lambda_functions.py
+-rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/test_ship.ship
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/total_equations.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/total_lambda_functions.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/yaw_hull_equations.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/docs/seaman/yaw_hull_lambda_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/models/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/.gitkeep
+-rw-r--r--   0        0        0   332654 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/01.00_MDL_select_runs.ipynb
+-rw-r--r--   0        0        0    27865 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/02.00_MDL_load_runs.ipynb
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/03.00_test_overview.ipynb
+-rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/04.01_PIT_nomoto.ipynb
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/04.02_PIT_linear_VMM.ipynb
+-rw-r--r--   0        0        0     9376 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/04.02_PIT_nomotos.ipynb
+-rw-r--r--   0        0        0    19255 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/04.02_PIT_nonlinear_VMM.ipynb
+-rw-r--r--   0        0        0    31214 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/04.03_PIT_VCT_linear_VMM.ipynb
+-rw-r--r--   0        0        0    32154 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/04.03_PIT_VCT_nonlinear_VMM.ipynb
+-rw-r--r--   0        0        0    34957 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/04.03_PIT_linear_VMM.ipynb
+-rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/05.01_acceleration_Kalman.ipynb
+-rw-r--r--   0        0        0   274069 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/05.02_transform_to_ship.ipynb
+-rw-r--r--   0        0        0   879206 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/05.03_cutting.ipynb
+-rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/05.semiempirical_rudder_wpcc.ipynb
+-rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/06.01_linear_VMM.ipynb
+-rw-r--r--   0        0        0    23562 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/06.01_linear_simplified_VMM.ipynb
+-rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/06.02_linear_VMM_wPCC_brix.ipynb
+-rw-r--r--   0        0        0  1165028 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/07.03_PIT_static_forces_nonlinear.ipynb
+-rw-r--r--   0        0        0    37675 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/07_01_static_forces_from_model_test.ipynb
+-rw-r--r--   0        0        0  1176968 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/07_02_static_forces_from_spirals.ipynb
+-rw-r--r--   0        0        0    48697 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/07_05_static_forces_from_model_test-many.ipynb
+-rw-r--r--   0        0        0    49041 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/08_01_PIT_summary.ipynb
+-rw-r--r--   0        0        0    44439 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/08_02_PIT_nonlinear_summary.ipynb
+-rw-r--r--   0        0        0    24616 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/09_01_PIT_tongton.ipynb
+-rw-r--r--   0        0        0    23537 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/09_02_PIT_tongton_SI.ipynb
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/10.01_EOM_air.ipynb
+-rw-r--r--   0        0        0    19914 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/10.02_kalman_PIT_sensitivity.ipynb
+-rw-r--r--   0        0        0    33006 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/10.03_lowpass_PIT.ipynb
+-rw-r--r--   0        0        0    30697 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/11.01_regression_revisited.ipynb
+-rw-r--r--   0        0        0    25508 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/12.01_regression_simulated_data.ipynb
+-rw-r--r--   0        0        0    25899 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/12.02_regression_simulated_data_nonlinear_EOM.ipynb
+-rw-r--r--   0        0        0    37550 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/12.03_regression_simulated_data_mariner.ipynb
+-rw-r--r--   0        0        0    24478 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/12.04_regression_too_little_simulated_data.ipynb
+-rw-r--r--   0        0        0    28072 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/12.05.5_regression_simulated_data_simple_nonlinear_BDF.ipynb
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/12.05_regression_simulated_data_acc_thrust.ipynb
+-rw-r--r--   0        0        0    27714 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/12.05_regression_simulated_data_simple_nonlinear.ipynb
+-rw-r--r--   0        0        0    24448 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/12.06.5_regression_simulated_data_BDF_numerical_gradient.ipynb
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/12.06_regression_simulated_data_numerical_gradient.ipynb
+-rw-r--r--   0        0        0    27318 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/12.07_regression_simulated_data_better_numerical_gradient.ipynb
+-rw-r--r--   0        0        0    22934 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/12.08_regression_simulated_data_gausian_noise.ipynb
+-rw-r--r--   0        0        0    24594 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/12.08_regression_simulated_more_data_gausian_noise.ipynb
+-rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/13.01_solve_ivp.ipynb
+-rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/14.01_EM_algorithm.ipynb
+-rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/14.01_hidden_states.ipynb
+-rw-r--r--   0        0        0    23581 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/14.02_hidden_states_gradient_regression.ipynb
+-rw-r--r--   0        0        0    24046 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/14.03_hidden_states_gradient_regression_linear.ipynb
+-rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.01_kalman_filter_unvariate.ipynb
+-rw-r--r--   0        0        0    21616 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.10_kalman_filter_multivariate.ipynb
+-rw-r--r--   0        0        0    31286 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.11_kalman_filter_linear_manoeuvring.ipynb
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.20_EM-algorithm.ipynb
+-rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.30_KF_fossen.ipynb
+-rw-r--r--   0        0        0    12804 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.31_EKF_fossen.ipynb
+-rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.39_KF_nomoto.ipynb
+-rw-r--r--   0        0        0    15487 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.40_EKF_nomoto.ipynb
+-rw-r--r--   0        0        0    18938 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.41_EKF_PIT_nomoto.ipynb
+-rw-r--r--   0        0        0    21033 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.42_EKF_EM_nomoto.ipynb
+-rw-r--r--   0        0        0    19373 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.42_EKF_PIT_2_nomoto.ipynb
+-rw-r--r--   0        0        0    17287 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.44_KF_EM_RTS_nomoto.ipynb
+-rw-r--r--   0        0        0   299798 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.45_KF_EM_RTS_nomoto.ipynb
+-rw-r--r--   0        0        0    14125 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.46_EKF_Abkowitz.ipynb
+-rw-r--r--   0        0        0    45662 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.47_EKF_3DOF.ipynb
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.47_EKF_3DOF.py
+-rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.48_EK_smoother_3DOF.ipynb
+-rw-r--r--   0        0        0    29295 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.49_EK_smoother_3DOF_thrust.ipynb
+-rw-r--r--   0        0        0    15522 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.50_KF_EM_RTS_nomoto.ipynb
+-rw-r--r--   0        0        0    21888 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.51_EK_inverse_dynamics.ipynb
+-rw-r--r--   0        0        0    10993 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/15.52_inverse_static.ipynb
+-rw-r--r--   0        0        0    17497 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/16.01_PIT_VCT_revisited_linear.ipynb
+-rw-r--r--   0        0        0    19792 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/16.02_PIT_VCT_revisited_nonlinear.ipynb
+-rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/16.03_model_simulate.ipynb
+-rw-r--r--   0        0        0    25951 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/17.01_RTS_manoeuvring_PIT.ipynb
+-rw-r--r--   0        0        0    19422 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/21.01_parameter_drift.ipynb
+-rw-r--r--   0        0        0    17265 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/21.02_parameter_drift.ipynb
+-rw-r--r--   0        0        0    23816 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/21.03_parameter_drift.ipynb
+-rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/21.04_perfect_captive.ipynb
+-rw-r--r--   0        0        0    13073 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/21.05_perfect_captive_truncated.ipynb
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/22.01_scaling_VCT_captive.ipynb
+-rw-r--r--   0        0        0   334166 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/30.01_joke.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/__init__.py
+-rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/ai_research.png
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/example_ship2.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/imports.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/logbook.ipynb
+-rw-r--r--   0        0        0    33486 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/matplotlibrc
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/research.ipynb
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/model_simulate/01.01_run_simulations.py
+-rw-r--r--   0        0        0    10404 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/model_simulate/02.01_analyze_runs.ipynb
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/notebooks/model_simulate/templates/16.03_model_simulate.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/references/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/reports/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/reports/figures/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/.gitkeep
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_EKF_PIT_Nomot.py
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_KF_Nomoto.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_diff_eq_to_matrix.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_extended_kalman_filter.py
+-rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_extended_kalman_vmm.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_force_regression.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_kalman_filter.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_last_known_value_interpolation.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_linear_vmm.py
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_model_simulator.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_parameter_denominator.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_prime_system.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_rts_smoother.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/tests/test_vmm_simple_nonliear.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/__init__.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/angles.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/apparent_wind.py
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/bias_variance_tradeoff.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/equation_helpers.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/equations.py
+-rw-r--r--   0        0        0    14321 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/extended_kalman_filter.py
+-rw-r--r--   0        0        0    26990 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/extended_kalman_vmm.py
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/feature_selection.py
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/kalman_filter.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/linear_vmm_equations.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/linear_vmm_simplified_equations.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/logger.py
+-rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/mlflow_utils.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/nonlinear_abkowitz_vmm_equations.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/nonlinear_martin_vmm_equations.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/nonlinear_vmm_equations.py
+-rw-r--r--   0        0        0    12924 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/notebook_to_latex.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/parameter_helpers.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/parameters.py
+-rw-r--r--   0        0        0    11382 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/prime_system.py
+-rw-r--r--   0        0        0     7240 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/substitute_dynamic_symbols.py
+-rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/symbols.py
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/system_equations.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/to_mlflow.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/twin_simulations.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/vct_scaling.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/vmm_equations_VCT.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/__init__.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/case_0.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/case_1.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/kalman_filter.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/lowpass_filter.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/make_dataset.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/mdl.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/wpcc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/features/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/features/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/features/build_features.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/.gitkeep
+-rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/IMO_simulations.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/MMG_hull.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/MMG_propeller.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/MMG_rudder.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/ModelSimulatorWithPropellerSemiempiricalRudder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/__init__.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/abkowitz_rudder_system.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/brix_coefficients.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/captive_variation.py
+-rw-r--r--   0        0        0    10864 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/diff_eq_to_matrix.py
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/force_from_motion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/linear_nomoto.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/linear_vmm.py
+-rw-r--r--   0        0        0    24175 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/modular_simulator.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/nonlinear_martin_vmm.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/nonlinear_vmm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/predict_model.py
+-rw-r--r--   0        0        0    10361 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/propeller.py
+-rw-r--r--   0        0        0    22054 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/regression.py
+-rw-r--r--   0        0        0    13420 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/result.py
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/semiempirical_covered.py
+-rw-r--r--   0        0        0    10839 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/semiempirical_rudder.py
+-rw-r--r--   0        0        0    15005 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/semiempirical_rudder_MAK.py
+-rw-r--r--   0        0        0    13855 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/subsystem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/train_model.py
+-rw-r--r--   0        0        0    32818 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_7m_vct.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_MMG.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_VCT.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_abkowitz.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_abkowitz_expanded.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_abkowitz_no_thrust.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_air.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_gsi.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_linear.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_mariner.py
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_martin.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_martin_linear.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_martin_simple.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_nonlinear_EOM.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_perturbed.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_simple.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_simple_nonlinear.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/wind_force.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/wind_force_helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vessels/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vessels/mariner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/visualization/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/visualization/__init__.py
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/visualization/book_format.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/visualization/equation.py
+-rw-r--r--   0        0        0    13763 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/visualization/plot.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/visualization/regression.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/visualization/visualize.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/LICENSE
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/README.md
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.7/PKG-INFO
```

### Comparing `vessel_manoeuvring_models-0.0.6/Makefile` & `vessel_manoeuvring_models-0.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/test_environment.py` & `vessel_manoeuvring_models-0.0.7/test_environment.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/data/interim/run_selection.csv` & `vessel_manoeuvring_models-0.0.7/data/interim/run_selection.csv`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/Makefile` & `vessel_manoeuvring_models-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/conf.py` & `vessel_manoeuvring_models-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/make.bat` & `vessel_manoeuvring_models-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/00.01_intro.md` & `vessel_manoeuvring_models-0.0.7/docs/book/00.01_intro.md`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/00.02_intro_example.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/book/00.02_intro_example.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/01.01_manoeuvring_simulation.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/book/01.01_manoeuvring_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/02.01_manoeuvring_PIT.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/book/02.01_manoeuvring_PIT.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/10.03_OLS_covariance.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/book/10.03_OLS_covariance.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/10.04_bias_variance.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/book/10.04_bias_variance.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/15.39_KF_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/book/15.39_KF_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/15.40_EKF_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/book/15.40_EKF_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/30.01_maximum_likelihood.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/book/30.01_maximum_likelihood.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/_config.yml` & `vessel_manoeuvring_models-0.0.7/docs/book/_config.yml`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/book.mplstyle` & `vessel_manoeuvring_models-0.0.7/docs/book/book.mplstyle`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/chapter.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/book/chapter.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/example_1.py` & `vessel_manoeuvring_models-0.0.7/docs/book/example_1.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/imports.py` & `vessel_manoeuvring_models-0.0.7/docs/book/imports.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/logo.png` & `vessel_manoeuvring_models-0.0.7/docs/book/logo.png`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/markdown.md` & `vessel_manoeuvring_models-0.0.7/docs/book/markdown.md`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/book/references.bib` & `vessel_manoeuvring_models-0.0.7/docs/book/references.bib`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/01.1_seaman_matematical_model.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/seaman/01.1_seaman_matematical_model.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/02.1_seaman_sway_hull_equation.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/seaman/02.1_seaman_sway_hull_equation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/03.1_seaman_yaw_hull_equation.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/seaman/03.1_seaman_yaw_hull_equation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/04.1_seaman_rudder_equation.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/seaman/04.1_seaman_rudder_equation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/04.2_seaman_rudder_equation_modified_drag.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/seaman/04.2_seaman_rudder_equation_modified_drag.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/05.1_seaman_surge_hull_equation.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/seaman/05.1_seaman_surge_hull_equation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/06.1_seaman_roll_hull_equation.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/seaman/06.1_seaman_roll_hull_equation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/10_seaman_rigid_body.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/seaman/10_seaman_rigid_body.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/11_manoeuvring_simulation.ipynb` & `vessel_manoeuvring_models-0.0.7/docs/seaman/11_manoeuvring_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/X_function.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/X_function.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/Y_function.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/Y_function.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/__init__.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/__init__.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/bis_system.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/bis_system.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/cd.png` & `vessel_manoeuvring_models-0.0.7/docs/seaman/cd.png`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/coordinateSystem.png` & `vessel_manoeuvring_models-0.0.7/docs/seaman/coordinateSystem.png`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/coordinate_system.png` & `vessel_manoeuvring_models-0.0.7/docs/seaman/coordinate_system.png`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/curve_fit.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/curve_fit.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/generate_input.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/generate_input.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/notebooks_to_html.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/notebooks_to_html.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/regression.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/regression.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/regression_old.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/regression_old.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/roll_hull_equations.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/roll_hull_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/rudder_equations.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/rudder_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/rudder_lambda_functions.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/rudder_lambda_functions.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/run_real_seaman.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/run_real_seaman.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/save_lambda_functions.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/save_lambda_functions.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/seaman_symbol.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/seaman_symbol.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/seaman_symbols.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/seaman_symbols.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/substitute_dynamic_symbols.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/substitute_dynamic_symbols.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/sway_hull_equations.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/sway_hull_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/sway_hull_lambda_functions.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/sway_hull_lambda_functions.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/test_ship.ship` & `vessel_manoeuvring_models-0.0.7/docs/seaman/test_ship.ship`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/total_equations.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/total_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/total_lambda_functions.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/total_lambda_functions.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/yaw_hull_equations.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/yaw_hull_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/docs/seaman/yaw_hull_lambda_functions.py` & `vessel_manoeuvring_models-0.0.7/docs/seaman/yaw_hull_lambda_functions.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/01.00_MDL_select_runs.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/01.00_MDL_select_runs.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/02.00_MDL_load_runs.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/02.00_MDL_load_runs.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/03.00_test_overview.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/03.00_test_overview.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/04.01_PIT_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/04.01_PIT_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/04.02_PIT_linear_VMM.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/04.02_PIT_linear_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/04.02_PIT_nomotos.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/04.02_PIT_nomotos.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/04.02_PIT_nonlinear_VMM.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/04.02_PIT_nonlinear_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/04.03_PIT_VCT_linear_VMM.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/04.03_PIT_VCT_linear_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/04.03_PIT_VCT_nonlinear_VMM.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/04.03_PIT_VCT_nonlinear_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/04.03_PIT_linear_VMM.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/04.03_PIT_linear_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/05.01_acceleration_Kalman.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/05.01_acceleration_Kalman.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/05.02_transform_to_ship.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/05.02_transform_to_ship.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/05.03_cutting.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/05.03_cutting.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/05.semiempirical_rudder_wpcc.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/05.semiempirical_rudder_wpcc.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/06.01_linear_VMM.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/06.01_linear_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/06.01_linear_simplified_VMM.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/06.01_linear_simplified_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/06.02_linear_VMM_wPCC_brix.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/06.02_linear_VMM_wPCC_brix.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/07.03_PIT_static_forces_nonlinear.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/07.03_PIT_static_forces_nonlinear.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/07_01_static_forces_from_model_test.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/07_01_static_forces_from_model_test.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/07_02_static_forces_from_spirals.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/07_02_static_forces_from_spirals.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/07_05_static_forces_from_model_test-many.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/07_05_static_forces_from_model_test-many.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/08_01_PIT_summary.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/08_01_PIT_summary.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/08_02_PIT_nonlinear_summary.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/08_02_PIT_nonlinear_summary.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/09_01_PIT_tongton.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/09_01_PIT_tongton.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/09_02_PIT_tongton_SI.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/09_02_PIT_tongton_SI.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/10.01_EOM_air.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/10.01_EOM_air.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/10.02_kalman_PIT_sensitivity.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/10.02_kalman_PIT_sensitivity.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/10.03_lowpass_PIT.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/10.03_lowpass_PIT.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/11.01_regression_revisited.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/11.01_regression_revisited.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/12.01_regression_simulated_data.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/12.01_regression_simulated_data.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/12.02_regression_simulated_data_nonlinear_EOM.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/12.02_regression_simulated_data_nonlinear_EOM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/12.03_regression_simulated_data_mariner.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/12.03_regression_simulated_data_mariner.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/12.04_regression_too_little_simulated_data.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/12.04_regression_too_little_simulated_data.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/12.05.5_regression_simulated_data_simple_nonlinear_BDF.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/12.05.5_regression_simulated_data_simple_nonlinear_BDF.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/12.05_regression_simulated_data_acc_thrust.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/12.05_regression_simulated_data_acc_thrust.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/12.05_regression_simulated_data_simple_nonlinear.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/12.05_regression_simulated_data_simple_nonlinear.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/12.06.5_regression_simulated_data_BDF_numerical_gradient.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/12.06.5_regression_simulated_data_BDF_numerical_gradient.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/12.06_regression_simulated_data_numerical_gradient.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/12.06_regression_simulated_data_numerical_gradient.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/12.07_regression_simulated_data_better_numerical_gradient.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/12.07_regression_simulated_data_better_numerical_gradient.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/12.08_regression_simulated_data_gausian_noise.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/12.08_regression_simulated_data_gausian_noise.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/12.08_regression_simulated_more_data_gausian_noise.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/12.08_regression_simulated_more_data_gausian_noise.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/13.01_solve_ivp.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/13.01_solve_ivp.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/14.01_EM_algorithm.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/14.01_EM_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/14.01_hidden_states.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/14.01_hidden_states.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/14.02_hidden_states_gradient_regression.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/14.02_hidden_states_gradient_regression.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/14.03_hidden_states_gradient_regression_linear.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/14.03_hidden_states_gradient_regression_linear.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.01_kalman_filter_unvariate.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.01_kalman_filter_unvariate.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.10_kalman_filter_multivariate.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.10_kalman_filter_multivariate.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.11_kalman_filter_linear_manoeuvring.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.11_kalman_filter_linear_manoeuvring.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.20_EM-algorithm.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.20_EM-algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.30_KF_fossen.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.30_KF_fossen.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.31_EKF_fossen.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.31_EKF_fossen.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.39_KF_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.39_KF_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.40_EKF_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.40_EKF_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.41_EKF_PIT_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.41_EKF_PIT_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.42_EKF_EM_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.42_EKF_EM_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.42_EKF_PIT_2_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.42_EKF_PIT_2_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.44_KF_EM_RTS_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.44_KF_EM_RTS_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.45_KF_EM_RTS_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.45_KF_EM_RTS_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.46_EKF_Abkowitz.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.46_EKF_Abkowitz.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.47_EKF_3DOF.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.47_EKF_3DOF.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.47_EKF_3DOF.py` & `vessel_manoeuvring_models-0.0.7/notebooks/15.47_EKF_3DOF.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.48_EK_smoother_3DOF.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.48_EK_smoother_3DOF.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.49_EK_smoother_3DOF_thrust.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.49_EK_smoother_3DOF_thrust.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.50_KF_EM_RTS_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.50_KF_EM_RTS_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.51_EK_inverse_dynamics.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.51_EK_inverse_dynamics.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/15.52_inverse_static.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/15.52_inverse_static.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/16.01_PIT_VCT_revisited_linear.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/16.01_PIT_VCT_revisited_linear.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/16.02_PIT_VCT_revisited_nonlinear.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/16.02_PIT_VCT_revisited_nonlinear.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/16.03_model_simulate.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/16.03_model_simulate.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/17.01_RTS_manoeuvring_PIT.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/17.01_RTS_manoeuvring_PIT.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/21.01_parameter_drift.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/21.01_parameter_drift.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/21.02_parameter_drift.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/21.02_parameter_drift.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/21.03_parameter_drift.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/21.03_parameter_drift.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/21.04_perfect_captive.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/21.04_perfect_captive.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/21.05_perfect_captive_truncated.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/21.05_perfect_captive_truncated.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/22.01_scaling_VCT_captive.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/22.01_scaling_VCT_captive.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/30.01_joke.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/30.01_joke.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/ai_research.png` & `vessel_manoeuvring_models-0.0.7/notebooks/ai_research.png`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/example_ship2.py` & `vessel_manoeuvring_models-0.0.7/notebooks/example_ship2.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/imports.py` & `vessel_manoeuvring_models-0.0.7/notebooks/imports.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/logbook.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/logbook.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/matplotlibrc` & `vessel_manoeuvring_models-0.0.7/notebooks/matplotlibrc`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/research.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/research.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/model_simulate/01.01_run_simulations.py` & `vessel_manoeuvring_models-0.0.7/notebooks/model_simulate/01.01_run_simulations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/model_simulate/02.01_analyze_runs.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/model_simulate/02.01_analyze_runs.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/notebooks/model_simulate/templates/16.03_model_simulate.ipynb` & `vessel_manoeuvring_models-0.0.7/notebooks/model_simulate/templates/16.03_model_simulate.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/tests/test_EKF_PIT_Nomot.py` & `vessel_manoeuvring_models-0.0.7/tests/test_EKF_PIT_Nomot.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/tests/test_KF_Nomoto.py` & `vessel_manoeuvring_models-0.0.7/tests/test_KF_Nomoto.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/tests/test_extended_kalman_filter.py` & `vessel_manoeuvring_models-0.0.7/tests/test_extended_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/tests/test_extended_kalman_vmm.py` & `vessel_manoeuvring_models-0.0.7/tests/test_extended_kalman_vmm.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/tests/test_force_regression.py` & `vessel_manoeuvring_models-0.0.7/tests/test_force_regression.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/tests/test_kalman_filter.py` & `vessel_manoeuvring_models-0.0.7/tests/test_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/tests/test_linear_vmm.py` & `vessel_manoeuvring_models-0.0.7/tests/test_linear_vmm.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/tests/test_model_simulator.py` & `vessel_manoeuvring_models-0.0.7/tests/test_model_simulator.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/tests/test_parameter_denominator.py` & `vessel_manoeuvring_models-0.0.7/tests/test_parameter_denominator.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/tests/test_prime_system.py` & `vessel_manoeuvring_models-0.0.7/tests/test_prime_system.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/tests/test_rts_smoother.py` & `vessel_manoeuvring_models-0.0.7/tests/test_rts_smoother.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/tests/test_vmm_simple_nonliear.py` & `vessel_manoeuvring_models-0.0.7/tests/test_vmm_simple_nonliear.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/bias_variance_tradeoff.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/bias_variance_tradeoff.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/extended_kalman_filter.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/extended_kalman_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import numpy as np
 from numpy.linalg.linalg import inv, pinv
 import pandas as pd
 from typing import AnyStr, Callable
 from copy import deepcopy
+import numpy as np
 
 from scipy.stats import multivariate_normal
 
+from vessel_manoeuvring_models.angles import smallest_signed_angle
+import logging
+
+log = logging.getLogger(__name__)
+
 
 def extended_kalman_filter(
     P_prd: np.ndarray,
     lambda_f: Callable,
     lambda_jacobian: Callable,
     data: pd.DataFrame,
     Qd: float,
     Rd: float,
     E: np.ndarray,
     Cd: np.ndarray,
     state_columns=["x0", "y0", "psi", "u", "v", "r"],
     measurement_columns=["x0", "y0", "psi"],
     input_columns=["delta"],
     x0: np.ndarray = None,
+    angle_columns=["psi"],
+    do_checks=True,
     **kwargs,
 ) -> list:
     """Example extended kalman filter
 
     Parameters
     ----------
     x0 : np.ndarray, default None
@@ -90,87 +98,123 @@
 
     measurement_columns: list
         name of columns in data that are measurements ex: ["x0", "y0", "psi"],
 
     input_columns: list
         name of columns in the data that are inputs ex: ["delta"]
 
+    angle_columns: list
+        name of columns that are angles ex: ["psi", "r"]
+        The "smallest signed angle" are used for these states when the predictor error "eps" is calculated
+
 
     Returns
     -------
     list
         list with time steps as dicts.
     """
 
     no_states = len(state_columns)
     no_measurement_states = len(measurement_columns)
 
     no_hidden_states = no_states - no_measurement_states
 
-    h = np.mean(np.diff(data.index))
-    inputs = data[input_columns]
-    ys = data[measurement_columns].values
-
     if x0 is None:
         x0 = data.iloc[0][state_columns].values
 
     ## Check dimensions:
-    assert (
-        len(x0) == no_states
-    ), f"This filter has {no_states} states ('no_states'), but initial state vector 'x0' should have length:{no_states}"
+    if do_checks:
+        assert (
+            len(x0) == no_states
+        ), f"This filter has {no_states} states ('no_states'), but initial state vector 'x0' should have length:{no_states}"
+
+        assert P_prd.shape == (
+            no_states,
+            no_states,
+        ), f"This filter has {no_states} states ('no_states'), the initial state covariance matrix ('P_prd') should have shape:{(no_states, no_states)}"
+
+        assert Qd.shape == (
+            no_hidden_states,
+            no_hidden_states,
+        ), f"This filter has {no_states} states ('no_states'), the Covariance matrix of the process model ('Qd') should have shape:{(no_hidden_states, no_hidden_states)}"
+
+        assert Rd.shape == (
+            no_measurement_states,
+            no_measurement_states,
+        ), f"This filter has {no_states} states ('no_states'), the Covariance matrix of the measurement ('Rd') should have shape:{(no_measurement_states, no_measurement_states)}"
+
+        assert E.shape == (
+            no_states,
+            no_hidden_states,
+        ), f"This filter has {no_states} states ('no_states'), ('E') should have shape:{(no_states,no_hidden_states)}"
+
+        assert Cd.shape == (
+            no_measurement_states,
+            no_states,
+        ), f"This filter has {no_states} states ('no_states'), ('Cd') should have shape:{(no_measurement_states,no_states)}"
 
-    assert P_prd.shape == (
-        no_states,
-        no_states,
-    ), f"This filter has {no_states} states ('no_states'), the initial state covariance matrix ('P_prd') should have shape:{(no_states, no_states)}"
-
-    assert Qd.shape == (
-        no_hidden_states,
-        no_hidden_states,
-    ), f"This filter has {no_states} states ('no_states'), the Covariance matrix of the process model ('Qd') should have shape:{(no_hidden_states, no_hidden_states)}"
-
-    assert Rd.shape == (
-        no_measurement_states,
-        no_measurement_states,
-    ), f"This filter has {no_states} states ('no_states'), the Covariance matrix of the measurement ('Rd') should have shape:{(no_measurement_states, no_measurement_states)}"
-
-    assert E.shape == (
-        no_states,
-        no_hidden_states,
-    ), f"This filter has {no_states} states ('no_states'), ('E') should have shape:{(no_states,no_hidden_states)}"
-
-    assert Cd.shape == (
-        no_measurement_states,
-        no_states,
-    ), f"This filter has {no_states} states ('no_states'), ('Cd') should have shape:{(no_measurement_states,no_states)}"
+    mask_angles = [key in angle_columns for key in measurement_columns]
 
     # Initial state:
     x_prd = np.array(x0).reshape(no_states, 1)
     P_prd = np.array(P_prd)
 
     time_steps = []
 
-    N = len(ys)
+    inputs = data[input_columns]
+    ys = data[measurement_columns]
+
+    assert inputs.notnull().all().all(), "inputs contains NaNs"
+    assert ys.notnull().all().all(), "measurements contains NaNs"
+
+    h_median = np.median(np.diff(data.index))
+    h = np.min(np.diff(data.index))
+    if h_median / h > 4:
+        log.warning(
+            f"Using the smallest timestep in data will produce a lot of interations in Kalman filter."
+        )
+
+    ts = np.arange(
+        data.index[0], data.index[-1], h
+    )  # Time signal with equal time steps
+
+    N = len(ts)
     Ed = h * E
 
-    for i in range(N):
-        t = i * h
+    for t in ts:
+        t_sample = find_closest(data=data, t=t)
 
-        input = inputs.iloc[i]  # input
-        y = np.array([ys[i]]).T  # measurement
+        if abs(t - t_sample) < 0.7 * h:
+            # Loading a measurement:
+            input = inputs.loc[t_sample]  # input
+            # y = np.array([ys[i]]).T  # measurement
+            y = ys.loc[t_sample]  # measurement
+            y = np.array([y.values]).T
+            Cd_ = Cd
+            # print("update")
+        else:
+            Cd_ = 0 * Cd  # no measurements
+            # print("dead reckoning")
 
         # Compute kalman gain:
         # S = Cd @ P_prd @ Cd.T + Rd  # System uncertainty
         # K = P_prd @ Cd.T @ inv(S)
-        K = P_prd @ Cd.T @ pinv(Cd @ P_prd @ Cd.T + Rd)
-        IKC = np.eye(no_states) - K @ Cd
+        try:
+            K = P_prd @ Cd_.T @ pinv(Cd_ @ P_prd @ Cd_.T + Rd)
+        except Exception as e:
+            raise TypeError(f"Crashed at iteration time: {t} s") from e
+
+        IKC = np.eye(no_states) - K @ Cd_
 
         ## State corrector:
         P_hat = IKC @ P_prd @ IKC.T + K @ Rd @ K.T
-        eps = y - Cd @ x_prd
+        eps = y - Cd_ @ x_prd
+        eps[mask_angles] = smallest_signed_angle(
+            eps[mask_angles]
+        )  # Smalles signed angle
         x_hat = x_prd + K @ eps
 
         ## discrete-time extended KF-model
         f_hat = lambda_f(x=x_hat.flatten(), input=input).reshape((no_states, 1))
 
         ## Predictor (k+1)
         ## Ad = I + h * A and Ed = h * E
@@ -195,27 +239,44 @@
         }
 
         time_steps.append(time_step)
 
     return time_steps
 
 
-def rts_smoother(time_steps: list, lambda_jacobian: Callable, Qd, lambda_f, E):
+def find_closest(data: pd.DataFrame, t: float) -> float:
+    """Find closes time stamp
 
+    Parameters
+    ----------
+    data : pd.DataFrame
+        _description_
+    t : float
+        _description_
+
+    Returns
+    -------
+    float
+        _description_
+    """
+    i = np.argmin(np.abs(data.index - t))
+    return data.index[i]
+
+
+def rts_smoother(time_steps: list, lambda_jacobian: Callable, Qd, lambda_f, E):
     no_states = len(time_steps[0]["x_hat"])
 
     n = len(time_steps)
 
     s = deepcopy(time_steps)
 
     h = s[1]["time"] - s[0]["time"]
     Ed = h * E
 
     for k in range(n - 2, -1, -1):
-
         input = s[k]["input"]
 
         Ad = lambda_jacobian(x=s[k]["x_hat"].flatten(), input=input)
         # Pp = Ad @ s[k]["P_hat"] @ Ad.T + Qd  # predicted covariance
         Pp = Ad @ s[k]["P_hat"] @ Ad.T + Ed @ Qd @ Ed.T  # predicted covariance
 
         s[k]["K"] = s[k]["P_hat"] @ Ad.T @ pinv(Pp)
@@ -332,15 +393,14 @@
     simdata = np.zeros((len(x0), len(t)))
     x_ = x0.reshape(len(x0), 1)
     h = t[1] - t[0]
     Ed = h * E
     inputs = data[input_columns]
 
     for i in range(len(t)):
-
         input = inputs.iloc[i]
         w_ = ws[i]
 
         w_ = w_.reshape(E.shape[1], 1)
         x_dot = lambda_f(x_.flatten(), input) + Ed @ w_
         x_ = x_ + h * x_dot
 
@@ -350,15 +410,14 @@
     df.index.name = "time"
     df[input_columns] = inputs.values
 
     return df
 
 
 def _loglikelihood(time_step: dict) -> float:
-
     mean = time_step["x_hat"].flatten()
     cov = time_step["P_hat"]
     x_prd = time_step["x_prd"]
     rv = multivariate_normal(mean=mean, cov=cov)
     return rv.logpdf(x_prd.flatten())
 
 
@@ -404,20 +463,23 @@
     return pd.DataFrame([time_step["input"] for time_step in time_steps], index=t)
 
 
 def variance(time_steps):
     return np.array([np.diagonal(time_step["P_hat"]) for time_step in time_steps]).T
 
 
+def K(time_steps):
+    return np.array([np.diagonal(time_step["K"]) for time_step in time_steps]).T
+
+
 def time_steps_to_df(
     time_steps: list,
     state_columns: list = ["x0", "y0", "psi", "u", "v", "r"],
     add_gradients=True,
 ) -> pd.DataFrame:
-
     x_hats = x_hat(time_steps)
     t = time(time_steps)
     inputs_ = inputs(time_steps)
 
     df = pd.DataFrame(
         data=x_hats.T,
         index=t,
```

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/feature_selection.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/feature_selection.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/kalman_filter.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/linear_vmm_equations.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/linear_vmm_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/linear_vmm_simplified_equations.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/linear_vmm_simplified_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/mlflow_utils.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/nonlinear_abkowitz_vmm_equations.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/nonlinear_abkowitz_vmm_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/nonlinear_martin_vmm_equations.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/nonlinear_martin_vmm_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/nonlinear_vmm_equations.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/nonlinear_vmm_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/notebook_to_latex.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/notebook_to_latex.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/parameters.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/parameters.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 df_parameters = pd.DataFrame(columns=["symbol", "dof", "coord", "state", "denominator"])
 dofs = ["X", "Y", "N"]
 coords = ["u", "v", "r", r"\delta"]
 states = ["", "dot"]
 
 
 def get_parameter_denominator(dof, coord, state=""):
-
     numerator = prime_system.get_denominator(key=dof)  # X,Y,N...
 
     keys = []
     if state == "dot":
         key = f"{coord}1d"
         keys.append(key)
     else:
@@ -28,15 +27,14 @@
         denominator *= prime_system.get_denominator(key=key)
 
     parameter_denominator = numerator / denominator
     return parameter_denominator
 
 
 def add_parameter(dof, coord, state=""):
-
     key = f"{dof}{coord}{state}"
     key = key.replace("\\", "")
 
     if len(state) > 0:
         symbol_name = r"%s_{\%s{%s}}" % (dof, state, coord)
     else:
         symbol_name = r"%s_{%s%s}" % (dof, state, coord)
@@ -52,14 +50,16 @@
 
 
 for dof in dofs:
     for coord in ["u", "v", "r"]:
         add_parameter(dof=dof, coord=coord, state="dot")
 
 add_parameter(dof="X", coord="thrust")
+add_parameter(dof="X", coord="thrustport")
+add_parameter(dof="X", coord="thruststbd")
 add_parameter(dof="N", coord="thrust")
 add_parameter(dof="Y", coord="thrust")
 add_parameter(dof="X", coord="rrthrust")
 add_parameter(dof="X", coord="0")
 add_parameter(dof="Y", coord="0")
 add_parameter(dof="Y", coord="0u")
 add_parameter(dof="Y", coord="0uu")
@@ -67,14 +67,21 @@
 add_parameter(dof="N", coord="0u")
 add_parameter(dof="N", coord="0uu")
 add_parameter(dof="Y", coord="thrustdelta")
 add_parameter(dof="N", coord="thrustdelta")
 add_parameter(dof="X", coord="vvvv")
 
 
+deg = 6
+for i in range(deg + 1):
+    for dof in ["X", "Y", "N"]:
+        name = f"C_{dof.lower()}{i}"
+        df_parameters.loc[name, "symbol"] = sp.symbols(name)
+        df_parameters.loc[name, "dof"] = dof
+
 ## Add all possible combinations:
 from sklearn.preprocessing import PolynomialFeatures
 import re
 
 df_ = pd.DataFrame(
     columns=[
         "u",
@@ -85,16 +92,17 @@
     data=np.zeros((10, 4)),
 )
 polynomial_features = PolynomialFeatures(degree=3, include_bias=False)
 polynomial_features.fit_transform(df_)
 try:
     feature_names = polynomial_features.get_feature_names(df_.columns)  # Old sklearn
 except Exception as e:
-    feature_names = polynomial_features.get_feature_names_out(df_.columns)  # New sklearn
-
+    feature_names = polynomial_features.get_feature_names_out(
+        df_.columns
+    )  # New sklearn
 
 
 def rename(result):
     return result.group(1) * int(result.group(2))
 
 
 feature_names = [
@@ -102,29 +110,44 @@
 ]
 feature_names = [name.replace(" ", "") for name in feature_names]
 for dof in dofs:
     for coord in feature_names:
         add_parameter(dof=dof, coord=coord)
 
 ## Parameters according to:
-Xudot_ = m / (π * sp.sqrt(L ** 3 / volume) - 14)  # [Brix] (SI)
-Xudot_prime = Xudot_ / (1 / 2 * rho * L ** 3)
+Xudot_ = m / (π * sp.sqrt(L**3 / volume) - 14)  # [Brix] (SI)
+Xudot_prime = Xudot_ / (1 / 2 * rho * L**3)
 df_parameters.loc["Xudot", "brix"] = Xudot_prime  # [Brix]
 df_parameters.loc["Yvdot", "brix"] = (
     -π * (T / L) ** 2 * (1 + 0.16 * CB * B / T - 5.1 * (B / L) ** 2)
 )  # [Clarke]
 df_parameters.loc["Yrdot", "brix"] = (
     -π * (T / L) ** 2 * (0.67 * B / L - 0.0033 * (B / T) ** 2)
 )  # [Clarke]
 df_parameters.loc["Nvdot", "brix"] = (
     -π * (T / L) ** 2 * (1.1 * B / L - 0.04 * (B / T))
 )  # [Clarke]
+
+
+Nrdot = (
+    0.5
+    * rho
+    * L**5
+    * (-sp.pi * (T / L) ** 2 * (0.0833 + 0.017 * (CB * B / T) - 0.0033 * (B / L)))
+)  # [Clarke]
+
 df_parameters.loc["Nrdot", "brix"] = (
-    -π * (T / L) ** 2 * (1 / 12 + 0.017 * CB * B / T - 0.33 * (B / L))
+    Nrdot / df_parameters.loc["Nrdot", "denominator"]
 )  # [Clarke]
+
+# df_parameters.loc["Nrdot", "brix"] = (
+#    -π * (T / L) ** 2 * (1 / 12 + 0.017 * CB * B / T - 0.33 * (B / L))
+# )  # [Clarke] (But with typo in Matusiak 2nd edition)
+
+
 df_parameters.loc["Yv", "brix"] = -π * (T / L) ** 2 * (1 + 0.4 * CB * B / T)  # [Clarke]
 df_parameters.loc["Yr", "brix"] = (
     -π * (T / L) ** 2 * (-1 / 2 + 2.2 * B / L - 0.08 * (B / T))
 )  # [Clarke]
 df_parameters.loc["Nv", "brix"] = -π * (T / L) ** 2 * (1 / 2 + 2.4 * T / L)  # [Clarke]
 df_parameters.loc["Nr", "brix"] = (
     -π * (T / L) ** 2 * (1 / 4 + 0.039 * B / T - 0.56 * B / L)
```

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/substitute_dynamic_symbols.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/substitute_dynamic_symbols.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import sympy as sp
 import sympy.physics.mechanics as me
 from inspect import signature
 import pandas as pd
 from sympy.core.numbers import Float
 import numpy as np
+import inspect
+from numpy import pi,sqrt,cos,sin,tan,arctan,log,select,less_equal,nan,greater,sign,array
 
 
 def substitute_dynamic_symbols(expression):
     dynamic_symbols = me.find_dynamicsymbols(expression)
     derivatives = find_derivatives(dynamic_symbols)
 
     derivative_list = []
@@ -69,16 +71,22 @@
     symbol = derivative.expr
 
     name = "%s%id" % (symbol.name, order)
 
     return name
 
 
-def lambdify(expression):
+def lambdify(expression, substitute_functions=False):
     new_expression = substitute_dynamic_symbols(expression)
+
+    if substitute_functions:
+        ## Replace a all functions "X_D(u,v,r,delta)" with symbols "X_D" etc.
+        subs = get_function_subs(new_expression)
+        new_expression = new_expression.subs(subs)
+
     args = new_expression.free_symbols
 
     # Rearranging to get the parameters in alphabetical order:
     symbol_dict = {symbol.name: symbol for symbol in args}
     symbols = []
     for symbol_name in sorted(symbol_dict.keys()):
         symbols.append(symbol_dict[symbol_name])
@@ -107,14 +115,31 @@
     s = signature(function)
     kwargs.update(inputs)
     parameters = list(s.parameters.keys())
     args = [kwargs[parameter] for parameter in parameters]
     return function(*args)
 
 
+def get_function_subs(expression):
+    """Get a substitution dict to replace a all functions "X_D(u,v,r,delta)" with symbols "X_D" etc."""
+    if isinstance(expression, sp.Function) and hasattr(expression, "name"):
+        return {expression: expression.name}
+    elif isinstance(expression, sp.Derivative):
+        # d/du X_D(...)
+        # is simplified as "dduX_D":
+        simplified_symbol = f"dd{expression.args[1][0]}{expression.args[0].name}"
+        return {expression: simplified_symbol}
+    else:
+        subs = {}
+        for part in expression.args:
+            subs.update(get_function_subs(part))
+
+    return subs
+
+
 def significant(number, precision=3):
     """
     Get the number with significant figures
     Parameters
     ----------
     number
         Sympy Float
@@ -154,7 +179,50 @@
                 part, significant(part, precision=precision)
             )
         elif hasattr(part, "args"):
             new_part = _significant_numbers(part, precision=precision)
             new_expression = new_expression.subs(part, new_part)
 
     return new_expression
+
+def fix_function_for_pickle(eq):
+    
+    functions = [part for part in eq.rhs.args if isinstance(part,sp.Function)]
+    
+    for function in functions: 
+        function.__class__.__module__ = "__main__"  # Fix for pickle
+
+def expression_to_python_code(expression, function_name:str, substitute_functions=False):
+    lambda_ = lambdify(expression=expression, substitute_functions=substitute_functions)
+    lines = inspect.getsourcelines(lambda_)[0]
+    s = signature(lambda_)
+    parameters = list(s.parameters.keys())
+    str_parameters = ",".join(parameters)
+    if len(str_parameters)>1:
+        str_parameters+=","
+        
+    str_def = f"def {function_name}({str_parameters}**kwargs):\n"
+    str_import = "    from numpy import array \n"
+    code = str_def + str_import + "".join(lines[1:])
+    return code
+      
+def equation_to_python_code(eq, substitute_functions=False, name=None):
+    expression = eq.rhs
+    if name is None:
+        function_name = str(eq.lhs)
+    else:
+        function_name = name
+    
+    return expression_to_python_code(expression=expression, function_name=function_name, substitute_functions=substitute_functions)
+
+def expression_to_python_method(expression, function_name:str, substitute_functions=False):
+    exec(expression_to_python_code(expression=expression, function_name=function_name, substitute_functions=substitute_functions))
+    return locals()[function_name]
+
+def equation_to_python_method(eq, substitute_functions=False, name=None):  
+    expression = eq.rhs
+    if name is None:
+        function_name = str(eq.lhs)
+    else:
+        function_name = name
+    
+    return expression_to_python_method(expression=expression, function_name=function_name, substitute_functions=substitute_functions)
```

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/symbols.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/symbols.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 """Fossen, T., 2011. Nonlinear maneuvering theory and path-following control. Marine Technology and Engineering 1, 445–460.
 """
 M = sp.symbols("M")  # Inertia matrix
 
 C = sp.symbols("C")  # Coriolis matrix
 D = sp.symbols("D")  # Damping matrix
 
-
+cog = sp.symbols("cog")  # course over ground
 x0_, y0, z0, phi, theta, psi = sp.symbols("x0, y0, z0, phi, theta, psi")
 u, v, w, p, q, r = sp.symbols("u, v, w, p, q, r")
 u_c, v_c, w_c = sp.symbols("u_c, v_c, w_c")
 
 eta = sp.symbols("eta")  # Positions
 nu = sp.symbols("nu")  # Velocities
 nu1d = sp.symbols(r"\dot{\nu}")
@@ -94,21 +94,31 @@
 eq_nu_steady = sp.Eq(nu_r1d, nu1d)
 
 
 x_0, x_01d = sp.symbols("x_0 \dot{x_0}")
 y_0, y_01d = sp.symbols("y_0 \dot{y_0}")
 psi, psi1d = sp.symbols("\Psi \dot{\Psi}")
 
-u, v, r, delta, thrust = sp.symbols("u v r delta thrust")
+u, v, r, delta, thrust, torque = sp.symbols("u v r delta thrust torque")
 (
     u1d,
     v1d,
     r1d,
 ) = sp.symbols(r"\dot{u} \dot{v} \dot{r}")
+thrust_propeller, torque_propeller = sp.symbols(
+    "thrust_propeller torque_propeller"
+)  # thrust/torque of one propeller (thrust/torque is the total values of all propellers)
+thrust_port, thrust_stbd = sp.symbols(
+    "thrust_port,thrust_stbd"
+)  # Thrust of port and starboard propellers
+
+P_d = sp.symbols("P_d", real=True)  # Delivered propeller power
 
+n_prop = sp.symbols("n_prop")  # Number of propellers
+n_rudd = sp.symbols("n_rudd")  # Number of rudders
 
 m, x_G, U, I_z, volume = sp.symbols("m x_G U I_z volume")
 π = sp.pi
 T, L, CB, B, rho, t, dt = sp.symbols("T L CB B rho t dt")
 
 f_ext_x, f_ext_y, m_ext_z = sp.symbols("f_ext_x,f_ext_y,m_ext_z")  # external forces
 
@@ -116,14 +126,17 @@
 X_X, X_Y, X_N = sp.symbols("X_X X_Y X_N")  # State matrixes
 
 X_force, Y_force, N_force = sp.symbols("X_force Y_force N_force")  # Force models
 
 X_D = sp.Function("X_D")(u, v, r, delta, thrust)  # damping
 Y_D = sp.Function("Y_D")(u, v, r, delta, thrust)  # damping
 N_D = sp.Function("N_D")(u, v, r, delta, thrust)  # damping
+X_D_ = sp.symbols("X_D")
+Y_D_ = sp.symbols("Y_D")
+N_D_ = sp.symbols("N_D")
 for item in [X_D, Y_D, N_D]:
     item.__class__.__module__ = "__main__"  # Fix for pickle
 
 n, delta_t = sp.symbols("n delta_t")  # Time step n
 
 n = sp.symbols("n")  # Number of points
 N = sp.symbols("N")  # Numver of degrees of freedome
@@ -138,30 +151,40 @@
 X_n = sp.Function("X")(n)  # X features
 Y_n = sp.Function("Y")(n)  # X features
 N_n = sp.Function("N")(n)  # X features
 
 
 ## MMG model:
 x_r = sp.symbols("x_r")  # X pos of rudder
-x_p = sp.symbols("x_r")  # X pos of propeller
+x_p = sp.symbols("x_p")  # X pos of propeller
+y_p = sp.symbols("y_p")  # Y pos of propeller
+y_p_port = sp.symbols("y_p_port")  # Y pos of port propeller
+y_p_stbd = sp.symbols("y_p_stbd")  # Y pos of stbd propeller
 R0 = sp.symbols("R0")
 X_H = sp.symbols("X_H")  # Hull surge force
 Y_H = sp.symbols("Y_H")  # Hull sway force
 N_H = sp.symbols("N_H")  # Hull yaw moment
 X_R = sp.symbols("X_R")  # Rudder surge force
 Y_R = sp.symbols("Y_R")  # Rudder sway force
 N_R = sp.symbols("N_R")  # Rudder yaw moment
+X_RHI, Y_RHI, N_RHI = sp.symbols("X_RHI,Y_RHI,N_RHI")  # Rudder hull iteraction forces
 X_P = sp.symbols("X_P")  # Propeller surge force
+Y_P = sp.symbols("Y_P")  # Propeller sway force
+N_P = sp.symbols("N_P")  # Propeller yaw force
 tdf = sp.symbols("tdf")  # Thrust deduction factor
 rev = sp.symbols("rev")  # propeller speed [1/s]
 K_T = sp.symbols("K_T")
+K_Q = sp.symbols("K_Q")
 k_2, k_1, k_0 = sp.symbols("k_2, k_1, k_0")  # K_T coefficients.
+k_q2, k_q1, k_q0 = sp.symbols("k_q2, k_q1, k_q0")  # K_Q coefficients.
 J = sp.symbols("J")  # Propeller advance ratio
+η0 = sp.symbols("eta_0")  # Open water propeller efficiency
 w_p = sp.symbols("w_p")  # Wake at propeller (including drift angle etc.)
 w_p0 = sp.symbols("w_p0")  # Taylor wake at straight course.
+eta_r = sp.symbols("eta_r")  # Propeller rotatative efficiency
 C_1, C_2 = sp.symbols("C_1, C_2")
 beta_p = sp.symbols(
     "beta_p"
 )  # geometrical inflow angle to the propeller in maneuvering motions
 F_N = sp.symbols("F_N")  # Rudder normal force
 U_R, u_R, v_R = sp.symbols("U_R, u_R, v_R")  # Velocities at rudder
 alpha_R = sp.symbols("alpha_R")  # inflow angle?
@@ -178,14 +201,23 @@
     "a_H x_H"
 )  # coefficients representing mainly hydrodynamic interaction between ship hull and rudder
 Lambda = sp.symbols("Lambda")  # Rudder aspect ratio
 H_R, C_R = sp.symbols("H_R C_R")  # Rudder height and choord.
 eta = sp.symbols("eta")  # Ratio of propeller diameter to rudder span (D/H_R)
 C_Th = sp.symbols("C_Th")
 
+## Wind:
+awa = sp.symbols("awa", real=True)  # Aparent wind angle [rad]
+twa = sp.symbols("twa", real=True)  # True wind angle [rad]
+tws = sp.symbols("tws", real=True)  # True wind speed [m/s]
+
+aws, A_XV, A_YV, rho_A, X_W, Y_W, N_W = sp.symbols(
+    "aws, A_XV, A_YV, rho_A, X_W, Y_W, N_W", real=True
+)
+
 
 def glue_equations(module):
     # Glue equations
     from myst_nb import glue
 
     from sympy.physics.vector.printing import vlatex
     from IPython.display import Math
```

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/system_equations.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/system_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/twin_simulations.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/twin_simulations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/vct_scaling.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/vct_scaling.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/vmm_equations_VCT.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/vmm_equations_VCT.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/case_0.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/case_0.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/case_1.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/case_1.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/kalman_filter.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/make_dataset.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/make_dataset.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/mdl.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/mdl.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/wpcc.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/data/wpcc.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/MMG_hull.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/MMG_hull.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/MMG_propeller.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/MMG_propeller.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/MMG_rudder.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/MMG_rudder.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/brix_coefficients.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/brix_coefficients.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/captive_variation.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/captive_variation.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/diff_eq_to_matrix.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/diff_eq_to_matrix.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         when parameters are excluded they need to be moved to LHS. And they are divided by this parameter.
 
         """
 
         self.ode = ode
         assert isinstance(self.ode, sp.Eq)
 
+        assert label.name != "y", "label name 'y' is not allowed."
         self.label = label
         assert isinstance(self.label, sp.Expr)
 
         self.base_features = base_features
 
         self.exclude_parameters = pd.Series(exclude_parameters)
 
@@ -80,93 +81,96 @@
         self.parts = self.get_parts()
 
         # Express the diff eq. as a regression problem in matrix form:
         self.get_labels_and_features()
 
     @property
     def X_lambda(self):
-
         ## If there is a constant in the equation eq_X will have a 1 that cannot go into the X_lambda
         if 1 in self.eq_X.rhs:
             return lambdify(
-                sp.matrices.immutable.ImmutableDenseMatrix(self.eq_X.rhs[1:])
+                sp.matrices.immutable.ImmutableDenseMatrix(
+                    self.eq_X.rhs[1:]
+                )  # (1 is always the first feature)
             )
         else:
             return lambdify(self.eq_X.rhs)
 
     @property
     def y_lambda(self):
         p = df_parameters["symbol"]
         subs = {value: key for key, value in p.items()}
 
         return lambdify(self.eq_y.rhs.subs(subs))
 
     @property
     def acceleration_lambda(self):
-
         subs = self.feature_names_subs()
         return lambdify(sp.solve(self.acceleration_equation.subs(subs), self.label)[0])
 
     def feature_names_subs(self):
-
         ## Rename:
         columns_raw = list(self.eq_beta.rhs)
         subs = {}
 
         regexp = re.compile(r"\\dot{([^}])+}")
 
         def replacer(match):
             return r"%sdot" % match.group(1)
 
         for symbol in columns_raw:
-
             ascii_symbol = str(symbol)
             ascii_symbol = regexp.sub(repl=replacer, string=ascii_symbol)
             ascii_symbol = ascii_symbol.replace("_", "")
             ascii_symbol = ascii_symbol.replace("{", "")
             ascii_symbol = ascii_symbol.replace("}", "")
             ascii_symbol = ascii_symbol.replace("\\", "")
             ascii_symbol = ascii_symbol.replace("-", "")  # Little bit dangerous
             subs[symbol] = ascii_symbol
 
         return subs
 
-    def calculate_features(self, data: pd.DataFrame, simplify_names=True):
-
-        X = run(function=self.X_lambda, **data)
+    def calculate_features(
+        self, data: pd.DataFrame, parameters={}, simplify_names=True
+    ):
+        X = run(function=self.X_lambda, **data, **parameters)
 
         try:
             X = X.reshape(X.shape[1], X.shape[-1]).T
         except Exception:
             X = X.reshape(X.shape[0], X.shape[-1]).T
 
         # If there is a constant in the equation eq_X will have a 1 that needs to adde as the first column manually
         if 1 in self.eq_X.rhs:
             ones = np.ones(shape=(len(data), 1))
-            X = np.concatenate([ones, X], axis=1)
+            if len(X) > 0:
+                X = np.concatenate([ones, X], axis=1)
+            else:
+                X = ones  # only a constant in rhs
 
         subs = self.feature_names_subs()
         if simplify_names:
             columns = list(subs.values())
         else:
-            columns = list(subs.keys())
+            columns = [str(key) for key in subs.keys()]
 
         X = pd.DataFrame(data=X, index=data.index, columns=columns)
 
         return X
 
     def calculate_label(self, y: np.ndarray):
         return self.y_lambda(y)
 
     def calculate_features_and_label(
-        self, data: pd.DataFrame, y: np.ndarray, simplify_names=True
+        self, data: pd.DataFrame, y: np.ndarray, simplify_names=True, parameters={}
     ):
-
         y = y.copy()
-        X = self.calculate_features(data=data, simplify_names=simplify_names)
+        X = self.calculate_features(
+            data=data, simplify_names=simplify_names, parameters=parameters
+        )
         y = self.calculate_label(y=y)
 
         ## Exclude parameters:
         keep = list(set(X.columns) - set(self.exclude_parameters.keys()))
         exclude = list(set(X.columns) & set(self.exclude_parameters.keys()))
 
         if len(exclude) > 0:
@@ -213,62 +217,86 @@
         return self.acceleration_equation.rhs.subs(
             [(c, 1) for c in self.coefficients]
         ).args
 
     def get_labels_and_features(self):
         """Express the diff eq. as a regression problem in matrix form"""
 
-        self.xs = [sp.symbols(f"x_{i}") for i in range(1, len(self.parts) + 1)]
         self.y_ = sp.symbols("y")
-        self.X_ = sp.MatrixSymbol("X", 1, len(self.xs))
-        self.beta_ = sp.MatrixSymbol("beta", len(self.xs), 1)
 
-        subs = {part: x for part, x in zip(self.parts, self.xs)}
+        # Remove excluded parameters
+        equation = self.acceleration_equation.copy()
+        # if an excluded parameter appears twice... (Xthrust*thrust_port + X_thrust*thrust_stbd)
+        # excludes = {key: 0 for key in self.exclude_parameters}
+        # equation = equation.subs(excludes)
+
+        ## Extract the coefficients (based on the base features)
+        subs = [(feature, 1) for feature in self.base_features]
+        parts = equation.rhs.subs(subs)
+        if isinstance(parts, sp.Symbol):
+            coefficients = [parts]  # If there is only one coefficient
+        else:
+            coefficients = [coeff for coeff in parts.args]
+        check_coefficients(coefficients)
 
-        self.acceleration_equation_x = sp.Eq(
-            self.y_, self.acceleration_equation.rhs.subs(subs)
-        )
+        ## Find the feature expression that is associated with each coefficient,
+        # and put it in a list: columns
+        subs = {coeff: 0 for coeff in coefficients}
+        columns = []
+        for coeff in coefficients:
+            subs_mask = subs.copy()
+            subs_mask[coeff] = 1
+            columns.append(equation.rhs.subs(subs_mask))
+
+        if 1 in columns:
+            index = columns.index(1)  # Where is the 1? (The constant)
+            coefficient_1 = coefficients[index]
+
+            ordered_coefficients = coefficients.copy()
+            ordered_coefficients.remove(coefficient_1)
+            ordered_coefficients = [
+                coefficient_1
+            ] + ordered_coefficients  # Put the constant coefficient first
+
+            ordered_columns = columns.copy()
+            ordered_columns.remove(1)
+            ordered_columns = [1] + ordered_columns  # Put the constant feature first
+        else:
+            ordered_coefficients = coefficients
+            ordered_columns = columns
 
-        # Ex1:
-        # The following equation will be transfered to matrix form:
-        #  0 = c1*x1 + c2*x2
-        # Matrix form:
-        # b_ = A_*X
-        # Which means that:
-        # A_ = [c1,c2]
-        # b_ = 0
-
-        A_, b_ = sp.linear_eq_to_matrix([self.acceleration_equation_x.rhs], self.xs)
-
-        # if the equation contains a constant
-        # Ex2:
-        # The following equation will be transfered to matrix form:
-        #  0 = c0 + c1*x1 + c2*x2
-        # first moving the constant to LHS:
-        #  -c0 = c1*x1 + c2*x2
-        # Matrix form:
-        # b_ = A_*X
-        # Which means that:
-        # A_ = [0, c1,c2]
-        # b_ = -c0
-        # But we vant to keep c0 in the A_ matrix, so we replace the 0 with -b_:
-        if 0 in A_:
-            for i, a_ in enumerate(A_):
-                if a_ == 0:
-                    A_[i] = -b_[0]
-                    break
+        ## Feature matrix
+        self.X_matrix = sp.Matrix(ordered_columns).T
 
-        self.eq_beta = sp.Eq(self.beta_, A_.T)
+        ## Put this into some equations:
+        self.beta_ = sp.MatrixSymbol("beta", len(ordered_columns), 1)
+        self.eq_beta = sp.Eq(self.beta_, sp.Matrix(ordered_coefficients))
 
-        self.X_matrix = sp.Matrix(list(subs.keys())).T
+        self.X_ = sp.MatrixSymbol("X", 1, len(ordered_columns))
         self.eq_X = sp.Eq(self.X_, self.X_matrix)
 
         self.eq_y = sp.Eq(self.y_, self.label)
 
 
+def check_coefficients(coefficients: list):
+    for coeff in coefficients:
+        ok = True
+        if len(coeff.args) == 2:
+            if not isinstance(coeff.args[0], sp.core.numbers.Integer):
+                ok = False
+
+        elif len(coeff.args) > 2:
+            ok = False
+
+        if not ok:
+            raise AssertionError(
+                f"Cannot find pure coefficients (found: {coeff}), perhaps alter the base_features?"
+            )
+
+
 def get_coefficients(eq, base_features: list) -> list:
     """Get a list of hydrodynamic derivatives (coefficients) as sympy symbols.
 
     Args:
     eq : sympy equation
     base_features : list of from sympy.physics.mechanics.dynamicsymbols
     Ex: base_features = [u,v,r,delta,thrust]
@@ -287,12 +315,11 @@
         derivatives.append(base_feature)
         derivatives.append(sp.symbols(r"\dot{" + name + "}"))
         derivatives.append(sp.symbols(r"\ddot{" + name + "}"))
 
     subs = [(feature, 1) for feature in reversed(derivatives)]
 
     for part in eq.rhs.args:
-
         coeff = part.subs(subs)
         coefficients.append(coeff)
 
     return coefficients
```

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/force_from_motion.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/force_from_motion.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/nonlinear_vmm.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/nonlinear_vmm.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/regression.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/regression.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/result.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/result.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 from os import stat
 from sklearn.metrics import r2_score
 from vessel_manoeuvring_models.models.diff_eq_to_matrix import DiffEqToMatrix
 import sympy as sp
 from vessel_manoeuvring_models.symbols import *
 import matplotlib.ticker as plticker
 from sklearn.metrics import r2_score
+from vessel_manoeuvring_models.apparent_wind import (
+    true_wind_speed_to_apparent,
+    true_wind_angle_to_apparent,
+)
+from scipy.spatial.transform import Rotation as R
+from vessel_manoeuvring_models.angles import smallest_signed_angle
 
 
 class Result:
     def __init__(
         self,
         simulator,
         solution,
@@ -56,14 +62,24 @@
             pass
 
         try:
             df_result["U"] = np.sqrt(df_result["u"] ** 2 + df_result["v"] ** 2)
         except:
             pass
 
+        if "tws" in self.df_control and "twa" in self.df_control:
+            x01d = derivative(df_result, key="x0")
+            y01d = derivative(df_result, key="y0")
+            df_result["cog"] = np.arctan2(y01d, x01d)
+            df_result["aws"] = true_wind_speed_to_apparent(**df_result)
+            awa = true_wind_angle_to_apparent(**df_result)
+            df_result["awa"] = smallest_signed_angle(
+                awa - (awa.iloc[0] - smallest_signed_angle(awa.iloc[0]))
+            )
+
         return df_result
 
     @property
     def result(self):
         df_result = self.simulation_result
 
         if self.include_accelerations:
@@ -120,24 +136,27 @@
 
             u1d_prime, v1d_prime, r1d_prime = run(
                 function=self.simulator.acceleration_lambda,
                 X_qs=run(
                     function=self.simulator.X_qs_lambda,
                     **inputs,
                     **self.parameters,
+                    **self.ship_parameters,
                 ),
                 Y_qs=run(
                     function=self.simulator.Y_qs_lambda,
                     **inputs,
                     **self.parameters,
+                    **self.ship_parameters,
                 ),
                 N_qs=run(
                     function=self.simulator.N_qs_lambda,
                     **inputs,
                     **self.parameters,
+                    **self.ship_parameters,
                 ),
                 **inputs,
                 **self.parameters,
                 **self.simulator.ship_parameters_prime,
             )
 
             df_accelerations_prime = pd.DataFrame(index=df_result.index)
@@ -310,39 +329,49 @@
         self.plot_parameter_contributions()
 
     def simulate_parameter_contributions(self):
 
         model = self.simulator
         df_result_prime = model.prime_system.prime(self.result, U=self.result["U"])
 
+        base_features = [delta, u, v, r, aws, awa, thrust, A_XV, A_YV, rho_A, L]
         X_ = sp.symbols("X_")
         diff_eq_X = DiffEqToMatrix(
-            ode=model.X_qs_eq.subs(X_D, X_), label=X_, base_features=[delta, u, v, r]
+            ode=model.X_qs_eq.subs(X_D, X_),
+            label=X_,
+            base_features=base_features,
+        )
+        parameters = model.prime_system.prime(self.ship_parameters)
+        X = diff_eq_X.calculate_features(
+            data=df_result_prime,
+            parameters=parameters,
         )
-        X = diff_eq_X.calculate_features(data=df_result_prime)
         X_parameters = self.simulator.parameters[
             model.get_coefficients_X(sympy_symbols=False)
         ]
         X_forces = X * X_parameters
         X_forces.index = df_result_prime.index
 
         Y_ = sp.symbols("Y_")
         diff_eq_Y = DiffEqToMatrix(
-            ode=model.Y_qs_eq.subs(Y_D, Y_), label=Y_, base_features=[delta, u, v, r]
+            ode=model.Y_qs_eq.subs(Y_D, Y_), label=Y_, base_features=base_features
+        )
+        X = diff_eq_Y.calculate_features(
+            data=df_result_prime,
+            parameters=parameters,
         )
-        X = diff_eq_Y.calculate_features(data=df_result_prime)
         Y_parameters = model.parameters[model.get_coefficients_Y(sympy_symbols=False)]
         Y_forces = X * Y_parameters
         Y_forces.index = df_result_prime.index
 
         N_ = sp.symbols("N_")
         diff_eq_N = DiffEqToMatrix(
-            ode=model.N_qs_eq.subs(N_D, N_), label=N_, base_features=[delta, u, v, r]
+            ode=model.N_qs_eq.subs(N_D, N_), label=N_, base_features=base_features
         )
-        X = diff_eq_N.calculate_features(data=df_result_prime)
+        X = diff_eq_N.calculate_features(data=df_result_prime, parameters=parameters)
         N_parameters = model.parameters[model.get_coefficients_N(sympy_symbols=False)]
         N_forces = X * N_parameters
         N_forces.index = df_result_prime.index
 
         return X_forces, Y_forces, N_forces
 
     def plot_parameter_contributions(self, to_mlflow=True):
@@ -382,7 +411,13 @@
             if key in self.df_model_test:
 
                 r2s[key] = r2_score(
                     y_true=self.df_model_test[key], y_pred=self.result[key]
                 )
 
         return r2s
+
+
+def derivative(df, key):
+    d = np.diff(df[key]) / np.diff(df.index)
+    d = np.concatenate((d, [d[-1]]))
+    return d
```

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 import vessel_manoeuvring_models.models.diff_eq_to_matrix
 import dill
 from vessel_manoeuvring_models.models.result import Result
 from sklearn.utils import Bunch
 from copy import deepcopy
 from sympy.printing import pretty
 from vessel_manoeuvring_models.models.propeller import predictor
+from vessel_manoeuvring_models.apparent_wind import (
+    true_wind_speed_to_apparent,
+    true_wind_angle_to_apparent,
+)
+from vessel_manoeuvring_models.angles import smallest_signed_angle
 
 
 class VMM:
     """Vessel Manoeuvring Model
     Holding the equation of motions (EOM) and damping force equation for one model
     """
 
@@ -262,14 +267,15 @@
         Returns
         -------
         np.ndarray
             states derivatives for next time step
         """
 
         u, v, r, x0, y0, psi = states
+        V = np.sqrt(u**2 + v**2)
 
         states_dict = {
             "u": u,
             "v": v,
             "r": r,
             "x0": x0,
             "y0": y0,
@@ -281,33 +287,47 @@
         inputs.update(states_dict)
 
         if isinstance(control, pd.DataFrame):
             index = np.argmin(np.array(np.abs(control.index - t)))
             control_ = dict(control.iloc[index])
         else:
             control_ = control
+
+        rotation = R.from_euler("z", psi, degrees=False)
+        w = 0
+        velocities = rotation.apply([u, v, w])
+        x01d = velocities[0]
+        y01d = velocities[1]
+
+        if "tws" in control_ and "twa" in control_:
+            ## Calculate apparent wind:
+            cog = np.arctan2(y01d, x01d)
+            tws = control_.pop("tws")
+            twa = control_.pop("twa")
+            control_["aws"] = true_wind_speed_to_apparent(
+                U=V, cog=cog, twa=twa, tws=tws
+            )
+            control_["awa"] = smallest_signed_angle(
+                true_wind_angle_to_apparent(U=V, cog=cog, psi=psi, twa=twa, tws=tws)
+            )
+
         inputs.update(control_)
 
         inputs["U"] = U0  # initial velocity constant [1]
 
         inputs["X_qs"] = run(function=self.X_qs_lambda, **inputs)
         inputs["Y_qs"] = run(function=self.Y_qs_lambda, **inputs)
         inputs["N_qs"] = run(function=self.N_qs_lambda, **inputs)
         u1d, v1d, r1d = run(function=self.acceleration_lambda, **inputs)
 
         # get rid of brackets:
         u1d = u1d[0]
         v1d = v1d[0]
         r1d = r1d[0]
 
-        rotation = R.from_euler("z", psi, degrees=False)
-        w = 0
-        velocities = rotation.apply([u, v, w])
-        x01d = velocities[0]
-        y01d = velocities[1]
         psi1d = r
         dstates = [
             u1d,
             v1d,
             r1d,
             x01d,
             y01d,
@@ -524,15 +544,31 @@
             self._N_qs_lambda = lambdify(self.N_qs_eq.rhs.subs(subs))
 
         return self._N_qs_lambda
 
 
 def get_coefficients(eq, sympy_symbols=True):
     coefficients = vessel_manoeuvring_models.models.diff_eq_to_matrix.get_coefficients(
-        eq=eq, base_features=[u, v, r, delta, thrust]
+        eq=eq,
+        base_features=[
+            u,
+            v,
+            r,
+            delta,
+            thrust,
+            awa,
+            aws,
+            rho_A,
+            A_XV,
+            A_YV,
+            L,
+            # U,
+            # tws,
+            # twa,
+        ],
     )
     if sympy_symbols:
         return coefficients
     else:
         subs = {value: key for key, value in p.items()}
         string_coefficients = [subs[coefficient] for coefficient in coefficients]
         return string_coefficients
@@ -977,7 +1013,99 @@
             model_neg=self.model_neg,
             data=data,
             propeller_coefficients=self.propeller_coefficients,
             ship_data=self.ship_parameters,
         )
 
         return control
+
+
+class ModelSimulatorWithPropeller(ModelSimulator):
+    def __init__(
+        self,
+        simulator: Simulator,
+        parameters: dict,
+        ship_parameters: dict,
+        prime_system: PrimeSystem,
+        lambda_thrust,
+        control_keys: list = ["delta", "rev"],
+        name="simulation",
+        primed_parameters=True,
+        include_accelerations=True,
+    ):
+        """Generate a simulator that is specific to one ship with a specific set of parameters.
+        This is done by making a copy of an existing simulator object and add freezed parameters.
+
+        Parameters
+        ----------
+        simulator : Simulator
+            Simulator object with predefined odes
+        parameters : dict
+            [description]
+        ship_parameters : dict
+            [description]
+        control_keys : list
+            [description]
+        prime_system : PrimeSystem
+            [description]
+        lambda_thrust
+            method that calculates the thrust, based on current state and parameters
+        name : str, optional
+            [description], by default 'simulation'
+        primed_parameters : bool, optional
+            [description], by default True
+        """
+        super().__init__(
+            simulator=simulator,
+            parameters=parameters,
+            ship_parameters=ship_parameters,
+            control_keys=control_keys,
+            prime_system=prime_system,
+            name=name,
+            primed_parameters=primed_parameters,
+            include_accelerations=include_accelerations,
+        )
+        self.lambda_thrust = lambda_thrust
+
+    def control(self, t: float, states: np.ndarray, control: dict) -> dict:
+        """Controls, usually rudder angle and thrust
+        (Override this method if thrust should also be simulated)
+
+        Parameters
+        ----------
+        states : np.ndarray
+            _description_
+        control : dict
+            'delta' : rudder angle [rad]
+            'thrust': propeller thrust [N]
+
+        Returns
+        -------
+        dict
+            _description_
+        """
+
+        u, v, r, x0, y0, psi = states
+        index = np.argmin(np.array(np.abs(control.index - t)))
+        control_ = dict(control.iloc[index])
+
+        data = {
+            "u": u,
+            "v": v,
+            "r": r,
+            "x0": x0,
+            "y0": y0,
+            "psi": psi,
+            "delta": control_["delta"],
+            "rev": control_["rev"],
+        }
+        data["U"] = np.sqrt(data["u"] ** 2 + data["v"] ** 2)
+        data = pd.Series(data, dtype=float)
+
+        control["thrust"] = run(
+            function=self.lambda_thrust,
+            inputs=data,
+            **self.ship_parameters,
+            **self.parameters,
+        )
+
+        return control
```

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_MMG.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_MMG.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_abkowitz.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_abkowitz.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_abkowitz_expanded.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_abkowitz_expanded.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_abkowitz_no_thrust.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_abkowitz_no_thrust.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_air.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_air.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_gsi.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_gsi.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_linear.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_linear.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_mariner.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_mariner.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_martin.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_martin.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_martin_linear.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_martin_linear.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_martin_simple.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_martin_simple.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_nonlinear_EOM.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_nonlinear_EOM.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_perturbed.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_perturbed.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_simple.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_simple.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_simple_nonlinear.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vmm_simple_nonlinear.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vessels/mariner.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/models/vessels/mariner.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/book_format.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/visualization/book_format.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/equation.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/visualization/equation.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/plot.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/visualization/plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
 import plotly.express as px
+from copy import deepcopy
+import sympy as sp
 
 standard_styles = ["b", "r", "g", "m", "c", "y"]
 
 
 def plot(
     dataframes: dict,
     subplot=True,
@@ -13,16 +15,16 @@
     styles: list = None,
     keys: list = None,
     ncols=2,
     time_window=[0, np.inf],
     zero_origo=True,
     sort_keys=True,
     units={},
+    symbols={},
 ):
-
     if keys is None:
         keys = set()
         for label, df in dataframes.items():
             keys = keys | set(df.columns)
 
     if subplot:
         number_of_axes = len(keys)
@@ -37,28 +39,29 @@
     plot_kwargs = {}
 
     if isinstance(styles, list):
         plot_kwargs = {
             label: {"style": style} for label, style in zip(dataframes.keys(), styles)
         }
     elif isinstance(styles, dict):
-        plot_kwargs = styles
+        styles = styles.copy()
+        plot_kwargs = deepcopy(styles)
 
     standard_styles_ = standard_styles.copy()
     for key in dataframes.keys():
         if not key in plot_kwargs:
             plot_kwargs[key] = {}
 
-        if not "style" in plot_kwargs[key]:
-            if len(standard_styles_) > 1:
-                standard_style = standard_styles_.pop(0)
-            else:
-                standard_style = standard_styles_[0]
-
-            plot_kwargs[key]["style"] = standard_style
+        # if not "style" in plot_kwargs[key]:
+        #    if len(standard_styles_) > 1:
+        #        standard_style = standard_styles_.pop(0)
+        #    else:
+        #        standard_style = standard_styles_[0]
+        #
+        #    plot_kwargs[key]["style"] = standard_style
 
         if not "label" in plot_kwargs[key]:
             plot_kwargs[key]["label"] = key
 
     if sort_keys:
         iteration_keys = sorted(keys)
     else:
@@ -66,43 +69,65 @@
 
     for i, key in enumerate(iteration_keys):
         if subplot:
             ax = axes[i]
         else:
             fig, ax = plt.subplots()
 
-        for label, df in dataframes.items():
+        unit = units.get(key, "")
 
+        for label, df in dataframes.items():
             plot_kwarg = plot_kwargs.get(label, {})
 
             if key in df:
                 mask = (df.index >= time_window[0]) & (df.index <= time_window[1])
-                df.loc[mask].plot(y=key, ax=ax, **plot_kwarg)
+                df_ = df.loc[mask]
+                x = df_.index
+
+                if unit == "rad":
+                    y = np.rad2deg(df_[key])
+                else:
+                    y = df_[key]
+
+                if "style" in plot_kwarg:
+                    _plot_kwarg = plot_kwarg.copy()
+                    style = _plot_kwarg.pop("style")
+                    ax.plot(x, y, style, **_plot_kwarg)
+                else:
+                    ax.plot(x, y, **plot_kwarg)
 
         ax.grid(True)
 
         if zero_origo:
             ylims = ax.get_ylim()
             ax.set_ylim(min(0, ylims[0]), max(0, ylims[1]))
 
         legend = ax.get_legend()
         if legend:
             legend.set_visible(False)
 
-        y_label = f"{key} $[{units[key]}]$" if key in units else key
+        symbol = symbols.get(key, key)
+        if isinstance(symbol, sp.Symbol):
+            symbol = sp.latex(symbol)
+        if unit == "rad":
+            unit = "deg"
+        y_label = f"${symbol}$ [{unit}]" if unit != "" else f"${symbol}$"
         ax.set_ylabel(y_label)
 
     lines = [len(ax.lines) for ax in axes]
     i = np.argmax(lines)
     axes[i].legend()
 
-    for ax in fig.axes[0:-1]:
+    for ax in fig.axes[0:-ncols]:
         ax.set_xticklabels([])
         ax.set_xlabel("")
 
+    for ax in fig.axes[-ncols:]:
+        ax.set_xlabel("Time [s]")
+
     plt.tight_layout()
     return fig
 
 
 def track_plots(
     dataframes: dict,
     lpp: float,
@@ -113,33 +138,32 @@
     y_dataset="y0",
     psi_dataset="psi",
     plot_boats=True,
     styles: dict = {},
     flip=False,
     time_window=[0, np.inf],
 ) -> plt.axes:
+    styles = styles.copy()
 
     if ax is None:
         fig, ax = plt.subplots()
 
-    standard_styles_ = standard_styles.copy()
+    # standard_styles_ = standard_styles.copy()
     for label, df in dataframes.items():
-
         if label in styles:
             style = styles[label]
 
         else:
-
-            if len(standard_styles_) > 1:
-                standard_style = standard_styles_.pop(0)
-            else:
-                standard_style = standard_styles_[0]
-
+            #    if len(standard_styles_) > 1:
+            #        standard_style = standard_styles_.pop(0)
+            #    else:
+            #        standard_style = standard_styles_[0]
+            #
             style = {}
-            style["style"] = standard_style
+        #    style["style"] = standard_style
 
         if not "label" in style:
             style["label"] = label
 
         track_plot(
             df=df,
             lpp=lpp,
@@ -171,15 +195,14 @@
     flip=False,
     time_window=[0, np.inf],
     start_color="g",
     stop_color="r",
     outline=False,
     **plot_kwargs,
 ):
-
     if ax is None:
         fig, ax = plt.subplots()
 
     mask = (df.index >= time_window[0]) & (df.index <= time_window[1])
     df = df.loc[mask].copy()
 
     if flip:
@@ -272,29 +295,32 @@
             ax=ax,
             color=color,
             alpha=alpha * alpha_,
             outline=outline,
         )
 
 
-def plot_ship(x, y, psi, ax, lpp, beam, color="y", alpha=0.1, outline=False):
+def plot_ship(x, y, psi, ax, lpp, beam, color="y", alpha=0.1, outline=False, **kwargs):
     """Plot a simplified contour od this ship"""
     recalculated_boat = get_countour(x, y, psi, lpp=lpp, beam=beam)
     x = recalculated_boat[1]
     y = recalculated_boat[0]
 
+    if not "zorder" in kwargs:
+        kwargs["zorder"] = 10
+
     if outline:
         outline_color = "k"
         outline_alpha = 1
-        ax.plot(x, y, outline_color, alpha=outline_alpha, zorder=10)
+        ax.plot(x, y, outline_color, alpha=outline_alpha, **kwargs)
     else:
         outline_color = color
         outline_alpha = alpha
-        ax.plot(x, y, outline_color, alpha=outline_alpha, zorder=10)
-        ax.fill(x, y, color, zorder=10, alpha=alpha)
+        ax.plot(x, y, outline_color, alpha=outline_alpha, **kwargs)
+        ax.fill(x, y, color, alpha=alpha, **kwargs)
 
 
 def get_countour(x, y, psi, lpp, beam):
     # (Old Matlab boat.m)
     tt1 = lpp / 2
     tt2 = 0.9
     tt3 = beam / 4
@@ -351,15 +377,14 @@
     df_captive: pd.DataFrame,
     dofs=["fx", "fy", "mz"],
     styles=["-", ".", "o"],
     right=0.80,
     add_legend=True,
     **kwargs,
 ):
-
     df_captive = df_captive.copy()
     df_captive["v*r"] = df_captive["v"] * df_captive["r"]
     df_captive["beta"] = -np.arctan2(df_captive["v"], df_captive["u"])
 
     colors = ["r", "g", "b"]
     color_map = {}
     for V in df_captive["V"].unique():
@@ -367,20 +392,18 @@
             color = colors.pop(0)
         else:
             color = colors[0]
 
         color_map[V] = color
 
     for test_type, df_ in df_captive.groupby(by="test type"):
-
         by_label = {}
         fig, axes = plt.subplots(ncols=len(dofs))
 
         for dof, ax in zip(dofs, axes):
-
             x_key = test_type_xplot.get(test_type, "V")
 
             if x_key == "u":
                 plot_V(
                     df_=df_,
                     x_key=x_key,
                     styles=styles,
@@ -416,17 +439,15 @@
             fig.tight_layout()
             fig.subplots_adjust(right=right)
         else:
             fig.tight_layout()
 
 
 def plot_V(df_, x_key, styles, ax, dof, color, **kwargs):
-
     for i, (item, df_item) in enumerate(df_.groupby(by="item")):
-
         if i < len(styles):
             style = styles[i]
         else:
             style = styles[-1]
 
         style += color
         df_item.sort_values(by=x_key).plot(
@@ -465,15 +486,14 @@
     fig, axes = plt.subplots(nrows=N)
     if N == 1:
         axes = [axes]
 
     # fig.set_size_inches(size_inches[0], N * size_inches[1])
 
     for i, ax in zip(range(N), axes):
-
         cut_start = cuts[i + 1]
         cut_stop = cuts[i]
 
         mask = (
             parameters["mean"].abs() > parameters["mean"].abs().quantile(cut_start)
         ) & (parameters["mean"].abs() <= parameters["mean"].abs().quantile(cut_stop))
 
@@ -482,36 +502,33 @@
     plt.tight_layout()
     return fig
 
 
 def parameter_contributions(
     data_prime: pd.DataFrame, diff_eq, parameters: dict
 ) -> pd.DataFrame:
-
     X = diff_eq.calculate_features(data_prime)
     parameters = pd.Series(parameters)
     mask = parameters != 0
     parameters = parameters[mask].copy()
     keys = list(set(X.columns) & set(parameters.keys()))
     forces = X.multiply(parameters[keys]).dropna(how="all", axis=1)
 
     return forces
 
 
 def plot_parameter_contributions(data: pd.DataFrame, model, regression):
-
     diff_eqs = {
         "X": regression.diff_eq_X,
         "Y": regression.diff_eq_Y,
         "N": regression.diff_eq_N,
     }
 
     parameters = model.parameters
     data_prime = model.prime_system.prime(data, U=data["U"])
 
     for dof, diff_eq in diff_eqs.items():
-
         forces = parameter_contributions(
             data_prime=data_prime, diff_eq=diff_eq, parameters=parameters
         )
         fig = px.line(forces, y=forces.columns, width=800, height=350, title=dof)
         display(fig)
```

### Comparing `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/regression.py` & `vessel_manoeuvring_models-0.0.7/vessel_manoeuvring_models/visualization/regression.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/LICENSE` & `vessel_manoeuvring_models-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.6/pyproject.toml` & `vessel_manoeuvring_models-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 description = "System identification of ship manoeuvring models"
 name = "vessel_manoeuvring_models"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.0.6"
+version = "0.0.7"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/martinlarsalbert/VesselManoeuvringModels/issues"
 "Homepage" = "https://github.com/martinlarsalbert/VesselManoeuvringModels"
 
 [build-system]
 build-backend = "hatchling.build"
```

### Comparing `vessel_manoeuvring_models-0.0.6/PKG-INFO` & `vessel_manoeuvring_models-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vessel_manoeuvring_models
-Version: 0.0.6
+Version: 0.0.7
 Summary: System identification of ship manoeuvring models
 Project-URL: Bug Tracker, https://github.com/martinlarsalbert/VesselManoeuvringModels/issues
 Project-URL: Homepage, https://github.com/martinlarsalbert/VesselManoeuvringModels
 Author-email: Martin Alexandersson <maralex@chalmers.se>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

