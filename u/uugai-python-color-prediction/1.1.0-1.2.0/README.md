# Comparing `tmp/uugai_python_color_prediction-1.1.0.tar.gz` & `tmp/uugai_python_color_prediction-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uugai_python_color_prediction-1.1.0.tar", last modified: Thu May 30 10:42:38 2024, max compression
+gzip compressed data, was "uugai_python_color_prediction-1.2.0.tar", last modified: Thu May 30 11:21:10 2024, max compression
```

## Comparing `uugai_python_color_prediction-1.1.0.tar` & `uugai_python_color_prediction-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:42:38.694785 uugai_python_color_prediction-1.1.0/
--rw-r--r--   0 glenn      (502) staff       (20)     4014 2024-05-30 10:42:38.694517 uugai_python_color_prediction-1.1.0/PKG-INFO
--rw-r--r--   0 glenn      (502) staff       (20)     3717 2024-05-30 09:44:37.000000 uugai_python_color_prediction-1.1.0/README.md
--rw-r--r--   0 glenn      (502) staff       (20)       38 2024-05-30 10:42:38.694888 uugai_python_color_prediction-1.1.0/setup.cfg
--rw-r--r--   0 glenn      (502) staff       (20)      497 2024-05-30 10:41:38.000000 uugai_python_color_prediction-1.1.0/setup.py
-drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:42:38.692375 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction/
--rw-r--r--   0 glenn      (502) staff       (20)        0 2024-05-30 09:40:23.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction/__init__.py
--rw-r--r--   0 glenn      (502) staff       (20)     9273 2024-05-30 08:51:51.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction/uug_ai_python_color_prediction.py
-drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:42:38.694125 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/
--rw-r--r--   0 glenn      (502) staff       (20)     4014 2024-05-30 10:42:38.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/PKG-INFO
--rw-r--r--   0 glenn      (502) staff       (20)      388 2024-05-30 10:42:38.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/SOURCES.txt
--rw-r--r--   0 glenn      (502) staff       (20)        1 2024-05-30 10:42:38.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/dependency_links.txt
--rw-r--r--   0 glenn      (502) staff       (20)      314 2024-05-30 10:42:38.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/requires.txt
--rw-r--r--   0 glenn      (502) staff       (20)       30 2024-05-30 10:42:38.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/top_level.txt
+drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 11:21:10.476981 uugai_python_color_prediction-1.2.0/
+-rw-r--r--   0 glenn      (502) staff       (20)     4088 2024-05-30 11:21:10.476666 uugai_python_color_prediction-1.2.0/PKG-INFO
+-rw-r--r--   0 glenn      (502) staff       (20)     3791 2024-05-30 11:19:14.000000 uugai_python_color_prediction-1.2.0/README.md
+-rw-r--r--   0 glenn      (502) staff       (20)       38 2024-05-30 11:21:10.477111 uugai_python_color_prediction-1.2.0/setup.cfg
+-rw-r--r--   0 glenn      (502) staff       (20)      497 2024-05-30 11:20:40.000000 uugai_python_color_prediction-1.2.0/setup.py
+drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 11:21:10.473816 uugai_python_color_prediction-1.2.0/uugai_python_color_prediction/
+-rw-r--r--   0 glenn      (502) staff       (20)        0 2024-05-30 09:40:23.000000 uugai_python_color_prediction-1.2.0/uugai_python_color_prediction/__init__.py
+-rw-r--r--   0 glenn      (502) staff       (20)     9854 2024-05-30 11:19:11.000000 uugai_python_color_prediction-1.2.0/uugai_python_color_prediction/uug_ai_python_color_prediction.py
+drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 11:21:10.476124 uugai_python_color_prediction-1.2.0/uugai_python_color_prediction.egg-info/
+-rw-r--r--   0 glenn      (502) staff       (20)     4088 2024-05-30 11:21:10.000000 uugai_python_color_prediction-1.2.0/uugai_python_color_prediction.egg-info/PKG-INFO
+-rw-r--r--   0 glenn      (502) staff       (20)      388 2024-05-30 11:21:10.000000 uugai_python_color_prediction-1.2.0/uugai_python_color_prediction.egg-info/SOURCES.txt
+-rw-r--r--   0 glenn      (502) staff       (20)        1 2024-05-30 11:21:10.000000 uugai_python_color_prediction-1.2.0/uugai_python_color_prediction.egg-info/dependency_links.txt
+-rw-r--r--   0 glenn      (502) staff       (20)      314 2024-05-30 11:21:10.000000 uugai_python_color_prediction-1.2.0/uugai_python_color_prediction.egg-info/requires.txt
+-rw-r--r--   0 glenn      (502) staff       (20)       30 2024-05-30 11:21:10.000000 uugai_python_color_prediction-1.2.0/uugai_python_color_prediction.egg-info/top_level.txt
```

### Comparing `uugai_python_color_prediction-1.1.0/PKG-INFO` & `uugai_python_color_prediction-1.2.0/uugai_python_color_prediction.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: uugai_python_color_prediction
-Version: 1.1.0
+Name: uugai-python-color-prediction
+Version: 1.2.0
 Summary: Color prediction Python library used to find the main colors in an image.
 Home-page: UNKNOWN
 Author: uug.ai
 Author-email: support@uug.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 This project aims to predict the color of an image using Python. It utilizes machine learning algorithms, specifically k-means clustering, to analyze the pixel values of an image and predict the dominant color.
 
 K-means clustering is a popular unsupervised learning algorithm used for clustering data points into groups. In the context of color prediction, k-means clustering is used to group similar pixel values together, allowing us to identify the dominant color in an image. The algorithm works by iteratively assigning each pixel to the cluster with the closest centroid, and then updating the centroids based on the new assignments. This process continues until the centroids no longer change significantly. By applying k-means clustering to the pixel values of an image, we can identify the cluster centroids, which represent the dominant colors. To use this project, simply follow the installation instructions below. 
 
 ## Installation TODO
 
 To get started with the Python color prediction function, simply install the package using pip and follow the provided documentation for configuration and usage instructions: `pip install uugai_python_color_prediction`
