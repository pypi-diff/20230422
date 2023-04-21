# Comparing `tmp/tkchart-0.0.3.1.tar.gz` & `tmp/tkchart-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "H:\Test Code\Python\Modules\uploads\tkchart\dist\.tmp-hxwjmkpt\tkchart-0.0.3.1.tar", last modified: Fri Dec  2 10:52:36 2022, max compression
+gzip compressed data, was "H:\Test Code\Python\Modules\uploads\tkchart\dist\.tmp-dt9uzvd0\tkchart-0.0.4.tar", last modified: Fri Apr 21 22:13:28 2023, max compression
```

## Comparing `tkchart-0.0.3.1.tar` & `tkchart-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-12-02 10:52:36.000000 tkchart-0.0.3.1/
--rw-rw-rw-   0        0        0     4776 2022-12-02 10:52:36.000000 tkchart-0.0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4305 2022-12-02 10:46:53.000000 tkchart-0.0.3.1/README.md
--rw-rw-rw-   0        0        0      482 2022-12-02 10:51:40.000000 tkchart-0.0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-02 10:52:36.000000 tkchart-0.0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-02 10:52:36.000000 tkchart-0.0.3.1/src/
-drwxrwxrwx   0        0        0        0 2022-12-02 10:52:36.000000 tkchart-0.0.3.1/src/tkchart/
--rw-rw-rw-   0        0        0      509 2022-11-29 21:22:42.000000 tkchart-0.0.3.1/src/tkchart/Line.py
--rw-rw-rw-   0        0        0    16320 2022-12-01 21:00:09.000000 tkchart-0.0.3.1/src/tkchart/LineChart.py
--rw-rw-rw-   0        0        0      447 2022-12-01 18:13:35.000000 tkchart-0.0.3.1/src/tkchart/RequredGeometry.py
--rw-rw-rw-   0        0        0       72 2022-12-02 10:51:55.000000 tkchart-0.0.3.1/src/tkchart/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:52:36.000000 tkchart-0.0.3.1/src/tkchart.egg-info/
--rw-rw-rw-   0        0        0     4776 2022-12-02 10:52:36.000000 tkchart-0.0.3.1/src/tkchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2022-12-02 10:52:36.000000 tkchart-0.0.3.1/src/tkchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-02 10:52:36.000000 tkchart-0.0.3.1/src/tkchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-12-02 10:52:36.000000 tkchart-0.0.3.1/src/tkchart.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 22:13:28.000000 tkchart-0.0.4/
+-rw-rw-rw-   0        0        0     5361 2023-04-21 22:13:28.000000 tkchart-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4892 2023-04-21 22:07:46.000000 tkchart-0.0.4/README.md
+-rw-rw-rw-   0        0        0      480 2023-04-21 22:08:50.000000 tkchart-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 22:13:28.000000 tkchart-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 22:13:28.000000 tkchart-0.0.4/src/
+-rw-rw-rw-   0        0        0     1336 2023-04-21 22:03:51.000000 tkchart-0.0.4/src/test.py
+drwxrwxrwx   0        0        0        0 2023-04-21 22:13:28.000000 tkchart-0.0.4/src/tkchart/
+-rw-rw-rw-   0        0        0     1150 2023-04-21 21:37:25.000000 tkchart-0.0.4/src/tkchart/Line.py
+-rw-rw-rw-   0        0        0    16951 2023-04-21 22:02:23.000000 tkchart-0.0.4/src/tkchart/LineChart.py
+-rw-rw-rw-   0        0        0      447 2022-12-01 18:13:35.000000 tkchart-0.0.4/src/tkchart/RequredGeometry.py
+-rw-rw-rw-   0        0        0       70 2023-04-21 21:01:02.000000 tkchart-0.0.4/src/tkchart/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 22:13:28.000000 tkchart-0.0.4/src/tkchart.egg-info/
+-rw-rw-rw-   0        0        0     5361 2023-04-21 22:13:28.000000 tkchart-0.0.4/src/tkchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-04-21 22:13:28.000000 tkchart-0.0.4/src/tkchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 22:13:28.000000 tkchart-0.0.4/src/tkchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-21 22:13:28.000000 tkchart-0.0.4/src/tkchart.egg-info/top_level.txt
```

### Comparing `tkchart-0.0.3.1/PKG-INFO` & `tkchart-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkchart
-Version: 0.0.3.1
+Version: 0.0.4
 Summary: tkchart -> Create Chart in tkinter windows
 Author: Thisal-D
 Project-URL: Homepage, https://github.com/Thisal-D/tkchart
 Project-URL: Bug Tracker, https://github.com/pypa/tkchart/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,55 +32,58 @@
 >customtkinter - pip install customtkinter
 
 <br>
 
 #  you can configure >>
 
 >attributes
