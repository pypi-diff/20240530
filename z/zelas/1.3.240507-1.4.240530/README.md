# Comparing `tmp/zelas-1.3.240507.tar.gz` & `tmp/zelas-1.4.240530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zelas-1.3.240507.tar", last modified: Tue May  7 10:03:57 2024, max compression
+gzip compressed data, was "zelas-1.4.240530.tar", last modified: Thu May 30 13:18:06 2024, max compression
```

## Comparing `zelas-1.3.240507.tar` & `zelas-1.4.240530.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 10:03:57.570114 zelas-1.3.240507/
--rw-rw-rw-   0        0        0      646 2024-05-07 10:03:57.570114 zelas-1.3.240507/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-07 10:03:57.570114 zelas-1.3.240507/setup.cfg
--rw-rw-rw-   0        0        0     1143 2024-05-07 10:02:32.000000 zelas-1.3.240507/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 10:03:57.557118 zelas-1.3.240507/zelas/
--r--r--r--   0        0        0    18970 2024-05-04 23:23:16.000000 zelas-1.3.240507/zelas/Ellipse.py
--r--r--r--   0        0        0    17674 2024-05-04 12:33:33.000000 zelas-1.3.240507/zelas/Multispectral.py
--r--r--r--   0        0        0    40295 2024-05-04 23:59:49.000000 zelas-1.3.240507/zelas/RedundancyElimination.py
--rw-rw-rw-   0        0        0     8775 2024-05-07 07:19:56.000000 zelas-1.3.240507/zelas/TheHeartOfTheMilitaryGod.py
--rw-rw-rw-   0        0        0      189 2024-05-05 10:27:30.000000 zelas-1.3.240507/zelas/__init__.py
--r--r--r--   0        0        0     9366 2024-05-04 12:41:19.000000 zelas-1.3.240507/zelas/ransac.py
--rw-rw-rw-   0        0        0     1141 2024-05-05 10:16:09.000000 zelas-1.3.240507/zelas/setup.py
--rw-rw-rw-   0        0        0    90398 2024-05-07 06:47:15.000000 zelas-1.3.240507/zelas/shield.py
--rw-rw-rw-   0        0        0    82564 2024-05-07 07:41:56.000000 zelas-1.3.240507/zelas/voxel.py
-drwxrwxrwx   0        0        0        0 2024-05-07 10:03:57.569080 zelas-1.3.240507/zelas.egg-info/
--rw-rw-rw-   0        0        0      646 2024-05-07 10:03:57.000000 zelas-1.3.240507/zelas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-07 10:03:57.000000 zelas-1.3.240507/zelas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 10:03:57.000000 zelas-1.3.240507/zelas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-07 10:03:57.000000 zelas-1.3.240507/zelas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 13:18:06.145840 zelas-1.4.240530/
+-rw-rw-rw-   0        0        0      678 2024-05-30 13:18:06.145840 zelas-1.4.240530/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-30 13:18:06.146833 zelas-1.4.240530/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2024-05-30 13:13:30.000000 zelas-1.4.240530/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:18:06.135540 zelas-1.4.240530/zelas/
+-rw-rw-rw-   0        0        0    23518 2024-05-30 13:07:04.000000 zelas-1.4.240530/zelas/Ellipse.py
+-rw-rw-rw-   0        0        0    17609 2024-05-19 01:01:44.000000 zelas-1.4.240530/zelas/Multispectral.py
+-rw-rw-rw-   0        0        0    40295 2024-05-04 23:59:49.000000 zelas-1.4.240530/zelas/RedundancyElimination.py
+-rw-rw-rw-   0        0        0     9543 2024-05-30 01:43:10.000000 zelas-1.4.240530/zelas/TheHeartOfTheMilitaryGod.py
+-rw-rw-rw-   0        0        0      189 2024-05-05 10:27:30.000000 zelas-1.4.240530/zelas/__init__.py
+-rw-rw-rw-   0        0        0     9366 2024-05-04 12:41:19.000000 zelas-1.4.240530/zelas/ransac.py
+-rw-rw-rw-   0        0        0     1141 2024-05-05 10:16:09.000000 zelas-1.4.240530/zelas/setup.py
+-rw-rw-rw-   0        0        0    96916 2024-05-30 13:16:48.000000 zelas-1.4.240530/zelas/shield.py
+-rw-rw-rw-   0        0        0    83345 2024-05-22 07:19:42.000000 zelas-1.4.240530/zelas/voxel.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:18:06.144844 zelas-1.4.240530/zelas.egg-info/
+-rw-rw-rw-   0        0        0      678 2024-05-30 13:18:06.000000 zelas-1.4.240530/zelas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-30 13:18:06.000000 zelas-1.4.240530/zelas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 13:18:06.000000 zelas-1.4.240530/zelas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 13:18:06.000000 zelas-1.4.240530/zelas.egg-info/top_level.txt
```

### Comparing `zelas-1.3.240507/setup.py` & `zelas-1.4.240530/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 '''
 # you need to change all these
-VERSION = '1.3.240507'
-DESCRIPTION = 'Professor Liying Wang official point clouds database '
+VERSION = '1.4.240530'
+DESCRIPTION = 'Professor Liying Wang official point clouds algorithm library '
 LONG_DESCRIPTION = 'Produced by CCG.Lidar Point Cloud Research Institute'
 
 setup(
     name="zelas",
     version=VERSION,
-    author="Zelas You",
+    author="Zelas You, Mengyao Gao,Yimo Geng",
     author_email="youze1997@163.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'las'],
```

### Comparing `zelas-1.3.240507/zelas/Ellipse.py` & `zelas-1.4.240530/zelas/Ellipse.py`

 * *Files 22% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     '并行计算拟合椭圆 Parallel computing for fitting ellipses'
     num_c = len(np.unique(c))  # 圆环数
     xzlwp = np.empty([num_c, 5])  # 新建一个存储每个椭圆参数的容器
     dis_all = np.zeros(len(points))  # 距离容器
     # 并行计算加速准备 #Accelerated preparation for parallel computing
     pool = mp.Pool(processes=num_cpu)  # 开启多进程池，数量为cpu
     tik = p0.cut_down(num_c)  # 分块器
-    tik2 = p0.cut_down(len(points))  # 分块器
+    # tik2 = p0.cut_down(len(points))  # 分块器
     tik_b = 0  # 分块输出计时器
     # 并行计算每个圆环 Parallel computing for each torus
     multi_res = [pool.apply_async(fit_Ellipse_block, args=(x, z, c, tik[i], tik[i + 1],points)) for i in
                  range(num_cpu)]  # 将每个block需要处理的点云区间发送到每个进程当中
     for res in multi_res:
         # xzlwp[tik[tik_b]:tik[tik_b + 1], :] = res.get()  # 将每个进程得到的结果分block的发送到容器当中
         res_block = res.get()
@@ -433,14 +433,119 @@
     j = 0  # 计数器
     for i in points_xz[b:e,:]:
         dis_ = E.find_distance2(i)  # 求单点
         dis_all_[j] = dis_["y"]  # 只要距离
         j += 1  # 刷新计数器
     return dis_all_
 
+def Find_dis_second_Ellipse_mp(xzc, xzlst, num_ps, C_un):
+    '单线程求点到椭圆的距离（精拟合）'
+    dis_all = np.empty(num_ps)  # 距离容器
+    tik = p0.cut_down(num_ps)  # 分块器
+    xzlstc = np.c_[xzlst, C_un]
+    for i in range(len(tik)-1):
+        start, end = tik[i], tik[i + 1]
+        dis_all[start:end] = find_dis_second_Ellipse_block(xzc, xzlstc, start, end)
+        print('求距离进度', i, '/', num_ps)
+    return dis_all
+
+def find_dis_second_Ellipse_block(xzc, xzlstc, b, e):
+    num_ = e - b  # 分块的点云数量
+    dis_all_ = np.empty(num_)  # 分块的距离容器
+    j = 0  # 计数器
+    for i in xzc[b:e, :]:
+        xzlst_ = xzlstc[xzlstc[:,-1]==i[-1],:-1]
+        # print(xzlst_)
+        E = Ellipse(xzlst_[0,0], xzlst_[0,1], xzlst_[0,2] * 2, xzlst_[0,3] * 2, xzlst_[0,4])  # 建立椭圆类
+        # print([i[0],i[1]])
+        dis_ = E.find_distance2(i[0:2])  # 求单点
+        dis_all_[j] = dis_["y"]  # 只要距离
+        '添加正负号'
+        sign_ = E_sign_single(i[:2],[xzlst_[0,0], xzlst_[0,1]],xzlst_[0,2],xzlst_[0,3],xzlst_[0,4])
+        dis_all_[j] = np.multiply(dis_all_[j], sign_)  # 融合距离和判断
+        j += 1  # 刷新计数器
+    return dis_all_
+
+def E_sign_single(points, Center, MA1, MA2,Theta):
+    '本函数只取得单点正负号'
+    x0, y0 = Center[0], Center[1]
+    a = MA1
+    b = MA2
+    phi = Theta
+    x, y = points[0], points[1]
+    cos_phi = np.cos(phi)
+    sin_phi = np.sin(phi)
+    X = x - x0
+    Y = y - y0
+    x_rot = cos_phi * X + sin_phi * Y
+    y_rot = -sin_phi * X + cos_phi * Y
+    distances = (x_rot / a) ** 2 + (y_rot / b) ** 2
+    # 获取正负号
+    distances -= 1
+    distances = np.sign(distances)
+    return distances
+
+def fit_ellipse_1(xyzic,xmax=3, xmin=-2.9, ymax=4.5, ymin=0.5):
+    '高精度拟合单个椭圆20240530'
+    # 1:限制坐标范围
+    xyzic_0 = xyzic[xyzic[:, 0] > xmin, :]
+    xyzic_0 = xyzic_0[xyzic_0[:, 0] < xmax, :]
+    xyzic_0 = xyzic_0[xyzic_0[:, 2] < ymax, :]
+    xyzic_0 = xyzic_0[xyzic_0[:, 2] > ymin, :]
+    # 2：第一次拟合
+    xz_0 = np.c_[xyzic_0[:, 0], xyzic_0[:, 2]]  # 对拟合点进行降维
+    reg = LsqEllipse().fit(xz_0)  # 输入二维点
+    center, width, height, phi = reg.as_parameters()  # 求解
+    print(f'center: {center[0]:.3f}, {center[1]:.3f}')
+    print(f'width: {width:.3f}')
+    print(f'height: {height:.3f}')
+    print(f'phi: {phi:.3f}')  # 打印
+    # 3：点到椭圆的距离
+    # arg_Ellipse = np.array([center[0], center[1], np.max([width, height]), np.min([width, height]), phi])  # 合并椭圆参数
+    # distances = ep.dis_ellipse(xyzic[:, 0], xyzic[:, 2], arg_Ellipse)  # 求点到椭圆的距离
+    dis = find_dis_mp(center[0], center[1], width, height, phi,xyzic[:,[0,2]])
+    print('mean',np.mean(dis))
+    print('std',np.std(dis))
+    # plt.hist(dis, bins=100)
+    # plt.show()
+    # p1.view_pointclouds(xyzic[:,:3],dis,'dis','jet')
+    td = 0.000
+    dis_td = dis[dis>=td]
+    xyzic_1 = xyzic[dis>=td,:]
+    td = 0.05
+    xyzic_1 = xyzic_1[dis_td <= td, :]
+    dis_td = dis_td[dis_td <= td]
+    # p1.view_pointclouds(xyzic_1[:, :3], dis_td, 'dis', 'jet')
+    # 4.第二次拟合
+    xz_0 = np.c_[xyzic_1[:, 0], xyzic_1[:, 2]]  # 对拟合点进行降维
+    reg = LsqEllipse().fit(xz_0)  # 输入二维点
+    center, width, height, phi = reg.as_parameters()  # 求解
+    print(f'center: {center[0]:.3f}, {center[1]:.3f}')
+    print(f'width: {width:.3f}')
+    print(f'height: {height:.3f}')
+    print(f'phi: {phi:.3f}')  # 打印
+    dis = find_dis_mp(center[0], center[1], width, height, phi,xyzic[:,[0,2]])
+    dis_min = find_dis_mp(center[0], center[1], width, height, phi,xyzic_1[:,[0,2]])
+    print('mean',np.mean(dis_min))
+    print('std',np.std(dis_min))
+    td = np.mean(dis_min)+1.4*np.std(dis_min)
+    xyzic_f = xyzic[np.abs(dis) <= td,:]
+    dis = dis[np.abs(dis) <= td]
+    # p1.view_pointclouds(xyzic_f[:, :3], dis, 'dis', 'jet')
+    # 5.最终参数
+    xz_0 = np.c_[xyzic_f[:, 0], xyzic_f[:, 2]]  # 对拟合点进行降维
+    reg = LsqEllipse().fit(xz_0)  # 输入二维点
+    center, width, height, phi = reg.as_parameters()  # 求解
+    print(f'center: {center[0]:.3f}, {center[1]:.3f}')
+    print(f'width: {width:.3f}')
+    print(f'height: {height:.3f}')
+    print(f'phi: {phi:.3f}')  # 打印
+    return np.array([center[0], center[1], width, height, phi]),xyzic_f  # 返回椭圆参数和在椭圆上的点
+
+
 if __name__ == '__main__':
     '椭圆拟合例子 Ellipse fitting example'
     # arg_Ellipse = fitellipse(xy) # size(xy) = [n,2]
     '点到椭圆例子Example of point to ellipse'
     eps = np.array([0, 0, 1, .5, np.pi / 6])  # Ellipse parameter
     # Plane point coordinates
     x = np.array([0.0,10.2,7.98760,1.198760,1.198730,0.198760,-4.999760])
```

### Comparing `zelas-1.3.240507/zelas/Multispectral.py` & `zelas-1.4.240530/zelas/Multispectral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #coding=utf-8
-#import zelas.RedundancyElimination as p1  # 第一篇论文的库
 import numpy as np  # numpy库
 import math  # 添加数学库
 import matplotlib.pyplot as plt  # 显示库
 import open3d as o3d  # open3d库
 from mpl_toolkits.mplot3d import Axes3D  # 空间三维画图
 import scipy.spatial as spt  # 求凸壳用的库
 from shapely.geometry import Polygon  # 求凸壳面积用的库
@@ -19,15 +18,15 @@
     polygon = xy[ID, :]  # 求凸壳数组
     area = Polygon(polygon).area  # 求多边形面积
     return area
 
 # 求每个点所占的平均面积
 def mean2Ddensity(num, Area):
     density = math.sqrt(Area/num)
-    print('点云平均密度为:', density)
+    print('平面平均点间距为:', density)
     return density
 
 # https://www.cnblogs.com/wt714/p/12545129.html
 # 对强度值数集进行归一化
 def normalization(intensity, threshold=1):
     max_i = max(intensity)
     min_i = min(intensity)
```

### Comparing `zelas-1.3.240507/zelas/RedundancyElimination.py` & `zelas-1.4.240530/zelas/RedundancyElimination.py`

 * *Files identical despite different names*

### Comparing `zelas-1.3.240507/zelas/TheHeartOfTheMilitaryGod.py` & `zelas-1.4.240530/zelas/TheHeartOfTheMilitaryGod.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import division
 # 这是一个关于私人用途的代码原文件库
 import numpy as np
 from numpy import *
 import sys  # maxint
 import matplotlib.pyplot as plt
 import pyvista as pv
-import matplotlib.cm as cm
+import polars as pl
+from PIL import Image
 
 
 # C-均值聚类
 def FCM_train(X, n_centers, m, max_iter=100, theta=1e-5, seed=0):
     rng = np.random.RandomState(seed)
     N, D = np.shape(X)
     # 随机初始化关系矩阵
@@ -206,13 +207,33 @@
     j = 0
     for i in colormaps:
         print('colormap', j, ':', i)
         j += 1
     return colormaps
 
 
-def view_pointclouds(xyz,i,i_name='intensity',colormap='gray'):
+def view_pointclouds(xyz,i,i_name='intensity',colormap='gray',eye=False):
     '基于pyvista显示点云'
     points = pv.PolyData(xyz)  # 建立pv类
     points[i_name] = i  # 将特征填入类
     # 显示点云
-    points.plot(eye_dome_lighting=True,cmap=colormap)
+    points.plot(eye_dome_lighting=eye,cmap=colormap)
+
+def ReadByPolars(path_file,sep=' '):
+    '通过polars读取txt点云'
+    xyzi = np.array(pl.read_csv(path_file, has_header=False, separator=sep))  # 读取点云
+    return xyzi
+
+
+def resize_image(input_image_path, output_image_path, new_width, new_height):
+    '''
+    对图像进行分辨率的修改（https://blog.csdn.net/m0_59799878/article/details/131571082）
+    :param input_image_path:读取图像路径
+    :param output_image_path:输出图像路径
+    :param new_width:输出图像分辨率宽
+    :param new_height:输出图像分辨率高
+    :return:
+    '''
+    image = Image.open(input_image_path)
+    resized_image = image.resize((new_width, new_height))
+    resized_image.save(output_image_path)
+
```

### Comparing `zelas-1.3.240507/zelas/ransac.py` & `zelas-1.4.240530/zelas/ransac.py`

 * *Files identical despite different names*

### Comparing `zelas-1.3.240507/zelas/setup.py` & `zelas-1.4.240530/zelas/setup.py`

 * *Files identical despite different names*

### Comparing `zelas-1.3.240507/zelas/shield.py` & `zelas-1.4.240530/zelas/shield.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python
 # coding=utf-8
 import numpy as np
-from matplotlib import pyplot as plt
-from matplotlib.patches import Circle
 import math
 import multiprocessing as mp  # 添加多进程（并行计算）库
 import pyransac3d as pyrsc
 import zelas.Multispectral as p1  # 添加自己的库
 import plotly.graph_objects as go  # 添加其他显示库
 import zelas.voxel as vl  # 添加体素类
 import zelas.ransac as rs
 import zelas.Ellipse as ep
+from ellipse import LsqEllipse  # 添加椭圆拟合算法
+from tqdm import tqdm
 
 
 def random_partition(n, n_data):
     """return n random rows of data and the other len(data) - n rows"""
     all_idxs = np.arange(n_data)  # 获取n_data下标索引
     np.random.shuffle(all_idxs)  # 打乱下标索引
     idxs1 = all_idxs[:n]
@@ -1971,12 +1971,137 @@
                 pass
         # 遍历Y，以公式查看O的范围，然后根据点的多少确定是否进行补点（最好建立一个O的左右范围点数量横切面直方图）
         # 进行补点
         # 返回到F_all
     return F_all
 
 
-def Fitellipse(xyz):
+def Fitellipse(xyzic, xmax=3, xmin=-2.9, ymax=4.5, ymin=0.5):
     '椭圆拟合'
-    EllipseParameter = np.empty(3)  # 存储椭圆的圆心、长半轴、短半轴
+    '1.限制坐标范围'
+    xyzic_0 = xyzic[xyzic[:, 0] > xmin, :]
+    xyzic_0 = xyzic_0[xyzic_0[:, 0] < xmax, :]
+    xyzic_0 = xyzic_0[xyzic_0[:, 2] < ymax, :]
+    xyzic_0 = xyzic_0[xyzic_0[:, 2] > ymin, :]
+    '2.整体拟合'
+    xz_0 = np.c_[xyzic_0[:, 0], xyzic_0[:, 2]]  # 对拟合点进行降维
+    reg = LsqEllipse().fit(xz_0)  # 输入二维点
+    center, width, height, phi = reg.as_parameters()  # 求解
+    print(f'center: {center[0]:.3f}, {center[1]:.3f}')  # 椭圆点中心
+    print(f'width: {width:.3f}')  # 椭圆长半轴
+    print(f'height: {height:.3f}')  # 椭圆短半轴
+    print(f'phi: {phi:.3f}')  # 椭圆旋转角
+    '3.求点到椭圆的距离'
+    arg_Ellipse = np.array([center[0], center[1], np.max([width, height]), np.min([width, height]), phi])  # 合并椭圆参数
+    distances = ep.dis_ellipse(xyzic[:, 0], xyzic[:, 2], arg_Ellipse)  # 求点到椭圆的距离
+    distances = np.nan_to_num(distances, nan=0)  # 将空值转换为0
+    '4.求均值和标准差'
+    dis_mean = np.mean(distances)
+    dis_std = np.std(distances)
+    print(dis_std, dis_mean)
+    m = -0.25  # 标准差倍数
+    threshold = dis_mean + dis_std * m  # 阈值
+    print(threshold)
+    xyzic_0 = xyzic[distances < threshold, :]
+    '5.第二次拟合'
+    index, outdex, xzlwp, dis = fit_Ellipse_starmap(xyzic_0[:, 0], xyzic_0[:, 2], xyzic_0[:, -1], xyzic)  # 求每个圆环的参数
+    xyzic_0 = xyzic[index, :]
+    return
+
+def fit_Ellipse_starmap(x, z, c, points,num_cpu=mp.cpu_count(), dr=0.05):
+    '异步并行计算拟合椭圆 Parallel computing for fitting ellipses'
+    c_un = np.unique(c)  # 所有序列数
+    num_c = len(c_un)  # 圆环数
+    xzlwp = np.empty([num_c, 5])  # 新建一个存储每个椭圆参数的容器
+    dis_all = np.zeros(len(points))  # 距离容器
+    # 并行计算加速准备 #Accelerated preparation for parallel computing
+    pool = mp.Pool(processes=num_cpu)  # 开启多进程池，数量为cpu
+    # tik = cut_down(num_c)  # 分块器
+    # tik2 = p0.cut_down(len(points))  # 分块器
+    j = 0  # 分块输出计时器
+    # 并行计算每个圆环 Parallel computing for each torus
+    # 并行计算
+    multi_res = pool.starmap_async(fit_Ellipse_single, ((x[c==c_un[i]], z[c==c_un[i]], c_un[i], points) for i in
+                 tqdm(range(num_c),desc='分配任务拟合单个椭圆参数',unit='个cross-section',total=num_c)))
+    # multi_res = [pool.starmap_async(fit_Ellipse_single, (x[c==c[i]].reshape(1,-1), z[c==c[i]].reshape(1,-1), c_un[i], points)) for i in
+    #              tqdm(range(num_c))]  # 将每个block需要处理的点云区间发送到每个进程当中
+    for res in tqdm(multi_res.get(), total=num_c, desc='导出单个椭圆参数', unit='个cross-section'):
+    # for res in tqdm(multi_res):
+        # xzlwp[tik[tik_b]:tik[tik_b + 1], :] = res.get()  # 将每个进程得到的结果分block的发送到容器当中
+        # res_block = res.get()
+        dis_all += res[0]
+        # dis_all += res_block[0]  # 距离累加
+        xzlwp[j, :] = res[1]  # 拟合值回归
+        j += 1
+    pool.close()  # 禁止进程池再接收任务  #Prohibit process pools from receiving tasks again
+    pool.join()  # 当所有进程全部计算完毕后，退出并行计算  #After all processes have completed their calculations, exit parallel computing
+    # 下标
+    index = dis_all <= dr
+    outdex = dis_all > dr
+    # RMSE
+    dis_index = dis_all[dis_all <= dr]  # 在椭圆上的距离集合
+    RMSE = np.sqrt(np.sum(dis_index**2)/len(dis_index))
+    print('RMSE:', RMSE)
+    print('保留点比例：',len(dis_index)/len(points))
+    return index, outdex, xzlwp, dis_all
 
-    return EllipseParameter
+def fit_Ellipse_single(x, z, c_, points):
+    '单环求椭圆参数 Calculating Ellipse Parameters by Blocks'
+    # num_ = e-b
+    # c_un = np.unique(c)
+    dis_ = np.zeros(len(points))
+    # dis_ = np.zeros(num_)
+    xzlwp = np.empty([5])
+    # j = 0  # 循环计数器 cycle counter
+    # for c1 in c_un[b:e]:
+    # x_c1 = x[c == c1]
+    # z_c1 = z[c == c1]  # 提取单环的全部点云二维坐标  Extract all point cloud 2D coordinates of a single ring
+    xz_ = np.vstack([x, z]).T
+    reg = LsqEllipse().fit(xz_)  # 输入二维点  Enter 2D points
+    center, width, height, phi = reg.as_parameters()  # 求解 solve
+    xzlwp[0] = center[0]
+    xzlwp[1] = center[1]
+    xzlwp[2] = np.max([width, height])
+    xzlwp[3] = np.min([width, height])
+    xzlwp[4] = phi
+    dis_[points[:, 4] == c_] = ep.dis_ellipse(points[points[:, 4]==c_, 0], points[points[:, 4]==c_, 2], xzlwp)
+    dis_ = np.nan_to_num(dis_, nan=0)  # 若距离为nan，则转换为1
+    return dis_,xzlwp
+
+def get_dis_θ(xz,xyzic):
+    '求单截面点云相邻点的角度差240530'
+    # num = len(xyzic)  # 点云数量
+    angle = np.arctan2(xyzic[:, 0]-xz[0], xyzic[:, 2]-xz[1]) * 180 / np.pi  # 点云求角度值
+    diff = np.diff(angle)  # 计算相邻角度差值
+    # plt.hist(diff, bins=3600)
+    # plt.show()
+    print('mean',np.mean(diff))
+    print('std',np.std(diff))
+    condition = (np.abs(diff) >= 0.03) & (np.abs(diff) <= 0.08)
+    new_xyzic = xyzic[1:][condition]
+    return new_xyzic,diff[condition]  # 符合条件的点云，相邻点角度差值
+
+def get_wrong(xzlwp_l,xzlwp_r,xyzic_l,xyzic_r,n=5000):
+    '基于实际变化的全局错台量分析20240530'
+    x0_m = np.mean([xzlwp_l[0], xzlwp_r[0]])
+    z0_m = np.mean([xzlwp_l[2], xzlwp_r[2]])  # 圆心轴
+    angle_l = np.arctan2(xyzic_l[:, 0] - x0_m, xyzic_l[:, 2] - z0_m) * 180 / np.pi  # 点云求角度值
+    angle_r = np.arctan2(xyzic_r[:, 0] - x0_m, xyzic_r[:, 2] - z0_m) * 180 / np.pi  # 点云求角度值
+    single_a = np.pi * 2 / n  # 求每个块的过渡
+    belong_l = np.floor(angle_l / single_a)
+    belong_r = np.floor(angle_r / single_a)  # 属于区间
+    b_l_un = np.unique(belong_l)
+    b_r_un = np.unique(belong_r)  # 排序
+    b_common = np.intersect1d(b_l_un, b_r_un)  # 共同区间
+    print('共同区间数量',len(b_common))
+    w_all = np.zeros([len(b_common)])  # 求错容器
+    j = 0
+    for i in b_common:
+        xyz_l_ = np.mean(xyzic_l[belong_l == i, :3], axis=0)
+        # print(xyz_l_)
+        xyz_r_ = np.mean(xyzic_r[belong_r == i, :3], axis=0)
+        # print(xyz_r_)
+        w_all[j] = np.linalg.norm(np.array([xyz_l_[0],xyz_l_[2]])-np.array([xyz_r_[0],xyz_r_[2]]))
+        print(w_all[j])
+        j += 1
+    # w_all = w_all[w_all <= 0.01]
+    return np.max(w_all)
```

### Comparing `zelas-1.3.240507/zelas/voxel.py` & `zelas-1.4.240530/zelas/voxel.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,30 +64,29 @@
             self.voxel_values[int(self.points_local[i, 0]), int(self.points_local[i, 1]), int(self.points_local[i, 2])] = values[i]  # 体素赋值
         del values  # 删除
         self.points_local = self.points_local.astype(int)  # 将点云位置进行整数化
         self.points_local_un = np.unique(self.points_local, axis=0)  # 有值体素位置精简化
         self.num_voxel = len(self.points_local_un)  # 有值体素数量
         print('体素赋值已完成')
         id_point, self.index = np.unique(self.points_local, axis=0, return_index=True)  # 体素位置升序排序按照（x,y,z），并返回下标
-        # id_point, _ = np.unique(self.points_local, axis=0, return_index=True)  # 体素位置升序排序按照（x,y,z），并返回下标
         self.num_voxel = len(id_point)  # 返回有效的体元数量
-        del id_point
+        # del id_point
         '''
         self.voxel_nei = nei_26_mp(self.points_local, self.VoxelLength, self.voxel_values)  # 寻找26邻域位置
         print('体素26邻域搜索已完成')
         return self.voxel_nei
         '''
 
     def Voxel2Pixel(self):
         '计算体素转像素（值为最低点高程，矩阵思想）'
         # 点云重新赋值
         self.voxel_values = np.ones(self.VoxelLength, dtype=np.float32)*10000
         self.P2V(self.points_local[:,2])  # 将高程值附给体素
         pixel_values_min = np.argmin(self.voxel_values,axis=2)
-        self.pixel_min_un = np.empty([self.VoxelLength[0]*self.VoxelLength[1],3])
+        self.pixel_min_un = np.empty([self.VoxelLength[0]*self.VoxelLength[1],3])  # 二维像素数组，值为高程最低值
         k = 0
         for i in range(self.VoxelLength[0]):
             for j in range(self.VoxelLength[1]):
                 self.pixel_min_un[k,0] = i
                 self.pixel_min_un[k,1] = j
                 self.pixel_min_un[k,2] = pixel_values_min[i,j]
                 k += 1
@@ -339,19 +338,19 @@
     area = Polygon(polygon).area  # 求多边形面积
     return area
 
 
 def nei_26_mp(id_point, num_v, binary, cpu=mp.cpu_count()):
     '''
     并行计算体素的26邻域有值体素函数