-To import the function into your own python file, use: `from uugai_python_color_prediction import find_main_colors`
+To import the function into your own python file, use: `from uugai_python_color_prediction import ColorPrediction`
 
 ## Usage
 The find_main_colors function is used to predict the dominant colors of an image. It takes several parameters:
 
 * image: The input image for color prediction, using `cv2.imread(IMAGE_PATH)`.
 * min_clusters and max_clusters: The minimum and maximum number of clusters to use for k-means clustering.
 * downsample_factor: A factor used to downsample the image before color prediction. Default value is 0.95.
@@ -29,21 +29,23 @@
 * verbose: A boolean value indicating whether to print verbose output during color prediction. Default value is False.
 * plot: A boolean value indicating whether to plot the color prediction results. Default value is False.
 
 To use the find_main_colors function, simply pass the required parameters and call the function. The function will return the predicted dominant colors of the image, optimal number of centroids ± the elbow offset and the percentages of pixels belonging to that centroid.
 
 ## Usage example
 ```Python
+from uugai_python_color_prediction import ColorPrediction
+
 IMAGE_PATH = 'python_color_prediction/data/flowers.jpeg'
 
 # Read the image
 image = cv2.imread(IMAGE_PATH)
 
 # Call the elbow_method function
-optimal_centroids, optimal_k, optimal_percentages = find_main_colors(image, min_clusters=1, max_clusters=10, downsample_factor=0.95, increase_elbow=0, verbose=True, plot=True)
+optimal_centroids, optimal_k, optimal_percentages = ColorPrediction.find_main_colors(image, min_clusters=1, max_clusters=10, downsample_factor=0.95, increase_elbow=0, verbose=True, plot=True)
 ```
 
 This would result in the following output, with `verbose = True`:
 
 ```
 Calculating for k =  1
 Calculating for k =  2
```

