# Comparing `tmp/edwh_auth_rbac-0.3.0.tar.gz` & `tmp/edwh_auth_rbac-0.4.0.tar.gz`

## Comparing `edwh_auth_rbac-0.3.0.tar` & `edwh_auth_rbac-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/.gitignore
--rw-r--r--   0        0        0     9928 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/class_index.html
--rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/coverage_html_cb_da166b87.js
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/favicon_32_cb_58284776.png
--rw-r--r--   0        0        0    36693 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/function_index.html
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/keybd_closed_cb_ce680311.png
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/status.json
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/style_cb_8e611ae1.css
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6___init___py.html
--rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_helpers_py.html
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_migrations_py.html
--rw-r--r--   0        0        0   109622 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_model_py.html
--rw-r--r--   0        0        0    61317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_rbac_py.html
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0    59418 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/helpers.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/migrations.py
--rw-r--r--   0        0        0    14401 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/model.py
--rw-r--r--   0        0        0     8098 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/rbac.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/tests/test_migrate.py
--rw-r--r--   0        0        0     7778 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/tests/test_rbac.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/.gitignore
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/README.md
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/class_index.html
+-rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/coverage_html_cb_da166b87.js
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/favicon_32_cb_58284776.png
+-rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/function_index.html
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/keybd_closed_cb_ce680311.png
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/status.json
+-rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/style_cb_8e611ae1.css
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6___init___py.html
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_helpers_py.html
+-rw-r--r--   0        0        0    15181 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_migrations_py.html
+-rw-r--r--   0        0        0   123833 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_model_py.html
+-rw-r--r--   0        0        0    61606 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_rbac_py.html
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    60186 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/helpers.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/migrations.py
+-rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/model.py
+-rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/rbac.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/tests/test_migrate.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/tests/test_rbac.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/.gitignore
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/README.md
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/PKG-INFO
```

### Comparing `edwh_auth_rbac-0.3.0/CHANGELOG.md` & `edwh_auth_rbac-0.4.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.0 (2024-05-30)
+
+### Feature
+
+* Support BYOG (bring your own gid) for all relevant add_ functions (item, group, user; not membership, permission) ([`aeb06d9`](https://github.com/educationwarehouse/edwh-auth-rbac/commit/aeb06d9ad7ba385c57fbc6836da878bd1775ae49))
+
 ## v0.3.0 (2024-05-29)
 
 ### Feature
 
 * Allow '*' privileges ([`2980fe1`](https://github.com/educationwarehouse/edwh-auth-rbac/commit/2980fe17038b456d7a101a4486499e3bd3e7a61b))
 
 ## v0.2.7 (2024-05-29)
```

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/class_index.html` & `edwh_auth_rbac-0.4.0/htmlcov/class_index.html`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
     <script src="coverage_html_cb_da166b87.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">82%</span>
+            <span class="pc_cov">84%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
@@ -51,15 +51,15 @@
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button current">Classes</a>
         </h2>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -93,44 +93,60 @@
                 <td class="name left"><a href="z_438b44bce6437be6_migrations_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
                 <td>3</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="3 3">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t15">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t15"><data value='DEFAULT'>DEFAULT</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t17">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t17"><data value='DEFAULT'>DEFAULT</data></a></td>
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t28">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t28"><data value='Password'>Password</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t30">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t30"><data value='Password'>Password</data></a></td>
                 <td>9</td>
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="7 9">78%</td>
             </tr>
             <tr class="region">
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t100">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t100"><data value='RbacKwargs'>RbacKwargs</data></a></td>
+                <td>0</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="0 0">100%</td>
+            </tr>
+            <tr class="region">
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t105">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t105"><data value='Identity'>Identity</data></a></td>
+                <td>0</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="0 0">100%</td>
+            </tr>
+            <tr class="region">
                 <td class="name left"><a href="z_438b44bce6437be6_model_py.html">src/edwh_auth_rbac/model.py</a></td>
                 <td class="name left"><a href="z_438b44bce6437be6_model_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
-                <td>42</td>
+                <td>57</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="42 42">100%</td>
+                <td class="right" data-ratio="57 57">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t11">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t11"><data value='AuthRbac'>AuthRbac</data></a></td>
-                <td>63</td>
-                <td>39</td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t19">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t19"><data value='AuthRbac'>AuthRbac</data></a></td>
+                <td>61</td>
+                <td>37</td>
                 <td>0</td>
-                <td class="right" data-ratio="24 63">38%</td>
+                <td class="right" data-ratio="24 61">39%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html">src/edwh_auth_rbac/rbac.py</a></td>
                 <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
                 <td>25</td>
                 <td>0</td>
                 <td>0</td>
@@ -143,22 +159,22 @@
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t24">tests/test_rbac.py</a></td>
                 <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t24"><data value='Database'>database.Database</data></a></td>
-                <td>5</td>
+                <td>6</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="5 5">100%</td>
+                <td class="right" data-ratio="6 6">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t51">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t51"><data value='TestSequentially'>TestSequentially</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t53">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t53"><data value='TestSequentially'>TestSequentially</data></a></td>
                 <td>57</td>
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="55 57">96%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html">tests/test_rbac.py</a></td>
@@ -169,30 +185,30 @@
                 <td class="right" data-ratio="33 33">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>241</td>
-                <td>43</td>
+                <td>255</td>
+                <td>41</td>
                 <td>0</td>
-                <td class="right" data-ratio="198 241">82%</td>
+                <td class="right" data-ratio="214 255">84%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,34 +1,38 @@
-************ CCoovveerraaggee rreeppoorrtt:: 8822%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 8844%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-16 17:13 +0200
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-22 15:42 +0200
 FFiillee                ccllaassss             ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/ _(_n_o_ _c_l_a_s_s_)        3          0       0        100%
 _____i_n_i_t_____._p_y
 _s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/ _(_n_o_ _c_l_a_s_s_)        1          0       0        100%
 _h_e_l_p_e_r_s_._p_y
 _s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/ _(_n_o_ _c_l_a_s_s_)        3          0       0        100%
 _m_i_g_r_a_t_i_o_n_s_._p_y
 _s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/ _D_E_F_A_U_L_T           0          0       0        100%
 _m_o_d_e_l_._p_y
 _s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/ _P_a_s_s_w_o_r_d          9          2       0        78%
 _m_o_d_e_l_._p_y
-_s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/ _(_n_o_ _c_l_a_s_s_)        42         0       0        100%
+_s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/ _R_b_a_c_K_w_a_r_g_s        0          0       0        100%
 _m_o_d_e_l_._p_y
-_s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/ _A_u_t_h_R_b_a_c          63         39      0        38%
+_s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/ _I_d_e_n_t_i_t_y          0          0       0        100%
+_m_o_d_e_l_._p_y
+_s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/ _(_n_o_ _c_l_a_s_s_)        57         0       0        100%
+_m_o_d_e_l_._p_y
+_s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/ _A_u_t_h_R_b_a_c          61         37      0        39%
 _r_b_a_c_._p_y
 _s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/ _(_n_o_ _c_l_a_s_s_)        25         0       0        100%
 _r_b_a_c_._p_y
 _t_e_s_t_s_/_____i_n_i_t_____._p_y   _(_n_o_ _c_l_a_s_s_)        0          0       0        100%
-_t_e_s_t_s_/_t_e_s_t___r_b_a_c_._p_y  _d_a_t_a_b_a_s_e_._D_a_t_a_b_a_s_e 5          0       0        100%
+_t_e_s_t_s_/_t_e_s_t___r_b_a_c_._p_y  _d_a_t_a_b_a_s_e_._D_a_t_a_b_a_s_e 6          0       0        100%
 _t_e_s_t_s_/_t_e_s_t___r_b_a_c_._p_y  _T_e_s_t_S_e_q_u_e_n_t_i_a_l_l_y  57         2       0        96%
 _t_e_s_t_s_/_t_e_s_t___r_b_a_c_._p_y  _(_n_o_ _c_l_a_s_s_)        33         0       0        100%
-Total                                 241        43      0        82%
+Total                                 255        41      0        84%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-16 17:13 +0200
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-22 15:42 +0200
```

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/coverage_html_cb_da166b87.js` & `edwh_auth_rbac-0.4.0/htmlcov/coverage_html_cb_da166b87.js`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/favicon_32_cb_58284776.png` & `edwh_auth_rbac-0.4.0/htmlcov/favicon_32_cb_58284776.png`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/function_index.html` & `edwh_auth_rbac-0.4.0/htmlcov/function_index.html`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
     <script src="coverage_html_cb_da166b87.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">78%</span>
+            <span class="pc_cov">80%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
@@ -51,15 +51,15 @@
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -117,328 +117,328 @@
                 <td class="name left"><a href="z_438b44bce6437be6_migrations_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
                 <td>3</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="3 3">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t23">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t23"><data value='unstr_datetime'>unstr_datetime</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t25">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t25"><data value='unstr_datetime'>unstr_datetime</data></a></td>
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t34">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t34"><data value='hmac_hash'>Password.hmac_hash</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t36">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t36"><data value='hmac_hash'>Password.hmac_hash</data></a></td>
                 <td>5</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="5 5">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t42">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t42"><data value='validate'>Password.validate</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t44">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t44"><data value='validate'>Password.validate</data></a></td>
                 <td>2</td>
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 2">0%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t47">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t47"><data value='encode'>Password.encode</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t49">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t49"><data value='encode'>Password.encode</data></a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t52">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t52"><data value='is_uuid'>is_uuid</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t54">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t54"><data value='is_uuid'>is_uuid</data></a></td>
                 <td>5</td>
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="3 5">60%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t60">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t60"><data value='key_lookup_query'>key_lookup_query</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t66">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t66"><data value='key_lookup_query'>key_lookup_query</data></a></td>
                 <td>10</td>
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="8 10">80%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t76">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t76"><data value='key_lookup'>key_lookup</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t82">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t82"><data value='key_lookup'>key_lookup</data></a></td>
                 <td>7</td>
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="5 7">71%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t95">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t95"><data value='define_auth_rbac_model'>define_auth_rbac_model</data></a></td>
-                <td>5</td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t115">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t115"><data value='define_auth_rbac_model'>define_auth_rbac_model</data></a></td>
+                <td>6</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="5 5">100%</td>
+                <td class="right" data-ratio="6 6">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t151">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t151"><data value='add_identity'>add_identity</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t181">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t181"><data value='add_identity'>add_identity</data></a></td>
                 <td>12</td>
                 <td>4</td>
                 <td>0</td>
                 <td class="right" data-ratio="8 12">67%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t175">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t175"><data value='add_group'>add_group</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t215">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t215"><data value='add_group'>add_group</data></a></td>
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t179">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t179"><data value='remove_identity'>remove_identity</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t219">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t219"><data value='remove_identity'>remove_identity</data></a></td>
                 <td>3</td>
                 <td>3</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 3">0%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t186">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t186"><data value='get_identity'>get_identity</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t226">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t226"><data value='get_identity'>get_identity</data></a></td>
                 <td>3</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="3 3">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t197">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t197"><data value='get_user'>get_user</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t237">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t237"><data value='get_user'>get_user</data></a></td>
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t206">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t206"><data value='get_group'>get_group</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t246">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t246"><data value='get_group'>get_group</data></a></td>
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t216">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t216"><data value='authenticate_user'>authenticate_user</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t256">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t256"><data value='authenticate_user'>authenticate_user</data></a></td>
                 <td>5</td>
                 <td>5</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 5">0%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t224">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t224"><data value='add_membership'>add_membership</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t264">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t264"><data value='add_membership'>add_membership</data></a></td>
                 <td>11</td>
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="9 11">82%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t241">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t241"><data value='remove_membership'>remove_membership</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t281">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t281"><data value='remove_membership'>remove_membership</data></a></td>
                 <td>7</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="7 7">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t251">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t251"><data value='get_memberships'>get_memberships</data></a></td>
-                <td>5</td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t291">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t291"><data value='get_memberships'>get_memberships</data></a></td>
+                <td>3</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="5 5">100%</td>
+                <td class="right" data-ratio="3 3">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t259">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t259"><data value='get_members'>get_members</data></a></td>
-                <td>5</td>
-                <td>5</td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t297">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t297"><data value='get_members'>get_members</data></a></td>
+                <td>3</td>
+                <td>3</td>
                 <td>0</td>
-                <td class="right" data-ratio="0 5">0%</td>
+                <td class="right" data-ratio="0 3">0%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t267">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t267"><data value='add_permission'>add_permission</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t303">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t303"><data value='add_permission'>add_permission</data></a></td>
                 <td>8</td>
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="6 8">75%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t288">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t288"><data value='remove_permission'>remove_permission</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t333">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t333"><data value='remove_permission'>remove_permission</data></a></td>
                 <td>13</td>
                 <td>13</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 13">0%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t307">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t307"><data value='with_alias'>with_alias</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t354">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t354"><data value='with_alias'>with_alias</data></a></td>
                 <td>13</td>
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="11 13">85%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t324">src/edwh_auth_rbac/model.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t324"><data value='has_permission'>has_permission</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t371">src/edwh_auth_rbac/model.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_model_py.html#t371"><data value='has_permission'>has_permission</data></a></td>
                 <td>16</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="16 16">100%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="z_438b44bce6437be6_model_py.html">src/edwh_auth_rbac/model.py</a></td>
                 <td class="name left"><a href="z_438b44bce6437be6_model_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
-                <td>42</td>
+                <td>57</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="42 42">100%</td>
+                <td class="right" data-ratio="57 57">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t14">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t14"><data value='init__'>AuthRbac.__init__</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t22">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t22"><data value='init__'>AuthRbac.__init__</data></a></td>
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t18">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t18"><data value='error'>AuthRbac._error</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t26">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t26"><data value='error'>AuthRbac._error</data></a></td>
                 <td>1</td>
                 <td>1</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 1">0%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t23">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t23"><data value='add_user'>AuthRbac.add_user</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t31">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t31"><data value='add_user'>AuthRbac.add_user</data></a></td>
                 <td>7</td>
                 <td>1</td>
                 <td>0</td>
                 <td class="right" data-ratio="6 7">86%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t40">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t40"><data value='add_item'>AuthRbac.add_item</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t49">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t49"><data value='add_item'>AuthRbac.add_item</data></a></td>
                 <td>7</td>
                 <td>7</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 7">0%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t55">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t55"><data value='add_identity'>AuthRbac.add_identity</data></a></td>
-                <td>9</td>
-                <td>9</td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t60">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t60"><data value='add_identity'>AuthRbac.add_identity</data></a></td>
+                <td>7</td>
+                <td>7</td>
                 <td>0</td>
-                <td class="right" data-ratio="0 9">0%</td>
+                <td class="right" data-ratio="0 7">0%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t72">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t72"><data value='add_group'>AuthRbac.add_group</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t73">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t73"><data value='add_group'>AuthRbac.add_group</data></a></td>
                 <td>7</td>
                 <td>1</td>
                 <td>0</td>
                 <td class="right" data-ratio="6 7">86%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t87">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t87"><data value='update_identity'>AuthRbac.update_identity</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t84">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t84"><data value='update_identity'>AuthRbac.update_identity</data></a></td>
                 <td>3</td>
                 <td>3</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 3">0%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t99">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t99"><data value='get_user'>AuthRbac.get_user</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t97">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t97"><data value='get_user'>AuthRbac.get_user</data></a></td>
                 <td>5</td>
                 <td>5</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 5">0%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t117">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t117"><data value='get_group'>AuthRbac.get_group</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t118">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t118"><data value='get_group'>AuthRbac.get_group</data></a></td>
                 <td>9</td>
                 <td>9</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 9">0%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t141">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t141"><data value='authenticate_user'>AuthRbac.authenticate_user</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t138">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t138"><data value='authenticate_user'>AuthRbac.authenticate_user</data></a></td>
                 <td>1</td>
                 <td>1</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 1">0%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t144">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t144"><data value='add_membership'>AuthRbac.add_membership</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t141">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t141"><data value='add_membership'>AuthRbac.add_membership</data></a></td>
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t147">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t147"><data value='remove_membership'>AuthRbac.remove_membership</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t144">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t144"><data value='remove_membership'>AuthRbac.remove_membership</data></a></td>
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t150">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t150"><data value='has_membership'>AuthRbac.has_membership</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t147">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t147"><data value='has_membership'>AuthRbac.has_membership</data></a></td>
                 <td>4</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="4 4">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t156">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t156"><data value='add_permission'>AuthRbac.add_permission</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t153">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t153"><data value='add_permission'>AuthRbac.add_permission</data></a></td>
                 <td>3</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="3 3">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t161">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t161"><data value='has_permission'>AuthRbac.has_permission</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t158">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t158"><data value='has_permission'>AuthRbac.has_permission</data></a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t165">src/edwh_auth_rbac/rbac.py</a></td>
-                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t165"><data value='remove_permission'>AuthRbac.remove_permission</data></a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t162">src/edwh_auth_rbac/rbac.py</a></td>
+                <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html#t162"><data value='remove_permission'>AuthRbac.remove_permission</data></a></td>
                 <td>2</td>
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 2">0%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html">src/edwh_auth_rbac/rbac.py</a></td>
@@ -471,150 +471,150 @@
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="4 4">100%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t25">tests/test_rbac.py</a></td>
                 <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t25"><data value='enter__'>database.Database.__enter__</data></a></td>
-                <td>4</td>
+                <td>5</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="4 4">100%</td>
+                <td class="right" data-ratio="5 5">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t32">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t32"><data value='exit__'>database.Database.__exit__</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t34">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t34"><data value='exit__'>database.Database.__exit__</data></a></td>
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t39">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t39"><data value='rbac'>rbac</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t41">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t41"><data value='rbac'>rbac</data></a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t45">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t45"><data value='store'>store</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t47">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t47"><data value='store'>store</data></a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t52">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t52"><data value='test_drop_all_test_users'>TestSequentially.test_drop_all_test_users</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t54">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t54"><data value='test_drop_all_test_users'>TestSequentially.test_drop_all_test_users</data></a></td>
                 <td>8</td>
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="6 8">75%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t63">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t63"><data value='test_user_creation'>TestSequentially.test_user_creation</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t67">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t67"><data value='test_user_creation'>TestSequentially.test_user_creation</data></a></td>
                 <td>3</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="3 3">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t68">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t68"><data value='test_group_creation'>TestSequentially.test_group_creation</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t72">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t72"><data value='test_group_creation'>TestSequentially.test_group_creation</data></a></td>
                 <td>4</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="4 4">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t74">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t74"><data value='test_item_creation'>TestSequentially.test_item_creation</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t78">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t78"><data value='test_item_creation'>TestSequentially.test_item_creation</data></a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t79">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t79"><data value='test_stash_users_in_groups'>TestSequentially.test_stash_users_in_groups</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t82">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t82"><data value='test_stash_users_in_groups'>TestSequentially.test_stash_users_in_groups</data></a></td>
                 <td>5</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="5 5">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t86">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t86"><data value='test_stash_items_in_groups'>TestSequentially.test_stash_items_in_groups</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t89">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t89"><data value='test_stash_items_in_groups'>TestSequentially.test_stash_items_in_groups</data></a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t90">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t90"><data value='test_add_some_permissions'>TestSequentially.test_add_some_permissions</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t93">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t93"><data value='test_add_some_permissions'>TestSequentially.test_add_some_permissions</data></a></td>
                 <td>3</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="3 3">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t95">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t95"><data value='test_first_level_memberships'>TestSequentially.test_first_level_memberships</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t98">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t98"><data value='test_first_level_memberships'>TestSequentially.test_first_level_memberships</data></a></td>
                 <td>4</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="4 4">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t101">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t101"><data value='test_second_level_memberships'>TestSequentially.test_second_level_memberships</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t104">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t104"><data value='test_second_level_memberships'>TestSequentially.test_second_level_memberships</data></a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t105">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t105"><data value='test_first_level_permissions'>TestSequentially.test_first_level_permissions</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t108">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t108"><data value='test_first_level_permissions'>TestSequentially.test_first_level_permissions</data></a></td>
                 <td>4</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="4 4">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t111">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t111"><data value='test_second_to_first_level_permissions'>TestSequentially.test_second_to_first_level_permissions</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t114">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t114"><data value='test_second_to_first_level_permissions'>TestSequentially.test_second_to_first_level_permissions</data></a></td>
                 <td>4</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="4 4">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t117">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t117"><data value='test_second_to_second_level_permissions'>TestSequentially.test_second_to_second_level_permissions</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t120">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t120"><data value='test_second_to_second_level_permissions'>TestSequentially.test_second_to_second_level_permissions</data></a></td>
                 <td>4</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="4 4">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t123">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t123"><data value='test_deeper_group_nesting'>TestSequentially.test_deeper_group_nesting</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t126">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t126"><data value='test_deeper_group_nesting'>TestSequentially.test_deeper_group_nesting</data></a></td>
                 <td>10</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="10 10">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t136">tests/test_rbac.py</a></td>
-                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t136"><data value='test_removing_a_nested_group'>TestSequentially.test_removing_a_nested_group</data></a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t140">tests/test_rbac.py</a></td>
+                <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html#t140"><data value='test_removing_a_nested_group'>TestSequentially.test_removing_a_nested_group</data></a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html">tests/test_rbac.py</a></td>
@@ -625,30 +625,30 @@
                 <td class="right" data-ratio="33 33">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>395</td>
-                <td>86</td>
+                <td>406</td>
+                <td>82</td>
                 <td>0</td>
-                <td class="right" data-ratio="309 395">78%</td>
+                <td class="right" data-ratio="324 406">80%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-************ CCoovveerraaggee rreeppoorrtt:: 7788%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 8800%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-16 17:13 +0200
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-22 15:42 +0200
 FFiillee            ffuunnccttiioonn                                                 ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _(_n_o_ _f_u_n_c_t_i_o_n_)                                            3          0       0        100%
 _____i_n_i_t_____._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _I_S___I_N___L_I_S_T                                               2          0       0        100%
 _h_e_l_p_e_r_s_._p_y
@@ -45,15 +45,15 @@
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _k_e_y___l_o_o_k_u_p___q_u_e_r_y                                         10         2       0        80%
 _m_o_d_e_l_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _k_e_y___l_o_o_k_u_p                                               7          2       0        71%
 _m_o_d_e_l_._p_y
 _s_r_c_/
-_e_d_w_h___a_u_t_h___r_b_a_c_/ _d_e_f_i_n_e___a_u_t_h___r_b_a_c___m_o_d_e_l                                   5          0       0        100%
+_e_d_w_h___a_u_t_h___r_b_a_c_/ _d_e_f_i_n_e___a_u_t_h___r_b_a_c___m_o_d_e_l                                   6          0       0        100%
 _m_o_d_e_l_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _a_d_d___i_d_e_n_t_i_t_y                                             12         4       0        67%
 _m_o_d_e_l_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _a_d_d___g_r_o_u_p                                                1          0       0        100%
 _m_o_d_e_l_._p_y
@@ -75,48 +75,48 @@
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _a_d_d___m_e_m_b_e_r_s_h_i_p                                           11         2       0        82%
 _m_o_d_e_l_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _r_e_m_o_v_e___m_e_m_b_e_r_s_h_i_p                                        7          0       0        100%
 _m_o_d_e_l_._p_y
 _s_r_c_/
-_e_d_w_h___a_u_t_h___r_b_a_c_/ _g_e_t___m_e_m_b_e_r_s_h_i_p_s                                          5          0       0        100%
+_e_d_w_h___a_u_t_h___r_b_a_c_/ _g_e_t___m_e_m_b_e_r_s_h_i_p_s                                          3          0       0        100%
 _m_o_d_e_l_._p_y
 _s_r_c_/
-_e_d_w_h___a_u_t_h___r_b_a_c_/ _g_e_t___m_e_m_b_e_r_s                                              5          5       0        0%
+_e_d_w_h___a_u_t_h___r_b_a_c_/ _g_e_t___m_e_m_b_e_r_s                                              3          3       0        0%
 _m_o_d_e_l_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _a_d_d___p_e_r_m_i_s_s_i_o_n                                           8          2       0        75%
 _m_o_d_e_l_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _r_e_m_o_v_e___p_e_r_m_i_s_s_i_o_n                                        13         13      0        0%
 _m_o_d_e_l_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _w_i_t_h___a_l_i_a_s                                               13         2       0        85%
 _m_o_d_e_l_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _h_a_s___p_e_r_m_i_s_s_i_o_n                                           16         0       0        100%
 _m_o_d_e_l_._p_y
 _s_r_c_/
-_e_d_w_h___a_u_t_h___r_b_a_c_/ _(_n_o_ _f_u_n_c_t_i_o_n_)                                            42         0       0        100%
+_e_d_w_h___a_u_t_h___r_b_a_c_/ _(_n_o_ _f_u_n_c_t_i_o_n_)                                            57         0       0        100%
 _m_o_d_e_l_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _A_u_t_h_R_b_a_c_._____i_n_i_t____                                        1          0       0        100%
 _r_b_a_c_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _A_u_t_h_R_b_a_c_.___e_r_r_o_r                                          1          1       0        0%
 _r_b_a_c_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _A_u_t_h_R_b_a_c_._a_d_d___u_s_e_r                                        7          1       0        86%
 _r_b_a_c_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _A_u_t_h_R_b_a_c_._a_d_d___i_t_e_m                                        7          7       0        0%
 _r_b_a_c_._p_y
 _s_r_c_/
-_e_d_w_h___a_u_t_h___r_b_a_c_/ _A_u_t_h_R_b_a_c_._a_d_d___i_d_e_n_t_i_t_y                                    9          9       0        0%
+_e_d_w_h___a_u_t_h___r_b_a_c_/ _A_u_t_h_R_b_a_c_._a_d_d___i_d_e_n_t_i_t_y                                    7          7       0        0%
 _r_b_a_c_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _A_u_t_h_R_b_a_c_._a_d_d___g_r_o_u_p                                       7          1       0        86%
 _r_b_a_c_._p_y
 _s_r_c_/
 _e_d_w_h___a_u_t_h___r_b_a_c_/ _A_u_t_h_R_b_a_c_._u_p_d_a_t_e___i_d_e_n_t_i_t_y                                 3          3       0        0%
 _r_b_a_c_._p_y
@@ -152,15 +152,15 @@
 _r_b_a_c_._p_y
 _t_e_s_t_s_/          _(_n_o_ _f_u_n_c_t_i_o_n_)                                            0          0       0        100%
 _____i_n_i_t_____._p_y
 _t_e_s_t_s_/          _t_m_p_d_i_r                                                   3          0       0        100%
 _t_e_s_t___r_b_a_c_._p_y
 _t_e_s_t_s_/          _d_a_t_a_b_a_s_e                                                 4          0       0        100%
 _t_e_s_t___r_b_a_c_._p_y
-_t_e_s_t_s_/          _d_a_t_a_b_a_s_e_._D_a_t_a_b_a_s_e_._____e_n_t_e_r____                              4          0       0        100%
+_t_e_s_t_s_/          _d_a_t_a_b_a_s_e_._D_a_t_a_b_a_s_e_._____e_n_t_e_r____                              5          0       0        100%
 _t_e_s_t___r_b_a_c_._p_y
 _t_e_s_t_s_/          _d_a_t_a_b_a_s_e_._D_a_t_a_b_a_s_e_._____e_x_i_t____                               1          0       0        100%
 _t_e_s_t___r_b_a_c_._p_y
 _t_e_s_t_s_/          _r_b_a_c                                                     2          0       0        100%
 _t_e_s_t___r_b_a_c_._p_y
 _t_e_s_t_s_/          _s_t_o_r_e                                                    2          0       0        100%
 _t_e_s_t___r_b_a_c_._p_y
@@ -190,10 +190,10 @@
 _t_e_s_t___r_b_a_c_._p_y
 _t_e_s_t_s_/          _T_e_s_t_S_e_q_u_e_n_t_i_a_l_l_y_._t_e_s_t___d_e_e_p_e_r___g_r_o_u_p___n_e_s_t_i_n_g               10         0       0        100%
 _t_e_s_t___r_b_a_c_._p_y
 _t_e_s_t_s_/          _T_e_s_t_S_e_q_u_e_n_t_i_a_l_l_y_._t_e_s_t___r_e_m_o_v_i_n_g___a___n_e_s_t_e_d___g_r_o_u_p            2          0       0        100%
 _t_e_s_t___r_b_a_c_._p_y
 _t_e_s_t_s_/          _(_n_o_ _f_u_n_c_t_i_o_n_)                                            33         0       0        100%
 _t_e_s_t___r_b_a_c_._p_y
-Total                                                                    395        86      0        78%
+Total                                                                    406        82      0        80%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-16 17:13 +0200
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-22 15:42 +0200
```

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/index.html` & `edwh_auth_rbac-0.4.0/htmlcov/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
     <script src="coverage_html_cb_da166b87.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">78%</span>
+            <span class="pc_cov">80%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
@@ -50,15 +50,15 @@
         <h2>
                 <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -89,60 +89,60 @@
                 <td>9</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="9 9">100%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="z_438b44bce6437be6_model_py.html">src/edwh_auth_rbac/model.py</a></td>
-                <td>183</td>
-                <td>44</td>
+                <td>195</td>
+                <td>42</td>
                 <td>0</td>
-                <td class="right" data-ratio="139 183">76%</td>
+                <td class="right" data-ratio="153 195">78%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="z_438b44bce6437be6_rbac_py.html">src/edwh_auth_rbac/rbac.py</a></td>
-                <td>88</td>
-                <td>39</td>
+                <td>86</td>
+                <td>37</td>
                 <td>0</td>
-                <td class="right" data-ratio="49 88">56%</td>
+                <td class="right" data-ratio="49 86">57%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="z_a44f0ac069e85531___init___py.html">tests/__init__.py</a></td>
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="z_a44f0ac069e85531_test_rbac_py.html">tests/test_rbac.py</a></td>
-                <td>106</td>
+                <td>107</td>
                 <td>2</td>
                 <td>0</td>
-                <td class="right" data-ratio="104 106">98%</td>
+                <td class="right" data-ratio="105 107">98%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>395</td>
-                <td>86</td>
+                <td>406</td>
+                <td>82</td>
                 <td>0</td>
-                <td class="right" data-ratio="309 395">78%</td>
+                <td class="right" data-ratio="324 406">80%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="z_a44f0ac069e85531_test_rbac_py.html"></a>
         <a id="nextFileLink" class="nav" href="z_438b44bce6437be6___init___py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-************ CCoovveerraaggee rreeppoorrtt:: 7788%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 8800%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-16 17:13 +0200
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-22 15:42 +0200
 FFiillee                             ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/_____i_n_i_t_____._p_y   3          0       0        100%
 _s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/_h_e_l_p_e_r_s_._p_y    6          1       0        83%
 _s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/_m_i_g_r_a_t_i_o_n_s_._p_y 9          0       0        100%
-_s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/_m_o_d_e_l_._p_y      183        44      0        76%
-_s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/_r_b_a_c_._p_y       88         39      0        56%
+_s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/_m_o_d_e_l_._p_y      195        42      0        78%
+_s_r_c_/_e_d_w_h___a_u_t_h___r_b_a_c_/_r_b_a_c_._p_y       86         37      0        57%
 _t_e_s_t_s_/_____i_n_i_t_____._p_y                0          0       0        100%
-_t_e_s_t_s_/_t_e_s_t___r_b_a_c_._p_y               106        2       0        98%
-Total                            395        86      0        78%
+_t_e_s_t_s_/_t_e_s_t___r_b_a_c_._p_y               107        2       0        98%
+Total                            406        82      0        80%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-16 17:13 +0200
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-22 15:42 +0200
```

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/keybd_closed_cb_ce680311.png` & `edwh_auth_rbac-0.4.0/htmlcov/keybd_closed_cb_ce680311.png`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/status.json` & `edwh_auth_rbac-0.4.0/htmlcov/status.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8874302455357143%*

 * *Differences: {"'files'": "{'z_438b44bce6437be6___init___py': {'hash': 'f865ba0db0b5030b5880dcb0d91dd67e'}, "*

 * *            "'z_438b44bce6437be6_helpers_py': {'hash': '9f7fb4f0d0f2f39171c2d5139e39a086'}, "*

 * *            "'z_438b44bce6437be6_migrations_py': {'hash': 'bd69707dc2fb2e840cce1c0d592b9364'}, "*

 * *            "'z_438b44bce6437be6_model_py': {'hash': 'd7db162b6ac1d9fb1faf7d9fa63d960b', 'index': "*

 * *            "{'nums': {'n_statements': 195, 'n_missing': 42}}}, 'z_438b44bce6437be6_rbac_py': "*

 * *            "{'hash': '91ee2b […]*

```diff
@@ -1,11 +1,11 @@
 {
     "files": {
         "z_438b44bce6437be6___init___py": {
-            "hash": "d505583c7eb86c5b4a6afc6c7f68b41c",
+            "hash": "f865ba0db0b5030b5880dcb0d91dd67e",
             "index": {
                 "description": "",
                 "file": "src/edwh_auth_rbac/__init__.py",
                 "nums": {
                     "n_branches": 0,
                     "n_excluded": 0,
                     "n_files": 1,
@@ -15,15 +15,15 @@
                     "n_statements": 3,
                     "precision": 0
                 },
                 "url": "z_438b44bce6437be6___init___py.html"
             }
         },
         "z_438b44bce6437be6_helpers_py": {
-            "hash": "fad6a7b5f1b1cbb706fc6350a7ef8224",
+            "hash": "9f7fb4f0d0f2f39171c2d5139e39a086",
             "index": {
                 "description": "",
                 "file": "src/edwh_auth_rbac/helpers.py",
                 "nums": {
                     "n_branches": 0,
                     "n_excluded": 0,
                     "n_files": 1,
@@ -33,15 +33,15 @@
                     "n_statements": 6,
                     "precision": 0
                 },
                 "url": "z_438b44bce6437be6_helpers_py.html"
             }
         },
         "z_438b44bce6437be6_migrations_py": {
-            "hash": "5d2d74acaa7d6bf153bebcc4cb6a3a06",
+            "hash": "bd69707dc2fb2e840cce1c0d592b9364",
             "index": {
                 "description": "",
                 "file": "src/edwh_auth_rbac/migrations.py",
                 "nums": {
                     "n_branches": 0,
                     "n_excluded": 0,
                     "n_files": 1,
@@ -51,51 +51,51 @@
                     "n_statements": 9,
                     "precision": 0
                 },
                 "url": "z_438b44bce6437be6_migrations_py.html"
             }
         },
         "z_438b44bce6437be6_model_py": {
-            "hash": "bd4f79b86d3c281865ac040508f86232",
+            "hash": "d7db162b6ac1d9fb1faf7d9fa63d960b",
             "index": {
                 "description": "",
                 "file": "src/edwh_auth_rbac/model.py",
                 "nums": {
                     "n_branches": 0,
                     "n_excluded": 0,
                     "n_files": 1,
-                    "n_missing": 44,
+                    "n_missing": 42,
                     "n_missing_branches": 0,
                     "n_partial_branches": 0,
-                    "n_statements": 183,
+                    "n_statements": 195,
                     "precision": 0
                 },
                 "url": "z_438b44bce6437be6_model_py.html"
             }
         },
         "z_438b44bce6437be6_rbac_py": {
-            "hash": "bc33d43b75e29ebaae5f21658b4c2779",
+            "hash": "91ee2b43a7a38fd87a04441b0e3497cf",
             "index": {
                 "description": "",
                 "file": "src/edwh_auth_rbac/rbac.py",
                 "nums": {
                     "n_branches": 0,
                     "n_excluded": 0,
                     "n_files": 1,
-                    "n_missing": 39,
+                    "n_missing": 37,
                     "n_missing_branches": 0,
                     "n_partial_branches": 0,
-                    "n_statements": 88,
+                    "n_statements": 86,
                     "precision": 0
                 },
                 "url": "z_438b44bce6437be6_rbac_py.html"
             }
         },
         "z_a44f0ac069e85531___init___py": {
-            "hash": "3c77fc9ef7f887ac2508d4109cf92472",
+            "hash": "e6baa73cda2916dad605215f937a92e1",
             "index": {
                 "description": "",
                 "file": "tests/__init__.py",
                 "nums": {
                     "n_branches": 0,
                     "n_excluded": 0,
                     "n_files": 1,
@@ -105,30 +105,30 @@
                     "n_statements": 0,
                     "precision": 0
                 },
                 "url": "z_a44f0ac069e85531___init___py.html"
             }
         },
         "z_a44f0ac069e85531_test_rbac_py": {
-            "hash": "c734e50fab72774ab300532af723340c",
+            "hash": "003b2c611f3c1529e284989a26b07525",
             "index": {
                 "description": "",
                 "file": "tests/test_rbac.py",
                 "nums": {
                     "n_branches": 0,
                     "n_excluded": 0,
                     "n_files": 1,
                     "n_missing": 2,
                     "n_missing_branches": 0,
                     "n_partial_branches": 0,
-                    "n_statements": 106,
+                    "n_statements": 107,
                     "precision": 0
                 },
                 "url": "z_a44f0ac069e85531_test_rbac_py.html"
             }
         }
     },
     "format": 5,
-    "globals": "5fa1e0f6e4d7cde75368d49f351fb614",
+    "globals": "16e587203e9df0eb24d83facc6663335",
     "note": "This file is an internal implementation detail to speed up HTML report generation. Its format can change at any time. You might be looking for the JSON report: https://coverage.rtfd.io/cmd.html#cmd-json",
     "version": "7.5.1"
 }
```

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/style_cb_8e611ae1.css` & `edwh_auth_rbac-0.4.0/htmlcov/style_cb_8e611ae1.css`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6___init___py.html` & `edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6___init___py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,41 +61,41 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="z_438b44bce6437be6_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
             <button type="button" class="button_next_file" data-shortcut="]"></button>
             <button type="button" class="button_to_index" data-shortcut="u"></button>
             <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.0.0"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.1.1"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">rbac</span> <span class="key">import</span> <span class="nam">Password</span><span class="op">,</span> <span class="nam">AuthRbac</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">model</span> <span class="key">import</span> <span class="nam">key_lookup</span><span class="op">,</span> <span class="nam">DEFAULT_STARTS</span><span class="op">,</span> <span class="nam">DEFAULT_ENDS</span><span class="op">,</span> <span class="nam">unstr_datetime</span><span class="op">,</span> <span class="nam">DEFAULT</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">model</span> <span class="key">import</span> <span class="nam">DEFAULT</span><span class="op">,</span> <span class="nam">DEFAULT_ENDS</span><span class="op">,</span> <span class="nam">DEFAULT_STARTS</span><span class="op">,</span> <span class="nam">key_lookup</span><span class="op">,</span> <span class="nam">unstr_datetime</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">rbac</span> <span class="key">import</span> <span class="nam">AuthRbac</span><span class="op">,</span> <span class="nam">Password</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="z_438b44bce6437be6_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 33 ssttaatteemmeennttss ?  33 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
-_1__version__ = "0.0.0" 
+22 15:42 +0200
+_1__version__ = "0.1.1" 
 _2 
-_3from .rbac import Password, AuthRbac 
-_4from .model import key_lookup, DEFAULT_STARTS, DEFAULT_ENDS, unstr_datetime,
-DEFAULT 
+_3from .model import DEFAULT, DEFAULT_ENDS, DEFAULT_STARTS, key_lookup,
+unstr_datetime 
+_4from .rbac import AuthRbac, Password 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
```

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_helpers_py.html` & `edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_helpers_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="z_438b44bce6437be6___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="z_438b44bce6437be6_migrations_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -80,27 +80,27 @@
     </div>
 </header>
 <main id="source">
     <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">def</span> <span class="nam">IS_IN_LIST</span><span class="op">(</span><span class="nam">allowed_values</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">    <span class="key">def</span> <span class="nam">execute</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">row</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">        <span class="com"># print('{} in {} ?'.format(value, allowed_values))</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">        <span class="key">if</span> <span class="nam">value</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">allowed_values</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">            <span class="key">return</span> <span class="nam">value</span><span class="op">,</span> <span class="str">'{} is not one of {}'</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">repr</span><span class="op">(</span><span class="nam">allowed_values</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">            <span class="key">return</span> <span class="nam">value</span><span class="op">,</span> <span class="str">"{} is not one of {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">repr</span><span class="op">(</span><span class="nam">allowed_values</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">            <span class="key">return</span> <span class="nam">value</span><span class="op">,</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="key">return</span> <span class="nam">execute</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="z_438b44bce6437be6___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="z_438b44bce6437be6_migrations_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 66 ssttaatteemmeennttss ?  55 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
 _1def IS_IN_LIST(allowed_values): 
 _2 def execute(value, row): 
 _3 # print('{} in {} ?'.format(value, allowed_values)) 
 _4 if value not in allowed_values: 
-_5 return value, '{} is not one of {}'.format(value, repr(allowed_values)) 
+_5 return value, "{} is not one of {}".format(value, repr(allowed_values)) 
 _6 else: 
 _7 return value, None 
 _8 
 _9 return execute 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
```

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_migrations_py.html` & `edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_migrations_py.html`

 * *Files 8% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="z_438b44bce6437be6_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="z_438b44bce6437be6_model_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -81,65 +81,73 @@
 </header>
 <main id="source">
     <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">from</span> <span class="nam">edwh_migrate</span> <span class="key">import</span> <span class="nam">migration</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="op">@</span><span class="nam">migration</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">def</span> <span class="nam">rbac_migrations</span><span class="op">(</span><span class="nam">db</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">executesql</span><span class="op">(</span><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="str">    drop view if exists recursive_memberships;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="str">    """</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">executesql</span><span class="op">(</span><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">create view recursive_memberships as</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">  -- each root is member of object_id, including one line for himself.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">  -- also for a user</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="str">  with RECURSIVE m(root, object_id, object_type, level, email, firstname, fullname) as (</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">        select object_id as root,  object_id, object_type, 0, email, firstname, fullname</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">          from identity</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">        union all</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">        select root, membership.member_of, i.object_type, m.level+1, i.email, i.firstname, i.fullname</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">          from membership join m on subject == m.object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="str">               join identity i on i.object_id = membership.member_of</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">        order by root, m.level+1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">    )</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">    select * from m</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">"""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">executesql</span><span class="op">(</span><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">drop view if exists recursive_members;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="str">    """</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">executesql</span><span class="op">(</span><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">create view recursive_members as</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    with RECURSIVE m(root, object_id, object_type, level, email, firstname, fullname) as (</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">        select object_id as root, object_id, object_type, 0, email, firstname, fullname</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="str">          from identity</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t"><span class="str">        union all</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t"><span class="str">        select root, membership.subject, i.object_type, m.level+1, i.email, i.firstname, i.fullname</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="str">          from membership join m on member_of== m.object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">               join identity i on i.object_id = membership.subject</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">        order by root</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="str">    )</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">    select * from m</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="str">    """</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">executesql</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="str">    drop view if exists recursive_memberships;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">executesql</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="str">create view recursive_memberships as</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">  -- each root is member of object_id, including one line for himself.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">  -- also for a user</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">  with RECURSIVE m(root, object_id, object_type, level, email, firstname, fullname) as (</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">        select object_id as root,  object_id, object_type, 0, email, firstname, fullname</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">          from identity</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="str">        union all</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">        select root, membership.member_of, i.object_type, m.level+1, i.email, i.firstname, i.fullname</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">          from membership join m on subject == m.object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">               join identity i on i.object_id = membership.member_of</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">        order by root, m.level+1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">    )</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">    select * from m</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">executesql</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">drop view if exists recursive_members;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">executesql</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">create view recursive_members as</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">    with RECURSIVE m(root, object_id, object_type, level, email, firstname, fullname) as (</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="str">        select object_id as root, object_id, object_type, 0, email, firstname, fullname</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">          from identity</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">        union all</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="str">        select root, membership.subject, i.object_type, m.level+1, i.email, i.firstname, i.fullname</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="str">          from membership join m on member_of== m.object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">               join identity i on i.object_id = membership.subject</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t"><span class="str">        order by root</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="str">    )</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="str">    select * from m</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="z_438b44bce6437be6_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="z_438b44bce6437be6_model_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,64 +6,72 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 99 ssttaatteemmeennttss ?  99 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
 _1from edwh_migrate import migration 
 _2 
 _3 
 _4@migration() 
 _5def rbac_migrations(db): 
-_6 db.executesql(""" 
-_7 drop view if exists recursive_memberships; 
-_8 """) 
-_9 db.executesql(""" 
-_1_0create view recursive_memberships as 
-_1_1 -- each root is member of object_id, including one line for himself. 
-_1_2 -- also for a user 
-_1_3 with RECURSIVE m(root, object_id, object_type, level, email, firstname,
+_6 db.executesql( 
+_7 """ 
+_8 drop view if exists recursive_memberships; 
+_9 """ 
+_1_0 ) 
+_1_1 db.executesql( 
+_1_2 """ 
+_1_3create view recursive_memberships as 
+_1_4 -- each root is member of object_id, including one line for himself. 
+_1_5 -- also for a user 
+_1_6 with RECURSIVE m(root, object_id, object_type, level, email, firstname,
 fullname) as ( 
-_1_4 select object_id as root, object_id, object_type, 0, email, firstname,
+_1_7 select object_id as root, object_id, object_type, 0, email, firstname,
 fullname 
-_1_5 from identity 
-_1_6 union all 
-_1_7 select root, membership.member_of, i.object_type, m.level+1, i.email,
+_1_8 from identity 
+_1_9 union all 
+_2_0 select root, membership.member_of, i.object_type, m.level+1, i.email,
 i.firstname, i.fullname 
-_1_8 from membership join m on subject == m.object_id 
-_1_9 join identity i on i.object_id = membership.member_of 
-_2_0 order by root, m.level+1 
-_2_1 ) 
-_2_2 select * from m 
-_2_3; 
-_2_4""") 
-_2_5 
-_2_6 db.executesql(""" 
-_2_7drop view if exists recursive_members; 
-_2_8  
-_2_9 """) 
-_3_0 
-_3_1 db.executesql(""" 
-_3_2create view recursive_members as 
-_3_3 with RECURSIVE m(root, object_id, object_type, level, email, firstname,
+_2_1 from membership join m on subject == m.object_id 
+_2_2 join identity i on i.object_id = membership.member_of 
+_2_3 order by root, m.level+1 
+_2_4 ) 
+_2_5 select * from m 
+_2_6; 
+_2_7""" 
+_2_8 ) 
+_2_9 
+_3_0 db.executesql( 
+_3_1 """ 
+_3_2drop view if exists recursive_members; 
+_3_3  
+_3_4 """ 
+_3_5 ) 
+_3_6 
+_3_7 db.executesql( 
+_3_8 """ 
+_3_9create view recursive_members as 
+_4_0 with RECURSIVE m(root, object_id, object_type, level, email, firstname,
 fullname) as ( 
-_3_4 select object_id as root, object_id, object_type, 0, email, firstname,
+_4_1 select object_id as root, object_id, object_type, 0, email, firstname,
 fullname 
-_3_5 from identity 
-_3_6 union all 
-_3_7 select root, membership.subject, i.object_type, m.level+1, i.email,
+_4_2 from identity 
+_4_3 union all 
+_4_4 select root, membership.subject, i.object_type, m.level+1, i.email,
 i.firstname, i.fullname 
-_3_8 from membership join m on member_of== m.object_id 
-_3_9 join identity i on i.object_id = membership.subject 
-_4_0 order by root 
-_4_1 ) 
-_4_2 select * from m 
-_4_3; 
-_4_4 
-_4_5 """) 
-_4_6 
-_4_7 db.commit() 
-_4_8 return True 
+_4_5 from membership join m on member_of== m.object_id 
+_4_6 join identity i on i.object_id = membership.subject 
+_4_7 order by root 
+_4_8 ) 
+_4_9 select * from m 
+_5_0; 
+_5_1 
+_5_2 """ 
+_5_3 ) 
+_5_4 
+_5_5 db.commit() 
+_5_6 return True 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
```

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_model_py.html` & `edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_model_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/edwh_auth_rbac/model.py: 76%</title>
+    <title>Coverage for src/edwh_auth_rbac/model.py: 78%</title>
     <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
     <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
     <script src="coverage_html_cb_da166b87.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/edwh_auth_rbac/model.py</b>:
-            <span class="pc_cov">76%</span>
+            <span class="pc_cov">78%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">183 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">139<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">44<span class="text"> missing</span></button>
+            <span class="text">195 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">153<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">42<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="z_438b44bce6437be6_migrations_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="z_438b44bce6437be6_rbac_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -77,369 +77,418 @@
             <button type="button" class="button_to_index" data-shortcut="u"></button>
             <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">copy</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">datetime</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">datetime</span> <span class="key">as</span> <span class="nam">dt</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">hashlib</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">hmac</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">uuid</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">dateutil</span><span class="op">.</span><span class="nam">parser</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span> <span class="key">import</span> <span class="nam">Field</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span> <span class="key">import</span> <span class="nam">SQLCustomType</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">objects</span> <span class="key">import</span> <span class="nam">SQLALL</span><span class="op">,</span> <span class="nam">Query</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">IS_IN_LIST</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">uuid</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">uuid</span> <span class="key">import</span> <span class="nam">UUID</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">import</span> <span class="nam">dateutil</span><span class="op">.</span><span class="nam">parser</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span> <span class="key">import</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">Field</span><span class="op">,</span> <span class="nam">SQLCustomType</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">objects</span> <span class="key">import</span> <span class="nam">SQLALL</span><span class="op">,</span> <span class="nam">Query</span><span class="op">,</span> <span class="nam">Table</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">class</span> <span class="nam">DEFAULT</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="nam">DEFAULT_STARTS</span> <span class="op">=</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">datetime</span><span class="op">(</span><span class="num">2000</span><span class="op">,</span> <span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="nam">DEFAULT_ENDS</span> <span class="op">=</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">datetime</span><span class="op">(</span><span class="num">3000</span><span class="op">,</span> <span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="key">def</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">s</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"""json helper... might values arrive as str """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="key">return</span> <span class="nam">dateutil</span><span class="op">.</span><span class="nam">parser</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">s</span><span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">s</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="nam">s</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="key">class</span> <span class="nam">Password</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="str">    Encode a password using: Password.encode('secret')</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="key">def</span> <span class="nam">hmac_hash</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">value</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">salt</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">digest_alg</span> <span class="op">=</span> <span class="nam">hashlib</span><span class="op">.</span><span class="nam">sha512</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="nam">d</span> <span class="op">=</span> <span class="nam">hmac</span><span class="op">.</span><span class="nam">new</span><span class="op">(</span><span class="nam">str</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">str</span><span class="op">(</span><span class="nam">value</span><span class="op">)</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">digest_alg</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="key">if</span> <span class="nam">salt</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="nam">d</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">str</span><span class="op">(</span><span class="nam">salt</span><span class="op">)</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="key">return</span> <span class="nam">d</span><span class="op">.</span><span class="nam">hexdigest</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="key">def</span> <span class="nam">validate</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">password</span><span class="op">,</span> <span class="nam">candidate</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">salt</span><span class="op">,</span> <span class="nam">hashed</span> <span class="op">=</span> <span class="nam">candidate</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">':'</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">hmac_hash</span><span class="op">(</span><span class="nam">value</span><span class="op">=</span><span class="nam">password</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="str">'secret_start'</span><span class="op">,</span> <span class="nam">salt</span><span class="op">=</span><span class="nam">salt</span><span class="op">)</span> <span class="op">==</span> <span class="nam">hashed</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="key">def</span> <span class="nam">encode</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">password</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">        <span class="nam">salt</span> <span class="op">=</span> <span class="nam">uuid</span><span class="op">.</span><span class="nam">uuid4</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">hex</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">return</span> <span class="nam">salt</span> <span class="op">+</span> <span class="str">':'</span> <span class="op">+</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">hmac_hash</span><span class="op">(</span><span class="nam">value</span><span class="op">=</span><span class="nam">password</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="str">'secret_start'</span><span class="op">,</span> <span class="nam">salt</span><span class="op">=</span><span class="nam">salt</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="key">def</span> <span class="nam">is_uuid</span><span class="op">(</span><span class="nam">s</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="nam">uuid</span><span class="op">.</span><span class="nam">UUID</span><span class="op">(</span><span class="nam">s</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="key">except</span> <span class="nam">Exception</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="key">def</span> <span class="nam">key_lookup_query</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">int</span> <span class="op">|</span> <span class="nam">uuid</span><span class="op">.</span><span class="nam">UUID</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Query</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="key">if</span> <span class="str">'@'</span> <span class="key">in</span> <span class="nam">str</span><span class="op">(</span><span class="nam">identity_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">email</span> <span class="op">==</span> <span class="nam">identity_key</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">identity_key</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">        <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">id</span> <span class="op">==</span> <span class="nam">identity_key</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="key">elif</span> <span class="nam">is_uuid</span><span class="op">(</span><span class="nam">identity_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">        <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">object_id</span> <span class="op">==</span> <span class="nam">identity_key</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">firstname</span> <span class="op">==</span> <span class="nam">identity_key</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="key">if</span> <span class="nam">object_type</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">object_type</span> <span class="op">==</span> <span class="nam">object_type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="key">return</span> <span class="nam">query</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">IS_IN_LIST</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">class</span> <span class="nam">DEFAULT</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="nam">DEFAULT_STARTS</span> <span class="op">=</span> <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span><span class="op">(</span><span class="num">2000</span><span class="op">,</span> <span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">DEFAULT_ENDS</span> <span class="op">=</span> <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span><span class="op">(</span><span class="num">3000</span><span class="op">,</span> <span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="key">def</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">s</span><span class="op">:</span> <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span> <span class="op">|</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"""json helper... might values arrive as str"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="key">return</span> <span class="nam">dateutil</span><span class="op">.</span><span class="nam">parser</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">s</span><span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">s</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="nam">s</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="key">class</span> <span class="nam">Password</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    Encode a password using: Password.encode('secret')</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="key">def</span> <span class="nam">hmac_hash</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">value</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">salt</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="nam">digest_alg</span> <span class="op">=</span> <span class="nam">hashlib</span><span class="op">.</span><span class="nam">sha512</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="nam">d</span> <span class="op">=</span> <span class="nam">hmac</span><span class="op">.</span><span class="nam">new</span><span class="op">(</span><span class="nam">str</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">str</span><span class="op">(</span><span class="nam">value</span><span class="op">)</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">digest_alg</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="key">if</span> <span class="nam">salt</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">            <span class="nam">d</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">str</span><span class="op">(</span><span class="nam">salt</span><span class="op">)</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="key">return</span> <span class="nam">d</span><span class="op">.</span><span class="nam">hexdigest</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="key">def</span> <span class="nam">validate</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">password</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">candidate</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="nam">salt</span><span class="op">,</span> <span class="nam">hashed</span> <span class="op">=</span> <span class="nam">candidate</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">":"</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">hmac_hash</span><span class="op">(</span><span class="nam">value</span><span class="op">=</span><span class="nam">password</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="str">"secret_start"</span><span class="op">,</span> <span class="nam">salt</span><span class="op">=</span><span class="nam">salt</span><span class="op">)</span> <span class="op">==</span> <span class="nam">hashed</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="key">def</span> <span class="nam">encode</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">password</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="nam">salt</span> <span class="op">=</span> <span class="nam">uuid</span><span class="op">.</span><span class="nam">uuid4</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">hex</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="key">return</span> <span class="nam">salt</span> <span class="op">+</span> <span class="str">":"</span> <span class="op">+</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">hmac_hash</span><span class="op">(</span><span class="nam">value</span><span class="op">=</span><span class="nam">password</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="str">"secret_start"</span><span class="op">,</span> <span class="nam">salt</span><span class="op">=</span><span class="nam">salt</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t"><span class="key">def</span> <span class="nam">is_uuid</span><span class="op">(</span><span class="nam">s</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="nam">UUID</span><span class="op">(</span><span class="nam">s</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="key">except</span> <span class="nam">Exception</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="nam">IdentityKey</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeAlias</span> <span class="op">=</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">int</span> <span class="op">|</span> <span class="nam">UUID</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="nam">ObjectTypes</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Literal</span><span class="op">[</span><span class="str">"user"</span><span class="op">,</span> <span class="str">"group"</span><span class="op">,</span> <span class="str">"item"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t"><span class="key">def</span> <span class="nam">key_lookup_query</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">:</span> <span class="nam">ObjectTypes</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Query</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="key">if</span> <span class="str">"@"</span> <span class="key">in</span> <span class="nam">str</span><span class="op">(</span><span class="nam">identity_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">email</span> <span class="op">==</span> <span class="nam">identity_key</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">identity_key</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">id</span> <span class="op">==</span> <span class="nam">identity_key</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="key">elif</span> <span class="nam">is_uuid</span><span class="op">(</span><span class="nam">identity_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">object_id</span> <span class="op">==</span> <span class="nam">identity_key</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">firstname</span> <span class="op">==</span> <span class="nam">identity_key</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="key">def</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">key_lookup_query</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="key">if</span> <span class="nam">object_type</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">object_type</span> <span class="op">==</span> <span class="nam">object_type</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="nam">rowset</span> <span class="op">=</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">object_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="key">return</span> <span class="nam">query</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">rowset</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="key">elif</span> <span class="nam">len</span><span class="op">(</span><span class="nam">rowset</span><span class="op">)</span> <span class="op">></span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">'Keep lookup for {} returned {} results.'</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">identity_key</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">rowset</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="key">return</span> <span class="nam">rowset</span><span class="op">.</span><span class="nam">first</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t"><span class="nam">my_datetime</span> <span class="op">=</span> <span class="nam">SQLCustomType</span><span class="op">(</span><span class="nam">type</span><span class="op">=</span><span class="str">'string'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">                            <span class="nam">native</span><span class="op">=</span><span class="str">'char(35)'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">                            <span class="nam">encoder</span><span class="op">=</span><span class="op">(</span><span class="key">lambda</span> <span class="nam">x</span><span class="op">:</span> <span class="nam">x</span><span class="op">.</span><span class="nam">isoformat</span><span class="op">(</span><span class="str">' '</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">                            <span class="nam">decoder</span><span class="op">=</span><span class="op">(</span><span class="key">lambda</span> <span class="nam">x</span><span class="op">:</span> <span class="nam">dateutil</span><span class="op">.</span><span class="nam">parser</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">x</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="key">def</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">:</span> <span class="nam">ObjectTypes</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">key_lookup_query</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="nam">rowset</span> <span class="op">=</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">object_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">rowset</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="key">elif</span> <span class="nam">len</span><span class="op">(</span><span class="nam">rowset</span><span class="op">)</span> <span class="op">></span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Keep lookup for {} returned {} results."</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">identity_key</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">rowset</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">    <span class="key">return</span> <span class="nam">rowset</span><span class="op">.</span><span class="nam">first</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="key">def</span> <span class="nam">define_auth_rbac_model</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">other_args</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span><span class="str">'identity'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">                    <span class="com"># std uuid from uuid libs are 36 chars long</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'object_id'</span><span class="op">,</span> <span class="str">'string'</span><span class="op">,</span> <span class="nam">length</span><span class="op">=</span><span class="num">36</span><span class="op">,</span> <span class="nam">unique</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">notnull</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">str</span><span class="op">(</span><span class="nam">uuid</span><span class="op">.</span><span class="nam">uuid4</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'object_type'</span><span class="op">,</span> <span class="str">'string'</span><span class="op">,</span> <span class="nam">requires</span><span class="op">=</span><span class="op">(</span><span class="nam">IS_IN_LIST</span><span class="op">(</span><span class="nam">other_args</span><span class="op">[</span><span class="str">'allowed_types'</span><span class="op">]</span><span class="op">)</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'created'</span><span class="op">,</span> <span class="str">'datetime'</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">datetime</span><span class="op">.</span><span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">                    <span class="com"># email needn't be unique, groups can share email addresses, and with people too</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'email'</span><span class="op">,</span> <span class="str">'string'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'firstname'</span><span class="op">,</span> <span class="str">'string'</span><span class="op">,</span> <span class="nam">comment</span><span class="op">=</span><span class="str">'also used as short code for groups'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'fullname'</span><span class="op">,</span> <span class="str">'string'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'encoded_password'</span><span class="op">,</span> <span class="str">'string'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">                    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span><span class="str">'membership'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">                    <span class="com"># beide zijn eigenlijk: reference:identity.object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'subject'</span><span class="op">,</span> <span class="str">'string'</span><span class="op">,</span> <span class="nam">length</span><span class="op">=</span><span class="num">36</span><span class="op">,</span> <span class="nam">notnull</span><span class="op">=</span><span class="key">True</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'member_of'</span><span class="op">,</span> <span class="str">'string'</span><span class="op">,</span> <span class="nam">length</span><span class="op">=</span><span class="num">36</span><span class="op">,</span> <span class="nam">notnull</span><span class="op">=</span><span class="key">True</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">                    <span class="com"># Field('starts','datetime', default=DEFAULT_STARTS),</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">                    <span class="com"># Field('ends','datetime', default=DEFAULT_ENDS),</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">                    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span><span class="str">'permission'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'privilege'</span><span class="op">,</span> <span class="str">'string'</span><span class="op">,</span> <span class="nam">length</span><span class="op">=</span><span class="num">20</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">                    <span class="com"># reference:identity.object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'identity_object_id'</span><span class="op">,</span> <span class="str">'string'</span><span class="op">,</span> <span class="nam">length</span><span class="op">=</span><span class="num">36</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'target_object_id'</span><span class="op">,</span> <span class="str">'string'</span><span class="op">,</span> <span class="nam">length</span><span class="op">=</span><span class="num">36</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">                    <span class="com"># Field('scope'), lets bail scope for now. every one needs a rule for everything</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">                    <span class="com"># just to make sure, no 'wildcards' and 'every dossier for org x' etc ...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'starts'</span><span class="op">,</span> <span class="nam">type</span><span class="op">=</span><span class="nam">my_datetime</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">DEFAULT_STARTS</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'ends'</span><span class="op">,</span> <span class="nam">type</span><span class="op">=</span><span class="nam">my_datetime</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">DEFAULT_ENDS</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">                    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span><span class="str">'recursive_memberships'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'root'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'object_id'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'object_type'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'level'</span><span class="op">,</span> <span class="str">'integer'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'email'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'firstname'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'fullname'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">                    <span class="nam">migrate</span><span class="op">=</span><span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">                    <span class="nam">primarykey</span><span class="op">=</span><span class="op">[</span><span class="str">'root'</span><span class="op">,</span> <span class="str">'object_id'</span><span class="op">]</span>  <span class="com"># composed, no primary key</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">                    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span><span class="str">'recursive_members'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'root'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'object_id'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'object_type'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'level'</span><span class="op">,</span> <span class="str">'integer'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'email'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'firstname'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">                    <span class="nam">Field</span><span class="op">(</span><span class="str">'fullname'</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">                    <span class="nam">migrate</span><span class="op">=</span><span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">                    <span class="nam">primarykey</span><span class="op">=</span><span class="op">[</span><span class="str">'root'</span><span class="op">,</span> <span class="str">'object_id'</span><span class="op">]</span>  <span class="com"># composed, no primary key</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">                    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t"><span class="key">def</span> <span class="nam">add_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">password</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">,</span> <span class="nam">name</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">firstname</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">fullname</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">gid</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">    <span class="str">"""paramaters name and firstname are equal. """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">    <span class="nam">email</span> <span class="op">=</span> <span class="nam">email</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">    <span class="key">if</span> <span class="nam">object_type</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">'object_type parameter expected'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">    <span class="nam">object_id</span> <span class="op">=</span> <span class="nam">gid</span> <span class="key">if</span> <span class="nam">gid</span> <span class="key">else</span> <span class="nam">str</span><span class="op">(</span><span class="nam">uuid</span><span class="op">.</span><span class="nam">uuid4</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">validate_and_insert</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="nam">object_id</span><span class="op">=</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="nam">object_type</span><span class="op">=</span><span class="nam">object_type</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">        <span class="nam">email</span><span class="op">=</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">        <span class="nam">firstname</span><span class="op">=</span><span class="nam">name</span> <span class="key">or</span> <span class="nam">firstname</span> <span class="key">or</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">        <span class="nam">fullname</span><span class="op">=</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">        <span class="nam">encoded_password</span><span class="op">=</span><span class="nam">Password</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="nam">password</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span> <span class="key">in</span> <span class="nam">member_of</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="nam">group_id</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="str">'group'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="key">if</span> <span class="nam">get_group</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">group_id</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">            <span class="com"># check each group if it exists.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">            <span class="nam">add_membership</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">=</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">=</span><span class="nam">group_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">    <span class="key">return</span> <span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t"><span class="key">def</span> <span class="nam">add_group</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">    <span class="key">return</span> <span class="nam">add_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="key">None</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">,</span> <span class="nam">name</span><span class="op">=</span><span class="nam">name</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="str">'group'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t"><span class="key">def</span> <span class="nam">remove_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">    <span class="nam">removed</span> <span class="op">=</span> <span class="nam">db</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">object_id</span> <span class="op">==</span> <span class="nam">object_id</span><span class="op">)</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="com"># todo: remove permissions and group memberships</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">    <span class="key">return</span> <span class="nam">removed</span> <span class="op">></span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t"><span class="key">def</span> <span class="nam">get_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t"><span class="str">    :param db: dal db connection</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t"><span class="str">    :param key: can be the email, id, or object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t"><span class="str">    :return: user record or None when not found</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">key_lookup_query</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">    <span class="nam">rows</span> <span class="op">=</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">    <span class="key">return</span> <span class="nam">rows</span><span class="op">.</span><span class="nam">first</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t"><span class="key">def</span> <span class="nam">get_user</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t"><span class="str">    :param db: dal db connection</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t"><span class="str">    :param key: can be the email, id, or object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t"><span class="str">    :return: user record or None when not found</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">    <span class="key">return</span> <span class="nam">get_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="str">'user'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t"><span class="key">def</span> <span class="nam">get_group</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t"><span class="str">    :param db: dal db connection</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t"><span class="str">    :param key: can be the name of the group, the id, object_id or email_address</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t"><span class="str">    :return: user record or None when not found</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">    <span class="key">return</span> <span class="nam">get_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="str">'group'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="nam">my_datetime</span> <span class="op">=</span> <span class="nam">SQLCustomType</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">    <span class="nam">type</span><span class="op">=</span><span class="str">"string"</span><span class="op">,</span> <span class="nam">native</span><span class="op">=</span><span class="str">"char(35)"</span><span class="op">,</span> <span class="nam">encoder</span><span class="op">=</span><span class="op">(</span><span class="key">lambda</span> <span class="nam">x</span><span class="op">:</span> <span class="nam">x</span><span class="op">.</span><span class="nam">isoformat</span><span class="op">(</span><span class="str">" "</span><span class="op">)</span><span class="op">)</span><span class="op">,</span> <span class="nam">decoder</span><span class="op">=</span><span class="op">(</span><span class="key">lambda</span> <span class="nam">x</span><span class="op">:</span> <span class="nam">dateutil</span><span class="op">.</span><span class="nam">parser</span><span class="op">.</span><span class="nam">parse</span><span class="op">(</span><span class="nam">x</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t"><span class="key">class</span> <span class="nam">RbacKwargs</span><span class="op">(</span><span class="nam">typing</span><span class="op">.</span><span class="nam">TypedDict</span><span class="op">,</span> <span class="nam">total</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">    <span class="nam">allowed_types</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="nam">migrate</span><span class="op">:</span> <span class="nam">bool</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t"><span class="key">class</span> <span class="nam">Identity</span><span class="op">(</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Protocol</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">    <span class="nam">object_id</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">    <span class="nam">object_type</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="nam">created</span><span class="op">:</span> <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">    <span class="nam">email</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">    <span class="nam">firstname</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="nam">fullname</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">    <span class="nam">encoded_password</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t"><span class="key">def</span> <span class="nam">define_auth_rbac_model</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">other_args</span><span class="op">:</span> <span class="nam">RbacKwargs</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">    <span class="nam">migrate</span> <span class="op">=</span> <span class="nam">other_args</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"migrate"</span><span class="op">,</span> <span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="str">"identity"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">        <span class="com"># std uuid from uuid libs are 36 chars long</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"object_id"</span><span class="op">,</span> <span class="str">"string"</span><span class="op">,</span> <span class="nam">length</span><span class="op">=</span><span class="num">36</span><span class="op">,</span> <span class="nam">unique</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">notnull</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">str</span><span class="op">(</span><span class="nam">uuid</span><span class="op">.</span><span class="nam">uuid4</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"object_type"</span><span class="op">,</span> <span class="str">"string"</span><span class="op">,</span> <span class="nam">requires</span><span class="op">=</span><span class="op">(</span><span class="nam">IS_IN_LIST</span><span class="op">(</span><span class="nam">other_args</span><span class="op">[</span><span class="str">"allowed_types"</span><span class="op">]</span><span class="op">)</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"created"</span><span class="op">,</span> <span class="str">"datetime"</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="com"># email needn't be unique, groups can share email addresses, and with people too</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"email"</span><span class="op">,</span> <span class="str">"string"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"firstname"</span><span class="op">,</span> <span class="str">"string"</span><span class="op">,</span> <span class="nam">comment</span><span class="op">=</span><span class="str">"also used as short code for groups"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"fullname"</span><span class="op">,</span> <span class="str">"string"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"encoded_password"</span><span class="op">,</span> <span class="str">"string"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">        <span class="nam">migrate</span><span class="op">=</span><span class="nam">migrate</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="str">"membership"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="com"># beide zijn eigenlijk: reference:identity.object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"subject"</span><span class="op">,</span> <span class="str">"string"</span><span class="op">,</span> <span class="nam">length</span><span class="op">=</span><span class="num">36</span><span class="op">,</span> <span class="nam">notnull</span><span class="op">=</span><span class="key">True</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"member_of"</span><span class="op">,</span> <span class="str">"string"</span><span class="op">,</span> <span class="nam">length</span><span class="op">=</span><span class="num">36</span><span class="op">,</span> <span class="nam">notnull</span><span class="op">=</span><span class="key">True</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="com"># Field('starts','datetime', default=DEFAULT_STARTS),</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="com"># Field('ends','datetime', default=DEFAULT_ENDS),</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="nam">migrate</span><span class="op">=</span><span class="nam">migrate</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="str">"permission"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"privilege"</span><span class="op">,</span> <span class="str">"string"</span><span class="op">,</span> <span class="nam">length</span><span class="op">=</span><span class="num">20</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="com"># reference:identity.object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"identity_object_id"</span><span class="op">,</span> <span class="str">"string"</span><span class="op">,</span> <span class="nam">length</span><span class="op">=</span><span class="num">36</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"target_object_id"</span><span class="op">,</span> <span class="str">"string"</span><span class="op">,</span> <span class="nam">length</span><span class="op">=</span><span class="num">36</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="com"># Field('scope'), lets bail scope for now. every one needs a rule for everything</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="com"># just to make sure, no 'wildcards' and 'every dossier for org x' etc ...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"starts"</span><span class="op">,</span> <span class="nam">type</span><span class="op">=</span><span class="nam">my_datetime</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">DEFAULT_STARTS</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"ends"</span><span class="op">,</span> <span class="nam">type</span><span class="op">=</span><span class="nam">my_datetime</span><span class="op">,</span> <span class="nam">default</span><span class="op">=</span><span class="nam">DEFAULT_ENDS</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">        <span class="nam">migrate</span><span class="op">=</span><span class="nam">migrate</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">        <span class="str">"recursive_memberships"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"root"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"object_id"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"object_type"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"level"</span><span class="op">,</span> <span class="str">"integer"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"email"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"firstname"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"fullname"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">        <span class="nam">migrate</span><span class="op">=</span><span class="key">False</span><span class="op">,</span>  <span class="com"># view</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="nam">primarykey</span><span class="op">=</span><span class="op">[</span><span class="str">"root"</span><span class="op">,</span> <span class="str">"object_id"</span><span class="op">]</span><span class="op">,</span>  <span class="com"># composed, no primary key</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="str">"recursive_members"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"root"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"object_id"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"object_type"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"level"</span><span class="op">,</span> <span class="str">"integer"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"email"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"firstname"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">        <span class="nam">Field</span><span class="op">(</span><span class="str">"fullname"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">        <span class="nam">migrate</span><span class="op">=</span><span class="key">False</span><span class="op">,</span>  <span class="com"># view</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">        <span class="nam">primarykey</span><span class="op">=</span><span class="op">[</span><span class="str">"root"</span><span class="op">,</span> <span class="str">"object_id"</span><span class="op">]</span><span class="op">,</span>  <span class="com"># composed, no primary key</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t"><span class="key">def</span> <span class="nam">add_identity</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">    <span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">    <span class="nam">email</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">    <span class="nam">member_of</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">IdentityKey</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">    <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="nam">firstname</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">    <span class="nam">fullname</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">    <span class="nam">password</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">    <span class="nam">gid</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">UUID</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">    <span class="nam">object_type</span><span class="op">:</span> <span class="nam">ObjectTypes</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">    <span class="str">"""paramaters name and firstname are equal."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">    <span class="nam">email</span> <span class="op">=</span> <span class="nam">email</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">    <span class="key">if</span> <span class="nam">object_type</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"object_type parameter expected"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">    <span class="nam">object_id</span> <span class="op">=</span> <span class="nam">gid</span> <span class="key">if</span> <span class="nam">gid</span> <span class="key">else</span> <span class="nam">uuid</span><span class="op">.</span><span class="nam">uuid4</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">validate_and_insert</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">        <span class="nam">object_id</span><span class="op">=</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">        <span class="nam">object_type</span><span class="op">=</span><span class="nam">object_type</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">        <span class="nam">email</span><span class="op">=</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">        <span class="nam">firstname</span><span class="op">=</span><span class="nam">name</span> <span class="key">or</span> <span class="nam">firstname</span> <span class="key">or</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">        <span class="nam">fullname</span><span class="op">=</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">        <span class="nam">encoded_password</span><span class="op">=</span><span class="nam">Password</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="nam">password</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span> <span class="key">in</span> <span class="nam">member_of</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">        <span class="nam">group_id</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="str">"group"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">        <span class="key">if</span> <span class="nam">get_group</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">group_id</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">            <span class="com"># check each group if it exists.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">            <span class="nam">add_membership</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">=</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">=</span><span class="nam">group_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">    <span class="key">return</span> <span class="nam">str</span><span class="op">(</span><span class="nam">object_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t"><span class="key">def</span> <span class="nam">authenticate_user</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">password</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">user</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">password</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">user</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">        <span class="nam">user</span> <span class="op">=</span> <span class="nam">get_user</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">    <span class="key">return</span> <span class="nam">Password</span><span class="op">.</span><span class="nam">validate</span><span class="op">(</span><span class="nam">password</span><span class="op">,</span> <span class="nam">user</span><span class="op">.</span><span class="nam">encoded_password</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t"><span class="key">def</span> <span class="nam">add_membership</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">    <span class="nam">identity_oid</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">    <span class="key">if</span> <span class="nam">identity_oid</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">'invalid identity_oid key: '</span> <span class="op">+</span> <span class="nam">identity_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">    <span class="nam">group</span> <span class="op">=</span> <span class="nam">get_group</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">group</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">'invalid group key: '</span> <span class="op">+</span> <span class="nam">group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">subject</span> <span class="op">==</span> <span class="nam">identity_oid</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">member_of</span> <span class="op">==</span> <span class="nam">group</span><span class="op">.</span><span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">    <span class="key">if</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">count</span><span class="op">(</span><span class="op">)</span> <span class="op">==</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">        <span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">validate_and_insert</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">            <span class="nam">subject</span><span class="op">=</span><span class="nam">identity_oid</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">            <span class="nam">member_of</span><span class="op">=</span><span class="nam">group</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t"><span class="key">def</span> <span class="nam">remove_membership</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">    <span class="nam">identity</span> <span class="op">=</span> <span class="nam">get_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">    <span class="nam">group</span> <span class="op">=</span> <span class="nam">get_group</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">subject</span> <span class="op">==</span> <span class="nam">identity</span><span class="op">.</span><span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">member_of</span> <span class="op">==</span> <span class="nam">group</span><span class="op">.</span><span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">    <span class="nam">deleted</span> <span class="op">=</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">    <span class="key">return</span> <span class="nam">deleted</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t"><span class="key">def</span> <span class="nam">get_memberships</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">,</span> <span class="nam">bare</span><span class="op">=</span><span class="key">True</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">recursive_memberships</span><span class="op">.</span><span class="nam">root</span> <span class="op">==</span> <span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">    <span class="nam">fields</span> <span class="op">=</span> <span class="op">[</span><span class="nam">db</span><span class="op">.</span><span class="nam">recursive_memberships</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">db</span><span class="op">.</span><span class="nam">recursive_memberships</span><span class="op">.</span><span class="nam">object_type</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">bare</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">        <span class="nam">fields</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="key">return</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span><span class="op">*</span><span class="nam">fields</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t"><span class="key">def</span> <span class="nam">get_members</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">,</span> <span class="nam">bare</span><span class="op">=</span><span class="key">True</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">recursive_members</span><span class="op">.</span><span class="nam">root</span> <span class="op">==</span> <span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">    <span class="nam">fields</span> <span class="op">=</span> <span class="op">[</span><span class="nam">db</span><span class="op">.</span><span class="nam">recursive_members</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">db</span><span class="op">.</span><span class="nam">recursive_members</span><span class="op">.</span><span class="nam">object_type</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">bare</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">        <span class="nam">fields</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">    <span class="key">return</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span><span class="op">*</span><span class="nam">fields</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t"><span class="key">def</span> <span class="nam">add_permission</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">starts</span><span class="op">=</span><span class="nam">DEFAULT_STARTS</span><span class="op">,</span> <span class="nam">ends</span><span class="op">=</span><span class="nam">DEFAULT_ENDS</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">    <span class="nam">identity_oid</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">    <span class="nam">starts</span> <span class="op">=</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">starts</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">    <span class="nam">ends</span> <span class="op">=</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">ends</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">    <span class="key">if</span> <span class="nam">has_permission</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_oid</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">when</span><span class="op">=</span><span class="nam">starts</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">        <span class="com"># permission already granted. just skip it</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">            <span class="str">'{privilege} permission already granted to {user_or_group_key} on {target_oid} @ {starts} '</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">                <span class="op">**</span><span class="nam">locals</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">        <span class="com"># print(db._lastsql)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">permission</span><span class="op">.</span><span class="nam">validate_and_insert</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">        <span class="nam">privilege</span><span class="op">=</span><span class="nam">privilege</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">        <span class="nam">identity_object_id</span><span class="op">=</span><span class="nam">identity_oid</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">        <span class="nam">target_object_id</span><span class="op">=</span><span class="nam">target_oid</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">        <span class="nam">starts</span><span class="op">=</span><span class="nam">starts</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">        <span class="nam">ends</span><span class="op">=</span><span class="nam">ends</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t"><span class="key">def</span> <span class="nam">remove_permission</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">when</span><span class="op">=</span><span class="nam">DEFAULT</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">    <span class="nam">identity_oid</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">    <span class="key">if</span> <span class="nam">when</span> <span class="key">is</span> <span class="nam">DEFAULT</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">        <span class="nam">when</span> <span class="op">=</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">        <span class="nam">when</span> <span class="op">=</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">when</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">    <span class="com"># base object is is the root to check for, user or group</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">    <span class="nam">permission</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">permission</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">identity_object_id</span> <span class="op">==</span> <span class="nam">identity_oid</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">target_object_id</span> <span class="op">==</span> <span class="nam">target_oid</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">privilege</span> <span class="op">==</span> <span class="nam">privilege</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">starts</span> <span class="op">&lt;=</span> <span class="nam">when</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">ends</span> <span class="op">>=</span> <span class="nam">when</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">    <span class="nam">result</span> <span class="op">=</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="op">)</span> <span class="op">></span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">    <span class="com"># print(db._lastsql)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t"><span class="key">def</span> <span class="nam">with_alias</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">source</span><span class="op">,</span> <span class="nam">alias</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">    <span class="nam">other</span> <span class="op">=</span> <span class="nam">copy</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="nam">source</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">    <span class="nam">other</span><span class="op">[</span><span class="str">'ALL'</span><span class="op">]</span> <span class="op">=</span> <span class="nam">SQLALL</span><span class="op">(</span><span class="nam">other</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">    <span class="nam">other</span><span class="op">[</span><span class="str">'_tablename'</span><span class="op">]</span> <span class="op">=</span> <span class="nam">alias</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">    <span class="key">for</span> <span class="nam">fieldname</span> <span class="key">in</span> <span class="nam">other</span><span class="op">.</span><span class="nam">fields</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">        <span class="nam">tmp</span> <span class="op">=</span> <span class="nam">source</span><span class="op">[</span><span class="nam">fieldname</span><span class="op">]</span><span class="op">.</span><span class="nam">clone</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">        <span class="nam">tmp</span><span class="op">.</span><span class="nam">bind</span><span class="op">(</span><span class="nam">other</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">        <span class="nam">other</span><span class="op">[</span><span class="nam">fieldname</span><span class="op">]</span> <span class="op">=</span> <span class="nam">tmp</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">    <span class="key">if</span> <span class="str">'id'</span> <span class="key">in</span> <span class="nam">source</span> <span class="key">and</span> <span class="str">'id'</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">other</span><span class="op">.</span><span class="nam">fields</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">        <span class="nam">other</span><span class="op">[</span><span class="str">'id'</span><span class="op">]</span> <span class="op">=</span> <span class="nam">other</span><span class="op">[</span><span class="nam">source</span><span class="op">.</span><span class="nam">id</span><span class="op">.</span><span class="nam">name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">    <span class="key">if</span> <span class="nam">source_id</span> <span class="op">:=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">source</span><span class="op">,</span> <span class="str">"_id"</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">        <span class="nam">other</span><span class="op">.</span><span class="nam">_id</span> <span class="op">=</span> <span class="nam">other</span><span class="op">[</span><span class="nam">source_id</span><span class="op">.</span><span class="nam">name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">    <span class="nam">db</span><span class="op">[</span><span class="nam">alias</span><span class="op">]</span> <span class="op">=</span> <span class="nam">other</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">    <span class="key">return</span> <span class="nam">other</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t"><span class="key">def</span> <span class="nam">has_permission</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">user_or_group_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">when</span><span class="op">=</span><span class="nam">DEFAULT</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">    <span class="nam">user_or_group_oid</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">user_or_group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">    <span class="com"># the permission system</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">    <span class="key">if</span> <span class="nam">when</span> <span class="key">is</span> <span class="nam">DEFAULT</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">        <span class="nam">when</span> <span class="op">=</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">        <span class="nam">when</span> <span class="op">=</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">when</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="com"># base object is is the root to check for, user or group</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">    <span class="nam">root_oid</span> <span class="op">=</span> <span class="nam">user_or_group_oid</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">    <span class="nam">permission</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">permission</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">    <span class="com"># ugly hack to satisfy pydal aliasing keyed tables /views</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">    <span class="nam">left</span> <span class="op">=</span> <span class="nam">with_alias</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">db</span><span class="op">.</span><span class="nam">recursive_memberships</span><span class="op">,</span> <span class="str">'left'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="nam">right</span> <span class="op">=</span> <span class="nam">with_alias</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">db</span><span class="op">.</span><span class="nam">recursive_memberships</span><span class="op">,</span> <span class="str">'right'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">    <span class="com"># left = db.recursive_memberships.with_alias('left')</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">    <span class="com"># right = db.recursive_memberships.with_alias('right')</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">    <span class="com"># end of ugly hack</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">left</span><span class="op">.</span><span class="nam">root</span> <span class="op">==</span> <span class="nam">root_oid</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">right</span><span class="op">.</span><span class="nam">root</span> <span class="op">==</span> <span class="nam">target_oid</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">identity_object_id</span> <span class="op">==</span> <span class="nam">left</span><span class="op">.</span><span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">target_object_id</span> <span class="op">==</span> <span class="nam">right</span><span class="op">.</span><span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">privilege</span> <span class="op">==</span> <span class="nam">privilege</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">starts</span> <span class="op">&lt;=</span> <span class="nam">when</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">ends</span> <span class="op">>=</span> <span class="nam">when</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">    <span class="key">return</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">count</span><span class="op">(</span><span class="op">)</span> <span class="op">></span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t"><span class="key">def</span> <span class="nam">add_group</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">email</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">IdentityKey</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">    <span class="key">return</span> <span class="nam">add_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">,</span> <span class="nam">name</span><span class="op">=</span><span class="nam">name</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="str">"group"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="key">def</span> <span class="nam">remove_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">    <span class="nam">removed</span> <span class="op">=</span> <span class="nam">db</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">object_id</span> <span class="op">==</span> <span class="nam">object_id</span><span class="op">)</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">    <span class="com"># todo: remove permissions and group memberships</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">    <span class="key">return</span> <span class="nam">removed</span> <span class="op">></span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t"><span class="key">def</span> <span class="nam">get_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">:</span> <span class="nam">ObjectTypes</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t"><span class="str">    :param db: dal db connection</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t"><span class="str">    :param key: can be the email, id, or object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t"><span class="str">    :return: user record or None when not found</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">key_lookup_query</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">    <span class="nam">rows</span> <span class="op">=</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">    <span class="key">return</span> <span class="nam">rows</span><span class="op">.</span><span class="nam">first</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="key">def</span> <span class="nam">get_user</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t"><span class="str">    :param db: dal db connection</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t"><span class="str">    :param key: can be the email, id, or object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t"><span class="str">    :return: user record or None when not found</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">    <span class="key">return</span> <span class="nam">get_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="str">"user"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t"><span class="key">def</span> <span class="nam">get_group</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t"><span class="str">    :param db: dal db connection</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="str">    :param key: can be the name of the group, the id, object_id or email_address</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t"><span class="str">    :return: user record or None when not found</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">    <span class="key">return</span> <span class="nam">get_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="str">"group"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t"><span class="key">def</span> <span class="nam">authenticate_user</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">password</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">user</span><span class="op">:</span> <span class="nam">Identity</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">IdentityKey</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">password</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">user</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">        <span class="nam">user</span> <span class="op">=</span> <span class="nam">get_user</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">    <span class="key">return</span> <span class="nam">Password</span><span class="op">.</span><span class="nam">validate</span><span class="op">(</span><span class="nam">password</span><span class="op">,</span> <span class="nam">user</span><span class="op">.</span><span class="nam">encoded_password</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t"><span class="key">def</span> <span class="nam">add_membership</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">    <span class="nam">identity_oid</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">    <span class="key">if</span> <span class="nam">identity_oid</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"invalid identity_oid key: "</span> <span class="op">+</span> <span class="nam">identity_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">    <span class="nam">group</span> <span class="op">=</span> <span class="nam">get_group</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">group</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"invalid group key: "</span> <span class="op">+</span> <span class="nam">group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">subject</span> <span class="op">==</span> <span class="nam">identity_oid</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">member_of</span> <span class="op">==</span> <span class="nam">group</span><span class="op">.</span><span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">    <span class="key">if</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">count</span><span class="op">(</span><span class="op">)</span> <span class="op">==</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">        <span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">validate_and_insert</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">            <span class="nam">subject</span><span class="op">=</span><span class="nam">identity_oid</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">            <span class="nam">member_of</span><span class="op">=</span><span class="nam">group</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t"><span class="key">def</span> <span class="nam">remove_membership</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">    <span class="nam">identity</span> <span class="op">=</span> <span class="nam">get_identity</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">    <span class="nam">group</span> <span class="op">=</span> <span class="nam">get_group</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">subject</span> <span class="op">==</span> <span class="nam">identity</span><span class="op">.</span><span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">member_of</span> <span class="op">==</span> <span class="nam">group</span><span class="op">.</span><span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">    <span class="nam">deleted</span> <span class="op">=</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">    <span class="key">return</span> <span class="nam">deleted</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t"><span class="key">def</span> <span class="nam">get_memberships</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span> <span class="nam">bare</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">recursive_memberships</span><span class="op">.</span><span class="nam">root</span> <span class="op">==</span> <span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">    <span class="nam">fields</span> <span class="op">=</span> <span class="op">[</span><span class="nam">db</span><span class="op">.</span><span class="nam">recursive_memberships</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">db</span><span class="op">.</span><span class="nam">recursive_memberships</span><span class="op">.</span><span class="nam">object_type</span><span class="op">]</span> <span class="key">if</span> <span class="nam">bare</span> <span class="key">else</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">    <span class="key">return</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span><span class="op">*</span><span class="nam">fields</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t"><span class="key">def</span> <span class="nam">get_members</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span> <span class="nam">bare</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">recursive_members</span><span class="op">.</span><span class="nam">root</span> <span class="op">==</span> <span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">    <span class="nam">fields</span> <span class="op">=</span> <span class="op">[</span><span class="nam">db</span><span class="op">.</span><span class="nam">recursive_members</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">db</span><span class="op">.</span><span class="nam">recursive_members</span><span class="op">.</span><span class="nam">object_type</span><span class="op">]</span> <span class="key">if</span> <span class="nam">bare</span> <span class="key">else</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">    <span class="key">return</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span><span class="op">*</span><span class="nam">fields</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t"><span class="key">def</span> <span class="nam">add_permission</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">    <span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">    <span class="nam">identity_key</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">    <span class="nam">target_oid</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">    <span class="nam">privilege</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">    <span class="nam">starts</span><span class="op">:</span> <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span> <span class="op">|</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">DEFAULT_STARTS</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">    <span class="nam">ends</span><span class="op">:</span> <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span> <span class="op">|</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">DEFAULT_ENDS</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">    <span class="nam">identity_oid</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">    <span class="nam">starts</span> <span class="op">=</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">starts</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">    <span class="nam">ends</span> <span class="op">=</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">ends</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">    <span class="key">if</span> <span class="nam">has_permission</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_oid</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">when</span><span class="op">=</span><span class="nam">starts</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">        <span class="com"># permission already granted. just skip it</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">            <span class="str">"{privilege} permission already granted to {user_or_group_key} on {target_oid} @ {starts} "</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">                <span class="op">**</span><span class="nam">locals</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">        <span class="com"># print(db._lastsql)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">permission</span><span class="op">.</span><span class="nam">validate_and_insert</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">        <span class="nam">privilege</span><span class="op">=</span><span class="nam">privilege</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">        <span class="nam">identity_object_id</span><span class="op">=</span><span class="nam">identity_oid</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">        <span class="nam">target_object_id</span><span class="op">=</span><span class="nam">target_oid</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">        <span class="nam">starts</span><span class="op">=</span><span class="nam">starts</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">        <span class="nam">ends</span><span class="op">=</span><span class="nam">ends</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t"><span class="key">def</span> <span class="nam">remove_permission</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">    <span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">when</span><span class="op">:</span> <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span> <span class="op">|</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">DEFAULT</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="nam">identity_oid</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">    <span class="key">if</span> <span class="nam">when</span> <span class="key">is</span> <span class="nam">DEFAULT</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">        <span class="nam">when</span> <span class="op">=</span> <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">        <span class="nam">when</span> <span class="op">=</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">when</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">    <span class="com"># base object is is the root to check for, user or group</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">    <span class="nam">permission</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">permission</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">identity_object_id</span> <span class="op">==</span> <span class="nam">identity_oid</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">target_object_id</span> <span class="op">==</span> <span class="nam">target_oid</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">privilege</span> <span class="op">==</span> <span class="nam">privilege</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">starts</span> <span class="op">&lt;=</span> <span class="nam">when</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">ends</span> <span class="op">>=</span> <span class="nam">when</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">    <span class="nam">result</span> <span class="op">=</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="op">)</span> <span class="op">></span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">    <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">    <span class="com"># print(db._lastsql)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t"><span class="key">def</span> <span class="nam">with_alias</span><span class="op">(</span><span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">source</span><span class="op">:</span> <span class="nam">Table</span><span class="op">,</span> <span class="nam">alias</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">    <span class="nam">other</span> <span class="op">=</span> <span class="nam">copy</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="nam">source</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">    <span class="nam">other</span><span class="op">[</span><span class="str">"ALL"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">SQLALL</span><span class="op">(</span><span class="nam">other</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">    <span class="nam">other</span><span class="op">[</span><span class="str">"_tablename"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">alias</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">    <span class="key">for</span> <span class="nam">fieldname</span> <span class="key">in</span> <span class="nam">other</span><span class="op">.</span><span class="nam">fields</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">        <span class="nam">tmp</span> <span class="op">=</span> <span class="nam">source</span><span class="op">[</span><span class="nam">fieldname</span><span class="op">]</span><span class="op">.</span><span class="nam">clone</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">        <span class="nam">tmp</span><span class="op">.</span><span class="nam">bind</span><span class="op">(</span><span class="nam">other</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">        <span class="nam">other</span><span class="op">[</span><span class="nam">fieldname</span><span class="op">]</span> <span class="op">=</span> <span class="nam">tmp</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">    <span class="key">if</span> <span class="str">"id"</span> <span class="key">in</span> <span class="nam">source</span> <span class="key">and</span> <span class="str">"id"</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">other</span><span class="op">.</span><span class="nam">fields</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">        <span class="nam">other</span><span class="op">[</span><span class="str">"id"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">other</span><span class="op">[</span><span class="nam">source</span><span class="op">.</span><span class="nam">id</span><span class="op">.</span><span class="nam">name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">    <span class="key">if</span> <span class="nam">source_id</span> <span class="op">:=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">source</span><span class="op">,</span> <span class="str">"_id"</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">        <span class="nam">other</span><span class="op">.</span><span class="nam">_id</span> <span class="op">=</span> <span class="nam">other</span><span class="op">[</span><span class="nam">source_id</span><span class="op">.</span><span class="nam">name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">    <span class="nam">db</span><span class="op">[</span><span class="nam">alias</span><span class="op">]</span> <span class="op">=</span> <span class="nam">other</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="key">return</span> <span class="nam">other</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t"><span class="key">def</span> <span class="nam">has_permission</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">    <span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">,</span> <span class="nam">user_or_group_key</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">:</span> <span class="nam">IdentityKey</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">when</span><span class="op">:</span> <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span> <span class="op">|</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">DEFAULT</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">    <span class="nam">user_or_group_oid</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">user_or_group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">    <span class="com"># the permission system</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">    <span class="key">if</span> <span class="nam">when</span> <span class="key">is</span> <span class="nam">DEFAULT</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">        <span class="nam">when</span> <span class="op">=</span> <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">        <span class="nam">when</span> <span class="op">=</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">when</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">    <span class="com"># base object is is the root to check for, user or group</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">    <span class="nam">root_oid</span> <span class="op">=</span> <span class="nam">user_or_group_oid</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">    <span class="nam">permission</span> <span class="op">=</span> <span class="nam">db</span><span class="op">.</span><span class="nam">permission</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">    <span class="com"># ugly hack to satisfy pydal aliasing keyed tables /views</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">    <span class="nam">left</span> <span class="op">=</span> <span class="nam">with_alias</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">db</span><span class="op">.</span><span class="nam">recursive_memberships</span><span class="op">,</span> <span class="str">"left"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">    <span class="nam">right</span> <span class="op">=</span> <span class="nam">with_alias</span><span class="op">(</span><span class="nam">db</span><span class="op">,</span> <span class="nam">db</span><span class="op">.</span><span class="nam">recursive_memberships</span><span class="op">,</span> <span class="str">"right"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">    <span class="com"># left = db.recursive_memberships.with_alias('left')</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">    <span class="com"># right = db.recursive_memberships.with_alias('right')</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">    <span class="com"># end of ugly hack</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">    <span class="nam">query</span> <span class="op">=</span> <span class="nam">left</span><span class="op">.</span><span class="nam">root</span> <span class="op">==</span> <span class="nam">root_oid</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">right</span><span class="op">.</span><span class="nam">root</span> <span class="op">==</span> <span class="nam">target_oid</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">identity_object_id</span> <span class="op">==</span> <span class="nam">left</span><span class="op">.</span><span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">target_object_id</span> <span class="op">==</span> <span class="nam">right</span><span class="op">.</span><span class="nam">object_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">privilege</span> <span class="op">==</span> <span class="nam">privilege</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">starts</span> <span class="op">&lt;=</span> <span class="nam">when</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="nam">query</span> <span class="op">&amp;=</span> <span class="nam">permission</span><span class="op">.</span><span class="nam">ends</span> <span class="op">>=</span> <span class="nam">when</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">    <span class="key">return</span> <span class="nam">db</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span><span class="op">.</span><span class="nam">count</span><span class="op">(</span><span class="op">)</span> <span class="op">></span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="z_438b44bce6437be6_migrations_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="z_438b44bce6437be6_rbac_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,381 +1,434 @@
-************ CCoovveerraaggee ffoorr ssrrcc//eeddwwhh__aauutthh__rrbbaacc//mmooddeell..ppyy:: 7766%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//eeddwwhh__aauutthh__rrbbaacc//mmooddeell..ppyy:: 7788%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 118833 ssttaatteemmeennttss ?  113399 rruunn 4444 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 119955 ssttaatteemmeennttss ?  115533 rruunn 4422 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
 _1import copy 
-_2import datetime 
+_2import datetime as dt 
 _3import hashlib 
 _4import hmac 
-_5import uuid 
-_6 
-_7import dateutil.parser 
-_8from pydal import Field 
-_9from pydal import SQLCustomType 
-_1_0from pydal.objects import SQLALL, Query 
-_1_1 
-_1_2from .helpers import IS_IN_LIST 
+_5import typing 
+_6import uuid 
+_7from typing import Optional 
+_8from uuid import UUID 
+_9 
+_1_0import dateutil.parser 
+_1_1from pydal import DAL, Field, SQLCustomType 
+_1_2from pydal.objects import SQLALL, Query, Table 
 _1_3 
-_1_4 
-_1_5class DEFAULT: 
-_1_6 pass 
-_1_7 
-_1_8 
-_1_9DEFAULT_STARTS = datetime.datetime(2000, 1, 1) 
-_2_0DEFAULT_ENDS = datetime.datetime(3000, 1, 1) 
-_2_1 
-_2_2 
-_2_3def unstr_datetime(s): 
-_2_4 """json helper... might values arrive as str """ 
-_2_5 return dateutil.parser.parse(s) if isinstance(s, str) else s 
-_2_6 
-_2_7 
-_2_8class Password: 
-_2_9 """ 
-_3_0 Encode a password using: Password.encode('secret') 
+_1_4from .helpers import IS_IN_LIST 
+_1_5 
+_1_6 
+_1_7class DEFAULT: 
+_1_8 pass 
+_1_9 
+_2_0 
+_2_1DEFAULT_STARTS = dt.datetime(2000, 1, 1) 
+_2_2DEFAULT_ENDS = dt.datetime(3000, 1, 1) 
+_2_3 
+_2_4 
+_2_5def unstr_datetime(s: dt.datetime | str) -> dt.datetime: 
+_2_6 """json helper... might values arrive as str""" 
+_2_7 return dateutil.parser.parse(s) if isinstance(s, str) else s 
+_2_8 
+_2_9 
+_3_0class Password: 
 _3_1 """ 
-_3_2 
-_3_3 @classmethod 
-_3_4 def hmac_hash(cls, value, key, salt=None): 
-_3_5 digest_alg = hashlib.sha512 
-_3_6 d = hmac.new(str(key).encode(), str(value).encode(), digest_alg) 
-_3_7 if salt: 
-_3_8 d.update(str(salt).encode()) 
-_3_9 return d.hexdigest() 
-_4_0 
-_4_1 @classmethod 
-_4_2 def validate(cls, password, candidate): 
-_4_3 salt, hashed = candidate.split(':', 1) 
-_4_4 return cls.hmac_hash(value=password, key='secret_start', salt=salt) ==
+_3_2 Encode a password using: Password.encode('secret') 
+_3_3 """ 
+_3_4 
+_3_5 @classmethod 
+_3_6 def hmac_hash(cls, value: str, key: str, salt: str = None) -> str: 
+_3_7 digest_alg = hashlib.sha512 
+_3_8 d = hmac.new(str(key).encode(), str(value).encode(), digest_alg) 
+_3_9 if salt: 
+_4_0 d.update(str(salt).encode()) 
+_4_1 return d.hexdigest() 
+_4_2 
+_4_3 @classmethod 
+_4_4 def validate(cls, password: str, candidate: str) -> bool: 
+_4_5 salt, hashed = candidate.split(":", 1) 
+_4_6 return cls.hmac_hash(value=password, key="secret_start", salt=salt) ==
 hashed 
-_4_5 
-_4_6 @classmethod 
-_4_7 def encode(cls, password): 
-_4_8 salt = uuid.uuid4().hex 
-_4_9 return salt + ':' + cls.hmac_hash(value=password, key='secret_start',
+_4_7 
+_4_8 @classmethod 
+_4_9 def encode(cls, password: str) -> str: 
+_5_0 salt = uuid.uuid4().hex 
+_5_1 return salt + ":" + cls.hmac_hash(value=password, key="secret_start",
 salt=salt) 
-_5_0 
-_5_1 
-_5_2def is_uuid(s): 
-_5_3 try: 
-_5_4 uuid.UUID(s) 
-_5_5 return True 
-_5_6 except Exception: 
-_5_7 return False 
-_5_8 
-_5_9 
-_6_0def key_lookup_query(db, identity_key: str | int | uuid.UUID,
-object_type=None) -> Query: 
-_6_1 if '@' in str(identity_key): 
-_6_2 query = db.identity.email == identity_key.lower() 
-_6_3 elif isinstance(identity_key, int): 
-_6_4 query = db.identity.id == identity_key 
-_6_5 elif is_uuid(identity_key): 
-_6_6 query = db.identity.object_id == identity_key.lower() 
-_6_7 else: 
-_6_8 query = db.identity.firstname == identity_key 
-_6_9 
-_7_0 if object_type: 
-_7_1 query &= db.identity.object_type == object_type 
-_7_2 
-_7_3 return query 
-_7_4 
+_5_2 
+_5_3 
+_5_4def is_uuid(s) -> bool: 
+_5_5 try: 
+_5_6 UUID(s) 
+_5_7 return True 
+_5_8 except Exception: 
+_5_9 return False 
+_6_0 
+_6_1 
+_6_2IdentityKey: typing.TypeAlias = str | int | UUID 
+_6_3ObjectTypes = typing.Literal["user", "group", "item"] 
+_6_4 
+_6_5 
+_6_6def key_lookup_query(db: DAL, identity_key: IdentityKey, object_type:
+ObjectTypes = None) -> Query: 
+_6_7 if "@" in str(identity_key): 
+_6_8 query = db.identity.email == identity_key.lower() 
+_6_9 elif isinstance(identity_key, int): 
+_7_0 query = db.identity.id == identity_key 
+_7_1 elif is_uuid(identity_key): 
+_7_2 query = db.identity.object_id == identity_key.lower() 
+_7_3 else: 
+_7_4 query = db.identity.firstname == identity_key 
 _7_5 
-_7_6def key_lookup(db, identity_key, object_type=None) -> str | None: 
-_7_7 query = key_lookup_query(db, identity_key, object_type) 
+_7_6 if object_type: 
+_7_7 query &= db.identity.object_type == object_type 
 _7_8 
-_7_9 rowset = db(query).select(db.identity.object_id) 
+_7_9 return query 
 _8_0 
-_8_1 if not rowset: 
-_8_2 return None 
-_8_3 elif len(rowset) > 1: 
-_8_4 raise ValueError('Keep lookup for {} returned {} results.'.format
+_8_1 
+_8_2def key_lookup(db: DAL, identity_key: IdentityKey, object_type: ObjectTypes =
+None) -> str | None: 
+_8_3 query = key_lookup_query(db, identity_key, object_type) 
+_8_4 
+_8_5 rowset = db(query).select(db.identity.object_id) 
+_8_6 
+_8_7 if not rowset: 
+_8_8 return None 
+_8_9 elif len(rowset) > 1: 
+_9_0 raise ValueError("Keep lookup for {} returned {} results.".format
 (identity_key, len(rowset))) 
-_8_5 
-_8_6 return rowset.first().object_id 
-_8_7 
-_8_8 
-_8_9my_datetime = SQLCustomType(type='string', 
-_9_0 native='char(35)', 
-_9_1 encoder=(lambda x: x.isoformat(' ')), 
-_9_2 decoder=(lambda x: dateutil.parser.parse(x))) 
+_9_1 
+_9_2 return rowset.first().object_id 
 _9_3 
 _9_4 
-_9_5def define_auth_rbac_model(db, other_args): 
-_9_6 db.define_table('identity', 
-_9_7 # std uuid from uuid libs are 36 chars long 
-_9_8 Field('object_id', 'string', length=36, unique=True, notnull=True,
+_9_5my_datetime = SQLCustomType( 
+_9_6 type="string", native="char(35)", encoder=(lambda x: x.isoformat(" ")),
+decoder=(lambda x: dateutil.parser.parse(x)) 
+_9_7) 
+_9_8 
+_9_9 
+_1_0_0class RbacKwargs(typing.TypedDict, total=False): 
+_1_0_1 allowed_types: list[str] 
+_1_0_2 migrate: bool 
+_1_0_3 
+_1_0_4 
+_1_0_5class Identity(typing.Protocol): 
+_1_0_6 object_id: str 
+_1_0_7 object_type: str 
+_1_0_8 created: dt.datetime 
+_1_0_9 email: str 
+_1_1_0 firstname: str 
+_1_1_1 fullname: str 
+_1_1_2 encoded_password: str 
+_1_1_3 
+_1_1_4 
+_1_1_5def define_auth_rbac_model(db: DAL, other_args: RbacKwargs): 
+_1_1_6 migrate = other_args.get("migrate", False) 
+_1_1_7 
+_1_1_8 db.define_table( 
+_1_1_9 "identity", 
+_1_2_0 # std uuid from uuid libs are 36 chars long 
+_1_2_1 Field("object_id", "string", length=36, unique=True, notnull=True,
 default=str(uuid.uuid4())), 
-_9_9 Field('object_type', 'string', requires=(IS_IN_LIST(other_args
-['allowed_types']))), 
-_1_0_0 Field('created', 'datetime', default=datetime.datetime.now), 
-_1_0_1 # email needn't be unique, groups can share email addresses, and with
+_1_2_2 Field("object_type", "string", requires=(IS_IN_LIST(other_args
+["allowed_types"]))), 
+_1_2_3 Field("created", "datetime", default=dt.datetime.now), 
+_1_2_4 # email needn't be unique, groups can share email addresses, and with
 people too 
-_1_0_2 Field('email', 'string'), 
-_1_0_3 Field('firstname', 'string', comment='also used as short code for
-groups'), 
-_1_0_4 Field('fullname', 'string'), 
-_1_0_5 Field('encoded_password', 'string'), 
-_1_0_6 ) 
-_1_0_7 
-_1_0_8 db.define_table('membership', 
-_1_0_9 # beide zijn eigenlijk: reference:identity.object_id 
-_1_1_0 Field('subject', 'string', length=36, notnull=True), 
-_1_1_1 Field('member_of', 'string', length=36, notnull=True), 
-_1_1_2 # Field('starts','datetime', default=DEFAULT_STARTS), 
-_1_1_3 # Field('ends','datetime', default=DEFAULT_ENDS), 
-_1_1_4 ) 
-_1_1_5 
-_1_1_6 db.define_table('permission', 
-_1_1_7 Field('privilege', 'string', length=20), 
-_1_1_8 # reference:identity.object_id 
-_1_1_9 Field('identity_object_id', 'string', length=36), 
-_1_2_0 Field('target_object_id', 'string', length=36), 
-_1_2_1 # Field('scope'), lets bail scope for now. every one needs a rule for
+_1_2_5 Field("email", "string"), 
+_1_2_6 Field("firstname", "string", comment="also used as short code for
+groups"), 
+_1_2_7 Field("fullname", "string"), 
+_1_2_8 Field("encoded_password", "string"), 
+_1_2_9 migrate=migrate, 
+_1_3_0 ) 
+_1_3_1 
+_1_3_2 db.define_table( 
+_1_3_3 "membership", 
+_1_3_4 # beide zijn eigenlijk: reference:identity.object_id 
+_1_3_5 Field("subject", "string", length=36, notnull=True), 
+_1_3_6 Field("member_of", "string", length=36, notnull=True), 
+_1_3_7 # Field('starts','datetime', default=DEFAULT_STARTS), 
+_1_3_8 # Field('ends','datetime', default=DEFAULT_ENDS), 
+_1_3_9 migrate=migrate, 
+_1_4_0 ) 
+_1_4_1 
+_1_4_2 db.define_table( 
+_1_4_3 "permission", 
+_1_4_4 Field("privilege", "string", length=20), 
+_1_4_5 # reference:identity.object_id 
+_1_4_6 Field("identity_object_id", "string", length=36), 
+_1_4_7 Field("target_object_id", "string", length=36), 
+_1_4_8 # Field('scope'), lets bail scope for now. every one needs a rule for
 everything 
-_1_2_2 # just to make sure, no 'wildcards' and 'every dossier for org x' etc ... 
-_1_2_3 Field('starts', type=my_datetime, default=DEFAULT_STARTS), 
-_1_2_4 Field('ends', type=my_datetime, default=DEFAULT_ENDS), 
-_1_2_5 ) 
-_1_2_6 
-_1_2_7 db.define_table('recursive_memberships', 
-_1_2_8 Field('root'), 
-_1_2_9 Field('object_id'), 
-_1_3_0 Field('object_type'), 
-_1_3_1 Field('level', 'integer'), 
-_1_3_2 Field('email'), 
-_1_3_3 Field('firstname'), 
-_1_3_4 Field('fullname'), 
-_1_3_5 migrate=False, 
-_1_3_6 primarykey=['root', 'object_id'] # composed, no primary key 
-_1_3_7 ) 
-_1_3_8 db.define_table('recursive_members', 
-_1_3_9 Field('root'), 
-_1_4_0 Field('object_id'), 
-_1_4_1 Field('object_type'), 
-_1_4_2 Field('level', 'integer'), 
-_1_4_3 Field('email'), 
-_1_4_4 Field('firstname'), 
-_1_4_5 Field('fullname'), 
-_1_4_6 migrate=False, 
-_1_4_7 primarykey=['root', 'object_id'] # composed, no primary key 
-_1_4_8 ) 
-_1_4_9 
-_1_5_0 
-_1_5_1def add_identity(db, email, password, member_of, name=None, firstname=None,
-fullname=None, gid=None, object_type=None): 
-_1_5_2 """paramaters name and firstname are equal. """ 
-_1_5_3 email = email.lower().strip() 
-_1_5_4 if object_type is None: 
-_1_5_5 raise ValueError('object_type parameter expected') 
-_1_5_6 object_id = gid if gid else str(uuid.uuid4()) 
-_1_5_7 db.identity.validate_and_insert( 
-_1_5_8 object_id=object_id, 
-_1_5_9 object_type=object_type, 
-_1_6_0 email=email, 
-_1_6_1 firstname=name or firstname or None, 
-_1_6_2 fullname=fullname, 
-_1_6_3 encoded_password=Password.encode(password) 
-_1_6_4 ) 
-_1_6_5 db.commit() 
-_1_6_6 for key in member_of: 
-_1_6_7 group_id = key_lookup(db, key, 'group') 
-_1_6_8 if get_group(db, group_id): 
-_1_6_9 # check each group if it exists. 
-_1_7_0 add_membership(db, identity_key=object_id, group_key=group_id) 
-_1_7_1 db.commit() 
-_1_7_2 return object_id 
-_1_7_3 
-_1_7_4 
-_1_7_5def add_group(db, email, name, member_of): 
-_1_7_6 return add_identity(db, email, None, member_of, name=name,
-object_type='group') 
-_1_7_7 
-_1_7_8 
-_1_7_9def remove_identity(db, object_id): 
-_1_8_0 removed = db(db.identity.object_id == object_id).delete() 
-_1_8_1 # todo: remove permissions and group memberships 
-_1_8_2 db.commit() 
-_1_8_3 return removed > 0 
-_1_8_4 
-_1_8_5 
-_1_8_6def get_identity(db, key, object_type=None): 
-_1_8_7 """ 
-_1_8_8 :param db: dal db connection 
-_1_8_9 :param key: can be the email, id, or object_id 
-_1_9_0 :return: user record or None when not found 
-_1_9_1 """ 
-_1_9_2 query = key_lookup_query(db, key, object_type) 
-_1_9_3 rows = db(query).select() 
-_1_9_4 return rows.first() 
-_1_9_5 
-_1_9_6 
-_1_9_7def get_user(db, key): 
-_1_9_8 """ 
-_1_9_9 :param db: dal db connection 
-_2_0_0 :param key: can be the email, id, or object_id 
-_2_0_1 :return: user record or None when not found 
-_2_0_2 """ 
-_2_0_3 return get_identity(db, key, object_type='user') 
-_2_0_4 
-_2_0_5 
-_2_0_6def get_group(db, key): 
-_2_0_7 """ 
-_2_0_8 
-_2_0_9 :param db: dal db connection 
-_2_1_0 :param key: can be the name of the group, the id, object_id or
-email_address 
-_2_1_1 :return: user record or None when not found 
-_2_1_2 """ 
-_2_1_3 return get_identity(db, key, object_type='group') 
+_1_4_9 # just to make sure, no 'wildcards' and 'every dossier for org x' etc ... 
+_1_5_0 Field("starts", type=my_datetime, default=DEFAULT_STARTS), 
+_1_5_1 Field("ends", type=my_datetime, default=DEFAULT_ENDS), 
+_1_5_2 migrate=migrate, 
+_1_5_3 ) 
+_1_5_4 
+_1_5_5 db.define_table( 
+_1_5_6 "recursive_memberships", 
+_1_5_7 Field("root"), 
+_1_5_8 Field("object_id"), 
+_1_5_9 Field("object_type"), 
+_1_6_0 Field("level", "integer"), 
+_1_6_1 Field("email"), 
+_1_6_2 Field("firstname"), 
+_1_6_3 Field("fullname"), 
+_1_6_4 migrate=False, # view 
+_1_6_5 primarykey=["root", "object_id"], # composed, no primary key 
+_1_6_6 ) 
+_1_6_7 db.define_table( 
+_1_6_8 "recursive_members", 
+_1_6_9 Field("root"), 
+_1_7_0 Field("object_id"), 
+_1_7_1 Field("object_type"), 
+_1_7_2 Field("level", "integer"), 
+_1_7_3 Field("email"), 
+_1_7_4 Field("firstname"), 
+_1_7_5 Field("fullname"), 
+_1_7_6 migrate=False, # view 
+_1_7_7 primarykey=["root", "object_id"], # composed, no primary key 
+_1_7_8 ) 
+_1_7_9 
+_1_8_0 
+_1_8_1def add_identity( 
+_1_8_2 db: DAL, 
+_1_8_3 email: str, 
+_1_8_4 member_of: list[IdentityKey], 
+_1_8_5 name: str = None, 
+_1_8_6 firstname: str = None, 
+_1_8_7 fullname: str = None, 
+_1_8_8 password: str = None, 
+_1_8_9 gid: str | UUID = None, 
+_1_9_0 object_type: ObjectTypes = None, 
+_1_9_1) -> str: 
+_1_9_2 """paramaters name and firstname are equal.""" 
+_1_9_3 email = email.lower().strip() 
+_1_9_4 if object_type is None: 
+_1_9_5 raise ValueError("object_type parameter expected") 
+_1_9_6 object_id = gid if gid else uuid.uuid4() 
+_1_9_7 db.identity.validate_and_insert( 
+_1_9_8 object_id=object_id, 
+_1_9_9 object_type=object_type, 
+_2_0_0 email=email, 
+_2_0_1 firstname=name or firstname or None, 
+_2_0_2 fullname=fullname, 
+_2_0_3 encoded_password=Password.encode(password), 
+_2_0_4 ) 
+_2_0_5 db.commit() 
+_2_0_6 for key in member_of: 
+_2_0_7 group_id = key_lookup(db, key, "group") 
+_2_0_8 if get_group(db, group_id): 
+_2_0_9 # check each group if it exists. 
+_2_1_0 add_membership(db, identity_key=object_id, group_key=group_id) 
+_2_1_1 db.commit() 
+_2_1_2 return str(object_id) 
+_2_1_3 
 _2_1_4 
-_2_1_5 
-_2_1_6def authenticate_user(db, password=None, user=None, key=None): 
-_2_1_7 if not password: 
-_2_1_8 return False 
-_2_1_9 if not user: 
-_2_2_0 user = get_user(db, key) 
-_2_2_1 return Password.validate(password, user.encoded_password) 
-_2_2_2 
-_2_2_3 
-_2_2_4def add_membership(db, identity_key, group_key): 
-_2_2_5 identity_oid = key_lookup(db, identity_key) 
-_2_2_6 if identity_oid is None: 
-_2_2_7 raise ValueError('invalid identity_oid key: ' + identity_key) 
-_2_2_8 group = get_group(db, group_key) 
-_2_2_9 if not group: 
-_2_3_0 raise ValueError('invalid group key: ' + group_key) 
-_2_3_1 query = db.membership.subject == identity_oid 
-_2_3_2 query &= db.membership.member_of == group.object_id 
-_2_3_3 if db(query).count() == 0: 
-_2_3_4 db.membership.validate_and_insert( 
-_2_3_5 subject=identity_oid, 
-_2_3_6 member_of=group.object_id, 
-_2_3_7 ) 
-_2_3_8 db.commit() 
-_2_3_9 
-_2_4_0 
-_2_4_1def remove_membership(db, identity_key, group_key): 
-_2_4_2 identity = get_identity(db, identity_key) 
-_2_4_3 group = get_group(db, group_key) 
-_2_4_4 query = db.membership.subject == identity.object_id 
-_2_4_5 query &= db.membership.member_of == group.object_id 
-_2_4_6 deleted = db(query).delete() 
-_2_4_7 db.commit() 
-_2_4_8 return deleted 
-_2_4_9 
-_2_5_0 
-_2_5_1def get_memberships(db, object_id, bare=True): 
-_2_5_2 query = db.recursive_memberships.root == object_id 
-_2_5_3 fields = [db.recursive_memberships.object_id,
-db.recursive_memberships.object_type] 
-_2_5_4 if not bare: 
-_2_5_5 fields = [] 
-_2_5_6 return db(query).select(*fields) 
-_2_5_7 
-_2_5_8 
-_2_5_9def get_members(db, object_id, bare=True): 
-_2_6_0 query = db.recursive_members.root == object_id 
-_2_6_1 fields = [db.recursive_members.object_id,
-db.recursive_members.object_type] 
-_2_6_2 if not bare: 
-_2_6_3 fields = [] 
-_2_6_4 return db(query).select(*fields) 
-_2_6_5 
-_2_6_6 
-_2_6_7def add_permission(db, identity_key, target_oid, privilege,
-starts=DEFAULT_STARTS, ends=DEFAULT_ENDS): 
-_2_6_8 identity_oid = key_lookup(db, identity_key) 
-_2_6_9 starts = unstr_datetime(starts) 
-_2_7_0 ends = unstr_datetime(ends) 
-_2_7_1 if has_permission(db, identity_oid, target_oid, privilege, when=starts): 
-_2_7_2 # permission already granted. just skip it 
-_2_7_3 print( 
-_2_7_4 '{privilege} permission already granted to {user_or_group_key} on
-{target_oid} @ {starts} '.format( 
-_2_7_5 **locals())) 
-_2_7_6 # print(db._lastsql) 
-_2_7_7 return 
-_2_7_8 db.permission.validate_and_insert( 
-_2_7_9 privilege=privilege, 
-_2_8_0 identity_object_id=identity_oid, 
-_2_8_1 target_object_id=target_oid, 
-_2_8_2 starts=starts, 
-_2_8_3 ends=ends, 
-_2_8_4 ) 
-_2_8_5 db.commit() 
-_2_8_6 
-_2_8_7 
-_2_8_8def remove_permission(db, identity_key, target_oid, privilege,
-when=DEFAULT): 
-_2_8_9 identity_oid = key_lookup(db, identity_key) 
-_2_9_0 if when is DEFAULT: 
-_2_9_1 when = datetime.datetime.now() 
-_2_9_2 else: 
-_2_9_3 when = unstr_datetime(when) 
-_2_9_4 # base object is is the root to check for, user or group 
-_2_9_5 permission = db.permission 
-_2_9_6 query = permission.identity_object_id == identity_oid 
-_2_9_7 query &= permission.target_object_id == target_oid 
-_2_9_8 query &= permission.privilege == privilege 
-_2_9_9 query &= permission.starts <= when 
-_3_0_0 query &= permission.ends >= when 
-_3_0_1 result = db(query).delete() > 0 
-_3_0_2 db.commit() 
-_3_0_3 # print(db._lastsql) 
-_3_0_4 return result 
-_3_0_5 
-_3_0_6 
-_3_0_7def with_alias(db, source, alias): 
-_3_0_8 other = copy.copy(source) 
-_3_0_9 other['ALL'] = SQLALL(other) 
-_3_1_0 other['_tablename'] = alias 
-_3_1_1 for fieldname in other.fields: 
-_3_1_2 tmp = source[fieldname].clone() 
-_3_1_3 tmp.bind(other) 
-_3_1_4 other[fieldname] = tmp 
-_3_1_5 if 'id' in source and 'id' not in other.fields: 
-_3_1_6 other['id'] = other[source.id.name] 
-_3_1_7 
-_3_1_8 if source_id := getattr(source, "_id", None): 
-_3_1_9 other._id = other[source_id.name] 
-_3_2_0 db[alias] = other 
-_3_2_1 return other 
-_3_2_2 
-_3_2_3 
-_3_2_4def has_permission(db, user_or_group_key, target_oid, privilege,
-when=DEFAULT): 
-_3_2_5 user_or_group_oid = key_lookup(db, user_or_group_key) 
-_3_2_6 # the permission system 
-_3_2_7 if when is DEFAULT: 
-_3_2_8 when = datetime.datetime.now() 
-_3_2_9 else: 
-_3_3_0 when = unstr_datetime(when) 
-_3_3_1 # base object is is the root to check for, user or group 
-_3_3_2 root_oid = user_or_group_oid 
-_3_3_3 permission = db.permission 
-_3_3_4 # ugly hack to satisfy pydal aliasing keyed tables /views 
-_3_3_5 left = with_alias(db, db.recursive_memberships, 'left') 
-_3_3_6 right = with_alias(db, db.recursive_memberships, 'right') 
-_3_3_7 # left = db.recursive_memberships.with_alias('left') 
-_3_3_8 # right = db.recursive_memberships.with_alias('right') 
-_3_3_9 
-_3_4_0 # end of ugly hack 
-_3_4_1 query = left.root == root_oid 
-_3_4_2 query &= right.root == target_oid 
-_3_4_3 query &= permission.identity_object_id == left.object_id 
-_3_4_4 query &= permission.target_object_id == right.object_id 
+_2_1_5def add_group(db: DAL, email: str, name: str, member_of: list[IdentityKey]):
+ 
+_2_1_6 return add_identity(db, email, member_of, name=name, object_type="group") 
+_2_1_7 
+_2_1_8 
+_2_1_9def remove_identity(db: DAL, object_id: IdentityKey): 
+_2_2_0 removed = db(db.identity.object_id == object_id).delete() 
+_2_2_1 # todo: remove permissions and group memberships 
+_2_2_2 db.commit() 
+_2_2_3 return removed > 0 
+_2_2_4 
+_2_2_5 
+_2_2_6def get_identity(db: DAL, key: IdentityKey, object_type: ObjectTypes =
+None): 
+_2_2_7 """ 
+_2_2_8 :param db: dal db connection 
+_2_2_9 :param key: can be the email, id, or object_id 
+_2_3_0 :return: user record or None when not found 
+_2_3_1 """ 
+_2_3_2 query = key_lookup_query(db, key, object_type) 
+_2_3_3 rows = db(query).select() 
+_2_3_4 return rows.first() 
+_2_3_5 
+_2_3_6 
+_2_3_7def get_user(db: DAL, key: IdentityKey): 
+_2_3_8 """ 
+_2_3_9 :param db: dal db connection 
+_2_4_0 :param key: can be the email, id, or object_id 
+_2_4_1 :return: user record or None when not found 
+_2_4_2 """ 
+_2_4_3 return get_identity(db, key, object_type="user") 
+_2_4_4 
+_2_4_5 
+_2_4_6def get_group(db: DAL, key: IdentityKey): 
+_2_4_7 """ 
+_2_4_8 
+_2_4_9 :param db: dal db connection 
+_2_5_0 :param key: can be the name of the group, the id, object_id or
+email_address 
+_2_5_1 :return: user record or None when not found 
+_2_5_2 """ 
+_2_5_3 return get_identity(db, key, object_type="group") 
+_2_5_4 
+_2_5_5 
+_2_5_6def authenticate_user(db: DAL, password: str = None, user: Identity = None,
+key: IdentityKey = None): 
+_2_5_7 if not password: 
+_2_5_8 return False 
+_2_5_9 if not user: 
+_2_6_0 user = get_user(db, key) 
+_2_6_1 return Password.validate(password, user.encoded_password) 
+_2_6_2 
+_2_6_3 
+_2_6_4def add_membership(db: DAL, identity_key: IdentityKey, group_key:
+IdentityKey): 
+_2_6_5 identity_oid = key_lookup(db, identity_key) 
+_2_6_6 if identity_oid is None: 
+_2_6_7 raise ValueError("invalid identity_oid key: " + identity_key) 
+_2_6_8 group = get_group(db, group_key) 
+_2_6_9 if not group: 
+_2_7_0 raise ValueError("invalid group key: " + group_key) 
+_2_7_1 query = db.membership.subject == identity_oid 
+_2_7_2 query &= db.membership.member_of == group.object_id 
+_2_7_3 if db(query).count() == 0: 
+_2_7_4 db.membership.validate_and_insert( 
+_2_7_5 subject=identity_oid, 
+_2_7_6 member_of=group.object_id, 
+_2_7_7 ) 
+_2_7_8 db.commit() 
+_2_7_9 
+_2_8_0 
+_2_8_1def remove_membership(db: DAL, identity_key: IdentityKey, group_key:
+IdentityKey): 
+_2_8_2 identity = get_identity(db, identity_key) 
+_2_8_3 group = get_group(db, group_key) 
+_2_8_4 query = db.membership.subject == identity.object_id 
+_2_8_5 query &= db.membership.member_of == group.object_id 
+_2_8_6 deleted = db(query).delete() 
+_2_8_7 db.commit() 
+_2_8_8 return deleted 
+_2_8_9 
+_2_9_0 
+_2_9_1def get_memberships(db: DAL, object_id: IdentityKey, bare: bool = True): 
+_2_9_2 query = db.recursive_memberships.root == object_id 
+_2_9_3 fields = [db.recursive_memberships.object_id,
+db.recursive_memberships.object_type] if bare else [] 
+_2_9_4 return db(query).select(*fields) 
+_2_9_5 
+_2_9_6 
+_2_9_7def get_members(db: DAL, object_id: IdentityKey, bare: bool = True): 
+_2_9_8 query = db.recursive_members.root == object_id 
+_2_9_9 fields = [db.recursive_members.object_id, db.recursive_members.object_type]
+if bare else [] 
+_3_0_0 return db(query).select(*fields) 
+_3_0_1 
+_3_0_2 
+_3_0_3def add_permission( 
+_3_0_4 db: DAL, 
+_3_0_5 identity_key: IdentityKey, 
+_3_0_6 target_oid: IdentityKey, 
+_3_0_7 privilege: str, 
+_3_0_8 starts: dt.datetime | str = DEFAULT_STARTS, 
+_3_0_9 ends: dt.datetime | str = DEFAULT_ENDS, 
+_3_1_0): 
+_3_1_1 identity_oid = key_lookup(db, identity_key) 
+_3_1_2 starts = unstr_datetime(starts) 
+_3_1_3 ends = unstr_datetime(ends) 
+_3_1_4 if has_permission(db, identity_oid, target_oid, privilege, when=starts): 
+_3_1_5 # permission already granted. just skip it 
+_3_1_6 print( 
+_3_1_7 "{privilege} permission already granted to {user_or_group_key} on
+{target_oid} @ {starts} ".format( 
+_3_1_8 **locals() 
+_3_1_9 ) 
+_3_2_0 ) 
+_3_2_1 # print(db._lastsql) 
+_3_2_2 return 
+_3_2_3 db.permission.validate_and_insert( 
+_3_2_4 privilege=privilege, 
+_3_2_5 identity_object_id=identity_oid, 
+_3_2_6 target_object_id=target_oid, 
+_3_2_7 starts=starts, 
+_3_2_8 ends=ends, 
+_3_2_9 ) 
+_3_3_0 db.commit() 
+_3_3_1 
+_3_3_2 
+_3_3_3def remove_permission( 
+_3_3_4 db: DAL, identity_key: IdentityKey, target_oid: IdentityKey, privilege:
+str, when: dt.datetime | str = DEFAULT 
+_3_3_5): 
+_3_3_6 identity_oid = key_lookup(db, identity_key) 
+_3_3_7 if when is DEFAULT: 
+_3_3_8 when = dt.datetime.now() 
+_3_3_9 else: 
+_3_4_0 when = unstr_datetime(when) 
+_3_4_1 # base object is is the root to check for, user or group 
+_3_4_2 permission = db.permission 
+_3_4_3 query = permission.identity_object_id == identity_oid 
+_3_4_4 query &= permission.target_object_id == target_oid 
 _3_4_5 query &= permission.privilege == privilege 
 _3_4_6 query &= permission.starts <= when 
 _3_4_7 query &= permission.ends >= when 
-_3_4_8 return db(query).count() > 0 
+_3_4_8 result = db(query).delete() > 0 
+_3_4_9 db.commit() 
+_3_5_0 # print(db._lastsql) 
+_3_5_1 return result 
+_3_5_2 
+_3_5_3 
+_3_5_4def with_alias(db: DAL, source: Table, alias: str): 
+_3_5_5 other = copy.copy(source) 
+_3_5_6 other["ALL"] = SQLALL(other) 
+_3_5_7 other["_tablename"] = alias 
+_3_5_8 for fieldname in other.fields: 
+_3_5_9 tmp = source[fieldname].clone() 
+_3_6_0 tmp.bind(other) 
+_3_6_1 other[fieldname] = tmp 
+_3_6_2 if "id" in source and "id" not in other.fields: 
+_3_6_3 other["id"] = other[source.id.name] 
+_3_6_4 
+_3_6_5 if source_id := getattr(source, "_id", None): 
+_3_6_6 other._id = other[source_id.name] 
+_3_6_7 db[alias] = other 
+_3_6_8 return other 
+_3_6_9 
+_3_7_0 
+_3_7_1def has_permission( 
+_3_7_2 db: DAL, user_or_group_key: IdentityKey, target_oid: IdentityKey,
+privilege: str, when: dt.datetime | str = DEFAULT 
+_3_7_3): 
+_3_7_4 user_or_group_oid = key_lookup(db, user_or_group_key) 
+_3_7_5 # the permission system 
+_3_7_6 if when is DEFAULT: 
+_3_7_7 when = dt.datetime.now() 
+_3_7_8 else: 
+_3_7_9 when = unstr_datetime(when) 
+_3_8_0 # base object is is the root to check for, user or group 
+_3_8_1 root_oid = user_or_group_oid 
+_3_8_2 permission = db.permission 
+_3_8_3 # ugly hack to satisfy pydal aliasing keyed tables /views 
+_3_8_4 left = with_alias(db, db.recursive_memberships, "left") 
+_3_8_5 right = with_alias(db, db.recursive_memberships, "right") 
+_3_8_6 # left = db.recursive_memberships.with_alias('left') 
+_3_8_7 # right = db.recursive_memberships.with_alias('right') 
+_3_8_8 
+_3_8_9 # end of ugly hack 
+_3_9_0 query = left.root == root_oid 
+_3_9_1 query &= right.root == target_oid 
+_3_9_2 query &= permission.identity_object_id == left.object_id 
+_3_9_3 query &= permission.target_object_id == right.object_id 
+_3_9_4 query &= permission.privilege == privilege 
+_3_9_5 query &= permission.starts <= when 
+_3_9_6 query &= permission.ends >= when 
+_3_9_7 return db(query).count() > 0 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
```

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_rbac_py.html` & `edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_rbac_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/edwh_auth_rbac/rbac.py: 56%</title>
+    <title>Coverage for src/edwh_auth_rbac/rbac.py: 57%</title>
     <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
     <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
     <script src="coverage_html_cb_da166b87.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/edwh_auth_rbac/rbac.py</b>:
-            <span class="pc_cov">56%</span>
+            <span class="pc_cov">57%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">88 statements &nbsp;</span>
+            <span class="text">86 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">49<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">39<span class="text"> missing</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">37<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="z_438b44bce6437be6_model_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="z_a44f0ac069e85531___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -79,186 +79,183 @@
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">logging</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span> <span class="key">import</span> <span class="nam">DAL</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">model</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">model</span> <span class="key">import</span> <span class="nam">Password</span><span class="op">,</span> <span class="nam">key_lookup</span><span class="op">,</span> <span class="nam">DEFAULT_STARTS</span><span class="op">,</span> <span class="nam">DEFAULT_ENDS</span><span class="op">,</span> <span class="nam">unstr_datetime</span><span class="op">,</span> <span class="nam">DEFAULT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="nam">_pylog</span> <span class="op">=</span> <span class="nam">logging</span><span class="op">.</span><span class="nam">getLogger</span><span class="op">(</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">_pylog</span><span class="op">.</span><span class="nam">setLevel</span><span class="op">(</span><span class="nam">logging</span><span class="op">.</span><span class="nam">INFO</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">class</span> <span class="nam">AuthRbac</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="nam">name</span> <span class="op">=</span> <span class="str">'auth_rbac'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">db</span> <span class="op">=</span> <span class="nam">db</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="op">@</span><span class="nam">staticmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="key">def</span> <span class="nam">_error</span><span class="op">(</span><span class="nam">msg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span><span class="str">'ERROR:'</span><span class="op">,</span> <span class="nam">msg</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="com"># gebruik event en rpc live templates (mobiel)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_user</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">firstname</span><span class="op">,</span> <span class="nam">fullname</span><span class="op">,</span> <span class="nam">password</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">        <span class="com"># check if exists</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="nam">email</span> <span class="op">=</span> <span class="nam">email</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="nam">user</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_user</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">if</span> <span class="nam">user</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">'User already exists'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">            <span class="nam">object_id</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">add_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">password</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">,</span> <span class="nam">firstname</span><span class="op">=</span><span class="nam">firstname</span><span class="op">,</span> <span class="nam">fullname</span><span class="op">=</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">                                           <span class="nam">object_type</span><span class="op">=</span><span class="str">'user'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">            <span class="nam">rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_user</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">            <span class="key">return</span> <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">                <span class="nam">object_id</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">                <span class="nam">email</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">                <span class="nam">firstname</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">                <span class="nam">fullname</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_item</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">password</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="com"># check if exists</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="nam">email</span> <span class="op">=</span> <span class="nam">email</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">item</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="str">'item'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="key">if</span> <span class="nam">item</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">'Item already exists'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">            <span class="nam">object_id</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">add_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="key">None</span><span class="op">,</span> <span class="nam">password</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="str">'item'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="nam">rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="str">'item'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">            <span class="key">return</span> <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">                <span class="nam">object_id</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">                <span class="nam">email</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">                <span class="nam">name</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">firstname</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">password</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="com"># check if exists</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="nam">email</span> <span class="op">=</span> <span class="nam">email</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">object_type</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">'object_type should be a string'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="nam">identity</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">        <span class="key">if</span> <span class="nam">identity</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">'Item already exists'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">            <span class="nam">object_id</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">add_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="key">None</span><span class="op">,</span> <span class="nam">password</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="nam">object_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">            <span class="nam">rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="nam">object_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="key">return</span> <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">                <span class="nam">object_id</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">                <span class="nam">email</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">                <span class="nam">name</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">name</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_group</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="com"># check if exists</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="nam">email</span> <span class="op">=</span> <span class="nam">email</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="nam">group</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_group</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="key">if</span> <span class="nam">group</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">'Group already exists'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="nam">object_id</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="nam">rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_group</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="key">return</span> <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">                <span class="nam">object_id</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">                <span class="nam">email</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">                <span class="nam">name</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">firstname</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="key">def</span> <span class="nam">update_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">,</span> <span class="nam">email</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">name</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">firstname</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">lastname</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">fullname</span><span class="op">=</span><span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">                        <span class="nam">password</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="nam">user</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="nam">user</span><span class="op">.</span><span class="nam">update_record</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">            <span class="nam">email</span><span class="op">=</span><span class="nam">email</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">email</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">            <span class="nam">firstname</span><span class="op">=</span><span class="nam">name</span> <span class="key">if</span> <span class="nam">name</span> <span class="key">else</span> <span class="nam">firstname</span> <span class="key">if</span> <span class="nam">firstname</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">            <span class="nam">lastname</span><span class="op">=</span><span class="nam">lastname</span> <span class="key">if</span> <span class="nam">lastname</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">lastname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">            <span class="nam">fullname</span><span class="op">=</span><span class="nam">fullname</span> <span class="key">if</span> <span class="nam">fullname</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">            <span class="nam">password</span><span class="op">=</span><span class="nam">Password</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="nam">password</span><span class="op">)</span> <span class="key">if</span> <span class="nam">password</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">encoded_password</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">    <span class="key">def</span> <span class="nam">get_user</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">return_memberhips</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_user</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="nam">object_id</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">            <span class="nam">email</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">            <span class="nam">firstname</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">            <span class="nam">fullname</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">        <span class="key">if</span> <span class="nam">return_memberhips</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">'memberships'</span><span class="op">]</span> <span class="op">=</span> <span class="op">[</span><span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">                <span class="nam">object_id</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">                <span class="nam">object_type</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">object_type</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">                <span class="nam">email</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">                <span class="nam">firstname</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">                <span class="nam">fullname</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">            <span class="op">)</span> <span class="key">for</span> <span class="nam">m</span> <span class="key">in</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_memberships</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">bare</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">    <span class="key">def</span> <span class="nam">get_group</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">return_members</span><span class="op">=</span><span class="key">True</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="nam">group_rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_group</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="nam">members</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">        <span class="key">if</span> <span class="nam">return_members</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">            <span class="nam">members</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_members</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">group_rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">bare</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">            <span class="nam">members</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">                <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">                    <span class="nam">object_id</span><span class="op">=</span><span class="nam">member</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">                    <span class="nam">object_type</span><span class="op">=</span><span class="nam">member</span><span class="op">.</span><span class="nam">object_type</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">                    <span class="nam">email</span><span class="op">=</span><span class="nam">member</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">                    <span class="nam">name</span><span class="op">=</span><span class="nam">member</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">                <span class="key">for</span> <span class="nam">member</span> <span class="key">in</span> <span class="nam">members</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">            <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">            <span class="nam">object_id</span><span class="op">=</span><span class="nam">group_rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">            <span class="nam">email</span><span class="op">=</span><span class="nam">group_rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">            <span class="nam">name</span><span class="op">=</span><span class="nam">group_rec</span><span class="op">.</span><span class="nam">firstname</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="key">if</span> <span class="nam">return_members</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">'members'</span><span class="op">]</span> <span class="op">=</span> <span class="nam">members</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">model</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">model</span> <span class="key">import</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">    <span class="nam">DEFAULT</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">    <span class="nam">DEFAULT_ENDS</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="nam">DEFAULT_STARTS</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="nam">Password</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">key_lookup</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="nam">unstr_datetime</span><span class="op">,</span> <span class="nam">IdentityKey</span><span class="op">,</span> <span class="nam">ObjectTypes</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="nam">_pylog</span> <span class="op">=</span> <span class="nam">logging</span><span class="op">.</span><span class="nam">getLogger</span><span class="op">(</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="nam">_pylog</span><span class="op">.</span><span class="nam">setLevel</span><span class="op">(</span><span class="nam">logging</span><span class="op">.</span><span class="nam">INFO</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">class</span> <span class="nam">AuthRbac</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="nam">name</span> <span class="op">=</span> <span class="str">"auth_rbac"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">db</span><span class="op">:</span> <span class="nam">DAL</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">db</span> <span class="op">=</span> <span class="nam">db</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="op">@</span><span class="nam">staticmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="key">def</span> <span class="nam">_error</span><span class="op">(</span><span class="nam">msg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span><span class="str">"ERROR:"</span><span class="op">,</span> <span class="nam">msg</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="com"># gebruik event en rpc live templates (mobiel)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_user</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">email</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">firstname</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">fullname</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">password</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">IdentityKey</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="com"># check if exists</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">email</span> <span class="op">=</span> <span class="nam">email</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">user</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_user</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">if</span> <span class="nam">user</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"User already exists"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="nam">object_id</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">add_identity</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">,</span> <span class="nam">password</span><span class="op">=</span><span class="nam">password</span><span class="op">,</span> <span class="nam">firstname</span><span class="op">=</span><span class="nam">firstname</span><span class="op">,</span> <span class="nam">fullname</span><span class="op">=</span><span class="nam">fullname</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="str">"user"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">            <span class="nam">rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_user</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="key">return</span> <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">                <span class="nam">object_id</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">                <span class="nam">email</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">                <span class="nam">firstname</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">                <span class="nam">fullname</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_item</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">password</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="com"># check if exists</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="nam">email</span> <span class="op">=</span> <span class="nam">email</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="nam">item</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="str">"item"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="key">if</span> <span class="nam">item</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Item already exists"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="nam">object_id</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">add_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">,</span> <span class="nam">name</span><span class="op">=</span><span class="nam">name</span><span class="op">,</span> <span class="nam">password</span><span class="op">=</span><span class="nam">password</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="str">"item"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="nam">rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="str">"item"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">            <span class="key">return</span> <span class="nam">dict</span><span class="op">(</span><span class="nam">object_id</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">email</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">firstname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">email</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">password</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">IdentityKey</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">                     <span class="nam">object_type</span><span class="op">:</span> <span class="nam">ObjectTypes</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="com"># check if exists</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="nam">email</span> <span class="op">=</span> <span class="nam">email</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="nam">identity</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">        <span class="key">if</span> <span class="nam">identity</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Item already exists"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">            <span class="nam">object_id</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">add_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">password</span><span class="op">=</span><span class="nam">password</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="nam">object_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">            <span class="nam">rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">,</span> <span class="nam">object_type</span><span class="op">=</span><span class="nam">object_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">            <span class="key">return</span> <span class="nam">dict</span><span class="op">(</span><span class="nam">object_id</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">email</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_group</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">email</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">IdentityKey</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="com"># check if exists</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="nam">email</span> <span class="op">=</span> <span class="nam">email</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="nam">group</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_group</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="key">if</span> <span class="nam">group</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Group already exists"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="nam">object_id</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">member_of</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="nam">rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_group</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">            <span class="key">return</span> <span class="nam">dict</span><span class="op">(</span><span class="nam">object_id</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">email</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">firstname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="key">def</span> <span class="nam">update_identity</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">,</span> <span class="nam">email</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">name</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">firstname</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">lastname</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">fullname</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">password</span><span class="op">=</span><span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="nam">user</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_identity</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">object_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="nam">user</span><span class="op">.</span><span class="nam">update_record</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">            <span class="nam">email</span><span class="op">=</span><span class="nam">email</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">email</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">            <span class="nam">firstname</span><span class="op">=</span><span class="nam">name</span> <span class="key">if</span> <span class="nam">name</span> <span class="key">else</span> <span class="nam">firstname</span> <span class="key">if</span> <span class="nam">firstname</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">            <span class="nam">lastname</span><span class="op">=</span><span class="nam">lastname</span> <span class="key">if</span> <span class="nam">lastname</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">lastname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">            <span class="nam">fullname</span><span class="op">=</span><span class="nam">fullname</span> <span class="key">if</span> <span class="nam">fullname</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">            <span class="nam">password</span><span class="op">=</span><span class="nam">Password</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="nam">password</span><span class="op">)</span> <span class="key">if</span> <span class="nam">password</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">encoded_password</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">def</span> <span class="nam">get_user</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">return_memberhips</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="nam">rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_user</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">            <span class="nam">object_id</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">            <span class="nam">email</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="nam">firstname</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">            <span class="nam">fullname</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="key">if</span> <span class="nam">return_memberhips</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">"memberships"</span><span class="op">]</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">                <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">                    <span class="nam">object_id</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">                    <span class="nam">object_type</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">object_type</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">                    <span class="nam">email</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">                    <span class="nam">firstname</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">                    <span class="nam">fullname</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">                <span class="key">for</span> <span class="nam">m</span> <span class="key">in</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_memberships</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">bare</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">            <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">    <span class="key">def</span> <span class="nam">get_group</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">return_members</span><span class="op">=</span><span class="key">True</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="nam">group_rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_group</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">        <span class="nam">members</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="key">if</span> <span class="nam">return_members</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">            <span class="nam">members</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_members</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">group_rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">bare</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">            <span class="nam">members</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">                <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">                    <span class="nam">object_id</span><span class="op">=</span><span class="nam">member</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">                    <span class="nam">object_type</span><span class="op">=</span><span class="nam">member</span><span class="op">.</span><span class="nam">object_type</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">                    <span class="nam">email</span><span class="op">=</span><span class="nam">member</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">                    <span class="nam">name</span><span class="op">=</span><span class="nam">member</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">                <span class="key">for</span> <span class="nam">member</span> <span class="key">in</span> <span class="nam">members</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">            <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">dict</span><span class="op">(</span><span class="nam">object_id</span><span class="op">=</span><span class="nam">group_rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span> <span class="nam">email</span><span class="op">=</span><span class="nam">group_rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span> <span class="nam">name</span><span class="op">=</span><span class="nam">group_rec</span><span class="op">.</span><span class="nam">firstname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="key">if</span> <span class="nam">return_members</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">"members"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">members</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">    <span class="key">def</span> <span class="nam">authenticate_user</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">password</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="key">return</span> <span class="nam">model</span><span class="op">.</span><span class="nam">authenticate_user</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">password</span><span class="op">=</span><span class="nam">password</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="key">def</span> <span class="nam">authenticate_user</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">password</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="key">return</span> <span class="nam">model</span><span class="op">.</span><span class="nam">authenticate_user</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">password</span><span class="op">=</span><span class="nam">password</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_membership</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="key">return</span> <span class="nam">model</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_membership</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="key">return</span> <span class="nam">model</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="key">def</span> <span class="nam">remove_membership</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="key">return</span> <span class="nam">model</span><span class="op">.</span><span class="nam">remove_membership</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">    <span class="key">def</span> <span class="nam">remove_membership</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="key">return</span> <span class="nam">model</span><span class="op">.</span><span class="nam">remove_membership</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">    <span class="key">def</span> <span class="nam">has_membership</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">user_or_group_key</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">        <span class="nam">key</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">user_or_group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">        <span class="nam">group</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">        <span class="nam">memberships</span> <span class="op">=</span> <span class="op">[</span><span class="nam">m</span><span class="op">.</span><span class="nam">object_id</span> <span class="key">for</span> <span class="nam">m</span> <span class="key">in</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_memberships</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">bare</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">        <span class="key">return</span> <span class="nam">group</span> <span class="key">in</span> <span class="nam">memberships</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_permission</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">starts</span><span class="op">=</span><span class="nam">DEFAULT_STARTS</span><span class="op">,</span> <span class="nam">ends</span><span class="op">=</span><span class="nam">DEFAULT_ENDS</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="nam">starts</span> <span class="op">=</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">starts</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="nam">ends</span> <span class="op">=</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">ends</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="nam">model</span><span class="op">.</span><span class="nam">add_permission</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">starts</span><span class="op">,</span> <span class="nam">ends</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">    <span class="key">def</span> <span class="nam">has_permission</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">when</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">        <span class="nam">when</span> <span class="op">=</span> <span class="nam">DEFAULT</span> <span class="key">if</span> <span class="nam">when</span> <span class="key">is</span> <span class="key">None</span> <span class="key">else</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">when</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">        <span class="key">return</span> <span class="nam">model</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">when</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">    <span class="key">def</span> <span class="nam">remove_permission</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">when</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">        <span class="nam">when</span> <span class="op">=</span> <span class="nam">DEFAULT</span> <span class="key">if</span> <span class="nam">when</span> <span class="key">is</span> <span class="key">None</span> <span class="key">else</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">when</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="key">return</span> <span class="nam">model</span><span class="op">.</span><span class="nam">remove_permission</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">when</span><span class="op">=</span><span class="nam">when</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">    <span class="key">def</span> <span class="nam">has_membership</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">user_or_group_key</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="nam">key</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">user_or_group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="nam">group</span> <span class="op">=</span> <span class="nam">key_lookup</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">group_key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">        <span class="nam">memberships</span> <span class="op">=</span> <span class="op">[</span><span class="nam">m</span><span class="op">.</span><span class="nam">object_id</span> <span class="key">for</span> <span class="nam">m</span> <span class="key">in</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_memberships</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">bare</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">        <span class="key">return</span> <span class="nam">group</span> <span class="key">in</span> <span class="nam">memberships</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_permission</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">starts</span><span class="op">=</span><span class="nam">DEFAULT_STARTS</span><span class="op">,</span> <span class="nam">ends</span><span class="op">=</span><span class="nam">DEFAULT_ENDS</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">        <span class="nam">starts</span> <span class="op">=</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">starts</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">        <span class="nam">ends</span> <span class="op">=</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">ends</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">        <span class="nam">model</span><span class="op">.</span><span class="nam">add_permission</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">starts</span><span class="op">,</span> <span class="nam">ends</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">    <span class="key">def</span> <span class="nam">has_permission</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">when</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="nam">when</span> <span class="op">=</span> <span class="nam">DEFAULT</span> <span class="key">if</span> <span class="nam">when</span> <span class="key">is</span> <span class="key">None</span> <span class="key">else</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">when</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">        <span class="key">return</span> <span class="nam">model</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">when</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">    <span class="key">def</span> <span class="nam">remove_permission</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">when</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">        <span class="nam">when</span> <span class="op">=</span> <span class="nam">DEFAULT</span> <span class="key">if</span> <span class="nam">when</span> <span class="key">is</span> <span class="key">None</span> <span class="key">else</span> <span class="nam">unstr_datetime</span><span class="op">(</span><span class="nam">when</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">        <span class="key">return</span> <span class="nam">model</span><span class="op">.</span><span class="nam">remove_permission</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">identity_key</span><span class="op">,</span> <span class="nam">target_oid</span><span class="op">,</span> <span class="nam">privilege</span><span class="op">,</span> <span class="nam">when</span><span class="op">=</span><span class="nam">when</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="z_438b44bce6437be6_model_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="z_a44f0ac069e85531___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,193 +1,192 @@
-************ CCoovveerraaggee ffoorr ssrrcc//eeddwwhh__aauutthh__rrbbaacc//rrbbaacc..ppyy:: 5566%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//eeddwwhh__aauutthh__rrbbaacc//rrbbaacc..ppyy:: 5577%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 8888 ssttaatteemmeennttss ?  4499 rruunn 3399 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 8866 ssttaatteemmeennttss ?  4499 rruunn 3377 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
 _1import logging 
 _2 
 _3from pydal import DAL 
-_4from . import model 
-_5from .model import Password, key_lookup, DEFAULT_STARTS, DEFAULT_ENDS,
-unstr_datetime, DEFAULT 
-_6 
-_7_pylog = logging.getLogger(__name__) 
-_8_pylog.setLevel(logging.INFO) 
-_9 
-_1_0 
-_1_1class AuthRbac: 
-_1_2 name = 'auth_rbac' 
-_1_3 
-_1_4 def __init__(self, db: DAL): 
-_1_5 self.db = db 
-_1_6 
-_1_7 @staticmethod 
-_1_8 def _error(msg): 
-_1_9 print('ERROR:', msg) 
-_2_0 
-_2_1 # gebruik event en rpc live templates (mobiel) 
-_2_2 
-_2_3 def add_user(self, email, firstname, fullname, password, member_of): 
-_2_4 # check if exists 
-_2_5 email = email.lower().strip() 
-_2_6 user = model.get_user(self.db, email) 
-_2_7 if user: 
-_2_8 raise ValueError('User already exists') 
-_2_9 else: 
-_3_0 object_id = model.add_identity(self.db, email, password, member_of,
-firstname=firstname, fullname=fullname, 
-_3_1 object_type='user') 
-_3_2 rec = model.get_user(self.db, object_id) 
-_3_3 return dict( 
-_3_4 object_id=rec.object_id, 
-_3_5 email=rec.email, 
-_3_6 firstname=rec.firstname, 
-_3_7 fullname=rec.fullname, 
-_3_8 ) 
-_3_9 
-_4_0 def add_item(self, email, name, password, member_of): 
-_4_1 # check if exists 
-_4_2 email = email.lower().strip() 
-_4_3 item = model.get_identity(self.db, email, 'item') 
-_4_4 if item: 
-_4_5 raise ValueError('Item already exists') 
-_4_6 else: 
-_4_7 object_id = model.add_identity(self.db, email, name, None, password,
-member_of, object_type='item') 
-_4_8 rec = model.get_identity(self.db, object_id, object_type='item') 
-_4_9 return dict( 
-_5_0 object_id=rec.object_id, 
-_5_1 email=rec.email, 
-_5_2 name=rec.firstname 
-_5_3 ) 
-_5_4 
-_5_5 def add_identity(self, email, name, password, member_of, object_type): 
-_5_6 # check if exists 
-_5_7 email = email.lower().strip() 
-_5_8 if not isinstance(object_type, str): 
-_5_9 raise ValueError('object_type should be a string') 
-_6_0 identity = model.get_identity(self.db, email, object_type) 
-_6_1 if identity: 
-_6_2 raise ValueError('Item already exists') 
-_6_3 else: 
-_6_4 object_id = model.add_identity(self.db, email, name, None, password,
-member_of, object_type=object_type) 
-_6_5 rec = model.get_identity(self.db, object_id, object_type=object_type) 
-_6_6 return dict( 
-_6_7 object_id=rec.object_id, 
-_6_8 email=rec.email, 
-_6_9 name=rec.name 
-_7_0 ) 
-_7_1 
-_7_2 def add_group(self, email, name, member_of): 
-_7_3 # check if exists 
-_7_4 email = email.lower().strip() 
-_7_5 group = model.get_group(self.db, email) 
-_7_6 if group: 
-_7_7 raise ValueError('Group already exists') 
-_7_8 else: 
-_7_9 object_id = model.add_group(self.db, email, name, member_of) 
-_8_0 rec = model.get_group(self.db, object_id) 
-_8_1 return dict( 
-_8_2 object_id=rec.object_id, 
-_8_3 email=rec.email, 
-_8_4 name=rec.firstname 
-_8_5 ) 
-_8_6 
-_8_7 def update_identity(self, object_id, email=None, name=None, firstname=None,
-lastname=None, fullname=None, 
-_8_8 password=None): 
-_8_9 user = model.get_identity(self.db, object_id) 
-_9_0 user.update_record( 
-_9_1 email=email.lower().strip() if email else user.email, 
-_9_2 firstname=name if name else firstname if firstname else user.firstname, 
-_9_3 lastname=lastname if lastname else user.lastname, 
-_9_4 fullname=fullname if fullname else user.fullname, 
-_9_5 password=Password.encode(password) if password else user.encoded_password, 
-_9_6 ) 
-_9_7 self.db.commit() 
-_9_8 
-_9_9 def get_user(self, key, return_memberhips=False): 
-_1_0_0 rec = model.get_user(self.db, key) 
-_1_0_1 result = dict( 
-_1_0_2 object_id=rec.object_id, 
-_1_0_3 email=rec.email, 
-_1_0_4 firstname=rec.firstname, 
-_1_0_5 fullname=rec.fullname, 
-_1_0_6 ) 
-_1_0_7 if return_memberhips: 
-_1_0_8 result['memberships'] = [dict( 
-_1_0_9 object_id=m.object_id, 
-_1_1_0 object_type=m.object_type, 
-_1_1_1 email=m.email, 
-_1_1_2 firstname=m.firstname, 
-_1_1_3 fullname=m.fullname, 
-_1_1_4 ) for m in model.get_memberships(self.db, rec.object_id, bare=False)] 
-_1_1_5 return result 
-_1_1_6 
-_1_1_7 def get_group(self, key, return_members=True): 
-_1_1_8 group_rec = model.get_group(self.db, key) 
-_1_1_9 members = [] 
-_1_2_0 if return_members: 
-_1_2_1 members = model.get_members(self.db, group_rec.object_id, bare=False) 
-_1_2_2 members = [ 
-_1_2_3 dict( 
-_1_2_4 object_id=member.object_id, 
-_1_2_5 object_type=member.object_type, 
-_1_2_6 email=member.email, 
-_1_2_7 name=member.firstname, 
-_1_2_8 ) 
-_1_2_9 for member in members 
-_1_3_0 ] 
-_1_3_1 
-_1_3_2 result = dict( 
-_1_3_3 object_id=group_rec.object_id, 
-_1_3_4 email=group_rec.email, 
-_1_3_5 name=group_rec.firstname 
-_1_3_6 ) 
-_1_3_7 if return_members: 
-_1_3_8 result['members'] = members 
-_1_3_9 return result 
+_4 
+_5from . import model 
+_6from .model import ( 
+_7 DEFAULT, 
+_8 DEFAULT_ENDS, 
+_9 DEFAULT_STARTS, 
+_1_0 Password, 
+_1_1 key_lookup, 
+_1_2 unstr_datetime, IdentityKey, ObjectTypes, 
+_1_3) 
+_1_4 
+_1_5_pylog = logging.getLogger(__name__) 
+_1_6_pylog.setLevel(logging.INFO) 
+_1_7 
+_1_8 
+_1_9class AuthRbac: 
+_2_0 name = "auth_rbac" 
+_2_1 
+_2_2 def __init__(self, db: DAL): 
+_2_3 self.db = db 
+_2_4 
+_2_5 @staticmethod 
+_2_6 def _error(msg): 
+_2_7 print("ERROR:", msg) 
+_2_8 
+_2_9 # gebruik event en rpc live templates (mobiel) 
+_3_0 
+_3_1 def add_user(self, email: str, firstname: str, fullname: str, password: str,
+member_of: list[IdentityKey]): 
+_3_2 # check if exists 
+_3_3 email = email.lower().strip() 
+_3_4 user = model.get_user(self.db, email) 
+_3_5 if user: 
+_3_6 raise ValueError("User already exists") 
+_3_7 else: 
+_3_8 object_id = model.add_identity( 
+_3_9 self.db, email, member_of, password=password, firstname=firstname,
+fullname=fullname, object_type="user" 
+_4_0 ) 
+_4_1 rec = model.get_user(self.db, object_id) 
+_4_2 return dict( 
+_4_3 object_id=rec.object_id, 
+_4_4 email=rec.email, 
+_4_5 firstname=rec.firstname, 
+_4_6 fullname=rec.fullname, 
+_4_7 ) 
+_4_8 
+_4_9 def add_item(self, email, name, password, member_of): 
+_5_0 # check if exists 
+_5_1 email = email.lower().strip() 
+_5_2 item = model.get_identity(self.db, email, "item") 
+_5_3 if item: 
+_5_4 raise ValueError("Item already exists") 
+_5_5 else: 
+_5_6 object_id = model.add_identity(self.db, email, member_of, name=name,
+password=password, object_type="item") 
+_5_7 rec = model.get_identity(self.db, object_id, object_type="item") 
+_5_8 return dict(object_id=rec.object_id, email=rec.email, name=rec.firstname) 
+_5_9 
+_6_0 def add_identity(self, email: str, name: str, password: str, member_of: list
+[IdentityKey], 
+_6_1 object_type: ObjectTypes): 
+_6_2 # check if exists 
+_6_3 email = email.lower().strip() 
+_6_4 
+_6_5 identity = model.get_identity(self.db, email, object_type) 
+_6_6 if identity: 
+_6_7 raise ValueError("Item already exists") 
+_6_8 else: 
+_6_9 object_id = model.add_identity(self.db, email, member_of, name,
+password=password, object_type=object_type) 
+_7_0 rec = model.get_identity(self.db, object_id, object_type=object_type) 
+_7_1 return dict(object_id=rec.object_id, email=rec.email, name=rec.name) 
+_7_2 
+_7_3 def add_group(self, email: str, name: str, member_of: list[IdentityKey]): 
+_7_4 # check if exists 
+_7_5 email = email.lower().strip() 
+_7_6 group = model.get_group(self.db, email) 
+_7_7 if group: 
+_7_8 raise ValueError("Group already exists") 
+_7_9 else: 
+_8_0 object_id = model.add_group(self.db, email, name, member_of) 
+_8_1 rec = model.get_group(self.db, object_id) 
+_8_2 return dict(object_id=rec.object_id, email=rec.email, name=rec.firstname) 
+_8_3 
+_8_4 def update_identity( 
+_8_5 self, object_id, email=None, name=None, firstname=None, lastname=None,
+fullname=None, password=None 
+_8_6 ): 
+_8_7 user = model.get_identity(self.db, object_id) 
+_8_8 user.update_record( 
+_8_9 email=email.lower().strip() if email else user.email, 
+_9_0 firstname=name if name else firstname if firstname else user.firstname, 
+_9_1 lastname=lastname if lastname else user.lastname, 
+_9_2 fullname=fullname if fullname else user.fullname, 
+_9_3 password=Password.encode(password) if password else user.encoded_password, 
+_9_4 ) 
+_9_5 self.db.commit() 
+_9_6 
+_9_7 def get_user(self, key, return_memberhips=False): 
+_9_8 rec = model.get_user(self.db, key) 
+_9_9 result = dict( 
+_1_0_0 object_id=rec.object_id, 
+_1_0_1 email=rec.email, 
+_1_0_2 firstname=rec.firstname, 
+_1_0_3 fullname=rec.fullname, 
+_1_0_4 ) 
+_1_0_5 if return_memberhips: 
+_1_0_6 result["memberships"] = [ 
+_1_0_7 dict( 
+_1_0_8 object_id=m.object_id, 
+_1_0_9 object_type=m.object_type, 
+_1_1_0 email=m.email, 
+_1_1_1 firstname=m.firstname, 
+_1_1_2 fullname=m.fullname, 
+_1_1_3 ) 
+_1_1_4 for m in model.get_memberships(self.db, rec.object_id, bare=False) 
+_1_1_5 ] 
+_1_1_6 return result 
+_1_1_7 
+_1_1_8 def get_group(self, key, return_members=True): 
+_1_1_9 group_rec = model.get_group(self.db, key) 
+_1_2_0 members = [] 
+_1_2_1 if return_members: 
+_1_2_2 members = model.get_members(self.db, group_rec.object_id, bare=False) 
+_1_2_3 members = [ 
+_1_2_4 dict( 
+_1_2_5 object_id=member.object_id, 
+_1_2_6 object_type=member.object_type, 
+_1_2_7 email=member.email, 
+_1_2_8 name=member.firstname, 
+_1_2_9 ) 
+_1_3_0 for member in members 
+_1_3_1 ] 
+_1_3_2 
+_1_3_3 result = dict(object_id=group_rec.object_id, email=group_rec.email,
+name=group_rec.firstname) 
+_1_3_4 if return_members: 
+_1_3_5 result["members"] = members 
+_1_3_6 return result 
+_1_3_7 
+_1_3_8 def authenticate_user(self, key, password): 
+_1_3_9 return model.authenticate_user(self.db, key=key, password=password) 
 _1_4_0 
-_1_4_1 def authenticate_user(self, key, password): 
-_1_4_2 return model.authenticate_user(self.db, key=key, password=password) 
+_1_4_1 def add_membership(self, identity_key, group_key): 
+_1_4_2 return model.add_membership(self.db, identity_key, group_key) 
 _1_4_3 
-_1_4_4 def add_membership(self, identity_key, group_key): 
-_1_4_5 return model.add_membership(self.db, identity_key, group_key) 
+_1_4_4 def remove_membership(self, identity_key, group_key): 
+_1_4_5 return model.remove_membership(self.db, identity_key, group_key) 
 _1_4_6 
-_1_4_7 def remove_membership(self, identity_key, group_key): 
-_1_4_8 return model.remove_membership(self.db, identity_key, group_key) 
-_1_4_9 
-_1_5_0 def has_membership(self, user_or_group_key, group_key): 
-_1_5_1 key = key_lookup(self.db, user_or_group_key) 
-_1_5_2 group = key_lookup(self.db, group_key) 
-_1_5_3 memberships = [m.object_id for m in model.get_memberships(self.db, key,
+_1_4_7 def has_membership(self, user_or_group_key, group_key): 
+_1_4_8 key = key_lookup(self.db, user_or_group_key) 
+_1_4_9 group = key_lookup(self.db, group_key) 
+_1_5_0 memberships = [m.object_id for m in model.get_memberships(self.db, key,
 bare=False)] 
-_1_5_4 return group in memberships 
-_1_5_5 
-_1_5_6 def add_permission(self, identity_key, target_oid, privilege,
+_1_5_1 return group in memberships 
+_1_5_2 
+_1_5_3 def add_permission(self, identity_key, target_oid, privilege,
 starts=DEFAULT_STARTS, ends=DEFAULT_ENDS): 
-_1_5_7 starts = unstr_datetime(starts) 
-_1_5_8 ends = unstr_datetime(ends) 
-_1_5_9 model.add_permission(self.db, identity_key, target_oid, privilege, starts,
+_1_5_4 starts = unstr_datetime(starts) 
+_1_5_5 ends = unstr_datetime(ends) 
+_1_5_6 model.add_permission(self.db, identity_key, target_oid, privilege, starts,
 ends) 
-_1_6_0 
-_1_6_1 def has_permission(self, identity_key, target_oid, privilege, when=None): 
-_1_6_2 when = DEFAULT if when is None else unstr_datetime(when) 
-_1_6_3 return model.has_permission(self.db, identity_key, target_oid, privilege,
+_1_5_7 
+_1_5_8 def has_permission(self, identity_key, target_oid, privilege, when=None): 
+_1_5_9 when = DEFAULT if when is None else unstr_datetime(when) 
+_1_6_0 return model.has_permission(self.db, identity_key, target_oid, privilege,
 when) 
-_1_6_4 
-_1_6_5 def remove_permission(self, identity_key, target_oid, privilege,
+_1_6_1 
+_1_6_2 def remove_permission(self, identity_key, target_oid, privilege,
 when=None): 
-_1_6_6 when = DEFAULT if when is None else unstr_datetime(when) 
-_1_6_7 return model.remove_permission(self.db, identity_key, target_oid,
+_1_6_3 when = DEFAULT if when is None else unstr_datetime(when) 
+_1_6_4 return model.remove_permission(self.db, identity_key, target_oid,
 privilege, when=when) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
```

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/z_a44f0ac069e85531___init___py.html` & `edwh_auth_rbac-0.4.0/htmlcov/z_a44f0ac069e85531___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="z_438b44bce6437be6_rbac_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="z_a44f0ac069e85531_test_rbac_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a class="nav" href="z_438b44bce6437be6_rbac_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="z_a44f0ac069e85531_test_rbac_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
```

### Comparing `edwh_auth_rbac-0.3.0/htmlcov/z_a44f0ac069e85531_test_rbac_py.html` & `edwh_auth_rbac-0.4.0/htmlcov/z_a44f0ac069e85531_test_rbac_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">106 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">104<span class="text"> run</span></button>
+            <span class="text">107 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">105<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">2<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="z_a44f0ac069e85531___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -77,159 +77,163 @@
             <button type="button" class="button_to_index" data-shortcut="u"></button>
             <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">tempfile</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span> <span class="key">import</span> <span class="nam">DAL</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">uuid</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">uuid</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">dotmap</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">pytest</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">dotmap</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span> <span class="key">import</span> <span class="nam">DAL</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">src</span><span class="op">.</span><span class="nam">edwh_auth_rbac</span><span class="op">.</span><span class="nam">model</span> <span class="key">import</span> <span class="nam">define_auth_rbac_model</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">src</span><span class="op">.</span><span class="nam">edwh_auth_rbac</span><span class="op">.</span><span class="nam">rbac</span> <span class="key">import</span> <span class="nam">AuthRbac</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">src</span><span class="op">.</span><span class="nam">edwh_auth_rbac</span><span class="op">.</span><span class="nam">migrations</span> <span class="key">import</span> <span class="nam">rbac_migrations</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">src</span><span class="op">.</span><span class="nam">edwh_auth_rbac</span><span class="op">.</span><span class="nam">migrations</span> <span class="key">import</span> <span class="nam">rbac_migrations</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">src</span><span class="op">.</span><span class="nam">edwh_auth_rbac</span><span class="op">.</span><span class="nam">model</span> <span class="key">import</span> <span class="nam">define_auth_rbac_model</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">src</span><span class="op">.</span><span class="nam">edwh_auth_rbac</span><span class="op">.</span><span class="nam">rbac</span> <span class="key">import</span> <span class="nam">AuthRbac</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="nam">namespace</span> <span class="op">=</span> <span class="nam">uuid</span><span class="op">.</span><span class="nam">UUID</span><span class="op">(</span><span class="str">'84f5c757-4be0-49c8-a3ba-4f4d79167839'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="nam">namespace</span> <span class="op">=</span> <span class="nam">uuid</span><span class="op">.</span><span class="nam">UUID</span><span class="op">(</span><span class="str">"84f5c757-4be0-49c8-a3ba-4f4d79167839"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="op">@</span><span class="nam">pytest</span><span class="op">.</span><span class="nam">fixture</span><span class="op">(</span><span class="nam">scope</span><span class="op">=</span><span class="str">"module"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">def</span> <span class="nam">tmpdir</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="key">with</span> <span class="nam">tempfile</span><span class="op">.</span><span class="nam">TemporaryDirectory</span><span class="op">(</span><span class="op">)</span> <span class="key">as</span> <span class="nam">tmpdirname</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span><span class="str">'new tempdir'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span><span class="str">"new tempdir"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="key">yield</span> <span class="nam">tmpdirname</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="op">@</span><span class="nam">pytest</span><span class="op">.</span><span class="nam">fixture</span><span class="op">(</span><span class="nam">scope</span><span class="op">=</span><span class="str">"module"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="key">def</span> <span class="nam">database</span><span class="op">(</span><span class="nam">tmpdir</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="key">class</span> <span class="nam">Database</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="key">def</span> <span class="nam">__enter__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">db</span> <span class="op">=</span> <span class="nam">DAL</span><span class="op">(</span><span class="str">'sqlite://auth_rbac.sqlite'</span><span class="op">,</span> <span class="nam">folder</span><span class="op">=</span><span class="nam">tmpdir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">db</span> <span class="op">=</span> <span class="nam">DAL</span><span class="op">(</span><span class="str">"sqlite://auth_rbac.sqlite"</span><span class="op">,</span> <span class="nam">folder</span><span class="op">=</span><span class="nam">tmpdir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">define_auth_rbac_model</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">dict</span><span class="op">(</span><span class="nam">allowed_types</span><span class="op">=</span><span class="op">[</span><span class="str">'user'</span><span class="op">,</span> <span class="str">'group'</span><span class="op">]</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">            <span class="nam">rbac_migrations</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">            <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="key">def</span> <span class="nam">__exit__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">exc_type</span><span class="op">,</span> <span class="nam">exc_value</span><span class="op">,</span> <span class="nam">traceback</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">close</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">return</span> <span class="nam">Database</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">settings</span> <span class="op">=</span> <span class="nam">dict</span><span class="op">(</span><span class="nam">allowed_types</span><span class="op">=</span><span class="op">[</span><span class="str">"user"</span><span class="op">,</span> <span class="str">"group"</span><span class="op">]</span><span class="op">,</span> <span class="nam">migrate</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">            <span class="nam">define_auth_rbac_model</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">settings</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">            <span class="nam">rbac_migrations</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">            <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="key">def</span> <span class="nam">__exit__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">exc_type</span><span class="op">,</span> <span class="nam">exc_value</span><span class="op">,</span> <span class="nam">traceback</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">close</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="op">@</span><span class="nam">pytest</span><span class="op">.</span><span class="nam">fixture</span><span class="op">(</span><span class="nam">scope</span><span class="op">=</span><span class="str">"module"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="key">def</span> <span class="nam">rbac</span><span class="op">(</span><span class="nam">database</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="key">with</span> <span class="nam">database</span> <span class="key">as</span> <span class="nam">db</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="key">yield</span> <span class="nam">AuthRbac</span><span class="op">(</span><span class="nam">db</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="op">@</span><span class="nam">pytest</span><span class="op">.</span><span class="nam">fixture</span><span class="op">(</span><span class="nam">scope</span><span class="op">=</span><span class="str">"module"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="key">def</span> <span class="nam">store</span><span class="op">(</span><span class="nam">_</span><span class="op">=</span><span class="nam">dotmap</span><span class="op">.</span><span class="nam">DotMap</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">'store'</span><span class="op">,</span> <span class="nam">_</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="key">return</span> <span class="nam">_</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="op">@</span><span class="nam">pytest</span><span class="op">.</span><span class="nam">mark</span><span class="op">.</span><span class="nam">incremental</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="key">class</span> <span class="nam">TestSequentially</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_drop_all_test_users</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">database</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="key">with</span> <span class="nam">database</span> <span class="key">as</span> <span class="nam">db</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">            <span class="nam">users</span> <span class="op">=</span> <span class="nam">db</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">email</span><span class="op">.</span><span class="nam">contains</span><span class="op">(</span><span class="str">'@test.nl'</span><span class="op">)</span><span class="op">)</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">            <span class="nam">db</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">email</span><span class="op">.</span><span class="nam">contains</span><span class="op">(</span><span class="str">'@test.nl'</span><span class="op">)</span><span class="op">)</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="key">for</span> <span class="nam">user</span> <span class="key">in</span> <span class="nam">users</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">                <span class="nam">db</span><span class="op">(</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">member_of</span> <span class="op">==</span> <span class="nam">user</span><span class="op">.</span><span class="nam">object_id</span><span class="op">)</span> <span class="op">|</span> <span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">subject</span> <span class="op">==</span> <span class="nam">user</span><span class="op">.</span><span class="nam">object_id</span><span class="op">)</span><span class="op">)</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">                <span class="nam">db</span><span class="op">(</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">permission</span><span class="op">.</span><span class="nam">identity_object_id</span> <span class="op">==</span> <span class="nam">user</span><span class="op">.</span><span class="nam">object_id</span><span class="op">)</span> <span class="op">|</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">                        <span class="nam">db</span><span class="op">.</span><span class="nam">permission</span><span class="op">.</span><span class="nam">target_object_id</span> <span class="op">==</span> <span class="nam">user</span><span class="op">.</span><span class="nam">object_id</span><span class="op">)</span><span class="op">)</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">            <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">            <span class="key">assert</span> <span class="nam">db</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">email</span><span class="op">.</span><span class="nam">contains</span><span class="op">(</span><span class="str">'@test.nl'</span><span class="op">)</span><span class="op">)</span><span class="op">.</span><span class="nam">count</span><span class="op">(</span><span class="op">)</span> <span class="op">==</span> <span class="num">0</span><span class="op">,</span> <span class="str">'Howcome @test.nl still exist?'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_user_creation</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">remco</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_user</span><span class="op">(</span><span class="str">'remco@test.nl'</span><span class="op">,</span> <span class="str">'remco'</span><span class="op">,</span> <span class="str">'remco test'</span><span class="op">,</span> <span class="str">'secret'</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">'object_id'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_user</span><span class="op">(</span><span class="str">'pietje@test.nl'</span><span class="op">,</span> <span class="str">'pietje'</span><span class="op">,</span> <span class="str">'pietje test'</span><span class="op">,</span> <span class="str">'secret'</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">'object_id'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">truus</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_user</span><span class="op">(</span><span class="str">'truus@test.nl'</span><span class="op">,</span> <span class="str">'truus'</span><span class="op">,</span> <span class="str">'truus test'</span><span class="op">,</span> <span class="str">'secret'</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">'object_id'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_group_creation</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="str">'articles@test.nl'</span><span class="op">,</span> <span class="str">'articles'</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">'object_id'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">all</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="str">'all@test.nl'</span><span class="op">,</span> <span class="str">'all'</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">'object_id'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">users</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="str">'users@test.nl'</span><span class="op">,</span> <span class="str">'users'</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">'object_id'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">admins</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="str">'admins@test.nl'</span><span class="op">,</span> <span class="str">'admins'</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">'object_id'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_item_creation</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="key">for</span> <span class="nam">name</span> <span class="key">in</span> <span class="str">'abcde'</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">            <span class="nam">store</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_user</span><span class="op">(</span><span class="str">'article_'</span> <span class="op">+</span> <span class="nam">name</span> <span class="op">+</span> <span class="str">'@test.nl'</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="str">'article'</span><span class="op">,</span> <span class="str">''</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">                <span class="str">'object_id'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_stash_users_in_groups</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">truus</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">all</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">all</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_stash_items_in_groups</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="key">for</span> <span class="nam">name</span> <span class="key">in</span> <span class="str">'abcde'</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">            <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_add_some_permissions</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">'read'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">'write'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">'read'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_first_level_memberships</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">)</span> <span class="key">is</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">)</span> <span class="key">is</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_second_level_memberships</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">all</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">all</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_first_level_permissions</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">'read'</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">'write'</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">'read'</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">'write'</span><span class="op">)</span> <span class="key">is</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_second_to_first_level_permissions</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">'read'</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">'write'</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">'read'</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">'write'</span><span class="op">)</span> <span class="key">is</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_second_to_second_level_permissions</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">a</span><span class="op">,</span> <span class="str">'read'</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">a</span><span class="op">,</span> <span class="str">'write'</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">a</span><span class="op">,</span> <span class="str">'read'</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">a</span><span class="op">,</span> <span class="str">'write'</span><span class="op">)</span> <span class="key">is</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_deeper_group_nesting</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">subadmins</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="str">'sub_admins@test.nl'</span><span class="op">,</span> <span class="str">'subadmins'</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">'object_id'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">subarticles</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="str">'sub_articles@test.nl'</span><span class="op">,</span> <span class="str">'subarticles'</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">'object_id'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">subarticles</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">subadmins</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">nested_admin</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_user</span><span class="op">(</span><span class="str">'nested_admin@test.nl'</span><span class="op">,</span> <span class="str">'nested_admin'</span><span class="op">,</span> <span class="str">'nested_admin test'</span><span class="op">,</span> <span class="str">'secret'</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">            <span class="str">'object_id'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">nested_admin</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">subadmins</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="key">for</span> <span class="nam">name</span> <span class="key">in</span> <span class="str">'stuvw'</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">            <span class="nam">store</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_user</span><span class="op">(</span><span class="str">'article_'</span> <span class="op">+</span> <span class="nam">name</span> <span class="op">+</span> <span class="str">'@test.nl'</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="str">'subarticle'</span><span class="op">,</span> <span class="str">''</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">'object_id'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">            <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">subarticles</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">nested_admin</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">s</span><span class="op">,</span> <span class="str">'read'</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_removing_a_nested_group</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">remove_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">nested_admin</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">subadmins</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">nested_admin</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">s</span><span class="op">,</span> <span class="str">'read'</span><span class="op">)</span> <span class="key">is</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">return</span> <span class="nam">Database</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="op">@</span><span class="nam">pytest</span><span class="op">.</span><span class="nam">fixture</span><span class="op">(</span><span class="nam">scope</span><span class="op">=</span><span class="str">"module"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="key">def</span> <span class="nam">rbac</span><span class="op">(</span><span class="nam">database</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="key">with</span> <span class="nam">database</span> <span class="key">as</span> <span class="nam">db</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="key">yield</span> <span class="nam">AuthRbac</span><span class="op">(</span><span class="nam">db</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="op">@</span><span class="nam">pytest</span><span class="op">.</span><span class="nam">fixture</span><span class="op">(</span><span class="nam">scope</span><span class="op">=</span><span class="str">"module"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t"><span class="key">def</span> <span class="nam">store</span><span class="op">(</span><span class="nam">_</span><span class="op">=</span><span class="nam">dotmap</span><span class="op">.</span><span class="nam">DotMap</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">"store"</span><span class="op">,</span> <span class="nam">_</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="key">return</span> <span class="nam">_</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="op">@</span><span class="nam">pytest</span><span class="op">.</span><span class="nam">mark</span><span class="op">.</span><span class="nam">incremental</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="key">class</span> <span class="nam">TestSequentially</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_drop_all_test_users</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">database</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">with</span> <span class="nam">database</span> <span class="key">as</span> <span class="nam">db</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="nam">users</span> <span class="op">=</span> <span class="nam">db</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">email</span><span class="op">.</span><span class="nam">contains</span><span class="op">(</span><span class="str">"@test.nl"</span><span class="op">)</span><span class="op">)</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="nam">db</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">email</span><span class="op">.</span><span class="nam">contains</span><span class="op">(</span><span class="str">"@test.nl"</span><span class="op">)</span><span class="op">)</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">            <span class="key">for</span> <span class="nam">user</span> <span class="key">in</span> <span class="nam">users</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">                <span class="nam">db</span><span class="op">(</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">member_of</span> <span class="op">==</span> <span class="nam">user</span><span class="op">.</span><span class="nam">object_id</span><span class="op">)</span> <span class="op">|</span> <span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">membership</span><span class="op">.</span><span class="nam">subject</span> <span class="op">==</span> <span class="nam">user</span><span class="op">.</span><span class="nam">object_id</span><span class="op">)</span><span class="op">)</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">                <span class="nam">db</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">                    <span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">permission</span><span class="op">.</span><span class="nam">identity_object_id</span> <span class="op">==</span> <span class="nam">user</span><span class="op">.</span><span class="nam">object_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">                    <span class="op">|</span> <span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">permission</span><span class="op">.</span><span class="nam">target_object_id</span> <span class="op">==</span> <span class="nam">user</span><span class="op">.</span><span class="nam">object_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">                <span class="op">)</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">            <span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">            <span class="key">assert</span> <span class="nam">db</span><span class="op">(</span><span class="nam">db</span><span class="op">.</span><span class="nam">identity</span><span class="op">.</span><span class="nam">email</span><span class="op">.</span><span class="nam">contains</span><span class="op">(</span><span class="str">"@test.nl"</span><span class="op">)</span><span class="op">)</span><span class="op">.</span><span class="nam">count</span><span class="op">(</span><span class="op">)</span> <span class="op">==</span> <span class="num">0</span><span class="op">,</span> <span class="str">"Howcome @test.nl still exist?"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_user_creation</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">remco</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_user</span><span class="op">(</span><span class="str">"remco@test.nl"</span><span class="op">,</span> <span class="str">"remco"</span><span class="op">,</span> <span class="str">"remco test"</span><span class="op">,</span> <span class="str">"secret"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">"object_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_user</span><span class="op">(</span><span class="str">"pietje@test.nl"</span><span class="op">,</span> <span class="str">"pietje"</span><span class="op">,</span> <span class="str">"pietje test"</span><span class="op">,</span> <span class="str">"secret"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">"object_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">truus</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_user</span><span class="op">(</span><span class="str">"truus@test.nl"</span><span class="op">,</span> <span class="str">"truus"</span><span class="op">,</span> <span class="str">"truus test"</span><span class="op">,</span> <span class="str">"secret"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">"object_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_group_creation</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="str">"articles@test.nl"</span><span class="op">,</span> <span class="str">"articles"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">"object_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">all</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="str">"all@test.nl"</span><span class="op">,</span> <span class="str">"all"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">"object_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">users</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="str">"users@test.nl"</span><span class="op">,</span> <span class="str">"users"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">"object_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">admins</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="str">"admins@test.nl"</span><span class="op">,</span> <span class="str">"admins"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">"object_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_item_creation</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="key">for</span> <span class="nam">name</span> <span class="key">in</span> <span class="str">"abcde"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="nam">store</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_user</span><span class="op">(</span><span class="str">"article_"</span> <span class="op">+</span> <span class="nam">name</span> <span class="op">+</span> <span class="str">"@test.nl"</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="str">"article"</span><span class="op">,</span> <span class="str">""</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">"object_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_stash_users_in_groups</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">truus</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">all</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">all</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_stash_items_in_groups</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="key">for</span> <span class="nam">name</span> <span class="key">in</span> <span class="str">"abcde"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">            <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_add_some_permissions</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">"read"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">"write"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">"read"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_first_level_memberships</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">)</span> <span class="key">is</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">)</span> <span class="key">is</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_second_level_memberships</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">all</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">all</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_first_level_permissions</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">"read"</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">"write"</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">"read"</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">users</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">"write"</span><span class="op">)</span> <span class="key">is</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_second_to_first_level_permissions</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">"read"</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">"write"</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">"read"</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">,</span> <span class="str">"write"</span><span class="op">)</span> <span class="key">is</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_second_to_second_level_permissions</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">a</span><span class="op">,</span> <span class="str">"read"</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">remco</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">a</span><span class="op">,</span> <span class="str">"write"</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">a</span><span class="op">,</span> <span class="str">"read"</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">pietje</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">a</span><span class="op">,</span> <span class="str">"write"</span><span class="op">)</span> <span class="key">is</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_deeper_group_nesting</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">subadmins</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="str">"sub_admins@test.nl"</span><span class="op">,</span> <span class="str">"subadmins"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">"object_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">subarticles</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_group</span><span class="op">(</span><span class="str">"sub_articles@test.nl"</span><span class="op">,</span> <span class="str">"subarticles"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">"object_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">subarticles</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">articles</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">subadmins</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">admins</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="nam">store</span><span class="op">.</span><span class="nam">nested_admin</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_user</span><span class="op">(</span><span class="str">"nested_admin@test.nl"</span><span class="op">,</span> <span class="str">"nested_admin"</span><span class="op">,</span> <span class="str">"nested_admin test"</span><span class="op">,</span> <span class="str">"secret"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">            <span class="str">"object_id"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">nested_admin</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">subadmins</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="key">for</span> <span class="nam">name</span> <span class="key">in</span> <span class="str">"stuvw"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">            <span class="nam">store</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span> <span class="op">=</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_user</span><span class="op">(</span><span class="str">"article_"</span> <span class="op">+</span> <span class="nam">name</span> <span class="op">+</span> <span class="str">"@test.nl"</span><span class="op">,</span> <span class="nam">name</span><span class="op">,</span> <span class="str">"subarticle"</span><span class="op">,</span> <span class="str">""</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span><span class="op">[</span><span class="str">"object_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">            <span class="nam">rbac</span><span class="op">.</span><span class="nam">add_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">subarticles</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">nested_admin</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">s</span><span class="op">,</span> <span class="str">"read"</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_removing_a_nested_group</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">rbac</span><span class="op">,</span> <span class="nam">store</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">rbac</span><span class="op">.</span><span class="nam">remove_membership</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">nested_admin</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">subadmins</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="key">assert</span> <span class="nam">rbac</span><span class="op">.</span><span class="nam">has_permission</span><span class="op">(</span><span class="nam">store</span><span class="op">.</span><span class="nam">nested_admin</span><span class="op">,</span> <span class="nam">store</span><span class="op">.</span><span class="nam">s</span><span class="op">,</span> <span class="str">"read"</span><span class="op">)</span> <span class="key">is</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="z_a44f0ac069e85531___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1">coverage.py v7.5.1</a>,
-            created at 2024-05-16 17:13 +0200
+            created at 2024-05-22 15:42 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -4,161 +4,165 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 110066 ssttaatteemmeennttss ?  110044 rruunn 22 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 110077 ssttaatteemmeennttss ?  110055 rruunn 22 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
 _1import tempfile 
-_2 
-_3from pydal import DAL 
-_4import uuid 
+_2import uuid 
+_3 
+_4import dotmap 
 _5import pytest 
-_6import dotmap 
+_6from pydal import DAL 
 _7 
-_8from src.edwh_auth_rbac.model import define_auth_rbac_model 
-_9from src.edwh_auth_rbac.rbac import AuthRbac 
-_1_0from src.edwh_auth_rbac.migrations import rbac_migrations 
+_8from src.edwh_auth_rbac.migrations import rbac_migrations 
+_9from src.edwh_auth_rbac.model import define_auth_rbac_model 
+_1_0from src.edwh_auth_rbac.rbac import AuthRbac 
 _1_1 
-_1_2namespace = uuid.UUID('84f5c757-4be0-49c8-a3ba-4f4d79167839') 
+_1_2namespace = uuid.UUID("84f5c757-4be0-49c8-a3ba-4f4d79167839") 
 _1_3 
 _1_4 
 _1_5@pytest.fixture(scope="module") 
 _1_6def tmpdir(): 
 _1_7 with tempfile.TemporaryDirectory() as tmpdirname: 
-_1_8 print('new tempdir') 
+_1_8 print("new tempdir") 
 _1_9 yield tmpdirname 
 _2_0 
 _2_1 
 _2_2@pytest.fixture(scope="module") 
 _2_3def database(tmpdir): 
 _2_4 class Database: 
 _2_5 def __enter__(self): 
-_2_6 self.db = DAL('sqlite://auth_rbac.sqlite', folder=tmpdir) 
+_2_6 self.db = DAL("sqlite://auth_rbac.sqlite", folder=tmpdir) 
 _2_7 
-_2_8 define_auth_rbac_model(self.db, dict(allowed_types=['user', 'group'])) 
-_2_9 rbac_migrations(self.db) 
-_3_0 return self.db 
-_3_1 
-_3_2 def __exit__(self, exc_type, exc_value, traceback): 
-_3_3 self.db.close() 
-_3_4 
-_3_5 return Database() 
+_2_8 settings = dict(allowed_types=["user", "group"], migrate=True) 
+_2_9 
+_3_0 define_auth_rbac_model(self.db, settings) 
+_3_1 rbac_migrations(self.db) 
+_3_2 return self.db 
+_3_3 
+_3_4 def __exit__(self, exc_type, exc_value, traceback): 
+_3_5 self.db.close() 
 _3_6 
-_3_7 
-_3_8@pytest.fixture(scope="module") 
-_3_9def rbac(database): 
-_4_0 with database as db: 
-_4_1 yield AuthRbac(db) 
-_4_2 
-_4_3 
-_4_4@pytest.fixture(scope="module") 
-_4_5def store(_=dotmap.DotMap()): 
-_4_6 print('store', _) 
-_4_7 return _ 
-_4_8 
-_4_9 
-_5_0@pytest.mark.incremental 
-_5_1class TestSequentially: 
-_5_2 def test_drop_all_test_users(self, database): 
-_5_3 with database as db: 
-_5_4 users = db(db.identity.email.contains('@test.nl')).select() 
-_5_5 db(db.identity.email.contains('@test.nl')).delete() 
-_5_6 for user in users: 
-_5_7 db((db.membership.member_of == user.object_id) | (db.membership.subject ==
+_3_7 return Database() 
+_3_8 
+_3_9 
+_4_0@pytest.fixture(scope="module") 
+_4_1def rbac(database): 
+_4_2 with database as db: 
+_4_3 yield AuthRbac(db) 
+_4_4 
+_4_5 
+_4_6@pytest.fixture(scope="module") 
+_4_7def store(_=dotmap.DotMap()): 
+_4_8 print("store", _) 
+_4_9 return _ 
+_5_0 
+_5_1 
+_5_2@pytest.mark.incremental 
+_5_3class TestSequentially: 
+_5_4 def test_drop_all_test_users(self, database): 
+_5_5 with database as db: 
+_5_6 users = db(db.identity.email.contains("@test.nl")).select() 
+_5_7 db(db.identity.email.contains("@test.nl")).delete() 
+_5_8 for user in users: 
+_5_9 db((db.membership.member_of == user.object_id) | (db.membership.subject ==
 user.object_id)).delete() 
-_5_8 db((db.permission.identity_object_id == user.object_id) | ( 
-_5_9 db.permission.target_object_id == user.object_id)).delete() 
-_6_0 db.commit() 
-_6_1 assert db(db.identity.email.contains('@test.nl')).count() == 0, 'Howcome
-@test.nl still exist?' 
-_6_2 
-_6_3 def test_user_creation(self, rbac, store): 
-_6_4 store.remco = rbac.add_user('remco@test.nl', 'remco', 'remco test',
-'secret', [])['object_id'] 
-_6_5 store.pietje = rbac.add_user('pietje@test.nl', 'pietje', 'pietje test',
-'secret', [])['object_id'] 
-_6_6 store.truus = rbac.add_user('truus@test.nl', 'truus', 'truus test',
-'secret', [])['object_id'] 
-_6_7 
-_6_8 def test_group_creation(self, rbac, store): 
-_6_9 store.articles = rbac.add_group('articles@test.nl', 'articles', [])
-['object_id'] 
-_7_0 store.all = rbac.add_group('all@test.nl', 'all', [])['object_id'] 
-_7_1 store.users = rbac.add_group('users@test.nl', 'users', [])['object_id'] 
-_7_2 store.admins = rbac.add_group('admins@test.nl', 'admins', [])['object_id'] 
-_7_3 
-_7_4 def test_item_creation(self, rbac, store): 
-_7_5 for name in 'abcde': 
-_7_6 store[name] = rbac.add_user('article_' + name + '@test.nl', name, 'article',
-'', [])[ 
-_7_7 'object_id'] 
-_7_8 
-_7_9 def test_stash_users_in_groups(self, rbac, store): 
-_8_0 rbac.add_membership(store.remco, store.admins) 
-_8_1 rbac.add_membership(store.pietje, store.users) 
-_8_2 rbac.add_membership(store.truus, store.users) 
-_8_3 rbac.add_membership(store.users, store.all) 
-_8_4 rbac.add_membership(store.admins, store.all) 
-_8_5 
-_8_6 def test_stash_items_in_groups(self, rbac, store): 
-_8_7 for name in 'abcde': 
-_8_8 rbac.add_membership(store[name], store.articles) 
-_8_9 
-_9_0 def test_add_some_permissions(self, rbac, store): 
-_9_1 rbac.add_permission(store.admins, store.articles, 'read') 
-_9_2 rbac.add_permission(store.admins, store.articles, 'write') 
-_9_3 rbac.add_permission(store.users, store.articles, 'read') 
-_9_4 
-_9_5 def test_first_level_memberships(self, rbac, store): 
-_9_6 assert rbac.has_membership(store.remco, store.admins) is True 
-_9_7 assert rbac.has_membership(store.pietje, store.users) is True 
-_9_8 assert rbac.has_membership(store.remco, store.users) is False 
-_9_9 assert rbac.has_membership(store.pietje, store.admins) is False 
-_1_0_0 
-_1_0_1 def test_second_level_memberships(self, rbac, store): 
-_1_0_2 assert rbac.has_membership(store.remco, store.all) is True 
-_1_0_3 assert rbac.has_membership(store.pietje, store.all) is True 
-_1_0_4 
-_1_0_5 def test_first_level_permissions(self, rbac, store): 
-_1_0_6 assert rbac.has_permission(store.admins, store.articles, 'read') is True 
-_1_0_7 assert rbac.has_permission(store.admins, store.articles, 'write') is True 
-_1_0_8 assert rbac.has_permission(store.users, store.articles, 'read') is True 
-_1_0_9 assert rbac.has_permission(store.users, store.articles, 'write') is False 
-_1_1_0 
-_1_1_1 def test_second_to_first_level_permissions(self, rbac, store): 
-_1_1_2 assert rbac.has_permission(store.remco, store.articles, 'read') is True 
-_1_1_3 assert rbac.has_permission(store.remco, store.articles, 'write') is True 
-_1_1_4 assert rbac.has_permission(store.pietje, store.articles, 'read') is True 
-_1_1_5 assert rbac.has_permission(store.pietje, store.articles, 'write') is False 
-_1_1_6 
-_1_1_7 def test_second_to_second_level_permissions(self, rbac, store): 
-_1_1_8 assert rbac.has_permission(store.remco, store.a, 'read') is True 
-_1_1_9 assert rbac.has_permission(store.remco, store.a, 'write') is True 
-_1_2_0 assert rbac.has_permission(store.pietje, store.a, 'read') is True 
-_1_2_1 assert rbac.has_permission(store.pietje, store.a, 'write') is False 
-_1_2_2 
-_1_2_3 def test_deeper_group_nesting(self, rbac, store): 
-_1_2_4 store.subadmins = rbac.add_group('sub_admins@test.nl', 'subadmins', [])
-['object_id'] 
-_1_2_5 store.subarticles = rbac.add_group('sub_articles@test.nl', 'subarticles',
-[])['object_id'] 
-_1_2_6 rbac.add_membership(store.subarticles, store.articles) 
-_1_2_7 rbac.add_membership(store.subadmins, store.admins) 
-_1_2_8 store.nested_admin = rbac.add_user('nested_admin@test.nl', 'nested_admin',
-'nested_admin test', 'secret', [])[ 
-_1_2_9 'object_id'] 
-_1_3_0 rbac.add_membership(store.nested_admin, store.subadmins) 
-_1_3_1 for name in 'stuvw': 
-_1_3_2 store[name] = rbac.add_user('article_' + name + '@test.nl', name,
-'subarticle', '', [])['object_id'] 
-_1_3_3 rbac.add_membership(store[name], store.subarticles) 
-_1_3_4 assert rbac.has_permission(store.nested_admin, store.s, 'read') is True 
-_1_3_5 
-_1_3_6 def test_removing_a_nested_group(self, rbac, store): 
-_1_3_7 rbac.remove_membership(store.nested_admin, store.subadmins) 
-_1_3_8 assert rbac.has_permission(store.nested_admin, store.s, 'read') is False 
+_6_0 db( 
+_6_1 (db.permission.identity_object_id == user.object_id) 
+_6_2 | (db.permission.target_object_id == user.object_id) 
+_6_3 ).delete() 
+_6_4 db.commit() 
+_6_5 assert db(db.identity.email.contains("@test.nl")).count() == 0, "Howcome
+@test.nl still exist?" 
+_6_6 
+_6_7 def test_user_creation(self, rbac, store): 
+_6_8 store.remco = rbac.add_user("remco@test.nl", "remco", "remco test",
+"secret", [])["object_id"] 
+_6_9 store.pietje = rbac.add_user("pietje@test.nl", "pietje", "pietje test",
+"secret", [])["object_id"] 
+_7_0 store.truus = rbac.add_user("truus@test.nl", "truus", "truus test",
+"secret", [])["object_id"] 
+_7_1 
+_7_2 def test_group_creation(self, rbac, store): 
+_7_3 store.articles = rbac.add_group("articles@test.nl", "articles", [])
+["object_id"] 
+_7_4 store.all = rbac.add_group("all@test.nl", "all", [])["object_id"] 
+_7_5 store.users = rbac.add_group("users@test.nl", "users", [])["object_id"] 
+_7_6 store.admins = rbac.add_group("admins@test.nl", "admins", [])["object_id"] 
+_7_7 
+_7_8 def test_item_creation(self, rbac, store): 
+_7_9 for name in "abcde": 
+_8_0 store[name] = rbac.add_user("article_" + name + "@test.nl", name, "article",
+"", [])["object_id"] 
+_8_1 
+_8_2 def test_stash_users_in_groups(self, rbac, store): 
+_8_3 rbac.add_membership(store.remco, store.admins) 
+_8_4 rbac.add_membership(store.pietje, store.users) 
+_8_5 rbac.add_membership(store.truus, store.users) 
+_8_6 rbac.add_membership(store.users, store.all) 
+_8_7 rbac.add_membership(store.admins, store.all) 
+_8_8 
+_8_9 def test_stash_items_in_groups(self, rbac, store): 
+_9_0 for name in "abcde": 
+_9_1 rbac.add_membership(store[name], store.articles) 
+_9_2 
+_9_3 def test_add_some_permissions(self, rbac, store): 
+_9_4 rbac.add_permission(store.admins, store.articles, "read") 
+_9_5 rbac.add_permission(store.admins, store.articles, "write") 
+_9_6 rbac.add_permission(store.users, store.articles, "read") 
+_9_7 
+_9_8 def test_first_level_memberships(self, rbac, store): 
+_9_9 assert rbac.has_membership(store.remco, store.admins) is True 
+_1_0_0 assert rbac.has_membership(store.pietje, store.users) is True 
+_1_0_1 assert rbac.has_membership(store.remco, store.users) is False 
+_1_0_2 assert rbac.has_membership(store.pietje, store.admins) is False 
+_1_0_3 
+_1_0_4 def test_second_level_memberships(self, rbac, store): 
+_1_0_5 assert rbac.has_membership(store.remco, store.all) is True 
+_1_0_6 assert rbac.has_membership(store.pietje, store.all) is True 
+_1_0_7 
+_1_0_8 def test_first_level_permissions(self, rbac, store): 
+_1_0_9 assert rbac.has_permission(store.admins, store.articles, "read") is True 
+_1_1_0 assert rbac.has_permission(store.admins, store.articles, "write") is True 
+_1_1_1 assert rbac.has_permission(store.users, store.articles, "read") is True 
+_1_1_2 assert rbac.has_permission(store.users, store.articles, "write") is False 
+_1_1_3 
+_1_1_4 def test_second_to_first_level_permissions(self, rbac, store): 
+_1_1_5 assert rbac.has_permission(store.remco, store.articles, "read") is True 
+_1_1_6 assert rbac.has_permission(store.remco, store.articles, "write") is True 
+_1_1_7 assert rbac.has_permission(store.pietje, store.articles, "read") is True 
+_1_1_8 assert rbac.has_permission(store.pietje, store.articles, "write") is False 
+_1_1_9 
+_1_2_0 def test_second_to_second_level_permissions(self, rbac, store): 
+_1_2_1 assert rbac.has_permission(store.remco, store.a, "read") is True 
+_1_2_2 assert rbac.has_permission(store.remco, store.a, "write") is True 
+_1_2_3 assert rbac.has_permission(store.pietje, store.a, "read") is True 
+_1_2_4 assert rbac.has_permission(store.pietje, store.a, "write") is False 
+_1_2_5 
+_1_2_6 def test_deeper_group_nesting(self, rbac, store): 
+_1_2_7 store.subadmins = rbac.add_group("sub_admins@test.nl", "subadmins", [])
+["object_id"] 
+_1_2_8 store.subarticles = rbac.add_group("sub_articles@test.nl", "subarticles",
+[])["object_id"] 
+_1_2_9 rbac.add_membership(store.subarticles, store.articles) 
+_1_3_0 rbac.add_membership(store.subadmins, store.admins) 
+_1_3_1 store.nested_admin = rbac.add_user("nested_admin@test.nl", "nested_admin",
+"nested_admin test", "secret", [])[ 
+_1_3_2 "object_id" 
+_1_3_3 ] 
+_1_3_4 rbac.add_membership(store.nested_admin, store.subadmins) 
+_1_3_5 for name in "stuvw": 
+_1_3_6 store[name] = rbac.add_user("article_" + name + "@test.nl", name,
+"subarticle", "", [])["object_id"] 
+_1_3_7 rbac.add_membership(store[name], store.subarticles) 
+_1_3_8 assert rbac.has_permission(store.nested_admin, store.s, "read") is True 
+_1_3_9 
+_1_4_0 def test_removing_a_nested_group(self, rbac, store): 
+_1_4_1 rbac.remove_membership(store.nested_admin, store.subadmins) 
+_1_4_2 assert rbac.has_permission(store.nested_admin, store.s, "read") is False 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1, created at 2024-05-
-16 17:13 +0200
+22 15:42 +0200
```

### Comparing `edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/migrations.py` & `edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/model.py` & `edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,23 +202,23 @@
         migrate=False,  # view
         redefine=redefine,
         primarykey=["root", "object_id"],  # composed, no primary key
     )
 
 
 def add_identity(
-        db: DAL,
-        email: str,
-        member_of: list[IdentityKey],
-        name: Optional[str] = None,
-        firstname: Optional[str] = None,
-        fullname: Optional[str] = None,
-        password: Optional[str] = None,
-        gid: Optional[IdentityKey] = None,
-        object_type: Optional[ObjectTypes] = None,
+    db: DAL,
+    email: str,
+    member_of: list[IdentityKey],
+    name: Optional[str] = None,
+    firstname: Optional[str] = None,
+    fullname: Optional[str] = None,
+    password: Optional[str] = None,
+    gid: Optional[IdentityKey] = None,
+    object_type: Optional[ObjectTypes] = None,
 ) -> str:
     """paramaters name and firstname are equal."""
     email = email.lower().strip()
     if object_type is None:
         raise ValueError("object_type parameter expected")
     object_id = gid or uuid.uuid4()
     result = db.identity.validate_and_insert(
@@ -239,16 +239,16 @@
         if get_group(db, group_id):
             # check each group if it exists.
             add_membership(db, identity_key=object_id, group_key=group_id)
     # db.commit()
     return str(object_id)
 
 
-def add_group(db: DAL, email: str, name: str, member_of: list[IdentityKey]):
-    return add_identity(db, email, member_of, name=name, object_type="group")
+def add_group(db: DAL, email: str, name: str, member_of: list[IdentityKey], gid: Optional[str] = None):
+    return add_identity(db, email, member_of, name=name, object_type="group", gid=gid)
 
 
 def remove_identity(db: DAL, object_id: IdentityKey):
     removed = db(db.identity.object_id == object_id).delete()
     # todo: remove permissions and group memberships
     # db.commit()
     return removed > 0
@@ -286,15 +286,15 @@
     :param key: can be the name of the group, the id, object_id or email_address
     :return: user record or None when not found
     """
     return get_identity(db, key, object_type="group")
 
 
 def authenticate_user(
-        db: DAL, password: Optional[str] = None, user: Optional[Identity] = None, key: Optional[IdentityKey] = None
+    db: DAL, password: Optional[str] = None, user: Optional[Identity] = None, key: Optional[IdentityKey] = None
 ) -> bool:
     if not password:
         return False
 
     if not user and key:
         user = get_user(db, key)
 
@@ -342,20 +342,20 @@
 def get_members(db: DAL, object_id: IdentityKey, bare: bool = True):
     query = db.recursive_members.root == object_id
     fields = [db.recursive_members.object_id, db.recursive_members.object_type] if bare else []
     return db(query).select(*fields)
 
 
 def add_permission(
-        db: DAL,
-        identity_key: IdentityKey | typing.Literal["*"],
-        target_oid: IdentityKey | typing.Literal["*"],
-        privilege: str,
-        starts: dt.datetime | str = DEFAULT_STARTS,
-        ends: dt.datetime | str = DEFAULT_ENDS,
+    db: DAL,
+    identity_key: IdentityKey | typing.Literal["*"],
+    target_oid: IdentityKey | typing.Literal["*"],
+    privilege: str,
+    starts: dt.datetime | str = DEFAULT_STARTS,
+    ends: dt.datetime | str = DEFAULT_ENDS,
 ) -> None:
     identity_oid = key_lookup(db, identity_key)
     starts = unstr_datetime(starts)
     ends = unstr_datetime(ends)
     if has_permission(db, identity_oid, target_oid, privilege, when=starts):
         # permission already granted. just skip it
         print(
@@ -374,15 +374,15 @@
     )
     if e := result.get("errors"):
         raise ValueError(e)
     # db.commit()
 
 
 def remove_permission(
-        db: DAL, identity_key: IdentityKey, target_oid: IdentityKey, privilege: str, when: When | None = DEFAULT
+    db: DAL, identity_key: IdentityKey, target_oid: IdentityKey, privilege: str, when: When | None = DEFAULT
 ) -> bool:
     identity_oid = key_lookup(db, identity_key)
     if when is DEFAULT:
         when = dt.datetime.now()
     else:
         when = unstr_datetime(when)
     # base object is is the root to check for, user or group
@@ -412,15 +412,15 @@
     if source_id := getattr(source, "_id", None):
         other._id = other[source_id.name]
     db[alias] = other
     return other
 
 
 def has_permission(
-        db: DAL, user_or_group_key: IdentityKey, target_oid: IdentityKey, privilege: str, when: When | None = DEFAULT
+    db: DAL, user_or_group_key: IdentityKey, target_oid: IdentityKey, privilege: str, when: When | None = DEFAULT
 ) -> bool:
     root_oid = key_lookup(db, user_or_group_key)
     # the permission system
     if when is DEFAULT:
         when = dt.datetime.now()
     else:
         when = unstr_datetime(when)
```

### Comparing `edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/rbac.py` & `edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/rbac.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,24 +59,37 @@
     @staticmethod
     def _error(msg):
         print("ERROR:", msg)
 
     # gebruik event en rpc live templates (mobiel)
 
     def add_user(
-        self, email: str, firstname: str, fullname: str, password: str, member_of: list[IdentityKey]
+        self,
+        email: str,
+        firstname: str,
+        fullname: str,
+        password: str,
+        member_of: list[IdentityKey],
+        gid: Optional[str] = None,
     ) -> UserDict:
         # check if exists
         email = email.lower().strip()
-        user = model.get_user(self.db, email)
+        user = model.get_user(self.db, gid or email)
         if user:
             raise ValueError("User already exists")
         else:
             object_id = model.add_identity(
-                self.db, email, member_of, password=password, firstname=firstname, fullname=fullname, object_type="user"
+                self.db,
+                email,
+                member_of,
+                password=password,
+                firstname=firstname,
+                fullname=fullname,
+                object_type="user",
+                gid=gid,
             )
             rec = model.get_user(self.db, object_id)
             return dict(
                 object_id=rec.object_id,
                 email=rec.email,
                 firstname=rec.firstname,
                 fullname=rec.fullname,
@@ -113,25 +126,33 @@
     ) -> MinimalIdentityDict:
         # check if exists
         email = email.lower().strip()
 
         if model.get_identity(self.db, email, object_type):
             raise ValueError("Item already exists")
         else:
-            object_id = model.add_identity(self.db, email, member_of, name, password=password, object_type=object_type)
+            object_id = model.add_identity(
+                self.db, email, member_of, name, password=password, object_type=object_type, gid=gid
+            )
             rec = model.get_identity(self.db, object_id, object_type=object_type)
             return dict(object_id=rec.object_id, email=rec.email, name=rec.fullname)
 
-    def add_group(self, email: str, name: str, member_of: list[IdentityKey]) -> MinimalIdentityDict:
+    def add_group(
+        self,
+        email: str,
+        name: str,
+        member_of: list[IdentityKey],
+        gid: Optional[str] = None,
+    ) -> MinimalIdentityDict:
         # check if exists
         email = email.lower().strip()
-        if model.get_group(self.db, email):
+        if model.get_group(self.db, gid or email):
             raise ValueError("Group already exists")
         else:
-            object_id = model.add_group(self.db, email, name, member_of)
+            object_id = model.add_group(self.db, email, name, member_of, gid=gid)
             rec = model.get_group(self.db, object_id)
             return dict(object_id=rec.object_id, email=rec.email, name=rec.firstname)
 
     def update_identity(
         self,
         object_id: IdentityKey,
         email: Optional[str] = None,
```

### Comparing `edwh_auth_rbac-0.3.0/tests/test_migrate.py` & `edwh_auth_rbac-0.4.0/tests/test_migrate.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tempfile
 
+import pytest
 from pydal import DAL
 from testcontainers.postgres import PostgresContainer
-import pytest
 
 DB_NAME = "edwh_rbac_test"
 
 postgres = PostgresContainer("postgres:16-alpine", dbname=DB_NAME)
 
 
 @pytest.fixture(scope="module", autouse=True)
```

### Comparing `edwh_auth_rbac-0.3.0/tests/test_rbac.py` & `edwh_auth_rbac-0.4.0/tests/test_rbac.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from src.edwh_auth_rbac.migrations import rbac_views
 from src.edwh_auth_rbac.model import define_auth_rbac_model
 from src.edwh_auth_rbac.rbac import AuthRbac
 
 namespace = uuid.UUID("84f5c757-4be0-49c8-a3ba-4f4d79167839")
 
 FAKE_TEMPDIR = False
+
+
 # FAKE_TEMPDIR = True
 
 
 @pytest.fixture(scope="module")
 def tmpdir():
     with tempfile.TemporaryDirectory() as tmpdirname:
         if FAKE_TEMPDIR:
@@ -176,7 +178,23 @@
         admin1 = rbac.add_user("admin1@example", "Admin1", "Admin One", "secure", [admins])
 
         assert rbac.has_permission(admin1, item_gid, "read")
         assert rbac.has_permission(admin1, item_gid, "write")
 
         assert rbac.has_permission(user, item_gid, "read")
         assert not rbac.has_permission(user, item_gid, "write")
+
+    def test_existing_uuids(self, rbac):
+        assert (
+            rbac.add_user("c3@user", "c3", "c3 user", "verysecrets", [], gid="c3685794-5b9f-41d9-a7ec-d7efcd87d253")[
+                "object_id"
+            ]
+            == "c3685794-5b9f-41d9-a7ec-d7efcd87d253"
+        )
+        assert (
+            rbac.add_group("ec@group", "ec", [], gid="ecf43e58-a0ec-42fd-8634-bb498e2c4273")["object_id"]
+            == "ecf43e58-a0ec-42fd-8634-bb498e2c4273"
+        )
+        assert (
+            rbac.add_item("2d@item", "2d", [], gid="2d4d8ac4-921e-403f-be06-e34b353b4f43")["object_id"]
+            == "2d4d8ac4-921e-403f-be06-e34b353b4f43"
+        )
```

### Comparing `edwh_auth_rbac-0.3.0/pyproject.toml` & `edwh_auth_rbac-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.3.0/PKG-INFO` & `edwh_auth_rbac-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: edwh-auth-rbac
-Version: 0.3.0
+Version: 0.4.0
 Summary: Recursive Memberships and Permissions for the Education Warehouse Authentication System
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-auth-rbac#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-auth-rbac/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-auth-rbac
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 Keywords: edwh,omgeving,whitelabel
```

