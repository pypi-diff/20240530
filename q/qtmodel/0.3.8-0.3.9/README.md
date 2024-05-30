# Comparing `tmp/qtmodel-0.3.8.tar.gz` & `tmp/qtmodel-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmodel-0.3.8.tar", last modified: Tue May 21 02:58:42 2024, max compression
+gzip compressed data, was "qtmodel-0.3.9.tar", last modified: Wed May 29 08:23:54 2024, max compression
```

## Comparing `qtmodel-0.3.8.tar` & `qtmodel-0.3.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 02:58:42.032694 qtmodel-0.3.8/
--rw-rw-rw-   0        0        0    41242 2024-05-21 02:58:42.031692 qtmodel-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    40814 2024-05-21 02:58:02.000000 qtmodel-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 02:58:42.024146 qtmodel-0.3.8/qtmodel/
--rw-rw-rw-   0        0        0       59 2024-05-20 07:23:27.000000 qtmodel-0.3.8/qtmodel/__init__.py
--rw-rw-rw-   0        0        0     1637 2024-05-20 08:58:37.000000 qtmodel-0.3.8/qtmodel/qt_db.py
--rw-rw-rw-   0        0        0     2395 2024-05-20 07:25:48.000000 qtmodel-0.3.8/qtmodel/qt_helper.py
--rw-rw-rw-   0        0        0    94041 2024-05-21 02:56:46.000000 qtmodel-0.3.8/qtmodel/qt_mdb.py
--rw-rw-rw-   0        0        0    14370 2024-05-20 02:45:48.000000 qtmodel-0.3.8/qtmodel/res_db.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:58:42.029692 qtmodel-0.3.8/qtmodel.egg-info/
--rw-rw-rw-   0        0        0    41242 2024-05-21 02:58:41.000000 qtmodel-0.3.8/qtmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-21 02:58:41.000000 qtmodel-0.3.8/qtmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 02:58:41.000000 qtmodel-0.3.8/qtmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-21 02:58:41.000000 qtmodel-0.3.8/qtmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 02:58:42.032694 qtmodel-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-05-21 02:58:37.000000 qtmodel-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:23:54.640035 qtmodel-0.3.9/
+-rw-rw-rw-   0        0        0    47495 2024-05-29 08:23:54.639009 qtmodel-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    47067 2024-05-29 08:22:57.000000 qtmodel-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 08:23:54.630711 qtmodel-0.3.9/qtmodel/
+-rw-rw-rw-   0        0        0       93 2024-05-21 08:50:37.000000 qtmodel-0.3.9/qtmodel/__init__.py
+-rw-rw-rw-   0        0        0     2420 2024-05-21 08:28:12.000000 qtmodel-0.3.9/qtmodel/qt_db.py
+-rw-rw-rw-   0        0        0     2395 2024-05-20 07:25:48.000000 qtmodel-0.3.9/qtmodel/qt_helper.py
+-rw-rw-rw-   0        0        0    85749 2024-05-29 08:16:52.000000 qtmodel-0.3.9/qtmodel/qt_mdb.py
+-rw-rw-rw-   0        0        0    18763 2024-05-29 08:22:57.000000 qtmodel-0.3.9/qtmodel/qt_odb.py
+-rw-rw-rw-   0        0        0    14370 2024-05-20 02:45:48.000000 qtmodel-0.3.9/qtmodel/res_db.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:23:54.636986 qtmodel-0.3.9/qtmodel.egg-info/
+-rw-rw-rw-   0        0        0    47495 2024-05-29 08:23:54.000000 qtmodel-0.3.9/qtmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-29 08:23:54.000000 qtmodel-0.3.9/qtmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:23:54.000000 qtmodel-0.3.9/qtmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-29 08:23:54.000000 qtmodel-0.3.9/qtmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:23:54.640035 qtmodel-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      758 2024-05-29 08:17:54.000000 qtmodel-0.3.9/setup.py
```

### Comparing `qtmodel-0.3.8/PKG-INFO` & `qtmodel-0.3.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,242 +1,321 @@
-Metadata-Version: 2.1
-Name: qtmodel
-Version: 0.3.8
-Summary: python modeling for qt  24/05/06 
-Home-page: https://github.com/Inface0443/pyqt
-Author: dqy-zhj
-Author-email: 1105417715@qq.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
-# 最新版本 V0.3.8 - 2024.05.21 
+# 最新版本 V0.3.9 - 2024.05.29 
 > pip install --upgrade qtmodel
 - 优化部分调用
 
 ##  项目管理
+### update_model
+刷新模型信息
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.update_model()
+```  
+Returns: 无
+### update_app_stage
+切换模型前后处理状态
+> 参数:  
+> num: 1-前处理  2-后处理  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.update_app_stage(1)
+mdb.update_app_stage(2)
+```  
+Returns: 无
+### do_solve
+运行分析
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.do_solve()
+```  
+Returns: 无
 ### initial
 初始化模型,新建模型
+> 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.initial()
 ```  
+Returns: 无
 ### open_file
 打开bfmd文件
+> 参数:  
+> file_path: 文件全路径  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.open_file("a.bfmd")
 ```  
-### save_file
-保存bfmd文件
+Returns: 无
+### close_project
+关闭项目
+> 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.save_file("a.bfmd")
+mdb.close_project()
 ```  
-### close_project
-关闭项目
+Returns: 无
+### save_file
+保存bfmd文件
+> 参数:  
+> file_path: 文件全路径  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.close_project()
+mdb.save_file("a.bfmd")
 ```  
+Returns: 无
 ### import_command
 导入命令
 > 参数:  
 > command:命令字符  
-> command_type:命令类型 1-桥通命令  
+> command_type:命令类型 1-桥通命令 目前仅支持桥通命令  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.import_command("*SECTION")
 ```  
+Returns: 无
+### import_file
+导入文件
+> 参数:  
+> file_path:导入文件(.mct/.qdat/.dxf/.3dx)  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.import_file("a.mct")
+```  
+Returns: 无
 ### export_file
 导入命令
 > 参数:  
-> file_path:导出文件(.mct/.qdat/.PGF/.3dx)  
+> file_path:导出文件全路径，支持格式(.mct/.qdat/.PGF/.3dx)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.export_file("a.mct")
 ```  
-### import_file
-导入命令
+Returns: 无
+##  节点单元操作
+### add_nodes
+添加多个节点，可以选择指定节点编号
 > 参数:  
-> file_path:导入文件(.mct/.qdat/.dxf/.3dx)  
+> node_list:节点坐标信息 [[x1,y1,z1],...]或 [[id1,x1,y1,z1]...]  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.import_file("a.mct")
+mdb.add_nodes([[1,2,3],[4,5,6]])
+mdb.add_nodes([[1,1,2,3],[2,4,5,6]])
 ```  
-### do_solve
-运行分析
+Returns: 无
+### add_node
+根据坐标信息和节点编号添加节点，默认自动识别编号
+> 参数:  
+> x: 节点坐标x  
+> y: 节点坐标y  
+> z: 节点坐标z  
+> index: 节点编号，默认自动识别编号 (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.do_solve()
+mdb.add_node(1,2,3)
+mdb.add_node(x= 1,y = 2,z = 4,index = 2)
 ```  
-##  节点单元操作
+Returns: 无
+### update_node_id
+根据坐标信息和节点编号添加节点，默认自动识别编号
+> 参数:  
+> node_id: 节点编号  
+> new_id: 新节点编号  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.update_node_id(1,2)
+```  
+Returns: 无
+### merge_nodes
+根据坐标信息和节点编号添加节点，默认自动识别编号
+> 参数:  
+> ids: 合并节点集合  默认全部节点  
+> tolerance: 合并容许误差  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.merge_nodes()
+```  
+Returns: 无
+### remove_node
+删除指定节点,不输入参数时默认删除所有节点
+> 参数:  
+> ids:节点编号  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.remove_node()
+mdb.remove_node(ids=1)
+mdb.remove_node(ids=[1,2,3])
+```  
+Returns: 无
+### renumber_node
+节点编号重拍
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.renumber_node()
+```  
+Returns: 无
+### move_node
+移动节点坐标
+> 参数:  
+> node_id：节点号  
+> offset_x:X轴偏移量  
+> offset_y:Y轴偏移量  
+> offset_z:Z轴偏移量  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.move_node(1,1.5,1.5,1.5)
+```  
+Returns: 无
 ### add_structure_group
 添加结构组
 > 参数:  
 > name: 结构组名  
 > index: 结构组编号(非必须参数)，默认自动识别当前编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_structure_group(name="新建结构组1")
 mdb.add_structure_group(name="新建结构组2",index=2)
 ```  
+Returns: 无
 ### remove_structure_group
 可根据结构与组名或结构组编号删除结构组，当组名和组编号均为默认则删除所有结构组
 > 参数:  
 > name:结构组名称  
 > index:结构组编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_structure_group(name="新建结构组1")
 mdb.remove_structure_group(index = 2)
 ```  
+Returns: 无
 ### add_structure_to_group
 为结构组添加节点和/或单元
 > 参数:  
 > name: 结构组名  
 > node_ids: 节点编号列表(可选参数)  
 > element_ids: 单元编号列表(可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
 ```  