### Comparing `uugai_python_color_prediction-1.1.0/README.md` & `uugai_python_color_prediction-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This project aims to predict the color of an image using Python. It utilizes machine learning algorithms, specifically k-means clustering, to analyze the pixel values of an image and predict the dominant color.
 
 K-means clustering is a popular unsupervised learning algorithm used for clustering data points into groups. In the context of color prediction, k-means clustering is used to group similar pixel values together, allowing us to identify the dominant color in an image. The algorithm works by iteratively assigning each pixel to the cluster with the closest centroid, and then updating the centroids based on the new assignments. This process continues until the centroids no longer change significantly. By applying k-means clustering to the pixel values of an image, we can identify the cluster centroids, which represent the dominant colors. To use this project, simply follow the installation instructions below. 
 
 ## Installation TODO
 
 To get started with the Python color prediction function, simply install the package using pip and follow the provided documentation for configuration and usage instructions: `pip install uugai_python_color_prediction`
-To import the function into your own python file, use: `from uugai_python_color_prediction import find_main_colors`
+To import the function into your own python file, use: `from uugai_python_color_prediction import ColorPrediction`
 
 ## Usage
 The find_main_colors function is used to predict the dominant colors of an image. It takes several parameters:
 
 * image: The input image for color prediction, using `cv2.imread(IMAGE_PATH)`.
 * min_clusters and max_clusters: The minimum and maximum number of clusters to use for k-means clustering.
 * downsample_factor: A factor used to downsample the image before color prediction. Default value is 0.95.
@@ -18,21 +18,23 @@
 * verbose: A boolean value indicating whether to print verbose output during color prediction. Default value is False.
 * plot: A boolean value indicating whether to plot the color prediction results. Default value is False.
 
 To use the find_main_colors function, simply pass the required parameters and call the function. The function will return the predicted dominant colors of the image, optimal number of centroids ± the elbow offset and the percentages of pixels belonging to that centroid.
 
 ## Usage example
 ```Python
+from uugai_python_color_prediction import ColorPrediction
+
 IMAGE_PATH = 'python_color_prediction/data/flowers.jpeg'
 
 # Read the image
 image = cv2.imread(IMAGE_PATH)
 
 # Call the elbow_method function
-optimal_centroids, optimal_k, optimal_percentages = find_main_colors(image, min_clusters=1, max_clusters=10, downsample_factor=0.95, increase_elbow=0, verbose=True, plot=True)
+optimal_centroids, optimal_k, optimal_percentages = ColorPrediction.find_main_colors(image, min_clusters=1, max_clusters=10, downsample_factor=0.95, increase_elbow=0, verbose=True, plot=True)
 ```
 
 This would result in the following output, with `verbose = True`:
 
 ```
 Calculating for k =  1
 Calculating for k =  2
```

### Comparing `uugai_python_color_prediction-1.1.0/uugai_python_color_prediction/uug_ai_python_color_prediction.py` & `uugai_python_color_prediction-1.2.0/uugai_python_color_prediction/uug_ai_python_color_prediction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,257 +1,251 @@
 import cv2
 import numpy as np
 import matplotlib.pyplot as plt
 from kneed import KneeLocator
 from sklearn.cluster import KMeans
 
 
+IMAGE_PATH = 'uugai_python_color_prediction/data/flowers.jpeg'
 
