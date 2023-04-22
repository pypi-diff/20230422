# Comparing `tmp/imp3-0.1.1.tar.gz` & `tmp/imp3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imp3-0.1.1.tar", last modified: Sat Apr 22 10:10:08 2023, max compression
+gzip compressed data, was "imp3-0.1.2.tar", last modified: Sat Apr 22 12:45:01 2023, max compression
```

## Comparing `imp3-0.1.1.tar` & `imp3-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:10:08.063289 imp3-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-22 10:09:34.000000 imp3-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-22 10:10:08.063289 imp3-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-22 10:09:34.000000 imp3-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:10:08.059289 imp3-0.1.1/imp3/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 10:09:34.000000 imp3-0.1.1/imp3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22603 2023-04-22 10:09:34.000000 imp3-0.1.1/imp3/app.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 10:09:34.000000 imp3-0.1.1/imp3/cleaning_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-22 10:09:34.000000 imp3-0.1.1/imp3/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:10:08.063289 imp3-0.1.1/imp3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-22 10:10:08.000000 imp3-0.1.1/imp3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-22 10:10:08.000000 imp3-0.1.1/imp3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 10:10:08.000000 imp3-0.1.1/imp3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 10:10:08.000000 imp3-0.1.1/imp3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 10:10:08.000000 imp3-0.1.1/imp3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-22 10:10:08.000000 imp3-0.1.1/imp3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 10:10:08.000000 imp3-0.1.1/imp3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 10:10:08.063289 imp3-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-22 10:09:34.000000 imp3-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:10:08.063289 imp3-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 10:09:34.000000 imp3-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-22 10:09:34.000000 imp3-0.1.1/tests/unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:45:01.371867 imp3-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-22 12:44:26.000000 imp3-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-22 12:45:01.371867 imp3-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-22 12:44:26.000000 imp3-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:45:01.371867 imp3-0.1.2/imp3/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 12:44:26.000000 imp3-0.1.2/imp3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23896 2023-04-22 12:44:26.000000 imp3-0.1.2/imp3/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:44:26.000000 imp3-0.1.2/imp3/cleaning_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-22 12:44:26.000000 imp3-0.1.2/imp3/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:45:01.371867 imp3-0.1.2/imp3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-22 12:45:01.000000 imp3-0.1.2/imp3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-22 12:45:01.000000 imp3-0.1.2/imp3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:45:01.000000 imp3-0.1.2/imp3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 12:45:01.000000 imp3-0.1.2/imp3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:45:01.000000 imp3-0.1.2/imp3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-22 12:45:01.000000 imp3-0.1.2/imp3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 12:45:01.000000 imp3-0.1.2/imp3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 12:45:01.371867 imp3-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-22 12:44:26.000000 imp3-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:45:01.371867 imp3-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:44:26.000000 imp3-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-22 12:44:26.000000 imp3-0.1.2/tests/unit_test.py
```

### Comparing `imp3-0.1.1/LICENSE` & `imp3-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imp3-0.1.1/imp3/app.py` & `imp3-0.1.2/imp3/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         #step 0 : read the file 
         imput_im = Image.open(uploaded_file)
         imput_im_np = np.array(imput_im.convert('RGB'))
         im = imput_im_np
 
         #user input to resize the image or not
         # create a hprizontal line
+        # Section 0: resize the image
         st.markdown("""---""")
         st.subheader("resize input image")
         resize = st.radio('resize the image?', ['no', 'yes'], horizontal=True,)
         
         col1, col2 = st.columns( [0.5, 0.5])
         with col1:
             st.image(im)
@@ -56,14 +57,16 @@
                 width = st.sidebar.slider('width', 0, 1000, 500)
                 height = st.sidebar.slider('height', 0, 1000, 500)
                 st.sidebar.markdown("""---""")
                 im = cv2.resize(im, (width, height))
                 st.image(im)
                 st.write("resolution of resized image: ", im.shape)
 