+Returns: 无
 ### remove_structure_in_group
 为结构组删除节点和/或单元
 > 参数:  
 > name: 结构组名  
 > node_ids: 节点编号列表(可选参数)  
 > element_ids: 单元编号列表(可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
 ```  
-### add_node
-根据坐标信息和节点编号添加节点，默认自动识别编号
-> 参数:  
-> x: 节点坐标x  
-> y: 节点坐标y  
-> z: 节点坐标z  
-> index: 节点编号，默认自动识别编号 (可选参数)  
-```Python
-# 示例代码
-from qtmodel import mdb
-mdb.add_node(1,2,3)
-mdb.add_node(x= 1,y = 2,z = 4,index = 2)
-```  
-### add_nodes
-添加多个节点，可以选择指定节点编号
-> 参数:  
-> node_list:节点坐标信息 [[x1,y1,z1],...]或 [[id1,x1,y1,z1]...]  
-```Python
-# 示例代码
-from qtmodel import mdb
-mdb.add_nodes([[1,2,3],[4,5,6]])
-mdb.add_nodes([[1,1,2,3],[2,4,5,6]])
-```  
-### remove_node
-删除指定节点,不输入参数时默认删除所有节点
-> 参数:  
-> index:节点编号  
-```Python
-# 示例代码
-from qtmodel import mdb
-mdb.remove_node()
-mdb.remove_node(index=1)
-```  
+Returns: 无
 ### add_element
 根据单元编号和单元类型添加单元
 > 参数:  
 > index:单元编号  
 > ele_type:单元类型 1-梁 2-索 3-杆 4-板  
 > node_ids:单元对应的节点列表 [i,j] 或 [i,j,k,l]  
 > beta_angle:贝塔角  
 > mat_id:材料编号  
 > sec_id:截面编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_element(index=1,ele_type=1,node_ids=[1,2],beta_angle=1,mat_id=1,sec_id=1)
 ```  
+Returns: 无
 ### remove_element
 删除指定编号的单元
 > 参数:  
 > index: 单元编号,默认时删除所有单元  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_element()
 mdb.remove_element(index=1)
 ```  
+Returns: 无
 ##  材料操作
 ### add_material
 添加材料
 > 参数:  
 > index:材料编号,默认自动识别 (可选参数)  
 > name:材料名称  
-> material_type: 材料类型  
+> mat_type: 材料类型  
 > standard:规范名称  
 > database:数据库  
 > construct_factor:构造系数  
 > modified:是否修改默认材料参数,默认不修改 (可选参数)  
 > data_info:材料参数列表[弹性模量,容重,泊松比,热膨胀系数] (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.add_material(index=1,name="混凝土材料1",material_type="混凝土",standard="公路18规范",database="C50")
-mdb.add_material(index=1,name="自定义材料1",material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
+mdb.add_material(index=1,name="混凝土材料1",mat_type="混凝土",standard="公路18规范",database="C50")
+mdb.add_material(index=1,name="自定义材料1",mat_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
 ```  
+Returns: 无
 ### add_time_material
 添加收缩徐变材料
 > 参数:  
 > index: 指定收缩徐变编号,默认则自动识别 (可选参数)  
 > name: 收缩徐变名  
 > code_index: 收缩徐变规范索引  
 > time_parameter: 对应规范的收缩徐变参数列表,默认不改变规范中信息 (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_time_material(index=1,name="收缩徐变材料1",code_index=1)
 ```  
+Returns: 无
 ### update_material_creep
 将收缩徐变参数连接到材料
 > 参数:  
 > index: 材料编号  
 > creep_id: 收缩徐变编号  
 > f_cuk: 材料标准抗压强度,仅自定义材料是需要输入  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.update_material_creep(index=1,creep_id=1,f_cuk=5e7)
 ```  
+Returns: 无
 ### remove_material
 删除指定材料
 > 参数:  
 > index:指定材料编号，默认则删除所有材料  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_material()
 mdb.remove_material(index=1)
 ```  
+Returns: 无
 ##  截面操作
 ### add_parameter_section
 添加截面信息
 > 参数:  
 > index: 截面编号,默认自动识别  
 > name:截面名称  
 > sec_type:参数截面类型名称,支持以下类型  
@@ -262,14 +341,15 @@
 # 示例代码
 from qtmodel import mdb
 mdb.add_parameter_section(name="截面1",sec_type="矩形",sec_info=[2,4],bias_type="中心")
 mdb.add_parameter_section(name="截面2",sec_type="混凝土箱梁",box_height=2,box_number=3,
 sec_info=[0.02,0,12,3,1,2,1,5,6,0.2,0.4,0.1,0.13,0.28,0.3,0.5,0.5,0.5,0.2],
 charm_info=["1*0.2,0.1*0.2","0.5*0.15,0.3*0.2","0.4*0.2","0.5*0.2"])
 ```  
+Returns: 无
 ### add_steel_section
 添加钢梁截面,包括参数型钢梁截面和自定义带肋钢梁截面
 > 参数:  
 > index:  
 > name:  
 > sec_type:截面类型 1-工字钢梁  2-箱型钢梁  
 > sec_info:截面信息  
@@ -290,48 +370,55 @@
 from qtmodel import mdb
 mdb.add_steel_section(name="钢梁截面1",sec_type=1,sec_info=[0,0,0.5,0.5,0.5,0.5,0.7,0.02,0.02,0.02])
 mdb.add_steel_section(name="钢梁截面2",sec_type=2,sec_info=[0,0.15,0.25,0.5,0.25,0.15,0.4,0.15,0.7,0.02,0.02,0.02,0.02],
 rib_info = {"板肋1": [0.1,0.02],"T形肋1":[0.1,0.02,0.02,0.02]},
 rib_place = [(0, 0, 0, [(0.1, "板肋1", 2, "默认名称1"), (0.2, "板肋1", 2, "默认名称2")]), (0, 0, 1, [(0.1, "T形肋1", 0, "默认名称3")])],
 bias_type="中上")
 ```  
+Returns: 无
 ### add_user_section
 添加自定义截面,目前仅支持特性截面
 > 参数:  
 > index:截面编号  
 > name:截面名称  
 > sec_type:截面类型  
 > property_info:截面特性列表  
+> main_loop:主线圈坐标集合 [(-1,-1),(5,0),(5,5),(-1,5)] 目前只支持单一线圈  
+> sub_loops:次线圈坐标集合 [[(0,0),(0,1),(1,1,)], [(2,2),(3,2),(3,3)]]  
+> sec_lines:线宽集合[(x1,y1,x2,y3,thick),]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_user_section(name="自定义特性截面",property_info=[i for i in range(25)])
 ```  
+Returns: 无
 ### add_tapper_section
 添加变截面,需先建立单一截面
 > 参数:  
 > index:截面编号  
 > name:截面名称  
 > begin_id:截面始端编号  
 > end_id:截面末端编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_tapper_section(name="变截面1",begin_id=1,end_id=2)
 ```  
+Returns: 无
 ### remove_section
 删除截面信息
 > 参数:  
 > index: 截面编号,参数为默认时删除全部截面  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_section()
 mdb.remove_section(1)
 ```  
+Returns: 无
 ##  板厚操作
 ### add_thickness
 添加板厚
 > 参数:  
 > index: 板厚id  
 > name: 板厚名称  
 > t:   板厚度  
@@ -345,24 +432,26 @@
 > rib_l: 横向肋板信息  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_thickness(name="厚度1", t=0.2,thick_type=0,bias_info=(0,0.8))
 mdb.add_thickness(name="厚度2", t=0.2,thick_type=1,rib_pos=0,dist_v=0.1,rib_v=[1,1,0.02,0.02])
 ```  
+Returns: 无
 ### remove_thickness
 删除板厚
 > 参数:  
 > index:板厚编号,默认时删除所有板厚信息  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_thickness()
 mdb.remove_thickness(index=1)
 ```  
+Returns: 无
 ### add_tapper_section_group
 添加变截面组
 > 参数:  
 > ids:变截面组编号  
 > name: 变截面组名  
 > factor_w: 宽度方向变化阶数 线性(1.0) 非线性(!=1.0)  
 > factor_h: 高度方向变化阶数 线性(1.0) 非线性(!=1.0)  
@@ -371,106 +460,115 @@
 > dis_w: 宽度方向距离  
 > dis_h: 高度方向距离  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_tapper_section_group(ids=[1,2,3,4],name="变截面组1")
 ```  
+Returns: 无
 ### update_section_bias
 更新截面偏心
 > 参数:  
 > index:截面编号  
 > bias_type:偏心类型  
 > center_type:中心类型  
 > shear_consider:考虑剪切  
 > bias_point:自定义偏心点(仅自定义类型偏心需要)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.update_section_bias(index=1,bias_type="中上",center_type="几何中心")
 mdb.update_section_bias(index=1,bias_type="自定义",bias_point=[0.1,0.2])
 ```  
+Returns: 无
 ##  边界操作
 ### add_boundary_group
 新建边界组
 > 参数:  
 > name:边界组名  
 > index:边界组编号，默认自动识别当前编号 (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_boundary_group(name="边界组1")
 ```  
+Returns: 无
 ### remove_boundary_group
 按照名称删除边界组
 > 参数:  
 > name: 边界组名称，默认删除所有边界组 (非必须参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_boundary_group()
 mdb.remove_boundary_group(name="边界组1")
 ```  
+Returns: 无
 ### remove_all_boundary
 根据边界组名称、边界的类型和编号删除边界信息,默认时删除所有边界信息
 > 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_all_boundary()
 ```  
+Returns: 无
 ### remove_boundary
 根据节点号删除一般支撑、弹性支承/根据单元号删除梁端约束/根据主节点号删除主从约束/根据从节点号删除约束方程
 > 参数:  
 > remove_id:节点号 or 单元号 or主节点号  or 从节点号  
 > bd_type:边界类型  
 > _1-一般支承 2-弹性支承 3-主从约束 4-弹性连接 5-约束方程 6-梁端约束_  
 > group:边界所处边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_boundary(remove_id = 1, bd_type = 1,group="边界组1")
 ```  
+Returns: 无
 ### add_general_support
 添加一般支承
 > 参数:  
 > node_id:节点编号  
 > boundary_info:边界信息  [X,Y,Z,Rx,Ry,Rz]  
 > _ture-固定 false-自由_  
 > group_name:边界组名,默认为默认边界组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_general_support(node_id=1, boundary_info=[True,True,True,False,False,False])
 ```  
+Returns: 无
 ### add_elastic_support
 添加弹性支承
 > 参数:  
 > node_id:节点编号  
 > support_type:支承类型 1-线性  2-受拉  3-受压  
 > boundary_info:边界信息 受拉和受压时列表长度为1  线性时列表长度为6  
 > group_name:边界组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_elastic_support(node_id=1,support_type=1,boundary_info=[1e6,0,1e6,0,0,0])
 ```  
+Returns: 无
 ### add_master_slave_link
 添加主从约束
 > 参数:  
 > master_id:主节点号  
 > slave_id:从节点号  
 > boundary_info:边界信息 [X,Y,Z,Rx,Ry,Rz]  
 > _ture-固定 false-自由_  
 > group_name:边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_master_slave_link(master_id=1,slave_id=2,boundary_info=[True,True,True,False,False,False])
 ```  
+Returns: 无
 ### add_elastic_link
 添加弹性连接
 > 参数:  
 > link_type:节点类型  
 > _1-一般弹性连接 2-刚性连接 3-受拉弹性连接 4-受压弹性连接_  
 > start_id:起始节点号  
 > end_id:终节点号  
@@ -482,39 +580,42 @@
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_elastic_link(link_type=1,start_id=1,end_id=2,boundary_info=[1e6,1e6,1e6,0,0,0])
 mdb.add_elastic_link(link_type=2,start_id=1,end_id=2)
 mdb.add_elastic_link(link_type=3,start_id=1,end_id=2,kx=1e6)
 ```  
+Returns: 无
 ### add_beam_constraint
 添加梁端约束
 > 参数:  
 > beam_id:梁号  
 > info_i:i端约束信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > info_j:j端约束信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > group_name:边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_constraint(beam_id=2,info_i=[True,True,True,False,False,False],info_j=[True,True,True,False,False,False])
 ```  
+Returns: 无
 ### add_node_axis
 添加节点坐标
 > 参数:  
 > input_type:输入方式 1-角度 2-三点  3-向量  
 > node_id:节点号  
 > coord_info:局部坐标信息 -List<float>(角)  -List<List<float>>(三点 or 向量)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_node_axis(input_type=1,node_id=1,coord_info=[45,45,45])
 mdb.add_node_axis(input_type=2,node_id=1,coord_info=[[0,0,1],[0,1,0],[1,0,0]])
 mdb.add_node_axis(input_type=3,node_id=1,coord_info=[[0,0,1],[0,1,0]])
 ```  
+Returns: 无
 ##  移动荷载
 ### add_standard_vehicle
 添加标准车辆
 > 参数:  
 > name: 车辆荷载名称  
 > standard_code: 荷载规范  
 > _1-中国铁路桥涵规范(Q/CR 9300-2017)_  
@@ -533,48 +634,52 @@
 > load_length: 默认为0即不限制荷载长度  (铁路桥涵规范2017 所需参数)  
 > n:车厢数: 默认6节车厢 (城市轨道交通桥梁规范2017 所需参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_standard_vehicle("高速铁路",standard_code=1,load_type="高速铁路")
 ```  
+Returns: 无
 ### add_node_tandem
 添加节点纵列
 > 参数:  
 > name:节点纵列名  
 > start_id:起始节点号  
 > node_ids:节点列表  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_node_tandem("节点纵列1",1,[i+1 for i in range(12)])
 ```  
+Returns: 无
 ### add_influence_plane
 添加影响面
 > 参数:  
 > name:影响面名称  
 > tandem_names:节点纵列名称组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_influence_plane("影响面1",["节点纵列1","节点纵列2"])
 ```  
+Returns: 无
 ### add_lane_line
 添加车道线
 > 参数:  
 > name:车道线名称  
 > influence_name:影响面名称  
 > tandem_name:节点纵列名  
 > offset:偏移  
 > lane_width:车道宽度  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_lane_line("车道1","影响面1","节点纵列1",offset=0,lane_width=3.1)
 ```  
+Returns: 无
 ### add_live_load_case
 添加移动荷载工况
 > 参数:  
 > name:荷载工况名  
 > influence_plane:影响线名  
 > span:跨度  
 > car_detail: 汽车相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)  
@@ -582,89 +687,97 @@
 > metro_detail: 轻轨相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)  
 > sub_case:子工况信息 [(车辆名称,系数,["车道1","车道2"])...]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_live_load_case("活载工况1","影响面1",100,sub_case=[("车辆名称",1.0,["车道1","车道2"]),])
 ```  
+Returns: 无
 ### remove_vehicle
 删除车辆信息
 > 参数:  
 > index:车辆荷载编号  
 > name:车辆名称  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_vehicle(index=1)
 mdb.remove_vehicle(name="车辆名称")
 ```  
+Returns: 无
 ### remove_node_tandem
 按照 节点纵列编号/节点纵列名 删除节点纵列
 > 参数:  
 > index:节点纵列编号  
 > name:节点纵列名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_node_tandem(index=1)
 mdb.remove_node_tandem(name="节点纵列1")
 ```  
+Returns: 无
 ### remove_influence_plane
 按照 影响面编号/影响面名称 删除影响面
 > 参数:  
 > index:影响面编号  
 > name:影响面名称  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_influence_plane(index=1)
 mdb.remove_influence_plane(name="影响面1")
 ```  
+Returns: 无
 ### remove_lane_line
 按照 车道线编号/车道线名称 删除车道线
 > 参数:  
 > name:车道线名称  
 > index:车道线编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_lane_line(index=1)
 mdb.remove_lane_line(name="车道线1")
 ```  
+Returns: 无
 ### remove_live_load_case
 删除移动荷载工况
 > 参数:  
 > name:移动荷载工况名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_live_load_case(name="活载工况1")
 ```  
+Returns: 无
 ##  钢束操作
 ### add_tendon_group
 按照名称添加钢束组，添加时可指定钢束组id
 > 参数:  
 > name: 钢束组名称  
 > index: 钢束组编号(非必须参数)，默认自动识别  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_tendon_group(name="钢束组1")
 ```  
+Returns: 无
 ### remove_tendon_group
 按照钢束组名称或钢束组编号删除钢束组，两参数均为默认时删除所有钢束组
 > 参数:  
 > name:钢束组名称,默认自动识别 (可选参数)  
 > index:钢束组编号,默认自动识别 (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_tendon_group(name="钢束组1")
 mdb.remove_tendon_group(index=1)
 ```  
+Returns: 无
 ### add_tendon_property
 添加钢束特性
 > 参数:  
 > name:钢束特性名  
 > index:钢束编号,默认自动识别 (可选参数)  
 > tendon_type: 0-PRE 1-POST  
 > material_id: 钢材材料编号  
@@ -680,14 +793,15 @@
 > slip_info: 滑移信息[始端距离,末端距离] 默认为[0.006, 0.006]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_tendon_property(name="钢束1",tendon_type=0,material_id=1,duct_type=1,steel_type=1,
 steel_detail=[0.00014,0.10,0.25,0.0015],loos_detail=(1,1,1))
 ```  
+Returns: 无
 ### add_tendon_3d
 添加三维钢束
 > 参数:  
 > name:钢束名称  
 > property_name:钢束特性名称  
 > group_name:默认钢束组  
 > num:根数  
@@ -706,142 +820,155 @@
 # 示例代码
 from qtmodel import mdb
 mdb.add_tendon_3d("BB1",property_name="22-15",num=2,position_type=1,
 control_points=[(0,0,-1,0),(10,0,-1,0)],point_insert=(0,0,0))
 mdb.add_tendon_3d("BB1",property_name="22-15",num=2,position_type=2,
 control_points=[(0,0,-1,0),(10,0,-1,0)],point_insert=(1,1,1),track_group="轨迹线结构组1")
 ```  
+Returns: 无
 ### remove_tendon
 按照名称或编号删除钢束,默认时删除所有钢束
 > 参数:  
 > name:钢束名称  
 > index:钢束编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_tendon(name="钢束1")
 mdb.remove_tendon(index=1)
 mdb.remove_tendon()
 ```  
+Returns: 无
 ### remove_tendon_property
 按照名称或编号删除钢束组,默认时删除所有钢束组
 > 参数:  
 > name:钢束组名称  
 > index:钢束组编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_tendon_property(name="钢束特性1")
 mdb.remove_tendon_property(index=1)
 mdb.remove_tendon_property()
 ```  
+Returns: 无
 ### add_nodal_mass
 添加节点质量
 > 参数:  
 > node_id:节点编号  
 > mass_info:[m,rmX,rmY,rmZ]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_nodal_mass(node_id=1,mass_info=(100,0,0,0))
 ```  
+Returns: 无
 ### remove_nodal_mass
 删除节点质量
 > 参数:  
 > node_id:节点号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_nodal_mass(node_id=1)
 ```  
+Returns: 无
 ### add_pre_stress
 添加预应力
 > 参数:  
 > case_name:荷载工况名  
 > tendon_name:钢束名  
 > pre_type:预应力类型  
 > _0-始端 1-末端 2-两端_  
 > force:预应力  
 > group_name:边界组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_pre_stress(case_name="荷载工况名",tendon_name="钢束1",force=1390000)
 ```  
+Returns: 无
 ### remove_pre_stress
 删除预应力
 > 参数:  
 > case_name:荷载工况  
 > tendon_name:钢束组  
 > group_name:边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_pre_stress(case_name="工况1",tendon_name="钢束1",group_name="默认荷载组")
 ```  
+Returns: 无
 ##  荷载操作
 ### add_load_group
 根据荷载组名称添加荷载组
 > 参数:  
 > name: 荷载组名称  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_load_group(name="荷载组1")
 ```  
+Returns: 无
 ### remove_load_group
 根据荷载组名称或荷载组id删除荷载组,参数为默认时删除所有荷载组
 > 参数:  
 > name: 荷载组名称  
 > index: 荷载组编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_group(name="荷载组1")
 mdb.remove_load_group(index=1)
 ```  
+Returns: 无
 ### add_nodal_force
 添加节点荷载
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_nodal_force(case_name="荷载工况1",node_id=1,load_info=(1,1,1,1,1,1),group_name="默认结构组")
 ```  
+Returns: 无
 ### remove_nodal_force
 删除节点荷载
 > 参数:  
 > case_name:荷载工况名  
 > node_id:节点编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_nodal_force(case_name="荷载工况1",node_id=1)
 ```  
+Returns: 无
 ### add_node_displacement
 添加节点位移
 > 参数:  
 > node_id:节点编号  
 > case_name:荷载工况名  
 > load_info:节点位移列表 [Dx,Dy,Dz,Rx,Ry,Rz]  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_node_displacement(case_name="荷载工况1",node_id=1,load_info=(1,0,0,0,0,0),group_name="默认荷载组")
 ```  
+Returns: 无
 ### remove_nodal_displacement
 删除节点位移
 > 参数:  
 > node_id:节点编号  
 > case_name:荷载工况名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
 ```  
+Returns: 无
 ### add_beam_load
 添加梁单元荷载
 > 参数:  
 > beam_id:单元编号  
 > case_name:荷载工况名  
 > load_type:荷载类型  
 > _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩  
@@ -854,53 +981,57 @@
 > projected:是否投影  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0.4,0.8],list_load=[100,200])
 ```  
+Returns: 无
 ### remove_beam_load
 删除梁单元荷载
 > 参数:  
 > element_id:单元号  
 > case_name:荷载工况名  
 > load_type:荷载类型  
 > _1-集中力   2-集中弯矩  3-分布力   4-分布弯矩_  
 > group_name:边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_beam_load(case_name="工况1",element_id=1,load_type=1,group_name="默认荷载组")
 ```  
+Returns: 无
 ### add_initial_tension
 添加初始拉力
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > tension:初始拉力  
 > tension_type:张拉类型  1-全量   2-增量  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_initial_tension(element_id=1,case_name="工况1",tension=100,tension_type=1)
 ```  
+Returns: 无
 ### add_cable_length_load
 添加索长张拉
 > 参数:  
 > element_id:单元类型  
 > case_name:荷载工况名  
 > length:长度  
 > tension_type:张拉类型  1-全量   2-增量  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_cable_length_load(element_id=1,case_name="工况1",length=1,tension_type=1)
 ```  
+Returns: 无
 ### add_plate_element_load
 添加版单元荷载
 > 参数:  
 > element_id:单元id  
 > case_name:荷载工况名  
 > load_type:荷载类型  
 > _1-集中力  2-集中弯矩  3-分布力  4-分布弯矩_  
@@ -912,28 +1043,30 @@
 > load_list:荷载列表  
 > xy_list:荷载位置信息 [IJ方向绝对距离x,IL方向绝对距离y]  (仅集中荷载需要)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_plate_element_load(element_id=1,case_name="工况1",load_type=1,group_name="默认荷载组",load_list=[1000],xy_list=(0.2,0.5))
 ```  
+Returns: 无
 ### add_deviation_parameter
 添加制造误差
 > 参数:  
 > name:名称  
 > element_type:单元类型  1-梁单元  2-板单元  
 > parameters:参数列表  
 > _梁杆单元:[轴向,I端X向转角,I端Y向转角,I端Z向转角,J端X向转角,J端Y向转角,J端Z向转角]_  
 > _板单元:[X向位移,Y向位移,Z向位移,X向转角,Y向转角]_  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_deviation_parameter(name="梁端制造误差",element_type=1,parameters=[1,0,0,0,0,0,0])
 mdb.add_deviation_parameter(name="板端制造误差",element_type=1,parameters=[1,0,0,0,0])
 ```  
+Returns: 无
 ### add_deviation_load
 添加制造误差荷载
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > parameters:参数名列表  
 > _梁杆单元时-[制造误差参数名称]_  
@@ -941,34 +1074,37 @@
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_deviation_load(element_id=1,case_name="工况1",parameters=["梁端误差"])
 mdb.add_deviation_load(element_id=2,case_name="工况1",parameters=["板端误差1","板端误差2","板端误差3","板端误差4"])
 ```  
+Returns: 无
 ### add_element_temperature
 添加单元温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > temperature:最终温度  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_element_temperature(element_id=1,case_name="自重",temperature=1,group_name="默认荷载组")
 ```  
+Returns: 无
 ### add_gradient_temperature
 添加梯度温度
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_gradient_temperature(element_id=1,case_name="荷载工况1",group_name="荷载组名1",temperature=10)
 mdb.add_gradient_temperature(element_id=2,case_name="荷载工况2",group_name="荷载组名2",temperature=10,element_type=2)
 ```  
+Returns: 无
 ### add_beam_section_temperature
 添加梁截面温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > paving_thick:铺设厚度(m)  
 > temperature_type:温度类型  1-升温(默认) 2-降温  
@@ -978,136 +1114,150 @@
 > modify:是否修改规范温度  
 > temp_list:温度列表[T1,T2]  (仅修改时需要)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_section_temperature(element_id=1,case_name="工况1",paving_thick=0.1)
 ```  
+Returns: 无
 ### add_index_temperature
 添加指数温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > temperature:温差  
 > index:指数  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_index_temperature(element_id=1,case_name="工况1",temperature=20,index=2)
 ```  
+Returns: 无
 ### add_top_plate_temperature
 添加顶板温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载  
 > temperature:最终温度  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_top_plate_temperature(element_id=1,case_name="工况1",temperature=40,group_name="默认荷载组")
 ```  
+Returns: 无
 ##  沉降操作
 ### add_sink_group
 添加沉降组
 > 参数:  
 > name: 沉降组名  
 > sink: 沉降值  
 > node_ids: 节点编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_sink_group(name="沉降1",sink=0.1,node_ids=[1,2,3])
 ```  
+Returns: 无
 ### remove_sink_group
 按照名称删除沉降组
 > 参数:  
 > name:沉降组名,默认删除所有沉降组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_sink_group()
 mdb.remove_sink_group(name="沉降1")
 ```  
+Returns: 无
 ### add_sink_case
 添加沉降工况
 > 参数:  
 > name:荷载工况名  
 > sink_groups:沉降组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_sink_case(name="沉降工况1",sink_groups=["沉降1","沉降2"])
 ```  
+Returns: 无
 ### remove_sink_case
 按照名称删除沉降工况,不输入名称时默认删除所有沉降工况
 > 参数:  
 > name:沉降工况名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_sink_case()
 mdb.remove_sink_case(name="沉降1")
 ```  
+Returns: 无
 ### add_concurrent_reaction
 添加并发反力组
 > 参数:  
 > names: 结构组名称集合  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_concurrent_reaction(["默认结构组"])
 ```  
+Returns: 无
 ### remove_concurrent_reaction
 删除所有并发反力组
 > 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_concurrent_reaction()
 ```  
+Returns: 无
 ### add_concurrent_force
 创建并发内力组
 > 参数:  
 > names: 结构组名称集合  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_concurrent_force(["默认结构组"])
 ```  
+Returns: 无
 ### remove_concurrent_force
 删除所有并发内力组
+> 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_concurrent_force()
 ```  
+Returns: 无
 ### add_load_case
 添加荷载工况
 > 参数:  
 > name:沉降名  
 > case_type:荷载工况类型  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_load_case(name="工况1",case_type=1)
 ```  
+Returns: 无
 ### remove_load_case
 删除荷载工况,参数均为默认时删除全部荷载工况
 > 参数:  
 > index:荷载编号  
 > name:荷载名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_case(index=1)
 mdb.remove_load_case(name="工况1")
 mdb.remove_load_case()
 ```  
+Returns: 无
 ##  施工阶段
 ### add_construction_stage
 添加施工阶段信息
 > 参数:  
 > name:施工阶段信息  
 > duration:时长  
 > active_structures:激活结构组信息 [(结构组名,龄期,安装方法,计自重施工阶段id),...]  
@@ -1125,14 +1275,15 @@
 > index:施工阶段编号，默认自动添加  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
 ```  
+Returns: 无
 ### update_construction_stage
 添加施工阶段信息
 > 参数:  
 > name:施工阶段信息  
 > duration:时长  
 > active_structures:激活结构组信息 [(结构组名,龄期,安装方法,计自重施工阶段id),...]  
 > _计自重施工阶段id: 0-不计自重,1-本阶段 n-第n阶段)_  
@@ -1148,35 +1299,38 @@
 > temp_loads:临时荷载信息 [荷载组1，荷载组2,..]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.update_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
 ```  
+Returns: 无
 ### update_weight_stage
 添加施工阶段信息
 > 参数:  
 > stage_name:施工阶段信息  
 > structure_group_name:结构组名  
 > weight_stage_id: 计自重阶段号  
 > _0-不计自重,1-本阶段 n-第n阶段_  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.update_weight_stage(stage_name="施工阶段1",structure_group_name="默认结构组",weight_stage_id=1)
 ```  
+Returns: 无
 ### remove_construction_stage
 按照施工阶段名删除施工阶段,默认删除所有施工阶段
 > 参数:  
 > name:所删除施工阶段名称  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_construction_stage(name="施工阶段1")
 ```  
+Returns: 无
 ##  荷载组合
 ### add_load_combine
 添加荷载组合
 > 参数:  
 > name:荷载组合名  
 > combine_type:荷载组合类型 1-叠加  2-判别  3-包络  
 > describe:描述  
@@ -1184,82 +1338,181 @@
 > _"ST"-静力荷载工况  "CS"-施工阶段荷载工况  "CB"-荷载组合_  
 > _"MV"-移动荷载工况  "SM"-沉降荷载工况_  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_load_combine(name="荷载组合1",combine_type=1,describe="无",combine_info=[("CS","合计值",1),("CS","恒载",1)])
 ```  
+Returns: 无
 ### remove_load_combine
 删除荷载组合
 > 参数:  
 > name:指定删除荷载组合名，默认时则删除所有荷载组合  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_combine(name="荷载组合1")
-```
-## 结果提取
+```  
+Returns: 无
+
+##  静力结果查看
 ### get_element_stress
 获取单元应力,支持单个单元和单元列表
 > 参数:  
 > element_id: 单元编号  
-> stage_id: 施工极端号  
+> stage_id: 施工阶段号 -1-运营阶段  0-施工阶段包络 n-施工阶段号  
 > result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
 > increment_type: 1-全量    2-增量  
 > operation: 是否为运营阶段  
 > case_name: 运营阶段所需荷载工况名  
 ```Python
 # 示例代码