-IMAGE_PATH = 'python_color_prediction/data/flowers.jpeg'
+class ColorPrediction:
+    def __init__(self):
+        pass
 
 
-
-def find_main_colors(image, min_clusters, max_clusters, downsample_factor = 0.95, increase_elbow = 0, verbose=False, plot=False):
-    """Function to find the optimal number of clusters using the elbow method.
-    
-    Parameters:
-    ----------
-    data: numpy array
-        The data points to cluster.
-    min_clusters: int
-        The minimum number of clusters to consider.
-    max_clusters: int
-        The maximum number of clusters to consider.
-    downsample_factor: float
-        The factor to downsample the image by.
-    increase_elbow: int
-        The number of clusters to increase the elbow point by.
-    verbose: bool
-        Whether to print the optimal values.
-    plot: bool
-        Whether to plot the elbow plot and the optimal centroids.
-
-    """
-
-    def find_elbow_point(inertias, min_k, max_k):
-        """ Function to find the elbow point in the inertia plot.
-
+    def find_main_colors(image, min_clusters, max_clusters, downsample_factor = 0.95, increase_elbow = 0, verbose=False, plot=False):
+        """Function to find the optimal number of clusters using the elbow method.
+        
         Parameters:
         ----------
-        inertias: list
-            The list of inertia values for different k values.
-        min_k: int  
+        data: numpy array
+            The data points to cluster.
+        min_clusters: int
             The minimum number of clusters to consider.
-        max_k: int
+        max_clusters: int
             The maximum number of clusters to consider.
-        
-        """
+        downsample_factor: float
+            The factor to downsample the image by.
+        increase_elbow: int
+            The number of clusters to increase the elbow point by.
+        verbose: bool
+            Whether to print the optimal values.
+        plot: bool
+            Whether to plot the elbow plot and the optimal centroids.
 
-        # Generate the range of k values
-        K = range(min_k, max_k)
+        """
 
-        kn = KneeLocator(K, inertias, curve='convex', direction='decreasing')
-        return kn.elbow  
+        def find_elbow_point(inertias, min_k, max_k):
+            """ Function to find the elbow point in the inertia plot.
 
-    def sort_lists_based_on_first(percentages, rgb_colors):
-        """ Function to sort two lists based on the first list.
-        
-        Parameters:
-        ----------
-        percentages: list
-            The list of percentages.
-        rgb_colors: list
-            The list of RGB colors.
+            Parameters:
+            ----------
+            inertias: list
+                The list of inertia values for different k values.
+            min_k: int  
+                The minimum number of clusters to consider.
+            max_k: int
+                The maximum number of clusters to consider.
+            
+            """
 
-        """
+            # Generate the range of k values
+            K = range(min_k, max_k)
 