-![Sample image](https://user-images.githubusercontent.com/93121062/205255031-aefc7522-a8ba-44ee-b594-c5d2d7132c93.png?raw=True)
+![Sample image](https://user-images.githubusercontent.com/93121062/233741596-6575f82d-e501-433c-9380-5e3ecf68f853.png?raw=True)
 
 
  ## LineChart Object Configurations
 
 
-> ``` master : master of chart ``` master = frame1 | master = root
+> ``` master : master of chart ``` master = frame1 | master = root | widget
 
-> ```width :  width of chart ```width = 500
+> ```width :  width of chart ```width = 500 | integer or float
 
->```height : height of chart  ``` height = 500
+>```height : height of chart  ``` height = 500 | integer or float
 
 >```sections : show sections of chart  ``` sections = True | sections = False
 
 >```sections_fg : color of sections  ``` sections_fg = "red" | sections_fg = "#ff0000"
 
->```sections_count : no of sections  ``` sections_count = 10
+>```sections_count : no of sections  ``` sections_count = 10 | integer
 
 >```chart_bg : backgroud color of chart ``` chart_bg = "red" | chart_bg = "#ff0000"
 
 >```chart_fg : foreground color of chart ``` chart_fg = "red" | chart_fg = "#ff0000"
 
 >```horizontal_bar_fg : horizontal bar color ``` horizontal_bar_fg = "red" | horizontal_bar_fg = "#ff0000"
 
->```horizontal_bar_size : horizontal bar size ``` horizontal_bar_size = 10
+>```horizontal_bar_size : horizontal bar size ``` horizontal_bar_size = 10 | integer or float
 
 >```vertical_bar_fg : vertical bar color ``` vertical_bar_fg = "red" | vertical_bar_fg = "#ff0000"
 
->```vertical_bar_size : verticak bar size ``` verticak_bar_size = 10
+>```vertical_bar_size : verticak bar size ``` verticak_bar_size = 10 | integer or float
 
 >```text_color : colors of texts in chart ``` text_color = "red" | text_color = "#ff0000"
 
 >```font : font configure in chart ``` font = ('arial',15,'bold')
 
 >```values_labels : show values of labels  ``` values_labels = True | values_labels = False
 
->```values_labels_count : no. of labels  ``` values_labels_count = 10
+>```values_labels_count : no. of labels  ``` values_labels_count = 10 | integer
 
->```chart_line_len : length of chart line``` chart_line_len = 10 
+>```chart_line_len : length of chart line``` chart_line_len = 10 | integer or float
 
->```max_value : maximum display value```  max_value = 1800
+>```max_value : maximum display value```  max_value = 1800 | float or integer value
+
+
+<br>
 
 >configure spaces  \
 >```top_space : ```  top_space = 20 \
 >```bottom_space : ```  bottom_space = 20\
 >```right_space : ```  right_space = 20\
 >```right_space : ```  right_space = 20\
 >```x_space : ```  x_space = 100\
@@ -94,14 +97,21 @@
 
  ## Line Object Configurations
 
 >```height : height of chart  ``` height = 1 
 
 >```color : color of line  ``` color = "#101010" | color= "black"
 
+>********************************\
+>added new configuration**\
+>******************************\
+>```line_highlight : show circle in corners of chart``` line_highlight=True | line_highlight=False \
+>```line_highlight_size : circle size``` line_highlight_size=10 | line_highlight_size=5 | integer or float\
+>```line_highlight_color : circle color``` line_highlight_color="#ffffff" | line_highlight_color="white" |  string 
+
 
 
 # create Chart 
 
 ```
 #import module
```

### Comparing `tkchart-0.0.3.1/README.md` & `tkchart-0.0.4/src/tkchart.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: tkchart
+Version: 0.0.4
+Summary: tkchart -> Create Chart in tkinter windows
+Author: Thisal-D
+Project-URL: Homepage, https://github.com/Thisal-D/tkchart
+Project-URL: Bug Tracker, https://github.com/pypa/tkchart/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+
 # tkchart package 
 <br>
 
 ## create line chart in tkinter & customtkinter windows
 
 <br><br>
 
@@ -19,55 +32,58 @@
 >customtkinter - pip install customtkinter
 
 <br>
 
 #  you can configure >>
 
 >attributes
-![Sample image](https://user-images.githubusercontent.com/93121062/205255031-aefc7522-a8ba-44ee-b594-c5d2d7132c93.png?raw=True)
+![Sample image](https://user-images.githubusercontent.com/93121062/233741596-6575f82d-e501-433c-9380-5e3ecf68f853.png?raw=True)
 
 
  ## LineChart Object Configurations
 
 
-> ``` master : master of chart ``` master = frame1 | master = root
+> ``` master : master of chart ``` master = frame1 | master = root | widget
 
-> ```width :  width of chart ```width = 500
+> ```width :  width of chart ```width = 500 | integer or float
 
->```height : height of chart  ``` height = 500
+>```height : height of chart  ``` height = 500 | integer or float
 
 >```sections : show sections of chart  ``` sections = True | sections = False
 
 >```sections_fg : color of sections  ``` sections_fg = "red" | sections_fg = "#ff0000"
 
->```sections_count : no of sections  ``` sections_count = 10
+>```sections_count : no of sections  ``` sections_count = 10 | integer
 
 >```chart_bg : backgroud color of chart ``` chart_bg = "red" | chart_bg = "#ff0000"
 
 >```chart_fg : foreground color of chart ``` chart_fg = "red" | chart_fg = "#ff0000"
 
 >```horizontal_bar_fg : horizontal bar color ``` horizontal_bar_fg = "red" | horizontal_bar_fg = "#ff0000"
 
->```horizontal_bar_size : horizontal bar size ``` horizontal_bar_size = 10
+>```horizontal_bar_size : horizontal bar size ``` horizontal_bar_size = 10 | integer or float
 
 >```vertical_bar_fg : vertical bar color ``` vertical_bar_fg = "red" | vertical_bar_fg = "#ff0000"
 
->```vertical_bar_size : verticak bar size ``` verticak_bar_size = 10
+>```vertical_bar_size : verticak bar size ``` verticak_bar_size = 10 | integer or float
 
 >```text_color : colors of texts in chart ``` text_color = "red" | text_color = "#ff0000"
 
 >```font : font configure in chart ``` font = ('arial',15,'bold')
 
 >```values_labels : show values of labels  ``` values_labels = True | values_labels = False
 
->```values_labels_count : no. of labels  ``` values_labels_count = 10
+>```values_labels_count : no. of labels  ``` values_labels_count = 10 | integer
+
+>```chart_line_len : length of chart line``` chart_line_len = 10 | integer or float
 
->```chart_line_len : length of chart line``` chart_line_len = 10 
+>```max_value : maximum display value```  max_value = 1800 | float or integer value
 
->```max_value : maximum display value```  max_value = 1800
+
+<br>
 
 >configure spaces  \
 >```top_space : ```  top_space = 20 \
 >```bottom_space : ```  bottom_space = 20\
 >```right_space : ```  right_space = 20\
 >```right_space : ```  right_space = 20\
 >```x_space : ```  x_space = 100\
@@ -81,14 +97,21 @@
 
  ## Line Object Configurations
 
 >```height : height of chart  ``` height = 1 
 
 >```color : color of line  ``` color = "#101010" | color= "black"
 
+>********************************\
+>added new configuration**\
+>******************************\
+>```line_highlight : show circle in corners of chart``` line_highlight=True | line_highlight=False \
+>```line_highlight_size : circle size``` line_highlight_size=10 | line_highlight_size=5 | integer or float\
+>```line_highlight_color : circle color``` line_highlight_color="#ffffff" | line_highlight_color="white" |  string 
+
 
 
 # create Chart 
 
 ```
 #import module 
 
@@ -164,8 +187,8 @@
 
 ## More Infomations :- <a href = "https://github.com/Thisal-D/tkchart"> https://github.com/Thisal-D/tkchart </a>
 
 
 <br>
 <br>
 <br>
-## This is a tkchart package. Thanks For Using..!👌
+## This is a tkchart package. Thanks For Using..!👌
```

### Comparing `tkchart-0.0.3.1/src/tkchart/LineChart.py` & `tkchart-0.0.4/src/tkchart/LineChart.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 class LineChart():
    def __init__(self ,*args ,master=None ,width=600 ,height=300 
                 ,sections=None ,sections_count=10 ,sections_fg="#303030"
                 ,chart_bg = '#101010' ,chart_fg = '#202020' 
                 ,horizontal_bar_fg = "#404040" ,horizontal_bar_size=2 ,vertical_bar_fg = "#404040" ,vertical_bar_size=2
                 ,text_color = "#ffffff" ,font=None ,values_labels=False ,values_labels_count=10 ,max_value=1000 
                 ,chart_line_len = 30 
-                ,top_space=10 ,bottom_space=10 ,left_space=10 ,right_space=10 ,x_space=40 ,y_space=40) :
+                ,top_space=10 ,bottom_space=10 ,left_space=10 ,right_space=10 ,x_space=40 ,y_space=40
+                ) :
       
       # user input main width & height
       self.main_width = width
       self.main_height = height
       
       #get master of chart widget
       try:
@@ -64,25 +65,35 @@
       self.configure_chart_geomatry()
       self.configure_chart_colors()
       
       if self.sections == True :
          self.configure_sections()
       if self.values_labels == True :
          self.configure_values_label()
-      
-               
+         
    def configure_chart_geomatry(self):
-      self.chart_main_background.configure(width=self.main_width ,height=self.main_height)
-      self.chart_values_backgroud.place(width=self.left_space ,y=self.top_space+self.y_space+self.horizontal_bar_size ,height=self.main_height-(self.horizontal_bar_size*2+self.top_space+self.y_space+self.bottom_space ))
-      self.chart_vertical_bar.place(width=self.vertical_bar_size ,x=self.left_space ,y=self.top_space ,height=self.main_height-(self.top_space+self.bottom_space))
-      self.chart_horizontal_bar.place(height=self.horizontal_bar_size ,x=self.left_space ,y=self.main_height-self.bottom_space-self.horizontal_bar_size ,width=self.main_width-(self.left_space+self.right_space))
-      self.chart_canvas_backgroud.place(x=self.left_space+self.vertical_bar_size ,width=self.main_width-(self.left_space+self.vertical_bar_size+self.x_space+self.right_space) ,
-                                        y=self.top_space+self.y_space+self.horizontal_bar_size ,height=self.main_height-(self.horizontal_bar_size*2+self.top_space+self.y_space+self.bottom_space))
-      self.chart_canvas.place(x=0 ,width=self.main_width-5-(self.left_space+self.vertical_bar_size+self.x_space+self.right_space) ,
-                                        y=0,height=self.main_height-(self.horizontal_bar_size*2+self.top_space+self.y_space+self.bottom_space))   
+      self.chart_main_background.configure(width=self.main_width,
+                                           height=self.main_height)
+      self.chart_values_backgroud.place(y=self.top_space+self.y_space+self.horizontal_bar_size)
+      self.chart_vertical_bar.place(x=self.left_space,
+                                    y=self.top_space)
+      self.chart_horizontal_bar.place(x=self.left_space,
+                                      y=self.main_height-self.bottom_space-self.horizontal_bar_size)
+      self.chart_canvas_backgroud.place(x=self.left_space+self.vertical_bar_size,
+                                        y=self.top_space+self.y_space+self.horizontal_bar_size)
+      self.chart_canvas.place(x=0,y=0)   
+      
+      self.chart_values_backgroud.configure(width=self.left_space, height=self.main_height-(self.horizontal_bar_size*2+self.top_space+self.y_space+self.bottom_space ))
+      self.chart_vertical_bar.configure(width=self.vertical_bar_size ,height=self.main_height-(self.top_space+self.bottom_space))
+      self.chart_horizontal_bar.configure(height=self.horizontal_bar_size ,width=self.main_width-(self.left_space+self.right_space))
+      self.chart_canvas_backgroud.configure(width=self.main_width-(self.left_space+self.vertical_bar_size+self.x_space+self.right_space) ,
+                                            height=self.main_height-(self.horizontal_bar_size*2+self.top_space+self.y_space+self.bottom_space))
+      self.chart_canvas.configure(width=self.main_width-5-(self.left_space+self.vertical_bar_size+self.x_space+self.right_space) ,
+                                  height=self.main_height-(self.horizontal_bar_size*2+self.top_space+self.y_space+self.bottom_space))
+      
       self.re_display_chart() 
    def configure_chart_colors(self):
       self.chart_main_background.configure(fg_color=self.chart_bg)
       self.chart_values_backgroud.configure(fg_color=self.chart_bg)
       self.chart_vertical_bar.configure(fg_color=self.vertical_bar_fg )
       self.chart_horizontal_bar.configure(fg_color=self.horizontal_bar_fg)
       self.chart_canvas_backgroud.configure(fg_color=self.chart_fg)
@@ -122,15 +133,16 @@
  
    def configure(self ,master=None ,width=None ,height=None 
                 ,sections=None ,sections_count=None ,sections_fg=None
                 ,chart_bg = None ,chart_fg = None
                 ,horizontal_bar_fg = None ,horizontal_bar_size=None ,vertical_bar_fg =None ,vertical_bar_size=None
                 ,text_color = None ,font=None ,values_labels=None ,values_labels_count=None ,max_value=None 
                 ,chart_line_len = None 
-                ,top_space=None ,bottom_space=None ,left_space=None ,right_space=None ,x_space=None ,y_space=None) :
+                ,top_space=None ,bottom_space=None ,left_space=None ,right_space=None ,x_space=None ,y_space=None
+                ) :
       
 
       reset_chart_geomatry = False
       reset_chart_colors = False
       reset_left_space = False
       reset_sections = False
       reset_values_labels = False
@@ -266,45 +278,43 @@
       elif sections == False:
          self.delete_sections()
          self.sections = False
          
       if chart_line_len != None :
          self.chart_line_len = chart_line_len
          reset_chart_geomatry = True
-      
+   
       if reset_chart_colors == True:
          self.configure_chart_colors()
       if reset_chart_geomatry == True :
          self.configure_chart_geomatry()
          
          
-      
-   
-   
    def place(self ,x=None ,y=None ,rely=None ,relx=None ,anchor=None):
       self.chart_main_background.place(x=x ,y=y ,rely=rely ,relx=relx ,anchor=anchor)
       
    def pack(self ,x=None ,y=None ,pady=None ,padx=None ,before=None ,expand=None ,fill=None ,after=None 
             ,side=None ,ipadx=None ,ipady=None ,anchor=None):
-      self.chart_main_background.pack(x=x ,y=y ,pady=pady ,padx=padx ,before=before , expand=expand ,fill=fill
+      self.chart_main_background.pack(pady=pady ,padx=padx ,before=before , expand=expand ,fill=fill
                                ,after=after ,side=side ,ipadx=ipadx ,ipady=ipady ,anchor=anchor)
       
    def grid(self ,column=None ,columnspan=None ,ipadx=None ,ipady=None , padx=None , pady=None ,row=None 
             ,rowspan=None ,sticky=None):
       self.chart_main_background.grid(column=column ,columnspan=columnspan ,ipadx=ipadx ,ipady=ipady ,
                                padx=padx , pady=pady ,row=row ,rowspan=rowspan ,sticky=sticky)
       
       
    def reset_chart_canvas_place_info(self):
       self.chart_x = 0 
       self.chart_width = self.main_width-5-(self.left_space+self.vertical_bar_size+self.x_space+self.right_space)
       self.chart_height = self.main_height-(self.horizontal_bar_size*2+self.top_space+self.y_space+self.bottom_space)
-      self.chart_canvas.place(x=0 ,width=self.main_width-5-(self.left_space+self.vertical_bar_size+self.x_space+self.right_space) ,
-                                        y=0,height=self.main_height-(self.horizontal_bar_size*2+self.top_space+self.y_space+self.bottom_space))   
+      self.chart_canvas.place(x=0 ,y=0)   
       
+      self.chart_canvas.configure(width=self.main_width-5-(self.left_space+self.vertical_bar_size+self.x_space+self.right_space),
+                                  height=self.main_height-(self.horizontal_bar_size*2+self.top_space+self.y_space+self.bottom_space))
       self.chart_canvas.delete("all")
    
    def set_chart_canvas_info(self):
       self.chart_display_lines = []
       
    def reset(self):
       self.reset_chart_canvas_place_info()
@@ -335,39 +345,38 @@
             line.x_end =  self.chart_line_len*-1
             line.y_end = 0
             temp_values = line.values
             line.values = []
             if len(temp_values) != 0 :
                self.display(values=temp_values ,line=line)
 
-   def display(self ,line=None ,values=None):
+   def display(self ,line=None ,values:list=[]):
       if line not in self.chart_display_lines:
          self.chart_display_lines.append(line)
       
       line.values += values
       x_start = line.x_end
       y_start = line.y_end
 
       for value in values:
          line.x_end += self.chart_line_len
          line.y_end = (self.chart_height - (self.chart_height/100)*(value/self.max_value*100) + (line.line_height/2))
          self.chart_canvas.create_line(x_start,y_start,line.x_end,line.y_end
                                             ,fill=line.line_color ,width=line.line_height)
-
+         
+         if line.line_highlight :
+            self.chart_canvas.create_aa_circle(x_start,y_start,radius = line.line_highlight_size ,fill=line.line_highlight_color)
    
          
          if line.x_end > self.chart_width :
             self.chart_x -= self.chart_line_len
             self.chart_width += self.chart_line_len
             if self.chart_width > self.main_width*2 :
                self.re_display_chart()
             else:
-               self.chart_canvas.place(x=self.chart_x ,width=self.chart_width ,
-                                        y=0,height=self.main_height-(self.horizontal_bar_size*2+self.top_space+self.y_space+self.bottom_space))      
+               self.chart_canvas.place(x=self.chart_x,
+                                        y=0)      
+               self.chart_canvas.configure(width=self.chart_width
+                                           ,height=self.main_height-(self.horizontal_bar_size*2+self.top_space+self.y_space+self.bottom_space))
       
          x_start = line.x_end
-         y_start = line.y_end
-         
-      
-
-         
-     
+         y_start = line.y_end
```

### Comparing `tkchart-0.0.3.1/src/tkchart.egg-info/PKG-INFO` & `tkchart-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: tkchart
-Version: 0.0.3.1
-Summary: tkchart -> Create Chart in tkinter windows
-Author: Thisal-D
-Project-URL: Homepage, https://github.com/Thisal-D/tkchart
-Project-URL: Bug Tracker, https://github.com/pypa/tkchart/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-
 # tkchart package 
 <br>
 
 ## create line chart in tkinter & customtkinter windows
 
 <br><br>
 
@@ -32,55 +19,58 @@
 >customtkinter - pip install customtkinter
 
 <br>
 
 #  you can configure >>
 
 >attributes
-![Sample image](https://user-images.githubusercontent.com/93121062/205255031-aefc7522-a8ba-44ee-b594-c5d2d7132c93.png?raw=True)
+![Sample image](https://user-images.githubusercontent.com/93121062/233741596-6575f82d-e501-433c-9380-5e3ecf68f853.png?raw=True)
 
 
  ## LineChart Object Configurations
 
 
-> ``` master : master of chart ``` master = frame1 | master = root
+> ``` master : master of chart ``` master = frame1 | master = root | widget
 
-> ```width :  width of chart ```width = 500
+> ```width :  width of chart ```width = 500 | integer or float
 
->```height : height of chart  ``` height = 500
+>```height : height of chart  ``` height = 500 | integer or float
 
 >```sections : show sections of chart  ``` sections = True | sections = False
 
 >```sections_fg : color of sections  ``` sections_fg = "red" | sections_fg = "#ff0000"
 
->```sections_count : no of sections  ``` sections_count = 10
+>```sections_count : no of sections  ``` sections_count = 10 | integer
 
 >```chart_bg : backgroud color of chart ``` chart_bg = "red" | chart_bg = "#ff0000"
 
 >```chart_fg : foreground color of chart ``` chart_fg = "red" | chart_fg = "#ff0000"
 
 >```horizontal_bar_fg : horizontal bar color ``` horizontal_bar_fg = "red" | horizontal_bar_fg = "#ff0000"
 
->```horizontal_bar_size : horizontal bar size ``` horizontal_bar_size = 10
+>```horizontal_bar_size : horizontal bar size ``` horizontal_bar_size = 10 | integer or float
 
 >```vertical_bar_fg : vertical bar color ``` vertical_bar_fg = "red" | vertical_bar_fg = "#ff0000"
 
->```vertical_bar_size : verticak bar size ``` verticak_bar_size = 10
+>```vertical_bar_size : verticak bar size ``` verticak_bar_size = 10 | integer or float
 
 >```text_color : colors of texts in chart ``` text_color = "red" | text_color = "#ff0000"
 
 >```font : font configure in chart ``` font = ('arial',15,'bold')
 
 >```values_labels : show values of labels  ``` values_labels = True | values_labels = False
 
->```values_labels_count : no. of labels  ``` values_labels_count = 10
+>```values_labels_count : no. of labels  ``` values_labels_count = 10 | integer
+
+>```chart_line_len : length of chart line``` chart_line_len = 10 | integer or float
 
->```chart_line_len : length of chart line``` chart_line_len = 10 
+>```max_value : maximum display value```  max_value = 1800 | float or integer value
 
->```max_value : maximum display value```  max_value = 1800
+
+<br>
 
 >configure spaces  \
 >```top_space : ```  top_space = 20 \
 >```bottom_space : ```  bottom_space = 20\
 >```right_space : ```  right_space = 20\
 >```right_space : ```  right_space = 20\
 >```x_space : ```  x_space = 100\
@@ -94,14 +84,21 @@
 
  ## Line Object Configurations
 
 >```height : height of chart  ``` height = 1 
 
 >```color : color of line  ``` color = "#101010" | color= "black"
 
+>********************************\
+>added new configuration**\
+>******************************\
+>```line_highlight : show circle in corners of chart``` line_highlight=True | line_highlight=False \
+>```line_highlight_size : circle size``` line_highlight_size=10 | line_highlight_size=5 | integer or float\
+>```line_highlight_color : circle color``` line_highlight_color="#ffffff" | line_highlight_color="white" |  string 
+
 
 
 # create Chart 
 
 ```
 #import module 
 
@@ -177,8 +174,8 @@
 
 ## More Infomations :- <a href = "https://github.com/Thisal-D/tkchart"> https://github.com/Thisal-D/tkchart </a>
 
 
 <br>
 <br>
 <br>
-## This is a tkchart package. Thanks For Using..!👌
+## This is a tkchart package. Thanks For Using..!👌
```