-from qtmodel import mdb
-mdb.get_element_stress(1,stage_id=1)
-mdb.get_element_stress([1,2,3],stage_id=1)
-mdb.get_element_stress(1,operation=True,case_name="工况名")
+from qtmodel import *
+odb.get_element_stress(1,stage_id=1)
+odb.get_element_stress([1,2,3],stage_id=1)
+odb.get_element_stress(1,operation=True,case_name="工况名")
 ```  
+Returns: list[ElementStress] or ElementStress
 ### get_element_force
 获取单元内力,支持单个单元和单元列表
 > 参数:  
 > element_id: 单元编号  
-> stage_id: 施工极端号  
+> stage_id: 施工阶段号 -1-运营阶段  0-施工阶段包络 n-施工阶段号  
 > result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
 > increment_type: 1-全量    2-增量  
-> operation: 是否为运营阶段  
 > case_name: 运营阶段所需荷载工况名  
 ```Python
 # 示例代码
-from qtmodel import mdb
-mdb.get_element_force(1,stage_id=1)
-mdb.get_element_force([1,2,3],stage_id=1)
-mdb.get_element_force(1,operation=True,case_name="工况名")
+from qtmodel import *
+odb.get_element_force(1,stage_id=1)
+odb.get_element_force([1,2,3],stage_id=1)
+odb.get_element_force(1,operation=True,case_name="工况名")
 ```  
+Returns: list[ElementForce] or ElementForce
 ### get_reaction
 获取节点,支持单个节点和节点列表
 > 参数:  
 > node_id: 节点编号  
-> stage_id: 施工极端号  
+> stage_id: 施工阶段号 -1-运营阶段  0-施工阶段包络 n-施工阶段号  
 > result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
 > increment_type: 1-全量    2-增量  
-> operation: 是否为运营阶段  
 > case_name: 运营阶段所需荷载工况名  
 ```Python
 # 示例代码
-from qtmodel import mdb
-mdb.get_reaction(1,stage_id=1)
-mdb.get_reaction([1,2,3],stage_id=1)
-mdb.get_reaction(1,operation=True,case_name="工况名")
+from qtmodel import *
+odb.get_reaction(1,stage_id=1)
+odb.get_reaction([1,2,3],stage_id=1)
+odb.get_reaction(1,operation=True,case_name="工况名")
 ```  
+Returns: list[SupportReaction] or SupportReaction
 ### get_node_displacement
 获取节点,支持单个节点和节点列表
 > 参数:  
 > node_id: 节点号  
-> stage_id: 施工极端号  
+> stage_id: 施工阶段号 -1-运营阶段  0-施工阶段包络 n-施工阶段号  
 > result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
 > increment_type: 1-全量    2-增量  
-> operation: 是否为运营阶段  
 > case_name: 运营阶段所需荷载工况名  
 ```Python
 # 示例代码
-from qtmodel import mdb
-mdb.get_node_displacement(1,stage_id=1)
-mdb.get_node_displacement([1,2,3],stage_id=1)
-mdb.get_node_displacement(1,operation=True,case_name="工况名")
+from qtmodel import *
+odb.get_node_displacement(1,stage_id=1)
+odb.get_node_displacement([1,2,3],stage_id=1)
+odb.get_node_displacement(1,stage_id=-1,case_name="工况名")
+```  
+Returns: list[NodeDisplacement] or NodeDisplacement
+##  绘制模型结果
+### plot_reaction_result
+保存结果图片到指定文件甲
+> 参数:  
+> file_path: 保存路径名  
+> component: 分量编号 0-Fx 1-Fy 2-Fz 3-Fxyz 4-Mx 5-My 6-Mz 7-Mxyz  
+> load_case_name: 详细荷载工况名，参考桥通结果输出，例如： CQ:成桥(合计)  
+> stage_id: -1-运营阶段  0-施工阶段包络 n-施工阶段号  
+> envelope_type: 施工阶段包络类型 1-最大 2-最小  
+> show_number: 数值选项卡开启  
+> show_legend: 图例选项卡开启  
+> text_rotation: 数值选项卡内文字旋转角度  
+> show_max_min: 数值选项卡内最大最小值显示 -1-不显示最大最小值  0-显示最大值和最小值  1-最大绝对值 2-最大值 3-最小值  
+> digital_count: 小数点位数  
+> show_exponential: 指数显示开启  
+> increment: 是否显示增量结果  
+```Python
+# 示例代码
+from qtmodel import *
+odb.plot_reaction_result(r"aaa.png",component=0,load_case_name="CQ:成桥(合计)",stage_id=-1)     # 获取所有节点信息
+```  
+Returns: 无
+##  获取模型信息
+### get_node_data
+获取节点信息 默认获取所有节点信息
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_node_data()     # 获取所有节点信息
+odb.get_node_data(1)    # 获取单个节点信息
+odb.get_node_data([1,2])    # 获取多个节点信息
+```  
+Returns: list[Node] 或 Node
+### get_element_data
+获取单元信息
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_element_data() # 获取所有单元结果
+odb.get_element_data(1) # 获取指定编号单元信息
 ```  
+Returns: list[Element]
+### get_element_type
+获取单元类型
+> 参数:  
+> ele_id: 单元号  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_element_type(1) # 获取所有单元信息
+```  
+Returns: str类型 返回 BEAM PLATE CABLE LINK
+### get_beam_element
+获取梁单元信息
+> 参数:  
+> ids: 梁单元号，默认时获取所有梁单元  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_beam_element() # 获取所有单元信息
+```  
+Returns: list[Element]
+### get_plate_element
+获取板单元信息
+> 参数:  
+> ids: 板单元号，默认时获取所有板单元  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_plate_element() # 获取所有单元信息
+```  
+Returns: list[Element]
+### get_cable_element
+获取索单元信息
+> 参数:  
+> ids: 索单元号，默认时获取所有索单元  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_cable_element() # 获取所有单元信息
+```  
+Returns: list[Element]
+### get_link_element
+获取杆单元信息
+> 参数:  
+> ids: 杆单元号，默认时输出全部杆单元  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_link_element() # 获取所有单元信息
+```  
+Returns: list[Element]
+
```

### Comparing `qtmodel-0.3.8/README.md` & `qtmodel-0.3.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,228 +1,335 @@
-# 最新版本 V0.3.8 - 2024.05.21 
+Metadata-Version: 2.1
+Name: qtmodel
+Version: 0.3.9
+Summary: python modeling for qt  24/05/06 
+Home-page: https://github.com/Inface0443/pyqt
+Author: dqy-zhj
+Author-email: 1105417715@qq.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
+# 最新版本 V0.3.9 - 2024.05.29 
 > pip install --upgrade qtmodel
 - 优化部分调用
 
 ##  项目管理
+### update_model
+刷新模型信息
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.update_model()
+```  
+Returns: 无
+### update_app_stage
+切换模型前后处理状态
+> 参数:  
+> num: 1-前处理  2-后处理  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.update_app_stage(1)
+mdb.update_app_stage(2)
+```  
+Returns: 无
+### do_solve
+运行分析
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.do_solve()
+```  
+Returns: 无
 ### initial
 初始化模型,新建模型
+> 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.initial()
 ```  
+Returns: 无
 ### open_file
 打开bfmd文件
+> 参数:  
+> file_path: 文件全路径  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.open_file("a.bfmd")
 ```  
-### save_file
-保存bfmd文件
+Returns: 无
+### close_project
+关闭项目
+> 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.save_file("a.bfmd")
+mdb.close_project()
 ```  
-### close_project
-关闭项目
+Returns: 无
+### save_file
+保存bfmd文件
+> 参数:  
+> file_path: 文件全路径  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.close_project()
+mdb.save_file("a.bfmd")
 ```  
+Returns: 无
 ### import_command
 导入命令
 > 参数:  
 > command:命令字符  
-> command_type:命令类型 1-桥通命令  
+> command_type:命令类型 1-桥通命令 目前仅支持桥通命令  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.import_command("*SECTION")
 ```  
+Returns: 无
+### import_file
+导入文件
+> 参数:  
+> file_path:导入文件(.mct/.qdat/.dxf/.3dx)  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.import_file("a.mct")
+```  
+Returns: 无
 ### export_file
 导入命令
 > 参数:  
-> file_path:导出文件(.mct/.qdat/.PGF/.3dx)  
+> file_path:导出文件全路径，支持格式(.mct/.qdat/.PGF/.3dx)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.export_file("a.mct")
 ```  
-### import_file
-导入命令
+Returns: 无
+##  节点单元操作
+### add_nodes
+添加多个节点，可以选择指定节点编号
 > 参数:  
-> file_path:导入文件(.mct/.qdat/.dxf/.3dx)  
+> node_list:节点坐标信息 [[x1,y1,z1],...]或 [[id1,x1,y1,z1]...]  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.import_file("a.mct")
+mdb.add_nodes([[1,2,3],[4,5,6]])
+mdb.add_nodes([[1,1,2,3],[2,4,5,6]])
 ```  
-### do_solve
-运行分析
+Returns: 无
+### add_node
+根据坐标信息和节点编号添加节点，默认自动识别编号
+> 参数:  
+> x: 节点坐标x  
+> y: 节点坐标y  
+> z: 节点坐标z  
+> index: 节点编号，默认自动识别编号 (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.do_solve()
+mdb.add_node(1,2,3)
+mdb.add_node(x= 1,y = 2,z = 4,index = 2)
 ```  
-##  节点单元操作
+Returns: 无
+### update_node_id
+根据坐标信息和节点编号添加节点，默认自动识别编号
+> 参数:  
+> node_id: 节点编号  
+> new_id: 新节点编号  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.update_node_id(1,2)
+```  
+Returns: 无
+### merge_nodes
+根据坐标信息和节点编号添加节点，默认自动识别编号
+> 参数:  
+> ids: 合并节点集合  默认全部节点  
+> tolerance: 合并容许误差  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.merge_nodes()
+```  
+Returns: 无
+### remove_node
+删除指定节点,不输入参数时默认删除所有节点
+> 参数:  
+> ids:节点编号  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.remove_node()
+mdb.remove_node(ids=1)
+mdb.remove_node(ids=[1,2,3])
+```  
+Returns: 无
+### renumber_node
+节点编号重拍
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.renumber_node()
+```  
+Returns: 无
+### move_node
+移动节点坐标
+> 参数:  
+> node_id：节点号  
+> offset_x:X轴偏移量  
+> offset_y:Y轴偏移量  
+> offset_z:Z轴偏移量  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.move_node(1,1.5,1.5,1.5)
+```  
+Returns: 无
 ### add_structure_group
 添加结构组
 > 参数:  
 > name: 结构组名  
 > index: 结构组编号(非必须参数)，默认自动识别当前编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_structure_group(name="新建结构组1")
 mdb.add_structure_group(name="新建结构组2",index=2)
 ```  
+Returns: 无
 ### remove_structure_group
 可根据结构与组名或结构组编号删除结构组，当组名和组编号均为默认则删除所有结构组
 > 参数:  
 > name:结构组名称  
 > index:结构组编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_structure_group(name="新建结构组1")
 mdb.remove_structure_group(index = 2)
 ```  
+Returns: 无
 ### add_structure_to_group
 为结构组添加节点和/或单元
 > 参数:  
 > name: 结构组名  
 > node_ids: 节点编号列表(可选参数)  
 > element_ids: 单元编号列表(可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
 ```  