-        if len(percentages) != len(rgb_colors):
-            raise ValueError("The length of percentages and rgb_colors must be the same.")
-        
-        # Convert percentages to a numpy array
-        percentages_array = np.array(percentages)
-        
-        # Get the indices that would sort the percentages array
-        sorted_indices = np.argsort(percentages_array)[::-1]
-        
-        # Use the sorted indices to sort both lists
-        sorted_percentages = percentages_array[sorted_indices]
-        sorted_rgb_colors = np.array(rgb_colors)[sorted_indices]
-        
-        return sorted_percentages, sorted_rgb_colors
-    
-    def plot_rgb_squares_with_text(rgb_colors, text_labels, square_size=20):
-        """ Function to plot RGB color squares with text labels (percentages).
+            kn = KneeLocator(K, inertias, curve='convex', direction='decreasing')
+            return kn.elbow  
 
-        Parameters:
-        ----------
-        rgb_colors: list
-            The list of RGB colors.
-        text_labels: list
-            The list of text labels, usually percentages.
-        square_size: int
-            The size of the square to plot.
-        """
+        def sort_lists_based_on_first(percentages, rgb_colors):
+            """ Function to sort two lists based on the first list.
+            
+            Parameters:
+            ----------
+            percentages: list
+                The list of percentages.
+            rgb_colors: list
+                The list of RGB colors.
 
-        if len(rgb_colors) != len(text_labels):
-            raise ValueError("The length of rgb_colors and text_labels must be the same.")
-        
-        # Create an image array with the RGB colors
-        num_colors = len(rgb_colors)
-        image_array = np.zeros((square_size, square_size * num_colors, 3), dtype=np.uint8)
-        
-        for i, color in enumerate(rgb_colors):
-            image_array[:, i*square_size:(i+1)*square_size, :] = color
-        
-        # Plot the image array
-        fig, ax = plt.subplots(figsize=(num_colors, 2))
-        ax.imshow(image_array)
-        ax.axis('off')
-        
-        # Add text labels
-        for i, text in enumerate(text_labels):
-            ax.text(
-                (i + 0.5) * square_size,   # x position
-                square_size / 2,           # y position
-                str(text)+'%',                      # text
-                color='black',             # text color
-                fontsize=12,               # text size
-                ha='center',               # horizontal alignment
-                va='center',               # vertical alignment
-                bbox=dict(facecolor='white', alpha=0.5, boxstyle='round,pad=0.3'))  # background
-            
-
-    # Function to create a 3D scatter plot of the RGB color space with centroids 
-    def rgb_scatterplot(image, centroids = None):
-        """ Function to create a 3D scatter plot of the RGB color space, optionally add centroids.
+            """
 
-        Parameters:
-        ----------
-        image: numpy array
-            The image to plot.
-        downsample_factor: int
-            The factor to downsample the image by.
-        centroids: numpy array
-            The centroids to plot.
+            if len(percentages) != len(rgb_colors):
+                raise ValueError("The length of percentages and rgb_colors must be the same.")
+            
+            # Convert percentages to a numpy array
+            percentages_array = np.array(percentages)
+            
+            # Get the indices that would sort the percentages array
+            sorted_indices = np.argsort(percentages_array)[::-1]
+            
+            # Use the sorted indices to sort both lists
+            sorted_percentages = percentages_array[sorted_indices]
+            sorted_rgb_colors = np.array(rgb_colors)[sorted_indices]
+            
+            return sorted_percentages, sorted_rgb_colors
         
-        """
+        def plot_rgb_squares_with_text(rgb_colors, text_labels, square_size=20):
+            """ Function to plot RGB color squares with text labels (percentages).
 
-        # Reshape the image data
-        if image.ndim == 3:
-            h, w, c = image.shape
-            image_data = image.reshape((h * w, c))
-
-        # Normalize the image data
-        image_data = image_data / 255.0
-
-        # Create a matplotlib figure and axis
-        fig = plt.figure(figsize=(10, 8))
-        ax = fig.add_subplot(111, projection='3d')
-
-        # Scatter plot for the image data
-        ax.scatter(image_data[:, 0], image_data[:, 1], image_data[:, 2], c=image_data, marker='o')
-
-        # Plot centroids if provided
-        if centroids is not None:
-            # Normalize the centroids
-            centroids = centroids / 255.0
-            # Plot centroids as transparent spheres, in color representing the centroid
-            for centroid in centroids:
-                ax.scatter(centroid[0], centroid[1], centroid[2], color=centroid, s=2000, alpha=0.5, edgecolors='w', linewidths=2)
-
-        # Set the axis labels and title
-        ax.set_xlabel('Red')
-        ax.set_ylabel('Green')
-        ax.set_zlabel('Blue')
-        ax.set_title('3D RGB Color Space with Centroids')
+            Parameters:
+            ----------
+            rgb_colors: list
+                The list of RGB colors.
+            text_labels: list
+                The list of text labels, usually percentages.
+            square_size: int
+                The size of the square to plot.
+            """
 