+
+        # Section 1: map the image to different color spaces
         st.markdown("""---""")
         st.subheader("map input image to different color spaces")
         #step 1: map the colore spce
         color_space = st.radio('chage to following color space:', ['rgb','Gray scale','hsv', 'lab', 'brg', 'ch_one',
                                                                             'ch_two',
                                                                             'ch_three',
                                                                             'merge_first_two_ch',
@@ -109,30 +112,15 @@
                 #im = cv2.merge([ch2, ch3])
                 st.image(im)
             elif color_space == "merge_last_first_ch":
                 im[:, :, 1] = np.zeros((im.shape[0], im.shape[1]))
                 #im = cv2.merge([ch1, ch3])
                 st.image(im)
 
-        st.markdown("""---""")
-        st.subheader("Brightness and contrast")
-        st.sidebar.subheader("Controls for Brightness and contrast")
-        #step 2: change the brightness and contrast
-        col1, col2 = st.columns( [0.5, 0.5])
-        with col1:
-            st.image(im)
-            st.write("current state of the image")
-        with col2:
-            st.sidebar.markdown("""---""")
-            brightness = st.sidebar.slider('brightness', -100, 100, 0)
-            contrast = st.sidebar.slider('contrast', -100, 100, 0)
-            im = cv2.addWeighted(im, 1 + contrast/100., im, 0, brightness)
-            st.image(im)
-            st.write("Output image after brightness and contrast adjustment")
-
+        # Section 3: Smoothing
         st.markdown("""---""")
         st.subheader("smooting")
         blur_method = st.radio('chage to following color space:', ['None','Averaging', 'Gaussian', 
                                                                     'Median', 'Bilateral'], horizontal=True,)
         col3, col4 = st.columns( [0.5, 0.5])
 
         with col3:
@@ -164,18 +152,36 @@
                 st.sidebar.markdown("""---""")
                 st.sidebar.subheader("Controls for Bilateral smooting")
                 sigma_color = st.sidebar.slider('Adjust para 1 (sigma color)', min_value=1, max_value=11, value=9, step=1)
                 sigma_space = st.sidebar.slider('Adjust para 2 (sigma space)', min_value=1, max_value=150, value=75, step=1)
                 im = cv2.bilateralFilter(im,sigma_color,sigma_space,sigma_space)
                 st.image(im)
         
+        # Section 2: change the brightness and contrast
+        st.markdown("""---""")
+        st.subheader("Brightness and contrast")
+        st.sidebar.subheader("Controls for Brightness and contrast")
+        #step 2: change the brightness and contrast
+        col1, col2 = st.columns( [0.5, 0.5])
+        with col1:
+            st.image(im)
+            st.write("current state of the image")
+        with col2:
+            st.sidebar.markdown("""---""")
+            brightness = st.sidebar.slider('brightness', -100, 100, 0)
+            contrast = st.sidebar.slider('contrast', -100, 100, 0)
+            im = cv2.addWeighted(im, 1 + contrast/100., im, 0, brightness)
+            st.image(im)
+            st.write("Output image after brightness and contrast adjustment")
+
+        # Section 4: intensity histogram and histogram equalization
         st.markdown("""---""")
         st.subheader("Histogram")
         
-        hist_radio = st.radio('Compute Histogram:', ['None','Histogram', 'Histigram_equilisation'], horizontal=True,)
+        hist_radio = st.radio('Compute Histogram:', ['None','Histogram', 'Simple Histigram_equilisation (NEED GRAY SCALE AS INPUT)', 'Adaptive Histogram Equalization (CLAHE) (NEED GRAY SCALE AS INPUT)'], horizontal=True,)
 
         col11, col12 = st.columns( [0.5, 0.5])
 
         with col11:
             st.image(im)
             #width, height = imput_im.size
             st.write("current state of the image")
@@ -203,23 +209,31 @@
                     
                     for i, col in enumerate(colors):
                             hist = cv2.calcHist([im], [i], None, [256], [0, 256])
                             plt.plot(hist, color=col)
                             plt.xlim([0, 256])
 
                     st.pyplot(plt.figure(1))
-
-
-            elif hist_radio == "Histigram_equilisation":
+            elif hist_radio == "Simple Histigram_equilisation (NEED GRAY SCALE AS INPUT)":
+                st.sidebar.markdown("""---""")
+                # code for histogram equalization
+                im = cv2.equalizeHist(im)
+                st.image(im)
+            elif hist_radio == "Adaptive Histogram Equalization (CLAHE) (NEED GRAY SCALE AS INPUT)":
                 st.sidebar.markdown("""---""")
                 st.sidebar.subheader("Controls for Histigram_equilisation")
-                filter_hist = st.sidebar.slider('Adjust the filter size', min_value=1, max_value=11, value=5, step=2)
-                im = cv2.blur(im,(filter_hist,filter_hist))
+                # User input for CLAHE
+                clipLimit = st.sidebar.slider('Adjust the clip limit', min_value=1, max_value=10, value=2, step=1)
+                tileGridSize = st.sidebar.slider('Adjust the tile grid size', min_value=1, max_value=10, value=8, step=1)
+                # code for histogram equalization using CLAHE
+                clahe = cv2.createCLAHE(clipLimit=clipLimit, tileGridSize=(tileGridSize,tileGridSize))
+                im = clahe.apply(im)
                 st.image(im)
 
+        # Section 5: thresholding
         st.markdown("""---""")
         st.subheader("thresholding")
         st.sidebar.subheader("Controls for thresholding")
         thresh_method = st.radio('chage to following color space:', ['None','Thresholding', 'Adaptive thresholding', 
                                                                     'Otsu thresholding', ''], horizontal=True,)
 
         col13, col14 = st.columns( [0.5, 0.5])
@@ -266,15 +280,15 @@
                 st.sidebar.markdown("""---""")
                 st.sidebar.subheader("Controls for Otsu thresholding")
                 ret, im = cv2.threshold(im, 0, 255, cv2.THRESH_BINARY + 
                                                 cv2.THRESH_OTSU)   
                 st.image(im)
                 st.write("Otsu threshold is :", ret)
                 
-
+        # Section 6: edge detection
         st.markdown("""---""")
         st.subheader("canny")
         edge_option = st.radio('Edge detection:', ['None', 'Sobel','Lanlasian', 'Canny'], horizontal=True,)
         col5, col6 = st.columns( [0.5, 0.5])
 
         with col5:
             st.image(im)
@@ -296,14 +310,15 @@
                 st.sidebar.markdown("""---""")
                 st.sidebar.subheader("Controls for canny")
                 slider3 = st.sidebar.slider('Adjust minVal', min_value=0, max_value=255, value=150, step=1)
                 slider4 = st.sidebar.slider('Adjust maxVal', min_value=0, max_value=255, value=255, step=1)
                 im = cv2.Canny(im, slider3, slider4)
                 st.image(im)
         
+        # Section 7: dialate/erode
         st.markdown("""---""")
         st.subheader("Dialate/Erode")
         dia_ero_option = st.radio('Operations o0n the detected edges:', ['None', 'Dialate','Erode'], horizontal=True,)
 
         col7, col8 = st.columns( [0.5, 0.5])
 
         with col7:
@@ -324,14 +339,15 @@
             elif dia_ero_option == "Erode":
                 st.sidebar.markdown("""---""")
                 st.sidebar.subheader("Controls for Erode")
                 slider5 = st.sidebar.slider('Adjust the filter size', min_value=1, max_value=11, value=7, step=2)
                 im = cv2.GaussianBlur(im,(slider,slider),0)
                 st.image(im)
 
+        # Section 8: find contours
         st.markdown("""---""")
         st.subheader("find countours")
         contour_option = st.radio('Operations o0n the detected edges:', ['None','Detect contours'], horizontal=True,)
 
         col9, col10 = st.columns( [0.5, 0.5])
 
         with col9:
@@ -386,21 +402,25 @@
                     st.sidebar.write("Number for vetices in this contour is:", len(approx))
                     st.sidebar.write("area is:", area)
                     st.sidebar.write("perimeter is:", peri)
 
                     
                 st.image(img_cont)
         
+        # Section 9: shape matching with Hu moment on contour
         st.markdown("""---""")
         st.subheader("shape matching with Hu moment on contour")
+        # Section 10: feature extraction
         st.markdown("""---""")
         st.subheader("Feature extraction")
         st.markdown("""---""")
+        # Section 11: feature matching
         st.subheader("Feature Matching")
         st.markdown("""---""")
+        # Section 12: template matching and removal
         st.subheader("Template matching and removal, expecting gray image as imput template image can be color or gray")
         
         template_option = st.radio('options for template detection:', ['None','template matching'], horizontal=True,)
 
         col15, col16 = st.columns( [0.5, 0.5])
 
         with col15:
```

### Comparing `imp3-0.1.1/imp3/run.py` & `imp3-0.1.2/imp3/run.py`

 * *Files identical despite different names*

### Comparing `imp3-0.1.1/setup.py` & `imp3-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #     install_requires = f.read().splitlines()
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='imp3',
-    version='0.1.1',
+    version='0.1.2',
     author='Sudhir Arvind Deshmukh',
     description='Interactive tool for image pre-processing and automated pipeline creation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bokey007/imp3',
     packages=find_packages(),
     install_requires=[
```