+Returns: 无
 ### remove_structure_in_group
 为结构组删除节点和/或单元
 > 参数:  
 > name: 结构组名  
 > node_ids: 节点编号列表(可选参数)  
 > element_ids: 单元编号列表(可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
 ```  
-### add_node
-根据坐标信息和节点编号添加节点，默认自动识别编号
-> 参数:  
-> x: 节点坐标x  
-> y: 节点坐标y  
-> z: 节点坐标z  
-> index: 节点编号，默认自动识别编号 (可选参数)  
-```Python
-# 示例代码
-from qtmodel import mdb
-mdb.add_node(1,2,3)
-mdb.add_node(x= 1,y = 2,z = 4,index = 2)
-```  
-### add_nodes
-添加多个节点，可以选择指定节点编号
-> 参数:  
-> node_list:节点坐标信息 [[x1,y1,z1],...]或 [[id1,x1,y1,z1]...]  
-```Python
-# 示例代码
-from qtmodel import mdb
-mdb.add_nodes([[1,2,3],[4,5,6]])
-mdb.add_nodes([[1,1,2,3],[2,4,5,6]])
-```  
-### remove_node
-删除指定节点,不输入参数时默认删除所有节点
-> 参数:  
-> index:节点编号  
-```Python
-# 示例代码
-from qtmodel import mdb
-mdb.remove_node()
-mdb.remove_node(index=1)
-```  
+Returns: 无
 ### add_element
 根据单元编号和单元类型添加单元
 > 参数:  
 > index:单元编号  
 > ele_type:单元类型 1-梁 2-索 3-杆 4-板  
 > node_ids:单元对应的节点列表 [i,j] 或 [i,j,k,l]  
 > beta_angle:贝塔角  
 > mat_id:材料编号  
 > sec_id:截面编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_element(index=1,ele_type=1,node_ids=[1,2],beta_angle=1,mat_id=1,sec_id=1)
 ```  
+Returns: 无
 ### remove_element
 删除指定编号的单元
 > 参数:  
 > index: 单元编号,默认时删除所有单元  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_element()
 mdb.remove_element(index=1)
 ```  
+Returns: 无
 ##  材料操作
 ### add_material
 添加材料
 > 参数:  
 > index:材料编号,默认自动识别 (可选参数)  
 > name:材料名称  
-> material_type: 材料类型  
+> mat_type: 材料类型  
 > standard:规范名称  
 > database:数据库  
 > construct_factor:构造系数  
 > modified:是否修改默认材料参数,默认不修改 (可选参数)  
 > data_info:材料参数列表[弹性模量,容重,泊松比,热膨胀系数] (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.add_material(index=1,name="混凝土材料1",material_type="混凝土",standard="公路18规范",database="C50")
-mdb.add_material(index=1,name="自定义材料1",material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
+mdb.add_material(index=1,name="混凝土材料1",mat_type="混凝土",standard="公路18规范",database="C50")
+mdb.add_material(index=1,name="自定义材料1",mat_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
 ```  
+Returns: 无
 ### add_time_material
 添加收缩徐变材料
 > 参数:  
 > index: 指定收缩徐变编号,默认则自动识别 (可选参数)  
 > name: 收缩徐变名  
 > code_index: 收缩徐变规范索引  
 > time_parameter: 对应规范的收缩徐变参数列表,默认不改变规范中信息 (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_time_material(index=1,name="收缩徐变材料1",code_index=1)
 ```  
+Returns: 无
 ### update_material_creep
 将收缩徐变参数连接到材料
 > 参数:  
 > index: 材料编号  
 > creep_id: 收缩徐变编号  
 > f_cuk: 材料标准抗压强度,仅自定义材料是需要输入  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.update_material_creep(index=1,creep_id=1,f_cuk=5e7)
 ```  
+Returns: 无
 ### remove_material
 删除指定材料
 > 参数:  
 > index:指定材料编号，默认则删除所有材料  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_material()
 mdb.remove_material(index=1)
 ```  
+Returns: 无
 ##  截面操作
 ### add_parameter_section
 添加截面信息
 > 参数:  
 > index: 截面编号,默认自动识别  
 > name:截面名称  
 > sec_type:参数截面类型名称,支持以下类型  
@@ -248,14 +355,15 @@
 # 示例代码
 from qtmodel import mdb
 mdb.add_parameter_section(name="截面1",sec_type="矩形",sec_info=[2,4],bias_type="中心")
 mdb.add_parameter_section(name="截面2",sec_type="混凝土箱梁",box_height=2,box_number=3,
 sec_info=[0.02,0,12,3,1,2,1,5,6,0.2,0.4,0.1,0.13,0.28,0.3,0.5,0.5,0.5,0.2],
 charm_info=["1*0.2,0.1*0.2","0.5*0.15,0.3*0.2","0.4*0.2","0.5*0.2"])
 ```  
+Returns: 无
 ### add_steel_section
 添加钢梁截面,包括参数型钢梁截面和自定义带肋钢梁截面
 > 参数:  
 > index:  
 > name:  
 > sec_type:截面类型 1-工字钢梁  2-箱型钢梁  
 > sec_info:截面信息  
@@ -276,48 +384,55 @@
 from qtmodel import mdb
 mdb.add_steel_section(name="钢梁截面1",sec_type=1,sec_info=[0,0,0.5,0.5,0.5,0.5,0.7,0.02,0.02,0.02])
 mdb.add_steel_section(name="钢梁截面2",sec_type=2,sec_info=[0,0.15,0.25,0.5,0.25,0.15,0.4,0.15,0.7,0.02,0.02,0.02,0.02],
 rib_info = {"板肋1": [0.1,0.02],"T形肋1":[0.1,0.02,0.02,0.02]},
 rib_place = [(0, 0, 0, [(0.1, "板肋1", 2, "默认名称1"), (0.2, "板肋1", 2, "默认名称2")]), (0, 0, 1, [(0.1, "T形肋1", 0, "默认名称3")])],
 bias_type="中上")
 ```  
+Returns: 无
 ### add_user_section
 添加自定义截面,目前仅支持特性截面
 > 参数:  
 > index:截面编号  
 > name:截面名称  
 > sec_type:截面类型  
 > property_info:截面特性列表  
+> main_loop:主线圈坐标集合 [(-1,-1),(5,0),(5,5),(-1,5)] 目前只支持单一线圈  
+> sub_loops:次线圈坐标集合 [[(0,0),(0,1),(1,1,)], [(2,2),(3,2),(3,3)]]  
+> sec_lines:线宽集合[(x1,y1,x2,y3,thick),]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_user_section(name="自定义特性截面",property_info=[i for i in range(25)])
 ```  
+Returns: 无
 ### add_tapper_section
 添加变截面,需先建立单一截面
 > 参数:  
 > index:截面编号  
 > name:截面名称  
 > begin_id:截面始端编号  
 > end_id:截面末端编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_tapper_section(name="变截面1",begin_id=1,end_id=2)
 ```  
+Returns: 无
 ### remove_section
 删除截面信息
 > 参数:  
 > index: 截面编号,参数为默认时删除全部截面  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_section()
 mdb.remove_section(1)
 ```  
+Returns: 无
 ##  板厚操作
 ### add_thickness
 添加板厚
 > 参数:  
 > index: 板厚id  
 > name: 板厚名称  
 > t:   板厚度  
@@ -331,24 +446,26 @@
 > rib_l: 横向肋板信息  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_thickness(name="厚度1", t=0.2,thick_type=0,bias_info=(0,0.8))
 mdb.add_thickness(name="厚度2", t=0.2,thick_type=1,rib_pos=0,dist_v=0.1,rib_v=[1,1,0.02,0.02])
 ```  
+Returns: 无
 ### remove_thickness
 删除板厚
 > 参数:  
 > index:板厚编号,默认时删除所有板厚信息  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_thickness()
 mdb.remove_thickness(index=1)
 ```  
+Returns: 无
 ### add_tapper_section_group
 添加变截面组
 > 参数:  
 > ids:变截面组编号  
 > name: 变截面组名  
 > factor_w: 宽度方向变化阶数 线性(1.0) 非线性(!=1.0)  
 > factor_h: 高度方向变化阶数 线性(1.0) 非线性(!=1.0)  
@@ -357,106 +474,115 @@
 > dis_w: 宽度方向距离  
 > dis_h: 高度方向距离  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_tapper_section_group(ids=[1,2,3,4],name="变截面组1")
 ```  
+Returns: 无
 ### update_section_bias
 更新截面偏心
 > 参数:  
 > index:截面编号  
 > bias_type:偏心类型  
 > center_type:中心类型  
 > shear_consider:考虑剪切  
 > bias_point:自定义偏心点(仅自定义类型偏心需要)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.update_section_bias(index=1,bias_type="中上",center_type="几何中心")
 mdb.update_section_bias(index=1,bias_type="自定义",bias_point=[0.1,0.2])
 ```  
+Returns: 无
 ##  边界操作
 ### add_boundary_group
 新建边界组
 > 参数:  
 > name:边界组名  
 > index:边界组编号，默认自动识别当前编号 (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_boundary_group(name="边界组1")
 ```  
+Returns: 无
 ### remove_boundary_group
 按照名称删除边界组
 > 参数:  
 > name: 边界组名称，默认删除所有边界组 (非必须参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_boundary_group()
 mdb.remove_boundary_group(name="边界组1")
 ```  
+Returns: 无
 ### remove_all_boundary
 根据边界组名称、边界的类型和编号删除边界信息,默认时删除所有边界信息
 > 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_all_boundary()
 ```  
+Returns: 无
 ### remove_boundary
 根据节点号删除一般支撑、弹性支承/根据单元号删除梁端约束/根据主节点号删除主从约束/根据从节点号删除约束方程
 > 参数:  
 > remove_id:节点号 or 单元号 or主节点号  or 从节点号  
 > bd_type:边界类型  
 > _1-一般支承 2-弹性支承 3-主从约束 4-弹性连接 5-约束方程 6-梁端约束_  
 > group:边界所处边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_boundary(remove_id = 1, bd_type = 1,group="边界组1")
 ```  
+Returns: 无
 ### add_general_support
 添加一般支承
 > 参数:  
 > node_id:节点编号  
 > boundary_info:边界信息  [X,Y,Z,Rx,Ry,Rz]  
 > _ture-固定 false-自由_  
 > group_name:边界组名,默认为默认边界组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_general_support(node_id=1, boundary_info=[True,True,True,False,False,False])
 ```  
+Returns: 无
 ### add_elastic_support
 添加弹性支承
 > 参数:  
 > node_id:节点编号  
 > support_type:支承类型 1-线性  2-受拉  3-受压  
 > boundary_info:边界信息 受拉和受压时列表长度为1  线性时列表长度为6  
 > group_name:边界组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_elastic_support(node_id=1,support_type=1,boundary_info=[1e6,0,1e6,0,0,0])
 ```  
+Returns: 无
 ### add_master_slave_link
 添加主从约束
 > 参数:  
 > master_id:主节点号  
 > slave_id:从节点号  
 > boundary_info:边界信息 [X,Y,Z,Rx,Ry,Rz]  
 > _ture-固定 false-自由_  
 > group_name:边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_master_slave_link(master_id=1,slave_id=2,boundary_info=[True,True,True,False,False,False])
 ```  
+Returns: 无
 ### add_elastic_link
 添加弹性连接
 > 参数:  
 > link_type:节点类型  
 > _1-一般弹性连接 2-刚性连接 3-受拉弹性连接 4-受压弹性连接_  
 > start_id:起始节点号  
 > end_id:终节点号  
@@ -468,39 +594,42 @@
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_elastic_link(link_type=1,start_id=1,end_id=2,boundary_info=[1e6,1e6,1e6,0,0,0])
 mdb.add_elastic_link(link_type=2,start_id=1,end_id=2)
 mdb.add_elastic_link(link_type=3,start_id=1,end_id=2,kx=1e6)
 ```  
+Returns: 无
 ### add_beam_constraint
 添加梁端约束
 > 参数:  
 > beam_id:梁号  
 > info_i:i端约束信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > info_j:j端约束信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > group_name:边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_constraint(beam_id=2,info_i=[True,True,True,False,False,False],info_j=[True,True,True,False,False,False])
 ```  
+Returns: 无
 ### add_node_axis
 添加节点坐标
 > 参数:  
 > input_type:输入方式 1-角度 2-三点  3-向量  
 > node_id:节点号  
 > coord_info:局部坐标信息 -List<float>(角)  -List<List<float>>(三点 or 向量)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_node_axis(input_type=1,node_id=1,coord_info=[45,45,45])
 mdb.add_node_axis(input_type=2,node_id=1,coord_info=[[0,0,1],[0,1,0],[1,0,0]])
 mdb.add_node_axis(input_type=3,node_id=1,coord_info=[[0,0,1],[0,1,0]])
 ```  
+Returns: 无
 ##  移动荷载
 ### add_standard_vehicle
 添加标准车辆
 > 参数:  
 > name: 车辆荷载名称  
 > standard_code: 荷载规范  
 > _1-中国铁路桥涵规范(Q/CR 9300-2017)_  
@@ -519,48 +648,52 @@
 > load_length: 默认为0即不限制荷载长度  (铁路桥涵规范2017 所需参数)  
 > n:车厢数: 默认6节车厢 (城市轨道交通桥梁规范2017 所需参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_standard_vehicle("高速铁路",standard_code=1,load_type="高速铁路")
 ```  
+Returns: 无
 ### add_node_tandem
 添加节点纵列
 > 参数:  
 > name:节点纵列名  
 > start_id:起始节点号  
 > node_ids:节点列表  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_node_tandem("节点纵列1",1,[i+1 for i in range(12)])
 ```  
+Returns: 无
 ### add_influence_plane
 添加影响面
 > 参数:  
 > name:影响面名称  
 > tandem_names:节点纵列名称组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_influence_plane("影响面1",["节点纵列1","节点纵列2"])
 ```  
+Returns: 无
 ### add_lane_line
 添加车道线
 > 参数:  
 > name:车道线名称  
 > influence_name:影响面名称  
 > tandem_name:节点纵列名  
 > offset:偏移  
 > lane_width:车道宽度  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_lane_line("车道1","影响面1","节点纵列1",offset=0,lane_width=3.1)
 ```  
+Returns: 无
 ### add_live_load_case
 添加移动荷载工况
 > 参数:  
 > name:荷载工况名  
 > influence_plane:影响线名  
 > span:跨度  
 > car_detail: 汽车相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)  
@@ -568,89 +701,97 @@
 > metro_detail: 轻轨相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)  
 > sub_case:子工况信息 [(车辆名称,系数,["车道1","车道2"])...]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_live_load_case("活载工况1","影响面1",100,sub_case=[("车辆名称",1.0,["车道1","车道2"]),])
 ```  
+Returns: 无
 ### remove_vehicle
 删除车辆信息
 > 参数:  
 > index:车辆荷载编号  
 > name:车辆名称  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_vehicle(index=1)
 mdb.remove_vehicle(name="车辆名称")
 ```  
+Returns: 无
 ### remove_node_tandem
 按照 节点纵列编号/节点纵列名 删除节点纵列
 > 参数:  
 > index:节点纵列编号  
 > name:节点纵列名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_node_tandem(index=1)
 mdb.remove_node_tandem(name="节点纵列1")
 ```  
+Returns: 无
 ### remove_influence_plane
 按照 影响面编号/影响面名称 删除影响面
 > 参数:  
 > index:影响面编号  
 > name:影响面名称  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_influence_plane(index=1)
 mdb.remove_influence_plane(name="影响面1")
 ```  
+Returns: 无
 ### remove_lane_line
 按照 车道线编号/车道线名称 删除车道线
 > 参数:  
 > name:车道线名称  
 > index:车道线编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_lane_line(index=1)
 mdb.remove_lane_line(name="车道线1")
 ```  
+Returns: 无
 ### remove_live_load_case
 删除移动荷载工况
 > 参数:  
 > name:移动荷载工况名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_live_load_case(name="活载工况1")
 ```  
+Returns: 无
 ##  钢束操作
 ### add_tendon_group
 按照名称添加钢束组，添加时可指定钢束组id
 > 参数:  
 > name: 钢束组名称  
 > index: 钢束组编号(非必须参数)，默认自动识别  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_tendon_group(name="钢束组1")
 ```  
+Returns: 无
 ### remove_tendon_group
 按照钢束组名称或钢束组编号删除钢束组，两参数均为默认时删除所有钢束组
 > 参数:  
 > name:钢束组名称,默认自动识别 (可选参数)  
 > index:钢束组编号,默认自动识别 (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_tendon_group(name="钢束组1")
 mdb.remove_tendon_group(index=1)
 ```  
+Returns: 无
 ### add_tendon_property
 添加钢束特性
 > 参数:  
 > name:钢束特性名  
 > index:钢束编号,默认自动识别 (可选参数)  
 > tendon_type: 0-PRE 1-POST  
 > material_id: 钢材材料编号  
@@ -666,14 +807,15 @@
 > slip_info: 滑移信息[始端距离,末端距离] 默认为[0.006, 0.006]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_tendon_property(name="钢束1",tendon_type=0,material_id=1,duct_type=1,steel_type=1,
 steel_detail=[0.00014,0.10,0.25,0.0015],loos_detail=(1,1,1))
 ```  
+Returns: 无
 ### add_tendon_3d
 添加三维钢束
 > 参数:  
 > name:钢束名称  
 > property_name:钢束特性名称  
 > group_name:默认钢束组  
 > num:根数  
@@ -692,142 +834,155 @@
 # 示例代码
 from qtmodel import mdb
 mdb.add_tendon_3d("BB1",property_name="22-15",num=2,position_type=1,
 control_points=[(0,0,-1,0),(10,0,-1,0)],point_insert=(0,0,0))
 mdb.add_tendon_3d("BB1",property_name="22-15",num=2,position_type=2,
 control_points=[(0,0,-1,0),(10,0,-1,0)],point_insert=(1,1,1),track_group="轨迹线结构组1")
 ```  
+Returns: 无
 ### remove_tendon
 按照名称或编号删除钢束,默认时删除所有钢束
 > 参数:  
 > name:钢束名称  
 > index:钢束编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_tendon(name="钢束1")
 mdb.remove_tendon(index=1)
 mdb.remove_tendon()
 ```  
+Returns: 无
 ### remove_tendon_property
 按照名称或编号删除钢束组,默认时删除所有钢束组
 > 参数:  
 > name:钢束组名称  
 > index:钢束组编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_tendon_property(name="钢束特性1")
 mdb.remove_tendon_property(index=1)
 mdb.remove_tendon_property()
 ```  
+Returns: 无
 ### add_nodal_mass
 添加节点质量
 > 参数:  
 > node_id:节点编号  
 > mass_info:[m,rmX,rmY,rmZ]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_nodal_mass(node_id=1,mass_info=(100,0,0,0))
 ```  
+Returns: 无
 ### remove_nodal_mass
 删除节点质量
 > 参数:  
 > node_id:节点号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_nodal_mass(node_id=1)
 ```  
+Returns: 无
 ### add_pre_stress
 添加预应力
 > 参数:  
 > case_name:荷载工况名  
 > tendon_name:钢束名  
 > pre_type:预应力类型  
 > _0-始端 1-末端 2-两端_  
 > force:预应力  
 > group_name:边界组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_pre_stress(case_name="荷载工况名",tendon_name="钢束1",force=1390000)
 ```  
+Returns: 无
 ### remove_pre_stress
 删除预应力
 > 参数:  
 > case_name:荷载工况  
 > tendon_name:钢束组  
 > group_name:边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_pre_stress(case_name="工况1",tendon_name="钢束1",group_name="默认荷载组")
 ```  
+Returns: 无
 ##  荷载操作
 ### add_load_group
 根据荷载组名称添加荷载组
 > 参数:  
 > name: 荷载组名称  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_load_group(name="荷载组1")
 ```  
+Returns: 无
 ### remove_load_group
 根据荷载组名称或荷载组id删除荷载组,参数为默认时删除所有荷载组
 > 参数:  
 > name: 荷载组名称  
 > index: 荷载组编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_group(name="荷载组1")
 mdb.remove_load_group(index=1)
 ```  
+Returns: 无
 ### add_nodal_force
 添加节点荷载
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_nodal_force(case_name="荷载工况1",node_id=1,load_info=(1,1,1,1,1,1),group_name="默认结构组")
 ```  
+Returns: 无
 ### remove_nodal_force
 删除节点荷载
 > 参数:  
 > case_name:荷载工况名  
 > node_id:节点编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_nodal_force(case_name="荷载工况1",node_id=1)
 ```  
+Returns: 无
 ### add_node_displacement
 添加节点位移
 > 参数:  
 > node_id:节点编号  
 > case_name:荷载工况名  
 > load_info:节点位移列表 [Dx,Dy,Dz,Rx,Ry,Rz]  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_node_displacement(case_name="荷载工况1",node_id=1,load_info=(1,0,0,0,0,0),group_name="默认荷载组")
 ```  
+Returns: 无
 ### remove_nodal_displacement
 删除节点位移
 > 参数:  
 > node_id:节点编号  
 > case_name:荷载工况名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
 ```  
+Returns: 无
 ### add_beam_load
 添加梁单元荷载
 > 参数:  
 > beam_id:单元编号  
 > case_name:荷载工况名  
 > load_type:荷载类型  
 > _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩  
@@ -840,53 +995,57 @@
 > projected:是否投影  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0.4,0.8],list_load=[100,200])
 ```  
+Returns: 无
 ### remove_beam_load
 删除梁单元荷载
 > 参数:  
 > element_id:单元号  
 > case_name:荷载工况名  
 > load_type:荷载类型  
 > _1-集中力   2-集中弯矩  3-分布力   4-分布弯矩_  
 > group_name:边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_beam_load(case_name="工况1",element_id=1,load_type=1,group_name="默认荷载组")
 ```  
+Returns: 无
 ### add_initial_tension
 添加初始拉力
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > tension:初始拉力  
 > tension_type:张拉类型  1-全量   2-增量  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_initial_tension(element_id=1,case_name="工况1",tension=100,tension_type=1)
 ```  
+Returns: 无
 ### add_cable_length_load
 添加索长张拉
 > 参数:  
 > element_id:单元类型  
 > case_name:荷载工况名  
 > length:长度  
 > tension_type:张拉类型  1-全量   2-增量  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_cable_length_load(element_id=1,case_name="工况1",length=1,tension_type=1)
 ```  
+Returns: 无
 ### add_plate_element_load
 添加版单元荷载
 > 参数:  
 > element_id:单元id  
 > case_name:荷载工况名  
 > load_type:荷载类型  
 > _1-集中力  2-集中弯矩  3-分布力  4-分布弯矩_  
@@ -898,28 +1057,30 @@
 > load_list:荷载列表  
 > xy_list:荷载位置信息 [IJ方向绝对距离x,IL方向绝对距离y]  (仅集中荷载需要)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_plate_element_load(element_id=1,case_name="工况1",load_type=1,group_name="默认荷载组",load_list=[1000],xy_list=(0.2,0.5))
 ```  
+Returns: 无
 ### add_deviation_parameter
 添加制造误差
 > 参数:  
 > name:名称  
 > element_type:单元类型  1-梁单元  2-板单元  
 > parameters:参数列表  
 > _梁杆单元:[轴向,I端X向转角,I端Y向转角,I端Z向转角,J端X向转角,J端Y向转角,J端Z向转角]_  
 > _板单元:[X向位移,Y向位移,Z向位移,X向转角,Y向转角]_  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_deviation_parameter(name="梁端制造误差",element_type=1,parameters=[1,0,0,0,0,0,0])
 mdb.add_deviation_parameter(name="板端制造误差",element_type=1,parameters=[1,0,0,0,0])
 ```  
+Returns: 无
 ### add_deviation_load
 添加制造误差荷载
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > parameters:参数名列表  
 > _梁杆单元时-[制造误差参数名称]_  
@@ -927,34 +1088,37 @@
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_deviation_load(element_id=1,case_name="工况1",parameters=["梁端误差"])
 mdb.add_deviation_load(element_id=2,case_name="工况1",parameters=["板端误差1","板端误差2","板端误差3","板端误差4"])
 ```  
+Returns: 无
 ### add_element_temperature
 添加单元温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > temperature:最终温度  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_element_temperature(element_id=1,case_name="自重",temperature=1,group_name="默认荷载组")
 ```  
+Returns: 无
 ### add_gradient_temperature
 添加梯度温度
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_gradient_temperature(element_id=1,case_name="荷载工况1",group_name="荷载组名1",temperature=10)
 mdb.add_gradient_temperature(element_id=2,case_name="荷载工况2",group_name="荷载组名2",temperature=10,element_type=2)
 ```  
+Returns: 无
 ### add_beam_section_temperature
 添加梁截面温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > paving_thick:铺设厚度(m)  
 > temperature_type:温度类型  1-升温(默认) 2-降温  
@@ -964,136 +1128,150 @@
 > modify:是否修改规范温度  
 > temp_list:温度列表[T1,T2]  (仅修改时需要)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_section_temperature(element_id=1,case_name="工况1",paving_thick=0.1)
 ```  
+Returns: 无
 ### add_index_temperature
 添加指数温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > temperature:温差  
 > index:指数  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_index_temperature(element_id=1,case_name="工况1",temperature=20,index=2)
 ```  
+Returns: 无
 ### add_top_plate_temperature
 添加顶板温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载  
 > temperature:最终温度  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_top_plate_temperature(element_id=1,case_name="工况1",temperature=40,group_name="默认荷载组")
 ```  
+Returns: 无
 ##  沉降操作
 ### add_sink_group
 添加沉降组
 > 参数:  
 > name: 沉降组名  
 > sink: 沉降值  
 > node_ids: 节点编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_sink_group(name="沉降1",sink=0.1,node_ids=[1,2,3])
 ```  
+Returns: 无
 ### remove_sink_group
 按照名称删除沉降组
 > 参数:  
 > name:沉降组名,默认删除所有沉降组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_sink_group()
 mdb.remove_sink_group(name="沉降1")
 ```  
+Returns: 无
 ### add_sink_case
 添加沉降工况
 > 参数:  
 > name:荷载工况名  
 > sink_groups:沉降组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_sink_case(name="沉降工况1",sink_groups=["沉降1","沉降2"])
 ```  
+Returns: 无
 ### remove_sink_case
 按照名称删除沉降工况,不输入名称时默认删除所有沉降工况
 > 参数:  
 > name:沉降工况名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_sink_case()
 mdb.remove_sink_case(name="沉降1")
 ```  
+Returns: 无
 ### add_concurrent_reaction
 添加并发反力组
 > 参数:  
 > names: 结构组名称集合  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_concurrent_reaction(["默认结构组"])
 ```  
+Returns: 无
 ### remove_concurrent_reaction
 删除所有并发反力组
 > 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_concurrent_reaction()
 ```  
+Returns: 无
 ### add_concurrent_force
 创建并发内力组
 > 参数:  
 > names: 结构组名称集合  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_concurrent_force(["默认结构组"])
 ```  
+Returns: 无
 ### remove_concurrent_force
 删除所有并发内力组
+> 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_concurrent_force()
 ```  
+Returns: 无
 ### add_load_case
 添加荷载工况
 > 参数:  
 > name:沉降名  
 > case_type:荷载工况类型  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_load_case(name="工况1",case_type=1)
 ```  
+Returns: 无
 ### remove_load_case
 删除荷载工况,参数均为默认时删除全部荷载工况
 > 参数:  
 > index:荷载编号  
 > name:荷载名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_case(index=1)
 mdb.remove_load_case(name="工况1")
 mdb.remove_load_case()
 ```  
+Returns: 无
 ##  施工阶段
 ### add_construction_stage
 添加施工阶段信息
 > 参数:  
 > name:施工阶段信息  
 > duration:时长  
 > active_structures:激活结构组信息 [(结构组名,龄期,安装方法,计自重施工阶段id),...]  