-    def downsample_image(image, scale_factor):
-        """ Downsample the given image by the specified scale factor.
+            if len(rgb_colors) != len(text_labels):
+                raise ValueError("The length of rgb_colors and text_labels must be the same.")
+            
+            # Create an image array with the RGB colors
+            num_colors = len(rgb_colors)
+            image_array = np.zeros((square_size, square_size * num_colors, 3), dtype=np.uint8)
+            
+            for i, color in enumerate(rgb_colors):
+                image_array[:, i*square_size:(i+1)*square_size, :] = color
+            
+            # Plot the image array
+            fig, ax = plt.subplots(figsize=(num_colors, 2))
+            ax.imshow(image_array)
+            ax.axis('off')
+            
+            # Add text labels
+            for i, text in enumerate(text_labels):
+                ax.text(
+                    (i + 0.5) * square_size,   # x position
+                    square_size / 2,           # y position
+                    str(text)+'%',                      # text
+                    color='black',             # text color
+                    fontsize=12,               # text size
+                    ha='center',               # horizontal alignment
+                    va='center',               # vertical alignment
+                    bbox=dict(facecolor='white', alpha=0.5, boxstyle='round,pad=0.3'))  # background
+                
+
+        # Function to create a 3D scatter plot of the RGB color space with centroids 
+        def rgb_scatterplot(image, centroids = None):
+            """ Function to create a 3D scatter plot of the RGB color space, optionally add centroids.
+
+            Parameters:
+            ----------
+            image: numpy array
+                The image to plot.
+            downsample_factor: int
+                The factor to downsample the image by.
+            centroids: numpy array
+                The centroids to plot.
+            
+            """
 
-        Parameters:
-        ----------
-        image: numpy array
-            The image to downsample.
-        scale_factor: float
-            The scale factor to downsample the image by.
+            # Reshape the image data
+            if image.ndim == 3:
+                h, w, c = image.shape
+                image_data = image.reshape((h * w, c))
+
+            # Normalize the image data
+            image_data = image_data / 255.0
+
+            # Create a matplotlib figure and axis
+            fig = plt.figure(figsize=(10, 8))
+            ax = fig.add_subplot(111, projection='3d')
+
+            # Scatter plot for the image data
+            ax.scatter(image_data[:, 0], image_data[:, 1], image_data[:, 2], c=image_data, marker='o')
+
+            # Plot centroids if provided
+            if centroids is not None:
+                # Normalize the centroids
+                centroids = centroids / 255.0
+                # Plot centroids as transparent spheres, in color representing the centroid
+                for centroid in centroids:
+                    ax.scatter(centroid[0], centroid[1], centroid[2], color=centroid, s=2000, alpha=0.5, edgecolors='w', linewidths=2)
+
+            # Set the axis labels and title
+            ax.set_xlabel('Red')
+            ax.set_ylabel('Green')
+            ax.set_zlabel('Blue')
+            ax.set_title('3D RGB Color Space with Centroids')
+
+        def downsample_image(image, scale_factor):
+            """ Downsample the given image by the specified scale factor.
+
+            Parameters:
+            ----------
+            image: numpy array
+                The image to downsample.
+            scale_factor: float
+                The scale factor to downsample the image by.
+
+            """
+
+            # Calculate the new dimensions
+            new_width = int(image.shape[1] * (1 - scale_factor))
+            new_height = int(image.shape[0] * (1 - scale_factor))
+            new_dimensions = (new_width, new_height)
+
+            # Downsample the image
+            downsampled_image = cv2.resize(image, new_dimensions, interpolation=cv2.INTER_AREA)
+            return downsampled_image
+
+        # Also look for clusters equal to max_clusters
+        max_clusters  += 1
+
+        # Convert the image to RGB color space
+        image_rgb = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+        downsampled_image = downsample_image(image_rgb, downsample_factor)
+        # Get the pixel color values as an array
+        data = downsampled_image.reshape(-1, 3)
+
+        # Initialize lists to store the inertias, percentages, and centroids
+        inertias = []
+        percentages = []
+        centroids = []
+
+        # Iterate over the range of k values
+        K = range(min_clusters, max_clusters)
+        for k in K:
+            
+            if verbose:
+                print("Calculating for k = ", k)
 
-        """
+            # Initialise the KMeans algorithm, fit and append the inertia values to the list
+            kmeans = KMeans(n_clusters=k, algorithm='lloyd')
+            kmeans.fit(data)
+            inertias.append(kmeans.inertia_)
+
+            # Calculate the percentage of points in each cluster
+            _, counts = np.unique(kmeans.labels_, return_counts=True)
+            centroids.append(kmeans.cluster_centers_)
+            percentages.append(counts / len(data) * 100)
+            
+        # Plot the elbow plot
+        if plot:
+            plt.figure(figsize=(8, 4))
+            plt.plot(K, inertias, 'bx-')
+            plt.xlabel('Number of clusters')
+            plt.ylabel('Inertia')
+            plt.title('Elbow Method For Optimal k')
+        
+        # Find the optimal k, centroids, and percentages
+        optimal_k = find_elbow_point(inertias, min_clusters, max_clusters)
+        if optimal_k is None:
+            print("The elbow point could not be found. Try increasing the range of k values.")
+            return None, None, None
+
+        optimal_centroids = centroids[optimal_k - min_clusters + increase_elbow].astype(int)
+        optimal_percentages = percentages[optimal_k - min_clusters + increase_elbow].astype(int)
+        optimal_percentages, optimal_centroids = sort_lists_based_on_first(optimal_percentages, optimal_centroids)
 