-    :param id_point: 点云所在体素位置数组
-    :param num_v: 体素长宽高
-    :param binary: 三维体素
-    :param cpu: 并行计算分块数，默认为cpu的最大物理线程数
-    :return: 每个体素的周围26邻域中的有值体素位置
+    :param id_point: 点云所在体素位置数组 numpy[数量，3]
+    :param num_v: 体素长宽高 numpy[1,3]
+    :param binary: 三维体素 voxel.voxel_values numpy[长，宽，高]
+    :param cpu: 并行计算分块数，默认为cpu的最大物理线程数 Int
+    :return: 每个体素的周围26邻域中的有值体素位置 嵌套数组，参考voxel.voxel_nei
     '''
     # 函数准备
     num = len(id_point)
     tik = cut_down(num, cpu)  # 计算每个块的起止点
     a = [0 for x in range(num)]
     j = 0  # 分块输出计数器
     pool = mp.Pool(processes=cpu)  # 开启多进程池，数量为cpu
@@ -898,51 +897,57 @@
     for res in multi_res:
         belong[tik[tik_]:tik[tik_ + 1]] = res.get()
         tik_ += 1
     pool.close()  # 禁止进程池再接收任务
     pool.join()  # 当所有进程全部计算完毕后，退出并行计算
     return belong
 
+def XYZ2ρθY_1(xyzic, xzrc, n=3000):
+    '240522单点笛卡尔坐标系转成圆柱体坐标系'
+    xzr = xzrc[xzrc[:, -1] == xyzic[-1], :3]  # 圆心位置
+    R2 = (xyzic[0] - xzr[0, 0]) ** 2 + (xyzic[2] - xzr[0, 1]) ** 2  # 点到圆心的距离
+    ρ = np.sqrt(R2)
+    y = xyzic[1]
+    # 求角度
+    # d_yx_[j, 0] = (xzc_point[i, 1] - xz_c[0, 1])
+    # d_yx_[j, 1] = (xzc_point[i, 0] - xz_c[0, 0])
+    d_z = xyzic[2] - xzr[0, 1]
+    d_x = xyzic[0] - xzr[0, 0]
+    angle = np.arctan2(d_z, d_x)  # 求反正切值
+    # 将角度分解
+    single_a = np.pi * 2 / n  # 求每个块的过渡
+    θ = np.floor(angle / single_a)  # 点云归属标签赋值
+    ρθY = np.array([ρ,θ,y])
+    return ρθY
 
 def XYZ2ρθY(xyzic, xzrc, n=3000):
     '笛卡尔坐标系转成圆柱体坐标系'
     Y = xyzic[:, 1]  # y轴坐标为起点
     c = xzrc[:, -1]  # 所有圆环名
     ρ = np.empty([len(xyzic)])  # 新建一个存储点云p的容器
     '准备添加并行化'
     for i in range(len(xyzic)):
         xyz_ = xyzic[i, :3]  # 当前点的空间位置
         c_i = xyzic[i, -1]  # 当前点圆环名
         xzr_ = xzrc[c == c_i, :3]  # 圆心位置
         R2 = (xyz_[0] - xzr_[0, 0]) ** 2 + (xyz_[2] - xzr_[0, 1]) ** 2  # 点到圆心的距离
         # dis[i] = np.abs(R2 - xzr_[0, -1] ** 2)
         ρ[i] = np.sqrt(R2)  # 点云到中轴线的距离
-
     θ = np.empty([len(xyzic)])  # 新建一个存储点云θ的容器
     # 求角度
     xzc_point = np.c_[xyzic[:, 0], xyzic[:, 2], xyzic[:, -1]]
     xzc_c = np.c_[xzrc[:, :2], xzrc[:, -1]]
     θ = Split_ring_mp(xzc_point, xzc_c, n=n)
     ρθY = np.c_[ρ, θ, Y]
     # 归一化
     θ_min = np.min(ρθY[:, 1])  # 角度向量化后的最小值
     ρθY[:, 1] = ρθY[:, 1] - θ_min  # 使所有的角度都大于0
     Y_min = np.min(ρθY[:, -1])  # Y轴后的最小值
     ρθY[:, -1] = ρθY[:, -1] - Y_min  # Y轴归0
-    return ρθY
-
-
-def before_voxel_ρθY(xyzic, xzrc):
-    '极坐标体素化前的标准化处理'
-    ρθY = XYZ2ρθY(xyzic, xzrc)  # 合并圆柱位置和点云属性
-    # θ_min = np.min(ρθY[:, 1])  # 角度向量化后的最小值
-    # ρθY[:, 1] = ρθY[:, 1] - θ_min  # 使所有的角度都大于0
-    # Y_min = np.min(ρθY[:, -1])  # Y轴后的最小值
-    # ρθY[:, -1] = ρθY[:, -1] - Y_min  # Y轴归0
-    return ρθY  # 返回每个点云的极坐标
+    return ρθY,θ_min,Y_min
 
 
 class voxel_ρθY:
     '建立空间圆柱坐标系体素'
     def __init__(self, ρθY, pixel=np.array([0.004, 1, 0.004])):
         '建立构造函数'
         # 输入圆柱坐标以及默认的体元分辨率
@@ -951,14 +956,15 @@
         self.VoxelLengthDigit = None  # 体元数量位数
         self.VoxelLength = None  # 体素长宽高容器
         self.pixel = pixel  # 体素的点云分辨率
         self.voxel_values = None  # 体素特征值
         self.num = len(ρθY)  # 点云数量
         self.ρθY = ρθY  # 将矫正后的坐标放入进去（记得之前要矫正）
         self.SpaceBoundary = self.ρθY.max(axis=0)  # 求点云的最大边界
+        # self.SpaceBoundary = np.array([self.ρθY.max(axis=0), self.ρθY.min(axis=0)])  # 点云的边界
         self.find_VoxelLength()  # 求体素长宽高
         self.points_local = np.empty([self.num, 3])  # 每个点云所在的体素位置
 
     def find_VoxelLength(self):
         '求体素体积'
         self.VoxelLength = np.int16(np.ceil(self.SpaceBoundary / self.pixel) + 1)  # 求体素的长宽高
         print('体素的长宽高为', self.VoxelLength)
@@ -1040,24 +1046,31 @@
         grid = pv.UnstructuredGrid({pv.CellType.HEXAHEDRON: cells_hex}, voxel_8ps_2D)  # 建立体素网格
         if color == 0:
             color = np.c_[self.points_local_un_value, self.points_local_un_value, self.points_local_un_value]
         grid.plot(scalars=color, show_edges=True, cmap=cmap)  # 显示体素
         # grid.save('grid.ply')
         return
 
+    def θy2P(self,θy):
+        '体素θy转点云'
+        input_21 = θy[:, 0] + θy[:, 1] * (10 ** (self.VoxelLengthDigit[-1] * (-1)))
+        base_21 = self.points_local[:, 1] + self.points_local[:, 2] * (10 ** (self.VoxelLengthDigit[-1] * (-1)))
+        points_index = np.isin(base_21, input_21)  # 提取点云的下标 by:Zelas
+        return points_index
+
     def V2P(self, v_local_un):
         '体素转点云'
         lwd_321 = v_local_un[:, 0] * (10 ** self.VoxelLengthDigit[-2]) + v_local_un[:, 1] + v_local_un[:, 2] * (10 ** (self.VoxelLengthDigit[-1] * (-1)))
         p_lwd_321 = self.points_local[:, 0] * (10 ** self.VoxelLengthDigit[-2]) + self.points_local[:, 1] + self.points_local[:, 2] * (10 ** (self.VoxelLengthDigit[-1] * (-1)))
         points_index = np.isin(p_lwd_321, lwd_321)  # 提取点云的下标 by:Zelas
         return points_index
 
 
 def watch_o3d_voxel(xyzrgb, size=0.05):
-    '显示体素（注意rgb的值域∈【0，1】）'
+    '（已弃用）显示体素（注意rgb的值域∈【0，1】）'
     xyz_o3d = o3d.geometry.PointCloud()  # 建立open3d点云类容器
     xyz_o3d.points = o3d.utility.Vector3dVector(xyzrgb[:, :3])  # 赋予点坐标
     xyz_o3d.colors = o3d.utility.Vector3dVector(xyzrgb[:, 3:])  # 赋予点颜色
     voxel_grid = o3d.geometry.VoxelGrid.create_from_point_cloud(xyz_o3d, voxel_size=size)  # 体素化
     o3d.visualization.draw_geometries([voxel_grid])  # 显示体素
```