@@ -1111,14 +1289,15 @@
 > index:施工阶段编号，默认自动添加  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
 ```  
+Returns: 无
 ### update_construction_stage
 添加施工阶段信息
 > 参数:  
 > name:施工阶段信息  
 > duration:时长  
 > active_structures:激活结构组信息 [(结构组名,龄期,安装方法,计自重施工阶段id),...]  
 > _计自重施工阶段id: 0-不计自重,1-本阶段 n-第n阶段)_  
@@ -1134,35 +1313,38 @@
 > temp_loads:临时荷载信息 [荷载组1，荷载组2,..]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.update_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
 ```  
+Returns: 无
 ### update_weight_stage
 添加施工阶段信息
 > 参数:  
 > stage_name:施工阶段信息  
 > structure_group_name:结构组名  
 > weight_stage_id: 计自重阶段号  
 > _0-不计自重,1-本阶段 n-第n阶段_  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.update_weight_stage(stage_name="施工阶段1",structure_group_name="默认结构组",weight_stage_id=1)
 ```  
+Returns: 无
 ### remove_construction_stage
 按照施工阶段名删除施工阶段,默认删除所有施工阶段
 > 参数:  
 > name:所删除施工阶段名称  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_construction_stage(name="施工阶段1")
 ```  
+Returns: 无
 ##  荷载组合
 ### add_load_combine
 添加荷载组合
 > 参数:  
 > name:荷载组合名  
 > combine_type:荷载组合类型 1-叠加  2-判别  3-包络  
 > describe:描述  
@@ -1170,81 +1352,183 @@
 > _"ST"-静力荷载工况  "CS"-施工阶段荷载工况  "CB"-荷载组合_  
 > _"MV"-移动荷载工况  "SM"-沉降荷载工况_  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_load_combine(name="荷载组合1",combine_type=1,describe="无",combine_info=[("CS","合计值",1),("CS","恒载",1)])
 ```  
+Returns: 无
 ### remove_load_combine
 删除荷载组合
 > 参数:  
 > name:指定删除荷载组合名，默认时则删除所有荷载组合  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_combine(name="荷载组合1")
-```
-## 结果提取
+```  
+Returns: 无
+
+##  静力结果查看
 ### get_element_stress
 获取单元应力,支持单个单元和单元列表
 > 参数:  
 > element_id: 单元编号  
-> stage_id: 施工极端号  
+> stage_id: 施工阶段号 -1-运营阶段  0-施工阶段包络 n-施工阶段号  
 > result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
 > increment_type: 1-全量    2-增量  
 > operation: 是否为运营阶段  
 > case_name: 运营阶段所需荷载工况名  
 ```Python
 # 示例代码
-from qtmodel import mdb
-mdb.get_element_stress(1,stage_id=1)
-mdb.get_element_stress([1,2,3],stage_id=1)
-mdb.get_element_stress(1,operation=True,case_name="工况名")
+from qtmodel import *
+odb.get_element_stress(1,stage_id=1)
+odb.get_element_stress([1,2,3],stage_id=1)
+odb.get_element_stress(1,operation=True,case_name="工况名")
 ```  
+Returns: list[ElementStress] or ElementStress
 ### get_element_force
 获取单元内力,支持单个单元和单元列表
 > 参数:  
 > element_id: 单元编号  
-> stage_id: 施工极端号  
+> stage_id: 施工阶段号 -1-运营阶段  0-施工阶段包络 n-施工阶段号  
 > result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
 > increment_type: 1-全量    2-增量  
-> operation: 是否为运营阶段  
 > case_name: 运营阶段所需荷载工况名  
 ```Python
 # 示例代码
-from qtmodel import mdb
-mdb.get_element_force(1,stage_id=1)
-mdb.get_element_force([1,2,3],stage_id=1)
-mdb.get_element_force(1,operation=True,case_name="工况名")
+from qtmodel import *
+odb.get_element_force(1,stage_id=1)
+odb.get_element_force([1,2,3],stage_id=1)
+odb.get_element_force(1,operation=True,case_name="工况名")
 ```  
+Returns: list[ElementForce] or ElementForce
 ### get_reaction
 获取节点,支持单个节点和节点列表
 > 参数:  
 > node_id: 节点编号  
-> stage_id: 施工极端号  
+> stage_id: 施工阶段号 -1-运营阶段  0-施工阶段包络 n-施工阶段号  
 > result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
 > increment_type: 1-全量    2-增量  
-> operation: 是否为运营阶段  
 > case_name: 运营阶段所需荷载工况名  
 ```Python
 # 示例代码
-from qtmodel import mdb
-mdb.get_reaction(1,stage_id=1)
-mdb.get_reaction([1,2,3],stage_id=1)
-mdb.get_reaction(1,operation=True,case_name="工况名")
+from qtmodel import *
+odb.get_reaction(1,stage_id=1)
+odb.get_reaction([1,2,3],stage_id=1)
+odb.get_reaction(1,operation=True,case_name="工况名")
 ```  
+Returns: list[SupportReaction] or SupportReaction
 ### get_node_displacement
 获取节点,支持单个节点和节点列表
 > 参数:  
 > node_id: 节点号  
-> stage_id: 施工极端号  
+> stage_id: 施工阶段号 -1-运营阶段  0-施工阶段包络 n-施工阶段号  
 > result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
 > increment_type: 1-全量    2-增量  
-> operation: 是否为运营阶段  
 > case_name: 运营阶段所需荷载工况名  
 ```Python
 # 示例代码
-from qtmodel import mdb
-mdb.get_node_displacement(1,stage_id=1)
-mdb.get_node_displacement([1,2,3],stage_id=1)
-mdb.get_node_displacement(1,operation=True,case_name="工况名")
-```  
+from qtmodel import *
+odb.get_node_displacement(1,stage_id=1)
+odb.get_node_displacement([1,2,3],stage_id=1)
+odb.get_node_displacement(1,stage_id=-1,case_name="工况名")
+```  
+Returns: list[NodeDisplacement] or NodeDisplacement
+##  绘制模型结果
+### plot_reaction_result
+保存结果图片到指定文件甲
+> 参数:  
+> file_path: 保存路径名  
+> component: 分量编号 0-Fx 1-Fy 2-Fz 3-Fxyz 4-Mx 5-My 6-Mz 7-Mxyz  
+> load_case_name: 详细荷载工况名，参考桥通结果输出，例如： CQ:成桥(合计)  
+> stage_id: -1-运营阶段  0-施工阶段包络 n-施工阶段号  
+> envelope_type: 施工阶段包络类型 1-最大 2-最小  
+> show_number: 数值选项卡开启  
+> show_legend: 图例选项卡开启  
+> text_rotation: 数值选项卡内文字旋转角度  
+> show_max_min: 数值选项卡内最大最小值显示 -1-不显示最大最小值  0-显示最大值和最小值  1-最大绝对值 2-最大值 3-最小值  
+> digital_count: 小数点位数  
+> show_exponential: 指数显示开启  
+> increment: 是否显示增量结果  
+```Python
+# 示例代码
+from qtmodel import *
+odb.plot_reaction_result(r"aaa.png",component=0,load_case_name="CQ:成桥(合计)",stage_id=-1)     # 获取所有节点信息
+```  
+Returns: 无
+##  获取模型信息
+### get_node_data
+获取节点信息 默认获取所有节点信息
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_node_data()     # 获取所有节点信息
+odb.get_node_data(1)    # 获取单个节点信息
+odb.get_node_data([1,2])    # 获取多个节点信息
+```  
+Returns: list[Node] 或 Node
+### get_element_data
+获取单元信息
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_element_data() # 获取所有单元结果
+odb.get_element_data(1) # 获取指定编号单元信息
+```  
+Returns: list[Element]
+### get_element_type
+获取单元类型
+> 参数:  
+> ele_id: 单元号  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_element_type(1) # 获取所有单元信息
+```  
+Returns: str类型 返回 BEAM PLATE CABLE LINK
+### get_beam_element
+获取梁单元信息
+> 参数:  
+> ids: 梁单元号，默认时获取所有梁单元  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_beam_element() # 获取所有单元信息
+```  
+Returns: list[Element]
+### get_plate_element
+获取板单元信息
+> 参数:  
+> ids: 板单元号，默认时获取所有板单元  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_plate_element() # 获取所有单元信息
+```  
+Returns: list[Element]
+### get_cable_element
+获取索单元信息
+> 参数:  
+> ids: 索单元号，默认时获取所有索单元  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_cable_element() # 获取所有单元信息
+```  
+Returns: list[Element]
+### get_link_element
+获取杆单元信息
+> 参数:  
+> ids: 杆单元号，默认时输出全部杆单元  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_link_element() # 获取所有单元信息
+```  
+Returns: list[Element]
+
+
+
+
```

### Comparing `qtmodel-0.3.8/qtmodel/qt_helper.py` & `qtmodel-0.3.9/qtmodel/qt_helper.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.3.8/qtmodel/qt_mdb.py` & `qtmodel-0.3.9/qtmodel/qt_mdb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,116 +1,254 @@
-from .res_db import *
-from .qt_db import *
 from __main__ import qt_model
 
 
 class Mdb:
+    """
+    建模与模型修改计算，所有函数均无返回值
+    """
+
     # region 项目管理
     @staticmethod
+    def update_model():
+        """
+        刷新模型信息
+        Args: 无
+        example:
+            mdb.update_model()
+        Returns: 无
+        """
+        qt_model.UpdateModel()
+
+    @staticmethod
+    def update_app_stage(num: int = 1):
+        """
+        切换模型前后处理状态
+        Args:
+            num: 1-前处理  2-后处理
+        example:
+            mdb.update_app_stage(1)
+            mdb.update_app_stage(2)
+        Returns: 无
+        """
+
+    @staticmethod
+    def do_solve():
+        """
+        运行分析
+        Args: 无
+        example:
+            mdb.do_solve()
+        Returns: 无
+        """
+        qt_model.DoSolve()
+
+    @staticmethod
     def initial():
         """
         初始化模型,新建模型
+        Args: 无
         example:
-                mdb.initial()
+            mdb.initial()
         Returns: 无
         """
         qt_model.Initial()
 
     @staticmethod
     def open_file(file_path: str):
         """
-            打开bfmd文件
-            example:
-                    mdb.open_file("a.bfmd")
-            Returns: 无
+        打开bfmd文件
+        Args:
+            file_path: 文件全路径
+        example:
+            mdb.open_file("a.bfmd")
+        Returns: 无
         """
         if not file_path.endswith(".bfmd"):
             raise Exception("操作错误，仅支持bfmd文件")
         qt_model.OpenFile(file_path)
 
     @staticmethod
-    def save_file(file_path: str):
+    def close_project():
         """
-            保存bfmd文件
-            example:
-                    mdb.save_file("a.bfmd")
-            Returns: 无
+        关闭项目
+        Args: 无
+        example:
+            mdb.close_project()
+        Returns: 无
         """
-        qt_model.SaveFile(file_path)
+        qt_model.CloseFile()
 
     @staticmethod
-    def close_project():
+    def save_file(file_path: str):
         """
-            关闭项目
-            example:
-                mdb.close_project()
-            Returns: 无
+        保存bfmd文件
+        Args:
+            file_path: 文件全路径
+        example:
+            mdb.save_file("a.bfmd")
+        Returns: 无
         """
-        qt_model.CloseFile()
+        qt_model.SaveFile(file_path)
 
     @staticmethod
     def import_command(command: str, command_type: int = 1):
         """
-            导入命令
-            Args:
-                command:命令字符
-                command_type:命令类型 1-桥通命令
-            example:
-                mdb.import_command("*SECTION")
-            Returns: 无
+        导入命令
+        Args:
+            command:命令字符
+            command_type:命令类型 1-桥通命令 目前仅支持桥通命令
+        example:
+            mdb.import_command("*SECTION")
+        Returns: 无
         """
         qt_model.ImportQtCommand(command)
 
     @staticmethod
+    def import_file(file_path: str):
+        """
+        导入文件
+        Args:
+            file_path:导入文件(.mct/.qdat/.dxf/.3dx)
+        example:
+            mdb.import_file("a.mct")
+        Returns: 无
+        """
+        qt_model.ImportFile(file_path)
+
+    @staticmethod
     def export_file(file_path: str):
         """
-            导入命令
-            Args:
-                file_path:导出文件(.mct/.qdat/.PGF/.3dx)
-            example:
-                mdb.export_file("a.mct")
-            Returns: 无
+        导入命令
+        Args:
+            file_path:导出文件全路径，支持格式(.mct/.qdat/.PGF/.3dx)
+        example:
+            mdb.export_file("a.mct")
+        Returns: 无
         """
         qt_model.ExportFile(file_path)
 
+    # endregion
+
+    # region 节点单元操作
     @staticmethod
-    def import_file(file_path: str):
+    def add_nodes(node_list):
         """
-            导入命令
-            Args:
-                file_path:导入文件(.mct/.qdat/.dxf/.3dx)
-            example:
-                mdb.import_file("a.mct")
-            Returns: 无
+        添加多个节点，可以选择指定节点编号
+        Args:
+             node_list:节点坐标信息 [[x1,y1,z1],...]或 [[id1,x1,y1,z1]...]
+        example:
+            mdb.add_nodes([[1,2,3],[4,5,6]])
+            mdb.add_nodes([[1,1,2,3],[2,4,5,6]])
+        Returns: 无
         """
-        qt_model.ImportFile(file_path)
+        qt_model.AddNodes(dataList=node_list)
 
     @staticmethod
-    def do_solve():
+    def add_node(x: float = 1, y: float = 1, z: float = 1, index: int = -1):
         """
-            运行分析
-            example:
-                    mdb.do_solve()
-            Returns: 无
+        根据坐标信息和节点编号添加节点，默认自动识别编号
+        Args:
+             x: 节点坐标x
+             y: 节点坐标y
+             z: 节点坐标z
+             index: 节点编号，默认自动识别编号 (可选参数)
+        example:
+            mdb.add_node(1,2,3)
+            mdb.add_node(x= 1,y = 2,z = 4,index = 2)
+        Returns: 无
         """
-        qt_model.DoSolve()
+        if index != -1:
+            qt_model.AddNode(id=index, x=x, y=y, z=z)
+        else:
+            qt_model.AddNode(x=x, y=y, z=z)
 
-    # endregion
+    @staticmethod
+    def update_node_id(node_id: int, new_id: int):
+        """
+        根据坐标信息和节点编号添加节点，默认自动识别编号
+        Args:
+             node_id: 节点编号
+             new_id: 新节点编号
+        example:
+            mdb.update_node_id(1,2)
+        Returns: 无
+        """
+        qt_model.UpdateNodeId(nodeId=node_id, newId=new_id)
+
+    @staticmethod
+    def merge_nodes(ids: list[int] = None, tolerance: float = 1e-4):
+        """
+        根据坐标信息和节点编号添加节点，默认自动识别编号
+        Args:
+             ids: 合并节点集合  默认全部节点
+             tolerance: 合并容许误差
+        example:
+            mdb.merge_nodes()
+        Returns: 无
+        """
+        if ids is None:
+            qt_model.MergeNode(tolerance)
+        else:
+            qt_model.MergeNodeByIds(ids, tolerance)
+
+    @staticmethod
+    def remove_node(ids=None):
+        """
+        删除指定节点,不输入参数时默认删除所有节点
+        Args:
+            ids:节点编号
+        example:
+            mdb.remove_node()
+            mdb.remove_node(ids=1)
+            mdb.remove_node(ids=[1,2,3])
+        Returns: 无
+        """
+        if ids is None:
+            qt_model.RemoveAllNodes()
+        elif type(ids) == int:
+            qt_model.RemoveNode(id=ids)
+        else:
+            qt_model.RemoveNodes(ids=ids)
+
+    @staticmethod
+    def renumber_node():
+        """
+        节点编号重拍
+        Args: 无
+        example:
+            mdb.renumber_node()
+        Returns: 无
+        """
+        qt_model.RenumberNodeId()
+
+    @staticmethod
+    def move_node(node_id: int, offset_x: float = 0, offset_y: float = 0, offset_z: float = 0):
+        """
+        移动节点坐标
+        Args:
+            node_id：节点号
+            offset_x:X轴偏移量
+            offset_y:Y轴偏移量
+            offset_z:Z轴偏移量
+        example:
+            mdb.move_node(1,1.5,1.5,1.5)
+        Returns: 无
+        """
+        qt_model.MoveNode(node_id, offsets=[offset_x, offset_y, offset_z])
 
-    # region 节点单元操作
     @staticmethod
     def add_structure_group(name: str = "", index: int = -1):
         """
         添加结构组
         Args:
             name: 结构组名
             index: 结构组编号(非必须参数)，默认自动识别当前编号
         example:
-                mdb.add_structure_group(name="新建结构组1")
-                mdb.add_structure_group(name="新建结构组2",index=2)
+            mdb.add_structure_group(name="新建结构组1")
+            mdb.add_structure_group(name="新建结构组2",index=2)
         Returns: 无
         """
         qt_model.AddStructureGroup(name=name, id=index)
 
     @staticmethod
     def remove_structure_group(name: str = "", index: int = -1):
         """
@@ -163,64 +301,14 @@
         if node_ids is None:
             node_ids = []
         if element_ids is None:
             element_ids = []
         qt_model.RemoveStructureOnGroup(name=name, nodeIds=node_ids, elementIds=element_ids)
 
     @staticmethod
-    def add_node(x: float = 1, y: float = 1, z: float = 1, index: int = -1):
-        """
-        根据坐标信息和节点编号添加节点，默认自动识别编号
-        Args:
-             x: 节点坐标x
-             y: 节点坐标y
-             z: 节点坐标z
-             index: 节点编号，默认自动识别编号 (可选参数)
-        example:
-            mdb.add_node(1,2,3)
-            mdb.add_node(x= 1,y = 2,z = 4,index = 2)
-        Returns:无
-        """
-        if index != -1:
-            qt_model.AddNode(id=index, x=x, y=y, z=z)
-        else:
-            qt_model.AddNode(x=x, y=y, z=z)
-
-    @staticmethod
-    def add_nodes(node_list):
-        """
-        添加多个节点，可以选择指定节点编号
-        Args:
-             node_list:节点坐标信息 [[x1,y1,z1],...]或 [[id1,x1,y1,z1]...]
-        example:
-            mdb.add_nodes([[1,2,3],[4,5,6]])
-            mdb.add_nodes([[1,1,2,3],[2,4,5,6]])
-        Returns: 无
-        """
-        qt_model.AddNodes(dataList=node_list)
-
-    @staticmethod
-    def remove_node(index: int = None):
-        """
-        删除指定节点,不输入参数时默认删除所有节点
-        Args:
-            index:节点编号
-        example:
-            mdb.remove_node()
-            mdb.remove_node(index=1)
-        Returns: 无
-        """
-        if index is None:
-            qt_model.RemoveAllNodes()
-        elif type(index) == int:
-            qt_model.RemoveNode(id=index)
-        else:
-            qt_model.RemoveNodes(ids=index)
-
-    @staticmethod
     def add_element(index: int = 1, ele_type: int = 1, node_ids: list[int] = None, beta_angle: float = 0, mat_id: int = -1, sec_id: int = -1):
         """
         根据单元编号和单元类型添加单元
         Args:
             index:单元编号
             ele_type:单元类型 1-梁 2-索 3-杆 4-板
             node_ids:单元对应的节点列表 [i,j] 或 [i,j,k,l]
@@ -262,44 +350,44 @@
         else:
             qt_model.RemoveElement(index=index)
 
     # endregion
 
     # region 材料操作
     @staticmethod