-        # Calculate the new dimensions
-        new_width = int(image.shape[1] * (1 - scale_factor))
-        new_height = int(image.shape[0] * (1 - scale_factor))
-        new_dimensions = (new_width, new_height)
-
-        # Downsample the image
-        downsampled_image = cv2.resize(image, new_dimensions, interpolation=cv2.INTER_AREA)
-        return downsampled_image
-
-    # Also look for clusters equal to max_clusters
-    max_clusters  += 1
-
-    # Convert the image to RGB color space
-    image_rgb = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-    downsampled_image = downsample_image(image_rgb, downsample_factor)
-    # Get the pixel color values as an array
-    data = downsampled_image.reshape(-1, 3)
-
-    # Initialize lists to store the inertias, percentages, and centroids
-    inertias = []
-    percentages = []
-    centroids = []
-
-    # Iterate over the range of k values
-    K = range(min_clusters, max_clusters)
-    for k in K:
-        
+        # Print the optimal values
         if verbose:
-            print("Calculating for k = ", k)
-
-        # Initialise the KMeans algorithm, fit and append the inertia values to the list
-        kmeans = KMeans(n_clusters=k, algorithm='lloyd')
-        kmeans.fit(data)
-        inertias.append(kmeans.inertia_)
-
-        # Calculate the percentage of points in each cluster
-        _, counts = np.unique(kmeans.labels_, return_counts=True)
-        centroids.append(kmeans.cluster_centers_)
-        percentages.append(counts / len(data) * 100)
-        
-    # Plot the elbow plot
-    if plot:
-        plt.figure(figsize=(8, 4))
-        plt.plot(K, inertias, 'bx-')
-        plt.xlabel('Number of clusters')
-        plt.ylabel('Inertia')
-        plt.title('Elbow Method For Optimal k')
-    
-    # Find the optimal k, centroids, and percentages
-    optimal_k = find_elbow_point(inertias, min_clusters, max_clusters)
-    if optimal_k is None:
-        print("The elbow point could not be found. Try increasing the range of k values.")
-        return None, None, None
-
-    optimal_centroids = centroids[optimal_k - min_clusters + increase_elbow].astype(int)
-    optimal_percentages = percentages[optimal_k - min_clusters + increase_elbow].astype(int)
-    optimal_percentages, optimal_centroids = sort_lists_based_on_first(optimal_percentages, optimal_centroids)
-
-    # Print the optimal values
-    if verbose:
-        print("The optimal number of clusters is: ", optimal_k + increase_elbow)
-        print("The colors associated with each cluster are: \n", optimal_centroids)
-        print("The percentage of points in each cluster are: ", optimal_percentages)
-        
-    # Plot the optimal centroid colors with percentages and a 3D scatter plot
-    if plot:
-        plot_rgb_squares_with_text(optimal_centroids, optimal_percentages, square_size=50)
-        rgb_scatterplot(downsampled_image, optimal_centroids)
-        plt.show()
-
-    return optimal_centroids, optimal_k, optimal_percentages
-
-
-if __name__ == '__main__':
-    # Read the image
-    image = cv2.imread(IMAGE_PATH)
+            print("The optimal number of clusters is: ", optimal_k + increase_elbow)
+            print("The colors associated with each cluster are: \n", optimal_centroids)
+            print("The percentage of points in each cluster are: ", optimal_percentages)
+            
+        # Plot the optimal centroid colors with percentages and a 3D scatter plot
+        if plot:
+            plot_rgb_squares_with_text(optimal_centroids, optimal_percentages, square_size=50)
+            rgb_scatterplot(downsampled_image, optimal_centroids)
+            plt.show()
 