-    def add_material(index: int = -1, name: str = "", material_type: str = "混凝土", standard: str = "公路18规范", database: str = "C50",
+    def add_material(index: int = -1, name: str = "", mat_type: str = "混凝土", standard: str = "公路18规范", database: str = "C50",
                      construct_factor: float = 1, modified: bool = False, data_info: list[float] = None):
         """
         添加材料
         Args:
             index:材料编号,默认自动识别 (可选参数)
             name:材料名称
-            material_type: 材料类型
+            mat_type: 材料类型
             standard:规范名称
             database:数据库
             construct_factor:构造系数
             modified:是否修改默认材料参数,默认不修改 (可选参数)
             data_info:材料参数列表[弹性模量,容重,泊松比,热膨胀系数] (可选参数)
         example:
-            mdb.add_material(index=1,name="混凝土材料1",material_type="混凝土",standard="公路18规范",database="C50")
-            mdb.add_material(index=1,name="自定义材料1",material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
+            mdb.add_material(index=1,name="混凝土材料1",mat_type="混凝土",standard="公路18规范",database="C50")
+            mdb.add_material(index=1,name="自定义材料1",mat_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
         Returns: 无
         """
         list_material = ["混凝土", "钢材", "预应力", "钢丝", "钢筋", "自定义"]
-        if material_type not in list_material:
+        if mat_type not in list_material:
             raise Exception(f"操作错误,material_type不在指定列表:{list_material}中")
-        if material_type == "自定义":
+        if mat_type == "自定义":
             modified = True
         if modified and len(data_info) != 4:
             raise Exception("操作错误,modify_info数据无效!")
         if not modified:
-            qt_model.AddMaterial(id=index, name=name, materialType=material_type, standardName=standard,
+            qt_model.AddMaterial(id=index, name=name, materialType=mat_type, standardName=standard,
                                  database=database, constructFactor=construct_factor, isModified=modified)
         else:
-            qt_model.AddMaterial(id=index, name=name, materialType=material_type, standardName=standard,
+            qt_model.AddMaterial(id=index, name=name, materialType=mat_type, standardName=standard,
                                  database=database, constructFactor=construct_factor, isModified=modified,
                                  elasticModulus=data_info[0], unitWeight=data_info[1],
                                  posiRatio=data_info[2], temperatureCoefficient=data_info[3])
 
     @staticmethod
     def add_time_material(index: int = -1, name: str = "", code_index: int = 1, time_parameter: list[float] = None):
         """
@@ -307,15 +395,15 @@
         Args:
             index: 指定收缩徐变编号,默认则自动识别 (可选参数)
             name: 收缩徐变名
             code_index: 收缩徐变规范索引
             time_parameter: 对应规范的收缩徐变参数列表,默认不改变规范中信息 (可选参数)
         example:
             mdb.add_time_material(index=1,name="收缩徐变材料1",code_index=1)
-        Returns:无
+        Returns: 无
         """
         if time_parameter is None:  # 默认不修改收缩徐变相关参数
             qt_model.AddTimeParameter(id=index, name=name, codeId=code_index)
         elif code_index == 1:  # 公规 JTG 3362-2018
             if len(time_parameter) != 4:
                 raise Exception("操作错误,time_parameter数据无效!")
             qt_model.AddTimeParameter(id=index, name=name, codeId=code_index, rh=time_parameter[0], bsc=time_parameter[1],
@@ -476,15 +564,14 @@
             mdb.add_steel_section(name="钢梁截面1",sec_type=1,sec_info=[0,0,0.5,0.5,0.5,0.5,0.7,0.02,0.02,0.02])
             mdb.add_steel_section(name="钢梁截面2",sec_type=2,sec_info=[0,0.15,0.25,0.5,0.25,0.15,0.4,0.15,0.7,0.02,0.02,0.02,0.02],
                 rib_info = {"板肋1": [0.1,0.02],"T形肋1":[0.1,0.02,0.02,0.02]},
                 rib_place = [(0, 0, 0, [(0.1, "板肋1", 2, "默认名称1"), (0.2, "板肋1", 2, "默认名称2")]), (0, 0, 1, [(0.1, "T形肋1", 0, "默认名称3")])],
                 bias_type="中上")
         Returns: 无
         """
-
         if sec_info is None:
             raise Exception("操作错误,请输入此截面的截面信息，参数列表可参考截面定义窗口")
         section_type = "工字钢梁" if sec_type == 1 else "箱型钢梁"
         rib_names = list(rib_info.keys())
         rib_data = list(rib_info.values())
         qt_model.AddSteelSection(id=index, name=name, sectionType=section_type, sectionInfoList=sec_info,
                                  ribNameList=rib_names, ribInfoList=rib_data,
@@ -996,18 +1083,14 @@
              name:移动荷载工况名
         example:
             mdb.remove_live_load_case(name="活载工况1")
         Returns: 无
         """
         qt_model.RemoveLiveLoadCase(name=name)
 
-    @staticmethod
-    def update_model():
-        qt_model.UpdateModel()
-
     # endregion
 
     # region 钢束操作
     @staticmethod
     def add_tendon_group(name: str = "", index: int = -1):
         """
         按照名称添加钢束组，添加时可指定钢束组id
@@ -1650,14 +1733,15 @@
         """
         qt_model.AddConcurrentForce(names=names)
 
     @staticmethod
     def remove_concurrent_force():
         """
         删除所有并发内力组
+        Args: 无
         example:
             mdb.remove_concurrent_force()
         Returns: 无
         """
         qt_model.RemoveConcurrentForce()
 
     @staticmethod
@@ -1671,15 +1755,15 @@
             mdb.add_load_case(name="工况1",case_type=1)
         Returns: 无
         """
         case_type_list = ["施工阶段荷载", "恒载", "活载", "制动力", "风荷载",
                           "体系温度荷载", "梯度温度荷载", "长轨伸缩挠曲力荷载", "脱轨荷载", "船舶撞击荷载",
                           "汽车撞击荷载", "长轨断轨力荷载", "用户定义荷载"]
         if case_type < 1 or case_type > 13:
-            raise
+            raise TypeError("输入类型错误，荷载工况类型有误，仅支持int类型")
         qt_model.AddLoadCase(name=name, loadCaseType=case_type_list[case_type - 1])
 
     @staticmethod
     def remove_load_case(index: int = -1, name: str = ""):
         """
         删除荷载工况,参数均为默认时删除全部荷载工况
         Args:
@@ -1835,201 +1919,7 @@
         """
         if name != "":
             qt_model.DeleteLoadCombine(name=name)
         else:
             qt_model.DeleteAllLoadCombine()
 
     # endregion
-
-    # region 静力结果查看
-    @staticmethod
-    def get_element_stress(element_id, stage_id: int = 1, result_kind: int = 1, increment_type: int = 1, operation: bool = False, case_name=""):
-        """
-        获取单元应力,支持单个单元和单元列表
-        Args:
-            element_id: 单元编号
-            stage_id: 施工极端号
-            result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
-            increment_type: 1-全量    2-增量
-            operation: 是否为运营阶段
-            case_name: 运营阶段所需荷载工况名
-        example:
-            mdb.get_element_stress(1,stage_id=1)
-            mdb.get_element_stress([1,2,3],stage_id=1)
-            mdb.get_element_stress(1,operation=True,case_name="工况名")
-        Returns:
-            list[ElementStress] or ElementStress
-        """
-        if type(element_id) != int and type(element_id) != list:
-            raise TypeError("类型错误,element_id仅支持 int和 list[int]")
-        bf_list = qt_model.GetElementStress(element_id, stage_id, result_kind, increment_type, operation, case_name)
-        list_res = []
-        for item in bf_list:
-            if item.ElementType == "BEAM":
-                stress_i = [item.StressI[0], item.StressI[1], item.StressI[2], item.StressI[3], item.StressI[4], item.StressI[5],
-                            item.StressI[6], item.StressI[7], item.StressI[8]]
-                stress_j = [item.StressJ[0], item.StressJ[1], item.StressJ[2], item.StressJ[3], item.StressJ[4], item.StressJ[5],
-                            item.StressJ[6], item.StressJ[7], item.StressJ[8]]
-                list_res.append(BeamElementStress(item.ElementId, stress_i, stress_j))
-            elif item.ElementType == "SHELL":
-                stress_i = [item.StressI[0], item.StressI[1], item.StressI[2], item.StressI[3], item.StressI[4]]
-                stress_j = [item.StressJ[0], item.StressJ[1], item.StressJ[2], item.StressJ[3], item.StressJ[4]]
-                stress_k = [item.StressK[0], item.StressK[1], item.StressK[2], item.StressK[3], item.StressK[4]]
-                stress_l = [item.StressL[0], item.StressL[1], item.StressL[2], item.StressL[3], item.StressL[4]]
-                stress_i2 = [item.BotIStress[0], item.BotIStress[1], item.BotIStress[2], item.BotIStress[3], item.BotIStress[4]]
-                stress_j2 = [item.BotJStress[0], item.BotJStress[1], item.BotJStress[2], item.BotJStress[3], item.BotJStress[4]]
-                stress_k2 = [item.BotKStress[0], item.BotKStress[1], item.BotKStress[2], item.BotKStress[3], item.BotKStress[4]]
-                stress_l2 = [item.BotLStress[0], item.BotLStress[1], item.BotLStress[2], item.BotLStress[3], item.BotLStress[4]]
-                list_res.append(ShellElementStress(item.ElementId, stress_i, stress_j, stress_k, stress_l,
-                                                   stress_i2, stress_j2, stress_k2, stress_l2))
-            elif item.ElementType == "CABLE" or item.ElementType == "LINK":
-                stress_i = [item.StressI[0], item.StressI[1], item.StressI[2], item.StressI[3], item.StressI[4], item.StressI[5],
-                            item.StressI[6], item.StressI[7], item.StressI[8]]
-                stress_j = [item.StressJ[0], item.StressJ[1], item.StressJ[2], item.StressJ[3], item.StressJ[4], item.StressJ[5],
-                            item.StressJ[6], item.StressJ[7], item.StressJ[8]]
-                list_res.append(TrussElementStress(item.ElementId, stress_i, stress_j))
-            else:
-                raise TypeError(f"操作错误，不存在{item.ElementType}类型")
-        if len(list_res) == 1:
-            return list_res[0]
-        return list_res
-
-    @staticmethod
-    def get_element_force(element_id, stage_id: int = 1, result_kind: int = 1, increment_type: int = 1, operation: bool = False, case_name=""):
-        """
-        获取单元内力,支持单个单元和单元列表
-        Args:
-            element_id: 单元编号
-            stage_id: 施工极端号
-            result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
-            increment_type: 1-全量    2-增量
-            operation: 是否为运营阶段
-            case_name: 运营阶段所需荷载工况名
-        example:
-            mdb.get_element_force(1,stage_id=1)
-            mdb.get_element_force([1,2,3],stage_id=1)
-            mdb.get_element_force(1,operation=True,case_name="工况名")
-        Returns:
-            list[ElementForce] or ElementForce
-        """
-        if type(element_id) != int and type(element_id) != list:
-            raise TypeError("类型错误,element_id仅支持 int和 list[int]")
-        bf_list = qt_model.GetElementForce(element_id, stage_id, result_kind, increment_type, operation, case_name)
-        list_res = []
-        for item in bf_list:
-            if item.ElementType == "BEAM":
-                force_i = [item.ForceI.Fx, item.ForceI.Fy, item.ForceI.Fz, item.ForceI.Mx, item.ForceI.My, item.ForceI.Mz]
-                force_j = [item.ForceJ.Fx, item.ForceJ.Fy, item.ForceJ.Fz, item.ForceJ.Mx, item.ForceJ.My, item.ForceJ.Mz]
-                list_res.append(BeamElementForce(item.ElementId, force_i, force_j))
-            elif item.ElementType == "PLATE":
-                force_i = [item.ForceI.Fx, item.ForceI.Fy, item.ForceI.Fz, item.ForceI.Mx, item.ForceI.My, item.ForceI.Mz]
-                force_j = [item.ForceJ.Fx, item.ForceJ.Fy, item.ForceJ.Fz, item.ForceJ.Mx, item.ForceJ.My, item.ForceJ.Mz]
-                force_k = [item.ForceK.Fx, item.ForceK.Fy, item.ForceK.Fz, item.ForceK.Mx, item.ForceK.My, item.ForceK.Mz]
-                force_l = [item.ForceL.Fx, item.ForceL.Fy, item.ForceL.Fz, item.ForceL.Mx, item.ForceL.My, item.ForceL.Mz]
-                list_res.append(ShellElementForce(item.ElementId, force_i, force_j, force_k, force_l))
-            elif item.ElementType == "CABLE" or item.ElementType == "LINK":
-                force_i = [item.ForceI.Fx, item.ForceI.Fy, item.ForceI.Fz, item.ForceI.Mx, item.ForceI.My, item.ForceI.Mz]
-                force_j = [item.ForceJ.Fx, item.ForceJ.Fy, item.ForceJ.Fz, item.ForceJ.Mx, item.ForceJ.My, item.ForceJ.Mz]
-                list_res.append(TrussElementForce(item.ElementId, force_i, force_j))
-            else:
-                raise TypeError(f"操作错误，不存在{item.ElementType}类型")
-        if len(list_res) == 1:
-            return list_res[0]
-        return list_res
-
-    @staticmethod
-    def get_reaction(node_id, stage_id: int = 1, result_kind: int = 1, increment_type: int = 1, operation: bool = False, case_name=""):
-        """
-        获取节点,支持单个节点和节点列表
-        Args:
-            node_id: 节点编号
-            stage_id: 施工极端号
-            result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
-            increment_type: 1-全量    2-增量
-            operation: 是否为运营阶段
-            case_name: 运营阶段所需荷载工况名
-        example:
-            mdb.get_reaction(1,stage_id=1)
-            mdb.get_reaction([1,2,3],stage_id=1)
-            mdb.get_reaction(1,operation=True,case_name="工况名")
-        Returns:
-            list[SupportReaction] or SupportReaction
-        """
-        if type(node_id) != int and type(node_id) != list:
-            raise TypeError("类型错误,beam_id int和 list[int]")
-        bs_list = qt_model.GetSupportReaction(node_id, stage_id, result_kind, increment_type, operation, case_name)
-        list_res = []
-        for item in bs_list:
-            force = [item.Force.Fx, item.Force.Fy, item.Force.Fz, item.Force.Mx, item.Force.My, item.Force.Mz]
-            list_res.append(SupportReaction(item.NodeId, force))
-        if len(list_res) == 1:
-            return list_res[0]
-        return list_res
-
-    @staticmethod
-    def get_node_displacement(node_id, stage_id: int = 1, result_kind: int = 1, increment_type: int = 1, operation: bool = False, case_name=""):
-        """
-        获取节点,支持单个节点和节点列表
-        Args:
-            node_id: 节点号
-            stage_id: 施工极端号
-            result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载
-            increment_type: 1-全量    2-增量
-            operation: 是否为运营阶段
-            case_name: 运营阶段所需荷载工况名
-        example:
-            mdb.get_node_displacement(1,stage_id=1)
-            mdb.get_node_displacement([1,2,3],stage_id=1)
-            mdb.get_node_displacement(1,operation=True,case_name="工况名")
-        Returns:
-            list[NodeDisplacement] or NodeDisplacement
-        """
-        if type(node_id) != int and type(node_id) != list:
-            raise TypeError("类型错误,node_id仅支持 int和 list[int]")
-        bf_list = qt_model.GetNodeDisplacement(node_id, stage_id, result_kind, increment_type, operation, case_name)
-        list_res = []
-        for item in bf_list:
-            displacements = [item.Displacement.Dx, item.Displacement.Dy, item.Displacement.Dz,
-                             item.Displacement.Rx, item.Displacement.Ry, item.Displacement.Rz]
-            list_res.append(NodeDisplacement(item.NodeId, displacements))
-        if len(list_res) == 1:
-            return list_res[0]
-        return list_res
-
-    # endregion
-
-    # region
-    @staticmethod
-    def get_node_data(ids=None):
-        """
-        获取节点信息 默认获取所有节点信息
-        Args: 无
-        example:
-            mdb.get_node_data()
-            mdb.get_node_data(1)
-            mdb.get_node_data([1,2])
-        Returns:
-            list[Node] 或 Node
-        """
-        node_list = []
-        if ids is None:
-            node_list = qt_model.GetNodeData()
-        res_list = []
-        for item in node_list:
-            res_list.append(Node(item.Id, item.XCoor, item.YCoor, item.ZCoor))
-        return res_list
-
-    @staticmethod
-    def get_element_data():
-        """
-        获取单元信息
-        Args: 无
-        example:
-            mdb.get_element_data()
-        Returns:
-            list[Element]
-        """
-        # ele_list = []
-        # if ele_type == 1:
-        #     ele_list = qt_model.GetBeamElementData()
-
-    # endregion
```

### Comparing `qtmodel-0.3.8/qtmodel/res_db.py` & `qtmodel-0.3.9/qtmodel/res_db.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.3.8/qtmodel.egg-info/PKG-INFO` & `qtmodel-0.3.9/qtmodel.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,242 +1,335 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.3.8
+Version: 0.3.9
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# 最新版本 V0.3.8 - 2024.05.21 
+# 最新版本 V0.3.9 - 2024.05.29 
 > pip install --upgrade qtmodel
 - 优化部分调用
 
 ##  项目管理
+### update_model
+刷新模型信息
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.update_model()
+```  
+Returns: 无
+### update_app_stage
+切换模型前后处理状态
+> 参数:  
+> num: 1-前处理  2-后处理  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.update_app_stage(1)
+mdb.update_app_stage(2)
+```  
+Returns: 无
+### do_solve
+运行分析
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.do_solve()
+```  
+Returns: 无
 ### initial
 初始化模型,新建模型
+> 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.initial()
 ```  
+Returns: 无
 ### open_file
 打开bfmd文件
+> 参数:  
+> file_path: 文件全路径  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.open_file("a.bfmd")
 ```  
-### save_file
-保存bfmd文件
+Returns: 无
+### close_project
+关闭项目
+> 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.save_file("a.bfmd")
+mdb.close_project()
 ```  
-### close_project
-关闭项目
+Returns: 无
+### save_file
+保存bfmd文件
+> 参数:  
+> file_path: 文件全路径  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.close_project()
+mdb.save_file("a.bfmd")
 ```  
+Returns: 无
 ### import_command
 导入命令
 > 参数:  
 > command:命令字符  
-> command_type:命令类型 1-桥通命令  
+> command_type:命令类型 1-桥通命令 目前仅支持桥通命令  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.import_command("*SECTION")
 ```  
+Returns: 无
+### import_file
+导入文件
+> 参数:  
+> file_path:导入文件(.mct/.qdat/.dxf/.3dx)  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.import_file("a.mct")
+```  
+Returns: 无
 ### export_file
 导入命令
 > 参数:  
-> file_path:导出文件(.mct/.qdat/.PGF/.3dx)  
+> file_path:导出文件全路径，支持格式(.mct/.qdat/.PGF/.3dx)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.export_file("a.mct")
 ```  
-### import_file
-导入命令
+Returns: 无
+##  节点单元操作
+### add_nodes
+添加多个节点，可以选择指定节点编号
 > 参数:  
-> file_path:导入文件(.mct/.qdat/.dxf/.3dx)  
+> node_list:节点坐标信息 [[x1,y1,z1],...]或 [[id1,x1,y1,z1]...]  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.import_file("a.mct")
+mdb.add_nodes([[1,2,3],[4,5,6]])
+mdb.add_nodes([[1,1,2,3],[2,4,5,6]])
 ```  
-### do_solve
-运行分析
+Returns: 无
+### add_node
+根据坐标信息和节点编号添加节点，默认自动识别编号
+> 参数:  
+> x: 节点坐标x  
+> y: 节点坐标y  
+> z: 节点坐标z  
+> index: 节点编号，默认自动识别编号 (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.do_solve()
+mdb.add_node(1,2,3)
+mdb.add_node(x= 1,y = 2,z = 4,index = 2)
 ```  
-##  节点单元操作
+Returns: 无
+### update_node_id
+根据坐标信息和节点编号添加节点，默认自动识别编号
+> 参数:  
+> node_id: 节点编号  
+> new_id: 新节点编号  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.update_node_id(1,2)
+```  
+Returns: 无
+### merge_nodes
+根据坐标信息和节点编号添加节点，默认自动识别编号
+> 参数:  
+> ids: 合并节点集合  默认全部节点  
+> tolerance: 合并容许误差  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.merge_nodes()
+```  
+Returns: 无
+### remove_node
+删除指定节点,不输入参数时默认删除所有节点
+> 参数:  
+> ids:节点编号  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.remove_node()
+mdb.remove_node(ids=1)
+mdb.remove_node(ids=[1,2,3])
+```  
+Returns: 无
+### renumber_node
+节点编号重拍
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.renumber_node()
+```  
+Returns: 无
+### move_node
+移动节点坐标
+> 参数:  
+> node_id：节点号  
+> offset_x:X轴偏移量  
+> offset_y:Y轴偏移量  
+> offset_z:Z轴偏移量  
+```Python
+# 示例代码
+from qtmodel import mdb
+mdb.move_node(1,1.5,1.5,1.5)
+```  
+Returns: 无
 ### add_structure_group
 添加结构组
 > 参数:  
 > name: 结构组名  
 > index: 结构组编号(非必须参数)，默认自动识别当前编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_structure_group(name="新建结构组1")
 mdb.add_structure_group(name="新建结构组2",index=2)
 ```  
+Returns: 无
 ### remove_structure_group
 可根据结构与组名或结构组编号删除结构组，当组名和组编号均为默认则删除所有结构组
 > 参数:  
 > name:结构组名称  
 > index:结构组编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_structure_group(name="新建结构组1")
 mdb.remove_structure_group(index = 2)
 ```  
+Returns: 无
 ### add_structure_to_group
 为结构组添加节点和/或单元
 > 参数:  
 > name: 结构组名  
 > node_ids: 节点编号列表(可选参数)  
 > element_ids: 单元编号列表(可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
 ```  
+Returns: 无
 ### remove_structure_in_group
 为结构组删除节点和/或单元
 > 参数:  
 > name: 结构组名  
 > node_ids: 节点编号列表(可选参数)  
 > element_ids: 单元编号列表(可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
 ```  
-### add_node
-根据坐标信息和节点编号添加节点，默认自动识别编号
-> 参数:  
-> x: 节点坐标x  
-> y: 节点坐标y  
-> z: 节点坐标z  
-> index: 节点编号，默认自动识别编号 (可选参数)  
-```Python
-# 示例代码
-from qtmodel import mdb
-mdb.add_node(1,2,3)
-mdb.add_node(x= 1,y = 2,z = 4,index = 2)
-```  
-### add_nodes
-添加多个节点，可以选择指定节点编号
-> 参数:  
-> node_list:节点坐标信息 [[x1,y1,z1],...]或 [[id1,x1,y1,z1]...]  
-```Python
-# 示例代码
-from qtmodel import mdb
-mdb.add_nodes([[1,2,3],[4,5,6]])
-mdb.add_nodes([[1,1,2,3],[2,4,5,6]])
-```  
-### remove_node
-删除指定节点,不输入参数时默认删除所有节点
-> 参数:  
-> index:节点编号  
-```Python
-# 示例代码
-from qtmodel import mdb
-mdb.remove_node()
-mdb.remove_node(index=1)
-```  
+Returns: 无
 ### add_element
 根据单元编号和单元类型添加单元
 > 参数:  
 > index:单元编号  
 > ele_type:单元类型 1-梁 2-索 3-杆 4-板  
 > node_ids:单元对应的节点列表 [i,j] 或 [i,j,k,l]  
 > beta_angle:贝塔角  
 > mat_id:材料编号  
 > sec_id:截面编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_element(index=1,ele_type=1,node_ids=[1,2],beta_angle=1,mat_id=1,sec_id=1)
 ```  
+Returns: 无
 ### remove_element
 删除指定编号的单元
 > 参数:  
 > index: 单元编号,默认时删除所有单元  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_element()
 mdb.remove_element(index=1)
 ```  
+Returns: 无
 ##  材料操作
 ### add_material
 添加材料
 > 参数:  
 > index:材料编号,默认自动识别 (可选参数)  
 > name:材料名称  
-> material_type: 材料类型  
+> mat_type: 材料类型  
 > standard:规范名称  
 > database:数据库  
 > construct_factor:构造系数  
 > modified:是否修改默认材料参数,默认不修改 (可选参数)  
 > data_info:材料参数列表[弹性模量,容重,泊松比,热膨胀系数] (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
-mdb.add_material(index=1,name="混凝土材料1",material_type="混凝土",standard="公路18规范",database="C50")
-mdb.add_material(index=1,name="自定义材料1",material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
+mdb.add_material(index=1,name="混凝土材料1",mat_type="混凝土",standard="公路18规范",database="C50")
+mdb.add_material(index=1,name="自定义材料1",mat_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
 ```  
+Returns: 无
 ### add_time_material
 添加收缩徐变材料
 > 参数:  
 > index: 指定收缩徐变编号,默认则自动识别 (可选参数)  
 > name: 收缩徐变名  
 > code_index: 收缩徐变规范索引  
 > time_parameter: 对应规范的收缩徐变参数列表,默认不改变规范中信息 (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_time_material(index=1,name="收缩徐变材料1",code_index=1)
 ```  
+Returns: 无
 ### update_material_creep
 将收缩徐变参数连接到材料
 > 参数:  
 > index: 材料编号  
 > creep_id: 收缩徐变编号  
 > f_cuk: 材料标准抗压强度,仅自定义材料是需要输入  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.update_material_creep(index=1,creep_id=1,f_cuk=5e7)
 ```  
+Returns: 无
 ### remove_material
 删除指定材料
 > 参数:  
 > index:指定材料编号，默认则删除所有材料  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_material()
 mdb.remove_material(index=1)
 ```  
+Returns: 无
 ##  截面操作
 ### add_parameter_section
 添加截面信息
 > 参数:  
 > index: 截面编号,默认自动识别  
 > name:截面名称  
 > sec_type:参数截面类型名称,支持以下类型  
@@ -262,14 +355,15 @@
 # 示例代码
 from qtmodel import mdb
 mdb.add_parameter_section(name="截面1",sec_type="矩形",sec_info=[2,4],bias_type="中心")
 mdb.add_parameter_section(name="截面2",sec_type="混凝土箱梁",box_height=2,box_number=3,
 sec_info=[0.02,0,12,3,1,2,1,5,6,0.2,0.4,0.1,0.13,0.28,0.3,0.5,0.5,0.5,0.2],
 charm_info=["1*0.2,0.1*0.2","0.5*0.15,0.3*0.2","0.4*0.2","0.5*0.2"])
 ```  
+Returns: 无
 ### add_steel_section
 添加钢梁截面,包括参数型钢梁截面和自定义带肋钢梁截面
 > 参数:  
 > index:  
 > name:  
 > sec_type:截面类型 1-工字钢梁  2-箱型钢梁  
 > sec_info:截面信息  
@@ -290,48 +384,55 @@
 from qtmodel import mdb
 mdb.add_steel_section(name="钢梁截面1",sec_type=1,sec_info=[0,0,0.5,0.5,0.5,0.5,0.7,0.02,0.02,0.02])
 mdb.add_steel_section(name="钢梁截面2",sec_type=2,sec_info=[0,0.15,0.25,0.5,0.25,0.15,0.4,0.15,0.7,0.02,0.02,0.02,0.02],
 rib_info = {"板肋1": [0.1,0.02],"T形肋1":[0.1,0.02,0.02,0.02]},
 rib_place = [(0, 0, 0, [(0.1, "板肋1", 2, "默认名称1"), (0.2, "板肋1", 2, "默认名称2")]), (0, 0, 1, [(0.1, "T形肋1", 0, "默认名称3")])],
 bias_type="中上")
 ```  
+Returns: 无
 ### add_user_section
 添加自定义截面,目前仅支持特性截面
 > 参数:  
 > index:截面编号  
 > name:截面名称  
 > sec_type:截面类型  
 > property_info:截面特性列表  
+> main_loop:主线圈坐标集合 [(-1,-1),(5,0),(5,5),(-1,5)] 目前只支持单一线圈  
+> sub_loops:次线圈坐标集合 [[(0,0),(0,1),(1,1,)], [(2,2),(3,2),(3,3)]]  
+> sec_lines:线宽集合[(x1,y1,x2,y3,thick),]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_user_section(name="自定义特性截面",property_info=[i for i in range(25)])
 ```  
+Returns: 无
 ### add_tapper_section
 添加变截面,需先建立单一截面
 > 参数:  
 > index:截面编号  
 > name:截面名称  
 > begin_id:截面始端编号  
 > end_id:截面末端编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_tapper_section(name="变截面1",begin_id=1,end_id=2)
 ```  
+Returns: 无
 ### remove_section
 删除截面信息
 > 参数:  
 > index: 截面编号,参数为默认时删除全部截面  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_section()
 mdb.remove_section(1)
 ```  
+Returns: 无
 ##  板厚操作
 ### add_thickness
 添加板厚
 > 参数:  
 > index: 板厚id  
 > name: 板厚名称  
 > t:   板厚度  
@@ -345,24 +446,26 @@
 > rib_l: 横向肋板信息  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_thickness(name="厚度1", t=0.2,thick_type=0,bias_info=(0,0.8))
 mdb.add_thickness(name="厚度2", t=0.2,thick_type=1,rib_pos=0,dist_v=0.1,rib_v=[1,1,0.02,0.02])
 ```  
+Returns: 无
 ### remove_thickness
 删除板厚
 > 参数:  
 > index:板厚编号,默认时删除所有板厚信息  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_thickness()
 mdb.remove_thickness(index=1)
 ```  
+Returns: 无
 ### add_tapper_section_group
 添加变截面组
 > 参数:  
 > ids:变截面组编号  
 > name: 变截面组名  
 > factor_w: 宽度方向变化阶数 线性(1.0) 非线性(!=1.0)  
 > factor_h: 高度方向变化阶数 线性(1.0) 非线性(!=1.0)  
@@ -371,106 +474,115 @@
 > dis_w: 宽度方向距离  
 > dis_h: 高度方向距离  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_tapper_section_group(ids=[1,2,3,4],name="变截面组1")
 ```  
+Returns: 无
 ### update_section_bias
 更新截面偏心
 > 参数:  
 > index:截面编号  
 > bias_type:偏心类型  
 > center_type:中心类型  
 > shear_consider:考虑剪切  
 > bias_point:自定义偏心点(仅自定义类型偏心需要)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.update_section_bias(index=1,bias_type="中上",center_type="几何中心")
 mdb.update_section_bias(index=1,bias_type="自定义",bias_point=[0.1,0.2])
 ```  
+Returns: 无
 ##  边界操作
 ### add_boundary_group
 新建边界组
 > 参数:  
 > name:边界组名  
 > index:边界组编号，默认自动识别当前编号 (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_boundary_group(name="边界组1")
 ```  
+Returns: 无
 ### remove_boundary_group
 按照名称删除边界组
 > 参数:  
 > name: 边界组名称，默认删除所有边界组 (非必须参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_boundary_group()
 mdb.remove_boundary_group(name="边界组1")
 ```  
+Returns: 无
 ### remove_all_boundary
 根据边界组名称、边界的类型和编号删除边界信息,默认时删除所有边界信息
 > 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_all_boundary()
 ```  
+Returns: 无
 ### remove_boundary
 根据节点号删除一般支撑、弹性支承/根据单元号删除梁端约束/根据主节点号删除主从约束/根据从节点号删除约束方程
 > 参数:  
 > remove_id:节点号 or 单元号 or主节点号  or 从节点号  
 > bd_type:边界类型  
 > _1-一般支承 2-弹性支承 3-主从约束 4-弹性连接 5-约束方程 6-梁端约束_  
 > group:边界所处边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_boundary(remove_id = 1, bd_type = 1,group="边界组1")
 ```  
+Returns: 无
 ### add_general_support
 添加一般支承
 > 参数:  
 > node_id:节点编号  
 > boundary_info:边界信息  [X,Y,Z,Rx,Ry,Rz]  
 > _ture-固定 false-自由_  
 > group_name:边界组名,默认为默认边界组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_general_support(node_id=1, boundary_info=[True,True,True,False,False,False])
 ```  
+Returns: 无
 ### add_elastic_support
 添加弹性支承
 > 参数:  
 > node_id:节点编号  
 > support_type:支承类型 1-线性  2-受拉  3-受压  
 > boundary_info:边界信息 受拉和受压时列表长度为1  线性时列表长度为6  
 > group_name:边界组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_elastic_support(node_id=1,support_type=1,boundary_info=[1e6,0,1e6,0,0,0])
 ```  
+Returns: 无
 ### add_master_slave_link
 添加主从约束
 > 参数:  
 > master_id:主节点号  
 > slave_id:从节点号  
 > boundary_info:边界信息 [X,Y,Z,Rx,Ry,Rz]  
 > _ture-固定 false-自由_  
 > group_name:边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_master_slave_link(master_id=1,slave_id=2,boundary_info=[True,True,True,False,False,False])
 ```  
+Returns: 无
 ### add_elastic_link
 添加弹性连接
 > 参数:  
 > link_type:节点类型  
 > _1-一般弹性连接 2-刚性连接 3-受拉弹性连接 4-受压弹性连接_  
 > start_id:起始节点号  
 > end_id:终节点号  
@@ -482,39 +594,42 @@
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_elastic_link(link_type=1,start_id=1,end_id=2,boundary_info=[1e6,1e6,1e6,0,0,0])
 mdb.add_elastic_link(link_type=2,start_id=1,end_id=2)
 mdb.add_elastic_link(link_type=3,start_id=1,end_id=2,kx=1e6)
 ```  
+Returns: 无
 ### add_beam_constraint
 添加梁端约束
 > 参数:  
 > beam_id:梁号  
 > info_i:i端约束信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > info_j:j端约束信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > group_name:边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_constraint(beam_id=2,info_i=[True,True,True,False,False,False],info_j=[True,True,True,False,False,False])
 ```  
+Returns: 无
 ### add_node_axis
 添加节点坐标
 > 参数:  
 > input_type:输入方式 1-角度 2-三点  3-向量  
 > node_id:节点号  
 > coord_info:局部坐标信息 -List<float>(角)  -List<List<float>>(三点 or 向量)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_node_axis(input_type=1,node_id=1,coord_info=[45,45,45])
 mdb.add_node_axis(input_type=2,node_id=1,coord_info=[[0,0,1],[0,1,0],[1,0,0]])
 mdb.add_node_axis(input_type=3,node_id=1,coord_info=[[0,0,1],[0,1,0]])
 ```  
+Returns: 无
 ##  移动荷载
 ### add_standard_vehicle
 添加标准车辆
 > 参数:  
 > name: 车辆荷载名称  
 > standard_code: 荷载规范  
 > _1-中国铁路桥涵规范(Q/CR 9300-2017)_  
@@ -533,48 +648,52 @@
 > load_length: 默认为0即不限制荷载长度  (铁路桥涵规范2017 所需参数)  
 > n:车厢数: 默认6节车厢 (城市轨道交通桥梁规范2017 所需参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_standard_vehicle("高速铁路",standard_code=1,load_type="高速铁路")
 ```  
+Returns: 无
 ### add_node_tandem
 添加节点纵列
 > 参数:  
 > name:节点纵列名  
 > start_id:起始节点号  
 > node_ids:节点列表  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_node_tandem("节点纵列1",1,[i+1 for i in range(12)])
 ```  
+Returns: 无
 ### add_influence_plane
 添加影响面
 > 参数:  
 > name:影响面名称  
 > tandem_names:节点纵列名称组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_influence_plane("影响面1",["节点纵列1","节点纵列2"])
 ```  
+Returns: 无
 ### add_lane_line
 添加车道线
 > 参数:  
 > name:车道线名称  
 > influence_name:影响面名称  
 > tandem_name:节点纵列名  
 > offset:偏移  
 > lane_width:车道宽度  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_lane_line("车道1","影响面1","节点纵列1",offset=0,lane_width=3.1)
 ```  
+Returns: 无
 ### add_live_load_case
 添加移动荷载工况
 > 参数:  
 > name:荷载工况名  
 > influence_plane:影响线名  
 > span:跨度  
 > car_detail: 汽车相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)  
@@ -582,89 +701,97 @@
 > metro_detail: 轻轨相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)  
 > sub_case:子工况信息 [(车辆名称,系数,["车道1","车道2"])...]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_live_load_case("活载工况1","影响面1",100,sub_case=[("车辆名称",1.0,["车道1","车道2"]),])
 ```  
+Returns: 无
 ### remove_vehicle
 删除车辆信息
 > 参数:  
 > index:车辆荷载编号  
 > name:车辆名称  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_vehicle(index=1)
 mdb.remove_vehicle(name="车辆名称")
 ```  
+Returns: 无
 ### remove_node_tandem
 按照 节点纵列编号/节点纵列名 删除节点纵列
 > 参数:  
 > index:节点纵列编号  
 > name:节点纵列名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_node_tandem(index=1)
 mdb.remove_node_tandem(name="节点纵列1")
 ```  
+Returns: 无
 ### remove_influence_plane
 按照 影响面编号/影响面名称 删除影响面
 > 参数:  
 > index:影响面编号  
 > name:影响面名称  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_influence_plane(index=1)
 mdb.remove_influence_plane(name="影响面1")
 ```  
+Returns: 无
 ### remove_lane_line
 按照 车道线编号/车道线名称 删除车道线
 > 参数:  
 > name:车道线名称  
 > index:车道线编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_lane_line(index=1)
 mdb.remove_lane_line(name="车道线1")
 ```  
+Returns: 无
 ### remove_live_load_case
 删除移动荷载工况
 > 参数:  
 > name:移动荷载工况名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_live_load_case(name="活载工况1")
 ```  
+Returns: 无
 ##  钢束操作
 ### add_tendon_group
 按照名称添加钢束组，添加时可指定钢束组id
 > 参数:  
 > name: 钢束组名称  
 > index: 钢束组编号(非必须参数)，默认自动识别  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_tendon_group(name="钢束组1")
 ```  
+Returns: 无
 ### remove_tendon_group
 按照钢束组名称或钢束组编号删除钢束组，两参数均为默认时删除所有钢束组
 > 参数:  
 > name:钢束组名称,默认自动识别 (可选参数)  
 > index:钢束组编号,默认自动识别 (可选参数)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_tendon_group(name="钢束组1")
 mdb.remove_tendon_group(index=1)
 ```  
+Returns: 无
 ### add_tendon_property
 添加钢束特性
 > 参数:  
 > name:钢束特性名  
 > index:钢束编号,默认自动识别 (可选参数)  
 > tendon_type: 0-PRE 1-POST  
 > material_id: 钢材材料编号  
@@ -680,14 +807,15 @@
 > slip_info: 滑移信息[始端距离,末端距离] 默认为[0.006, 0.006]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_tendon_property(name="钢束1",tendon_type=0,material_id=1,duct_type=1,steel_type=1,
 steel_detail=[0.00014,0.10,0.25,0.0015],loos_detail=(1,1,1))
 ```  
+Returns: 无
 ### add_tendon_3d
 添加三维钢束
 > 参数:  
 > name:钢束名称  
 > property_name:钢束特性名称  
 > group_name:默认钢束组  
 > num:根数  
@@ -706,142 +834,155 @@
 # 示例代码
 from qtmodel import mdb
 mdb.add_tendon_3d("BB1",property_name="22-15",num=2,position_type=1,
 control_points=[(0,0,-1,0),(10,0,-1,0)],point_insert=(0,0,0))
 mdb.add_tendon_3d("BB1",property_name="22-15",num=2,position_type=2,
 control_points=[(0,0,-1,0),(10,0,-1,0)],point_insert=(1,1,1),track_group="轨迹线结构组1")
 ```  
+Returns: 无
 ### remove_tendon
 按照名称或编号删除钢束,默认时删除所有钢束
 > 参数:  
 > name:钢束名称  
 > index:钢束编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_tendon(name="钢束1")
 mdb.remove_tendon(index=1)
 mdb.remove_tendon()
 ```  
+Returns: 无
 ### remove_tendon_property
 按照名称或编号删除钢束组,默认时删除所有钢束组
 > 参数:  
 > name:钢束组名称  
 > index:钢束组编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_tendon_property(name="钢束特性1")
 mdb.remove_tendon_property(index=1)
 mdb.remove_tendon_property()
 ```  
+Returns: 无
 ### add_nodal_mass
 添加节点质量
 > 参数:  
 > node_id:节点编号  
 > mass_info:[m,rmX,rmY,rmZ]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_nodal_mass(node_id=1,mass_info=(100,0,0,0))
 ```  
+Returns: 无
 ### remove_nodal_mass
 删除节点质量
 > 参数:  
 > node_id:节点号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_nodal_mass(node_id=1)
 ```  
+Returns: 无
 ### add_pre_stress
 添加预应力
 > 参数:  
 > case_name:荷载工况名  
 > tendon_name:钢束名  
 > pre_type:预应力类型  
 > _0-始端 1-末端 2-两端_  
 > force:预应力  
 > group_name:边界组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_pre_stress(case_name="荷载工况名",tendon_name="钢束1",force=1390000)
 ```  
+Returns: 无
 ### remove_pre_stress
 删除预应力
 > 参数:  
 > case_name:荷载工况  
 > tendon_name:钢束组  
 > group_name:边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_pre_stress(case_name="工况1",tendon_name="钢束1",group_name="默认荷载组")
 ```  
+Returns: 无
 ##  荷载操作
 ### add_load_group
 根据荷载组名称添加荷载组
 > 参数:  
 > name: 荷载组名称  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_load_group(name="荷载组1")
 ```  
+Returns: 无
 ### remove_load_group
 根据荷载组名称或荷载组id删除荷载组,参数为默认时删除所有荷载组
 > 参数:  
 > name: 荷载组名称  
 > index: 荷载组编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_group(name="荷载组1")
 mdb.remove_load_group(index=1)
 ```  
+Returns: 无
 ### add_nodal_force
 添加节点荷载
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_nodal_force(case_name="荷载工况1",node_id=1,load_info=(1,1,1,1,1,1),group_name="默认结构组")
 ```  
+Returns: 无
 ### remove_nodal_force
 删除节点荷载
 > 参数:  
 > case_name:荷载工况名  
 > node_id:节点编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_nodal_force(case_name="荷载工况1",node_id=1)
 ```  
+Returns: 无
 ### add_node_displacement
 添加节点位移
 > 参数:  
 > node_id:节点编号  
 > case_name:荷载工况名  
 > load_info:节点位移列表 [Dx,Dy,Dz,Rx,Ry,Rz]  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_node_displacement(case_name="荷载工况1",node_id=1,load_info=(1,0,0,0,0,0),group_name="默认荷载组")
 ```  
+Returns: 无
 ### remove_nodal_displacement
 删除节点位移
 > 参数:  
 > node_id:节点编号  
 > case_name:荷载工况名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
 ```  
+Returns: 无
 ### add_beam_load
 添加梁单元荷载
 > 参数:  
 > beam_id:单元编号  
 > case_name:荷载工况名  
 > load_type:荷载类型  
 > _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩  
@@ -854,53 +995,57 @@
 > projected:是否投影  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0.4,0.8],list_load=[100,200])
 ```  
+Returns: 无
 ### remove_beam_load
 删除梁单元荷载
 > 参数:  
 > element_id:单元号  
 > case_name:荷载工况名  
 > load_type:荷载类型  
 > _1-集中力   2-集中弯矩  3-分布力   4-分布弯矩_  
 > group_name:边界组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_beam_load(case_name="工况1",element_id=1,load_type=1,group_name="默认荷载组")
 ```  
+Returns: 无
 ### add_initial_tension
 添加初始拉力
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > tension:初始拉力  
 > tension_type:张拉类型  1-全量   2-增量  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_initial_tension(element_id=1,case_name="工况1",tension=100,tension_type=1)
 ```  
+Returns: 无
 ### add_cable_length_load
 添加索长张拉
 > 参数:  
 > element_id:单元类型  
 > case_name:荷载工况名  
 > length:长度  
 > tension_type:张拉类型  1-全量   2-增量  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_cable_length_load(element_id=1,case_name="工况1",length=1,tension_type=1)
 ```  
+Returns: 无
 ### add_plate_element_load
 添加版单元荷载
 > 参数:  
 > element_id:单元id  
 > case_name:荷载工况名  
 > load_type:荷载类型  
 > _1-集中力  2-集中弯矩  3-分布力  4-分布弯矩_  
@@ -912,28 +1057,30 @@
 > load_list:荷载列表  
 > xy_list:荷载位置信息 [IJ方向绝对距离x,IL方向绝对距离y]  (仅集中荷载需要)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_plate_element_load(element_id=1,case_name="工况1",load_type=1,group_name="默认荷载组",load_list=[1000],xy_list=(0.2,0.5))
 ```  
+Returns: 无
 ### add_deviation_parameter
 添加制造误差
 > 参数:  
 > name:名称  
 > element_type:单元类型  1-梁单元  2-板单元  
 > parameters:参数列表  
 > _梁杆单元:[轴向,I端X向转角,I端Y向转角,I端Z向转角,J端X向转角,J端Y向转角,J端Z向转角]_  
 > _板单元:[X向位移,Y向位移,Z向位移,X向转角,Y向转角]_  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_deviation_parameter(name="梁端制造误差",element_type=1,parameters=[1,0,0,0,0,0,0])
 mdb.add_deviation_parameter(name="板端制造误差",element_type=1,parameters=[1,0,0,0,0])
 ```  
+Returns: 无
 ### add_deviation_load
 添加制造误差荷载
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > parameters:参数名列表  
 > _梁杆单元时-[制造误差参数名称]_  
@@ -941,34 +1088,37 @@
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_deviation_load(element_id=1,case_name="工况1",parameters=["梁端误差"])
 mdb.add_deviation_load(element_id=2,case_name="工况1",parameters=["板端误差1","板端误差2","板端误差3","板端误差4"])
 ```  
+Returns: 无
 ### add_element_temperature
 添加单元温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > temperature:最终温度  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_element_temperature(element_id=1,case_name="自重",temperature=1,group_name="默认荷载组")
 ```  
+Returns: 无
 ### add_gradient_temperature
 添加梯度温度
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_gradient_temperature(element_id=1,case_name="荷载工况1",group_name="荷载组名1",temperature=10)
 mdb.add_gradient_temperature(element_id=2,case_name="荷载工况2",group_name="荷载组名2",temperature=10,element_type=2)
 ```  
+Returns: 无
 ### add_beam_section_temperature
 添加梁截面温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > paving_thick:铺设厚度(m)  
 > temperature_type:温度类型  1-升温(默认) 2-降温  
@@ -978,136 +1128,150 @@
 > modify:是否修改规范温度  
 > temp_list:温度列表[T1,T2]  (仅修改时需要)  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_section_temperature(element_id=1,case_name="工况1",paving_thick=0.1)
 ```  
+Returns: 无
 ### add_index_temperature
 添加指数温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > temperature:温差  
 > index:指数  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_index_temperature(element_id=1,case_name="工况1",temperature=20,index=2)
 ```  
+Returns: 无
 ### add_top_plate_temperature
 添加顶板温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载  
 > temperature:最终温度  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_top_plate_temperature(element_id=1,case_name="工况1",temperature=40,group_name="默认荷载组")
 ```  
+Returns: 无
 ##  沉降操作
 ### add_sink_group
 添加沉降组
 > 参数:  
 > name: 沉降组名  
 > sink: 沉降值  
 > node_ids: 节点编号  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_sink_group(name="沉降1",sink=0.1,node_ids=[1,2,3])
 ```  
+Returns: 无
 ### remove_sink_group
 按照名称删除沉降组
 > 参数:  
 > name:沉降组名,默认删除所有沉降组  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_sink_group()
 mdb.remove_sink_group(name="沉降1")
 ```  
+Returns: 无
 ### add_sink_case
 添加沉降工况
 > 参数:  
 > name:荷载工况名  
 > sink_groups:沉降组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_sink_case(name="沉降工况1",sink_groups=["沉降1","沉降2"])
 ```  
+Returns: 无
 ### remove_sink_case
 按照名称删除沉降工况,不输入名称时默认删除所有沉降工况
 > 参数:  
 > name:沉降工况名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_sink_case()
 mdb.remove_sink_case(name="沉降1")
 ```  
+Returns: 无
 ### add_concurrent_reaction
 添加并发反力组
 > 参数:  
 > names: 结构组名称集合  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_concurrent_reaction(["默认结构组"])
 ```  
+Returns: 无
 ### remove_concurrent_reaction
 删除所有并发反力组
 > 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_concurrent_reaction()
 ```  
+Returns: 无
 ### add_concurrent_force
 创建并发内力组
 > 参数:  
 > names: 结构组名称集合  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_concurrent_force(["默认结构组"])
 ```  
+Returns: 无
 ### remove_concurrent_force
 删除所有并发内力组
+> 参数:  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_concurrent_force()
 ```  
+Returns: 无
 ### add_load_case
 添加荷载工况
 > 参数:  
 > name:沉降名  
 > case_type:荷载工况类型  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_load_case(name="工况1",case_type=1)
 ```  
+Returns: 无
 ### remove_load_case
 删除荷载工况,参数均为默认时删除全部荷载工况
 > 参数:  
 > index:荷载编号  
 > name:荷载名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_case(index=1)
 mdb.remove_load_case(name="工况1")
 mdb.remove_load_case()
 ```  
+Returns: 无
 ##  施工阶段
 ### add_construction_stage
 添加施工阶段信息
 > 参数:  
 > name:施工阶段信息  
 > duration:时长  
 > active_structures:激活结构组信息 [(结构组名,龄期,安装方法,计自重施工阶段id),...]  
@@ -1125,14 +1289,15 @@
 > index:施工阶段编号，默认自动添加  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
 ```  
+Returns: 无
 ### update_construction_stage
 添加施工阶段信息
 > 参数:  
 > name:施工阶段信息  
 > duration:时长  
 > active_structures:激活结构组信息 [(结构组名,龄期,安装方法,计自重施工阶段id),...]  
 > _计自重施工阶段id: 0-不计自重,1-本阶段 n-第n阶段)_  
@@ -1148,35 +1313,38 @@
 > temp_loads:临时荷载信息 [荷载组1，荷载组2,..]  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.update_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
 ```  
+Returns: 无
 ### update_weight_stage
 添加施工阶段信息
 > 参数:  
 > stage_name:施工阶段信息  
 > structure_group_name:结构组名  
 > weight_stage_id: 计自重阶段号  
 > _0-不计自重,1-本阶段 n-第n阶段_  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.update_weight_stage(stage_name="施工阶段1",structure_group_name="默认结构组",weight_stage_id=1)
 ```  
+Returns: 无
 ### remove_construction_stage
 按照施工阶段名删除施工阶段,默认删除所有施工阶段
 > 参数:  
 > name:所删除施工阶段名称  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_construction_stage(name="施工阶段1")
 ```  
+Returns: 无
 ##  荷载组合
 ### add_load_combine
 添加荷载组合
 > 参数:  
 > name:荷载组合名  
 > combine_type:荷载组合类型 1-叠加  2-判别  3-包络  
 > describe:描述  
@@ -1184,82 +1352,183 @@
 > _"ST"-静力荷载工况  "CS"-施工阶段荷载工况  "CB"-荷载组合_  
 > _"MV"-移动荷载工况  "SM"-沉降荷载工况_  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_load_combine(name="荷载组合1",combine_type=1,describe="无",combine_info=[("CS","合计值",1),("CS","恒载",1)])
 ```  
+Returns: 无
 ### remove_load_combine
 删除荷载组合
 > 参数:  
 > name:指定删除荷载组合名，默认时则删除所有荷载组合  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.remove_load_combine(name="荷载组合1")
-```
-## 结果提取
+```  
+Returns: 无
+
+##  静力结果查看
 ### get_element_stress
 获取单元应力,支持单个单元和单元列表
 > 参数:  
 > element_id: 单元编号  
-> stage_id: 施工极端号  
+> stage_id: 施工阶段号 -1-运营阶段  0-施工阶段包络 n-施工阶段号  
 > result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
 > increment_type: 1-全量    2-增量  
 > operation: 是否为运营阶段  
 > case_name: 运营阶段所需荷载工况名  
 ```Python
 # 示例代码
-from qtmodel import mdb
-mdb.get_element_stress(1,stage_id=1)
-mdb.get_element_stress([1,2,3],stage_id=1)
-mdb.get_element_stress(1,operation=True,case_name="工况名")
+from qtmodel import *
+odb.get_element_stress(1,stage_id=1)
+odb.get_element_stress([1,2,3],stage_id=1)
+odb.get_element_stress(1,operation=True,case_name="工况名")
 ```  
+Returns: list[ElementStress] or ElementStress
 ### get_element_force
 获取单元内力,支持单个单元和单元列表
 > 参数:  
 > element_id: 单元编号  
-> stage_id: 施工极端号  
+> stage_id: 施工阶段号 -1-运营阶段  0-施工阶段包络 n-施工阶段号  
 > result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
 > increment_type: 1-全量    2-增量  
-> operation: 是否为运营阶段  
 > case_name: 运营阶段所需荷载工况名  
 ```Python
 # 示例代码
-from qtmodel import mdb
-mdb.get_element_force(1,stage_id=1)
-mdb.get_element_force([1,2,3],stage_id=1)
-mdb.get_element_force(1,operation=True,case_name="工况名")
+from qtmodel import *
+odb.get_element_force(1,stage_id=1)
+odb.get_element_force([1,2,3],stage_id=1)
+odb.get_element_force(1,operation=True,case_name="工况名")
 ```  
+Returns: list[ElementForce] or ElementForce
 ### get_reaction
 获取节点,支持单个节点和节点列表
 > 参数:  
 > node_id: 节点编号  
-> stage_id: 施工极端号  
+> stage_id: 施工阶段号 -1-运营阶段  0-施工阶段包络 n-施工阶段号  
 > result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
 > increment_type: 1-全量    2-增量  
-> operation: 是否为运营阶段  
 > case_name: 运营阶段所需荷载工况名  
 ```Python
 # 示例代码
-from qtmodel import mdb
-mdb.get_reaction(1,stage_id=1)
-mdb.get_reaction([1,2,3],stage_id=1)
-mdb.get_reaction(1,operation=True,case_name="工况名")
+from qtmodel import *
+odb.get_reaction(1,stage_id=1)
+odb.get_reaction([1,2,3],stage_id=1)
+odb.get_reaction(1,operation=True,case_name="工况名")
 ```  
+Returns: list[SupportReaction] or SupportReaction
 ### get_node_displacement
 获取节点,支持单个节点和节点列表
 > 参数:  
 > node_id: 节点号  
-> stage_id: 施工极端号  
+> stage_id: 施工阶段号 -1-运营阶段  0-施工阶段包络 n-施工阶段号  
 > result_kind: 施工阶段数据的类型 1-合计 2-收缩徐变效应 3-预应力效应 4-恒载  
 > increment_type: 1-全量    2-增量  
-> operation: 是否为运营阶段  
 > case_name: 运营阶段所需荷载工况名  
 ```Python
 # 示例代码
-from qtmodel import mdb
-mdb.get_node_displacement(1,stage_id=1)
-mdb.get_node_displacement([1,2,3],stage_id=1)
-mdb.get_node_displacement(1,operation=True,case_name="工况名")
+from qtmodel import *
+odb.get_node_displacement(1,stage_id=1)
+odb.get_node_displacement([1,2,3],stage_id=1)
+odb.get_node_displacement(1,stage_id=-1,case_name="工况名")
+```  
+Returns: list[NodeDisplacement] or NodeDisplacement
+##  绘制模型结果
+### plot_reaction_result
+保存结果图片到指定文件甲
+> 参数:  
+> file_path: 保存路径名  
+> component: 分量编号 0-Fx 1-Fy 2-Fz 3-Fxyz 4-Mx 5-My 6-Mz 7-Mxyz  
+> load_case_name: 详细荷载工况名，参考桥通结果输出，例如： CQ:成桥(合计)  
+> stage_id: -1-运营阶段  0-施工阶段包络 n-施工阶段号  
+> envelope_type: 施工阶段包络类型 1-最大 2-最小  
+> show_number: 数值选项卡开启  
+> show_legend: 图例选项卡开启  
+> text_rotation: 数值选项卡内文字旋转角度  
+> show_max_min: 数值选项卡内最大最小值显示 -1-不显示最大最小值  0-显示最大值和最小值  1-最大绝对值 2-最大值 3-最小值  
+> digital_count: 小数点位数  
+> show_exponential: 指数显示开启  
+> increment: 是否显示增量结果  
+```Python
+# 示例代码
+from qtmodel import *
+odb.plot_reaction_result(r"aaa.png",component=0,load_case_name="CQ:成桥(合计)",stage_id=-1)     # 获取所有节点信息
+```  
+Returns: 无
+##  获取模型信息
+### get_node_data
+获取节点信息 默认获取所有节点信息
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_node_data()     # 获取所有节点信息
+odb.get_node_data(1)    # 获取单个节点信息
+odb.get_node_data([1,2])    # 获取多个节点信息
 ```  
+Returns: list[Node] 或 Node
+### get_element_data
+获取单元信息
+> 参数:  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_element_data() # 获取所有单元结果
+odb.get_element_data(1) # 获取指定编号单元信息
+```  
+Returns: list[Element]
+### get_element_type
+获取单元类型
+> 参数:  
+> ele_id: 单元号  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_element_type(1) # 获取所有单元信息
+```  
+Returns: str类型 返回 BEAM PLATE CABLE LINK
+### get_beam_element
+获取梁单元信息
+> 参数:  
+> ids: 梁单元号，默认时获取所有梁单元  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_beam_element() # 获取所有单元信息
+```  
+Returns: list[Element]
+### get_plate_element
+获取板单元信息
+> 参数:  
+> ids: 板单元号，默认时获取所有板单元  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_plate_element() # 获取所有单元信息
+```  
+Returns: list[Element]
+### get_cable_element
+获取索单元信息
+> 参数:  
+> ids: 索单元号，默认时获取所有索单元  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_cable_element() # 获取所有单元信息
+```  
+Returns: list[Element]
+### get_link_element
+获取杆单元信息
+> 参数:  
+> ids: 杆单元号，默认时输出全部杆单元  
+```Python
+# 示例代码
+from qtmodel import *
+odb.get_link_element() # 获取所有单元信息
+```  
+Returns: list[Element]
+
+
+
```

### Comparing `qtmodel-0.3.8/setup.py` & `qtmodel-0.3.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # 读取文件内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="qtmodel",
-    version="0.3.8",
+    version="0.3.9",
     author="dqy-zhj",
     author_email="1105417715@qq.com",
     description="python modeling for qt  24/05/06 ",
     long_description=long_description,  # 使用读取的 README.md 文件内容
     long_description_content_type="text/markdown",  # 指明内容格式为markdown
     url="https://github.com/Inface0443/pyqt",
     packages=find_packages(),
```