-    # Call the elbow_method function
-    optimal_centroids, optimal_k, optimal_percentages = find_main_colors(image, min_clusters=1, max_clusters=10, downsample_factor=0.98, increase_elbow=0, verbose=True, plot=True)
+        return optimal_centroids, optimal_k, optimal_percentages
```

### Comparing `uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/PKG-INFO` & `uugai_python_color_prediction-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: uugai-python-color-prediction
-Version: 1.1.0
+Name: uugai_python_color_prediction
+Version: 1.2.0
 Summary: Color prediction Python library used to find the main colors in an image.
 Home-page: UNKNOWN
 Author: uug.ai
 Author-email: support@uug.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 This project aims to predict the color of an image using Python. It utilizes machine learning algorithms, specifically k-means clustering, to analyze the pixel values of an image and predict the dominant color.
 
 K-means clustering is a popular unsupervised learning algorithm used for clustering data points into groups. In the context of color prediction, k-means clustering is used to group similar pixel values together, allowing us to identify the dominant color in an image. The algorithm works by iteratively assigning each pixel to the cluster with the closest centroid, and then updating the centroids based on the new assignments. This process continues until the centroids no longer change significantly. By applying k-means clustering to the pixel values of an image, we can identify the cluster centroids, which represent the dominant colors. To use this project, simply follow the installation instructions below. 
 
 ## Installation TODO
 
 To get started with the Python color prediction function, simply install the package using pip and follow the provided documentation for configuration and usage instructions: `pip install uugai_python_color_prediction`
-To import the function into your own python file, use: `from uugai_python_color_prediction import find_main_colors`
+To import the function into your own python file, use: `from uugai_python_color_prediction import ColorPrediction`
 
 ## Usage
 The find_main_colors function is used to predict the dominant colors of an image. It takes several parameters:
 
 * image: The input image for color prediction, using `cv2.imread(IMAGE_PATH)`.
 * min_clusters and max_clusters: The minimum and maximum number of clusters to use for k-means clustering.
 * downsample_factor: A factor used to downsample the image before color prediction. Default value is 0.95.
@@ -29,21 +29,23 @@
 * verbose: A boolean value indicating whether to print verbose output during color prediction. Default value is False.
 * plot: A boolean value indicating whether to plot the color prediction results. Default value is False.
 
 To use the find_main_colors function, simply pass the required parameters and call the function. The function will return the predicted dominant colors of the image, optimal number of centroids ± the elbow offset and the percentages of pixels belonging to that centroid.
 
 ## Usage example
 ```Python
+from uugai_python_color_prediction import ColorPrediction
+
 IMAGE_PATH = 'python_color_prediction/data/flowers.jpeg'
 
 # Read the image
 image = cv2.imread(IMAGE_PATH)
 
 # Call the elbow_method function
-optimal_centroids, optimal_k, optimal_percentages = find_main_colors(image, min_clusters=1, max_clusters=10, downsample_factor=0.95, increase_elbow=0, verbose=True, plot=True)
+optimal_centroids, optimal_k, optimal_percentages = ColorPrediction.find_main_colors(image, min_clusters=1, max_clusters=10, downsample_factor=0.95, increase_elbow=0, verbose=True, plot=True)
 ```
 
 This would result in the following output, with `verbose = True`:
 
 ```
 Calculating for k =  1
 Calculating for k =  2
```

