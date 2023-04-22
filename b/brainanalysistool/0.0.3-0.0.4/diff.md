# Comparing `tmp/brainanalysistool-0.0.3.tar.gz` & `tmp/brainanalysistool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainanalysistool-0.0.3.tar", last modified: Mon Mar 13 23:59:19 2023, max compression
+gzip compressed data, was "brainanalysistool-0.0.4.tar", last modified: Sat Apr 22 06:32:21 2023, max compression
```

## Comparing `brainanalysistool-0.0.3.tar` & `brainanalysistool-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 23:59:19.155520 brainanalysistool-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-03-02 01:48:52.000000 brainanalysistool-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      618 2023-03-13 23:59:19.154427 brainanalysistool-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-03-02 01:44:23.000000 brainanalysistool-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 23:59:19.146422 brainanalysistool-0.0.3/brainanalysistool/
--rw-rw-rw-   0        0        0     9770 2023-03-02 08:41:09.000000 brainanalysistool-0.0.3/brainanalysistool/WaveAnalysisFun.py
--rw-rw-rw-   0        0        0     5562 2023-03-04 12:42:35.000000 brainanalysistool-0.0.3/brainanalysistool/WaveletFun.py
--rw-rw-rw-   0        0        0      492 2023-03-13 23:56:54.000000 brainanalysistool-0.0.3/brainanalysistool/__init__.py
--rw-rw-rw-   0        0        0    17766 2023-03-04 12:42:25.000000 brainanalysistool-0.0.3/brainanalysistool/plotting.py
--rw-rw-rw-   0        0        0     2583 2023-03-01 18:52:03.000000 brainanalysistool-0.0.3/brainanalysistool/preprocessing.py
-drwxrwxrwx   0        0        0        0 2023-03-13 23:59:19.153424 brainanalysistool-0.0.3/brainanalysistool.egg-info/
--rw-rw-rw-   0        0        0      618 2023-03-13 23:59:18.000000 brainanalysistool-0.0.3/brainanalysistool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-03-13 23:59:19.000000 brainanalysistool-0.0.3/brainanalysistool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 23:59:18.000000 brainanalysistool-0.0.3/brainanalysistool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-03-13 23:59:18.000000 brainanalysistool-0.0.3/brainanalysistool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-03-13 23:59:18.000000 brainanalysistool-0.0.3/brainanalysistool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-13 23:59:19.155520 brainanalysistool-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-03-13 23:56:32.000000 brainanalysistool-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:32:21.150149 brainanalysistool-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-03-02 01:48:52.000000 brainanalysistool-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      677 2023-04-22 06:32:21.149844 brainanalysistool-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-03-14 00:14:53.000000 brainanalysistool-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 06:32:21.138848 brainanalysistool-0.0.4/brainanalysistool/
+-rw-rw-rw-   0        0        0    10070 2023-04-02 09:12:15.000000 brainanalysistool-0.0.4/brainanalysistool/WaveAnalysisFun.py
+-rw-rw-rw-   0        0        0     5899 2023-03-23 02:13:39.000000 brainanalysistool-0.0.4/brainanalysistool/WaveletFun.py
+-rw-rw-rw-   0        0        0      492 2023-04-22 06:19:02.000000 brainanalysistool-0.0.4/brainanalysistool/__init__.py
+-rw-rw-rw-   0        0        0    22078 2023-04-22 00:56:01.000000 brainanalysistool-0.0.4/brainanalysistool/plotting.py
+-rw-rw-rw-   0        0        0     3548 2023-04-02 07:49:48.000000 brainanalysistool-0.0.4/brainanalysistool/preprocessing.py
+drwxrwxrwx   0        0        0        0 2023-04-22 06:32:21.147848 brainanalysistool-0.0.4/brainanalysistool.egg-info/
+-rw-rw-rw-   0        0        0      677 2023-04-22 06:32:20.000000 brainanalysistool-0.0.4/brainanalysistool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-04-22 06:32:21.000000 brainanalysistool-0.0.4/brainanalysistool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 06:32:20.000000 brainanalysistool-0.0.4/brainanalysistool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2023-04-22 06:32:20.000000 brainanalysistool-0.0.4/brainanalysistool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-22 06:32:20.000000 brainanalysistool-0.0.4/brainanalysistool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 06:32:21.150149 brainanalysistool-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-04-22 06:32:14.000000 brainanalysistool-0.0.4/setup.py
```

### Comparing `brainanalysistool-0.0.3/LICENSE` & `brainanalysistool-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brainanalysistool-0.0.3/brainanalysistool/WaveAnalysisFun.py` & `brainanalysistool-0.0.4/brainanalysistool/WaveAnalysisFun.py`

 * *Files 3% similar despite different names*

```diff
@@ -240,14 +240,21 @@
     dataconv = np.fft.ifft(np.fft.fft(wavelet,n_conv_pow2)*datafft)
     dataconv = dataconv[0:n_convolution]
     dataconv = dataconv[int((n_wavelet-1)/2)-1:-2-int((n_wavelet-1)/2)].reshape(-1,n_wavelet)
 
     itpc = np.abs(np.mean(np.exp(1j*np.angle(dataconv)),0))
     return itpc
 
+def SNR_dB(sig,stim_start_pnt,response_period):
+    noise = sig[:stim_start_pnt]
+    # print(noise.shape)
+    x = sig[int(response_period[0]):int(response_period[1])]
+    # print(x.shape)
+    SNR_dB = 10*(np.log10( np.sum(x**2)/len(x))-np.log10(np.sum(noise**2)/len(noise)))
+    return SNR_dB
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `brainanalysistool-0.0.3/brainanalysistool/WaveletFun.py` & `brainanalysistool-0.0.4/brainanalysistool/WaveletFun.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,38 +18,47 @@
 
 plt.rcParams['font.sans-serif'] = ['SimHei'] #用来正常显示中文标签
 plt.rcParams['axes.unicode_minus'] = False #用来正常显示负号
 
 
 ######################################################连续小波变换##########
 # totalscal小波的尺度，对应频谱分析结果也就是分析几个（totalscal-1）频谱
-def TimeFrequencyCWT(data,fs,totalscal,wavelet='cgau8'):
+def TimeFrequencyCWT(data,fs,time_points,totalscal,band=[1,100],wavelet='cgau8',fig=None,ax=None,show_flag=False):
     # 采样数据的时间维度
     t = np.arange(data.shape[0])/fs
     # 中心频率
     wcf = pywt.central_frequency(wavelet=wavelet)
     # 计算对应频率的小波尺度
     cparam = 2 * wcf * totalscal
-    scales = cparam/np.arange(totalscal, 1, -1)
+    a = 2*band[1]/fs
+    scales = cparam/np.arange(totalscal*a, band[0]-1, -1)
     # print(scales)
     # 连续小波变换
     [cwtmatr, frequencies] = pywt.cwt(data, scales, wavelet, 1.0/fs)
     # print(frequencies)
     # 绘图
-    plt.figure(figsize=(8, 4))
-    plt.subplot(211)
-    plt.plot(t, data)
-    plt.xlabel(u"time(s)")
-    plt.title(u"Time spectrum")
-    plt.subplot(212)
-    plt.contourf(t, frequencies, abs(cwtmatr))
-    plt.ylabel(u"freq(Hz)")
-    plt.xlabel(u"time(s)")
-    plt.subplots_adjust(hspace=0.4)
-    plt.show()
+    # plt.figure(figsize=(8, 4))
+    # plt.subplot(211)
+    # plt.plot(t, data)
+    # plt.xlabel(u"time(s)")
+    # plt.title(u"Time spectrum")
+    # plt.subplot(212)
+    if ax==None:
+        if fig==None:
+            fig,ax = plt.subplots()
+        else:
+            ax = fig.add_subplot(111)
+    ax.contourf(time_points, frequencies, abs(cwtmatr),100,cmap='jet')
+    ax.set_ylabel(u"freq(Hz)")
+    ax.set_xlabel(u"time(s)")
+    ax.set_yscale('symlog')
+    # plt.subplots_adjust(hspace=0.4)
+    if show_flag:
+        plt.show()
+    return fig,ax
 
 ########################################小波包变换-重构造分析不同频段的特征(注意maxlevel，如果太小可能会导致)#########################
 def TimeFrequencyWP(data, fs, wavelet, maxlevel = 8):
     # 小波包变换这里的采样频率为250，如果maxlevel太小部分波段分析不到
     wp = pywt.WaveletPacket(data=data, wavelet=wavelet, mode='symmetric', maxlevel=maxlevel)
     # 频谱由低到高的对应关系，这里需要注意小波变换的频带排列默认并不是顺序排列，所以这里需要使用’freq‘排序。
     freqTree = [node.path for node in wp.get_level(maxlevel, 'freq')]
```

### Comparing `brainanalysistool-0.0.3/brainanalysistool/plotting.py` & `brainanalysistool-0.0.4/brainanalysistool/plotting.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,77 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from .preprocessing import butter_filt
 from .WaveAnalysisFun import *
 from scipy import signal
 
-def plot_vector_field(vec, norm=True, fig=None,ax=None, show_flag=True):
+
+
+
+
+def plot_vector_field(x, y, vec, pixel_spacing_x, pixel_spacing_y, norm=True, fig=None,ax=None, show_flag=True):
     #######
     # INPUT
     # ph - complex-valued scalar field representing vector directions
     # norm - whether to represent the norm of the vec 
     # OUTPUT
     # vector field plot
     #######
 
-    x = np.arange(vec.shape[1])+0.5
-    y = np.arange(vec.shape[0])+0.5
+    x = x-pixel_spacing_x/2
+    y = y-pixel_spacing_y/2
     if norm:
         u = np.real(vec)
         v = np.imag(vec)
     else:
         u = np.real(np.exp(1j*np.angle(vec)))
         v = np.imag(np.exp(1j*np.angle(vec)))
 
     if ax == None:
         if fig==None:
             fig = plt.figure()
         ax = fig.add_subplot(111)
-    ax.quiver(x, y, u, -v, color = 'k',scale=2,scale_units='xy',width=0.005)
-    ax.invert_yaxis()
+    ax.quiver(x, y, u, -v, color = 'k',scale=4,scale_units='xy',width=0.005)
+    
     if show_flag:
         plt.show()
     return fig,ax
 
 
 # # 绘制每个通道图像
-def show_channelwave(sig, grishape, fig=None, show_flag=True):
+def show_all_channelwave(sig, grishape, fig=None, show_flag=True):
     #######
     # input:
     # sig.shape = (channels,time) 
     #######
     if fig==None:
         fig = plt.figure()
     for id in range(sig.shape[0]):
         ax = fig.add_subplot(grishape[0],grishape[1],id+1)
         ax.plot(sig[id])
+        ax.set_ylabel('V/uV')
+    if show_flag:
+        plt.show()
+    return fig
+
+def show_channelwave(sig, fs, chan, fig=None, ax=None,show_flag=True):
+    #######
+    # input:
+    # sig.shape = (channels,time) 
+    #######
+    if ax==None:
+        if fig==None:
+            fig,ax = plt.subplots()
+        else:
+            ax = fig.add_subplot(111)
+    time_points = np.arange(0,len(sig),1)/fs
+    ax.plot(time_points,sig)
+    ax.set_xlabel('time(s)')
+    ax.set_ylabel('V/uV')
+    ax.set_title(f'Chan {chan+1}')
     if show_flag:
         plt.show()
     return fig
 
 
 # wave of each channel 
 def channel_wave(trial_sig, fs, time_points, lowband=[3,6], highband=[30,50],period=None, fig=None, fig1=None, show_flag=True):
@@ -65,15 +89,15 @@
     ax1 = fig1.add_subplot(211)
     ax2 = fig1.add_subplot(212)
 
     low_t_sig = butter_filt(trial_sig,fs,lowband,'bandpass')
     high_t_sig = butter_filt(trial_sig,fs,highband,'bandpass')
 
     # 每个试次图像
-    for trial in trial_sig.shape[0]:
+    for trial in range(trial_sig.shape[0]):          # gai++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
         ax0.plot(time_points,trial_sig[trial],color='0.1')
         ax1.plot(time_points[int(period[0]):int(period[1])],low_t_sig[trial][int(period[0]):int(period[1])],color='0.1')
         ax2.plot(time_points[int(period[0]):int(period[1])],high_t_sig[trial][int(period[0]):int(period[1])],color='0.1')
         # ax3.plot(time_points,channel_trial_wave2_[id][trial],color='0.1')
     # 试次间均值
     ax0.plot(time_points,np.mean(trial_sig,0),color='red')
     ax1.plot(time_points[int(period[0]):int(period[1])],np.mean(low_t_sig[:,int(period[0]):int(period[1])],0),color='red')
@@ -86,93 +110,141 @@
     fig1.suptitle('channel trial-mean LFP at different frequences')
     ax1.set_title('low-frequency')
     ax2.set_title('high-frequency')
     if show_flag:
         plt.show()
     return fig,fig1
 
+def chan_trail_ave_sig(trial_sig, time_points, chan, period=None, fig=None, ax=None, normed=False, show_flag=True):
+    # period : time point
+    if ax==None:
+        if fig==None:
+            fig,ax = plt.subplots()
+        else:
+            ax = fig.add_subplot(111)
+    if period==None:
+        for trial in range(trial_sig.shape[0]):
+            ax.plot(time_points,trial_sig[trial],color='0.1',linewidth =0.1)
+        ax.plot(time_points,np.mean(trial_sig,0),color='red')
+        ax.plot(time_points,np.mean(trial_sig,0)+np.std(trial_sig,0),color='red',linestyle='--',linewidth =0.5)
+        ax.plot(time_points,np.mean(trial_sig,0)-np.std(trial_sig,0),color='red',linestyle='--',linewidth =0.5)
+        
+
+    else:
+        period = [int(period[0]),int(period[1])]
+        for trial in range(trial_sig.shape[0]):
+            ax.plot(time_points[period[0]:period[1]],trial_sig[trial,period[0]:period[1]],color='0.1',linewidth =0.1)
+        ax.plot(time_points[period[0]:period[1]],np.mean(trial_sig[:,period[0]:period[1]],0),color='red')
+        ax.plot(time_points[period[0]:period[1]],np.mean(trial_sig[:,period[0]:period[1]],0)+np.std(trial_sig[:,period[0]:period[1]],0),color='red',linestyle='--',linewidth =0.5)
+        ax.plot(time_points[period[0]:period[1]],np.mean(trial_sig[:,period[0]:period[1]],0)-np.std(trial_sig[:,period[0]:period[1]],0),color='red',linestyle='--',linewidth =0.5)
+    ax.set_xlabel('time(s)')
+    
+    if normed:
+        ax.set_ylabel('Normed')
+    else:
+        ax.set_ylabel('V/uV')
+    ax.set_title(f'Chan {chan+1}')
+    if show_flag:
+        plt.show()
+    return fig,ax
+
 # # ITPC
 # # ITPC循环单通道（一次显示一个channellist中的通道）
-def ITPC_channel(trial_sig, fs, time_points, period, band=[1,70], fig=None, show_flag=True):
+def ITPC_channel(trial_sig, fs, time_points, period, chan, band=[1,70], fig=None,ax=None, show_flag=True):
     #######
     # input:
     # trial_sig:shape=(trial,time) type=np.array
     #######
     frequencies = np.logspace(np.log10(band[0]),np.log10(band[1]))
     itpc = np.zeros((len(frequencies),period))
     for idx,f in enumerate(frequencies):
         itpc[idx] = ITPC(trial_sig,fs,f)
     
-    if fig == None:
-        fig = plt.figure()
-    ax = fig.add_subplot(111)
+    if ax==None:
+        if fig==None:
+            fig,ax = plt.subplots()
+        else:
+            ax = fig.add_subplot(111)
     levels = [0,0.2,0.4,0.6,0.8,1]
     ax_ = ax.pcolormesh(time_points,frequencies,itpc,cmap='jet',vmin=0)
     # plt.contourf(time_points,frequencies,itpc_mean,100,cmap='jet',vmax=1,vmin=0, extend='min')
     ax.set_yscale('symlog')
     fig.colorbar(ax_,ax=ax,ticks=levels,label='ITPC')
     # plt.yticks([1,3,5,10,30,50])
-    ax.set_title('ITPC channel')
+    ax.set_title(f'ITPC channel {chan+1}')
+    ax.set_ylabel('freq(Hz)')
+    ax.set_xlabel('time(s)')
     if show_flag:
         plt.show()
-    return fig
+    return fig,ax
 
 # # ITPC_location
-def ITPC_location(ct_sig,t_interval,fs,freq_band,channel_list,gridshape,fig=None,show_flag=True):
+def ITPC_location(x,y,ct_sig,interval,fs,freq_band,channel_list,bad_chan_list,gridshape,fig=None,show_flag=True):
     ###########
     # INPUT:
     # ct_sig:(channels,trials,time)
-    interval = [1.5,4]
+
 
     itpc_location = []
     for id in channel_list:
+        if id in bad_chan_list:
+            itpc_location.append(float('inf'))
+            continue
         frequencies = np.linspace(freq_band[0],freq_band[1],40)
         itpc = np.zeros(len(frequencies),)
 
         for idx,f in enumerate(frequencies):
-            itpc[idx] = np.mean(ITPC(ct_sig[id,:,int(interval[0]*fs):int(interval[1]*fs)],fs,f))
+            itpc[idx] = np.mean(ITPC(ct_sig[id,:,int(interval[0]):int(interval[1])],fs,f))
         
         itpc_location.append(np.mean(itpc))
     itpc_location = np.array(itpc_location).reshape(gridshape[0],gridshape[1])
     if fig==None:
         fig = plt.figure()
     ax = fig.add_subplot(111)
-    ax_ = ax.matshow(itpc_location,cmap='jet')
+    # ax_ = ax.matshow(x_grid,y_grid,itpc_location,cmap='jet')
+    ax_ = ax.pcolor(x,y,itpc_location ,cmap='jet')
     # plt.gca().invert_yaxis()
-    ax.set_title('ITPC of each location')
+    ax.set_title(f'{freq_band[0]}-{freq_band[1]}Hz ITPC of each location')
     fig.colorbar(ax_,ax=ax,label='ITPC')
+    ax.set_xlabel('AP(ms)')
+    ax.set_ylabel('ML(ms)')
+    ax.invert_xaxis()
     if show_flag:
         plt.show()
     return fig
 
 
 # # Average filtered LFP traveling wave-like behavior
-def plot_traveling_wave_behavior(ct_sig, fs, t_period, travel_axis_list, fig=None,show_flag=True):
+def plot_traveling_wave_behavior(ct_sig, fs, t_period, show_axis_loc, start, travel_axis_list, band, fig=None,cmap='PRGn',show_flag=True):
     # INPUT:
     # ct_sig:shape(channels,trials,time)
 
     if fig == None:
         fig = plt.figure()
     ax = fig.add_subplot(111)
-    t_pnt = np.array(t_period)*fs
+    t = np.array(np.array(t_period)*fs,int)-start
+    t_pnts = np.arange(t_period[0],t_period[1],1/fs)
     tw_mat = np.zeros((len(travel_axis_list),ct_sig.shape[2]))
+    # y = np.arange(-1,-len(travel_axis_list)-1,-1)
     for i,id in enumerate(travel_axis_list):
         tw_mat[i] = np.mean(ct_sig[id],0)
 
-    ax_ = ax.pcolor(tw_mat[:,int(t_pnt[0]):int(t_pnt[1])], cmap='PRGn')
-    ax.set_title('Normalized low-frequency Wave')
-    ax.invert_yaxis()
+    ax_ = ax.pcolor(t_pnts,show_axis_loc,tw_mat[:,t[0]:t[1]], cmap=cmap)
+    ax.set_title(f'Normalized {band[0]}-{band[1]}Hz Wave')
+    ax.set_xlabel('time(s)')
+    ax.set_ylabel('AP(ms)')
+    # ax.invert_yaxis()
     fig.colorbar(ax_,ax = ax, label='Voltage (μV)')
     if show_flag:
         plt.show()
     return fig
 
 
 # Phase-amplitude coupling MI
-def Phase_amplitude_coupling(trial_sig_low, trial_sig_high, n_bin = 20, fig=None, show_flag=True):
+def Phase_amplitude_coupling(trial_sig_low, trial_sig_high, chan,n_bin = 20, fig=None, show_flag=True):
     # INPUT:
     # trial_sig:shape(trials,time)
     # low: baseband
     # high: carrier
     if fig==None:
         fig = plt.figure()
     ax = fig.add_subplot(111)
@@ -182,73 +254,82 @@
     mid_interval = np.arange(-np.pi,np.pi,2*np.pi/n_bin)+np.pi/n_bin
 
     Phase = np.angle(analytic_sig_low)
     Amp = np.abs(analytic_sig_high)
     MI, MeanAmp = PAC_MI(Phase,Amp,n_bin)
 
     ax.bar(mid_interval,MeanAmp)
-    ax.set_title(f'channel  MI = {MI:.4f}')
+    ax.set_title(f'channel {chan+1}  MI = {MI:.4f}')
     ax.set_ylabel('Amp')
     ax.set_xlabel('Phase')
 
     if show_flag:
         plt.show()
     return fig
 
     
-def MI_maxAmpPhase_location(ct_sig_low, ct_sig_high, channel_list, bad_channel_list, gridshape, n_bin=20, fig=None, fig1=None, show_flag=True):
+def MI_maxAmpPhase_location(x,y,ct_sig_low, ct_sig_high, channel_list, bad_channel_list, gridshape, n_bin=20, fig=None, fig1=None, show_flag=True):
     # Phase Coupling MI
 
     if fig==None:
         fig = plt.figure()
     if fig1==None:
         fig1 = plt.figure()
     
     analytic_low = signal.hilbert(ct_sig_low)
     analytic_high = signal.hilbert(ct_sig_high)
 
     MI_Gr = np.zeros((len(channel_list),))
     MeanAmp_ct = np.zeros((len(channel_list),n_bin))
     for loc,id in enumerate(channel_list):
+        if id in bad_channel_list:
+            MI_Gr[loc] = float('inf')
+            continue
         Phase = np.angle(analytic_low[id])
         Amp = np.abs(analytic_high[id])
         MI_Gr[loc], MeanAmp_ct[id] = PAC_MI(Phase,Amp,n_bin)
 
-        if id in bad_channel_list:
-            MI_Gr[loc] = float('inf')
+
     MI_Gr = MI_Gr.reshape(gridshape[0],gridshape[1])
 
 
     ax = fig.add_subplot(111)
-    ax_ = ax.pcolor(MI_Gr ,cmap='rainbow')
+    ax_ = ax.pcolor(x,y,MI_Gr ,cmap='rainbow')
     ax.set_title('Phase Coupling MI')
-    ax.invert_yaxis()
+    ax.set_xlabel('AP(ms)')
+    ax.set_ylabel('ML(ms)')
+    ax.invert_xaxis()
     fig.colorbar(ax_,ax = ax,label='MI')
     
     mid_interval = np.arange(-np.pi,np.pi,2*np.pi/n_bin)+np.pi/n_bin
     PA_Gr = np.zeros(len(channel_list))
     for loc,id in enumerate(channel_list):
-        bin_num = int(np.array(np.where(MeanAmp_ct[id] == np.max(MeanAmp_ct[id]))))
-        PA_Gr[loc] = mid_interval[bin_num]
         if id in bad_channel_list:
             PA_Gr[loc] = float('inf')
+            continue
+        # print(np.array(np.where(MeanAmp_ct[id] == np.max(MeanAmp_ct[id]))))
+        bin_num = int(np.array(np.where(MeanAmp_ct[id] == np.max(MeanAmp_ct[id]))))
+        PA_Gr[loc] = mid_interval[bin_num]
+
     PA_Gr = PA_Gr.reshape((gridshape[0],gridshape[1]))
 
     PA_ax = fig1.add_subplot(111)
-    PA_ax_ = PA_ax.pcolor(PA_Gr, vmin=-np.pi, vmax=np.pi, cmap='gist_rainbow')
-    PA_ax.set_title('low_fre Phase with Maximum high_fre Amplitude')
-    PA_ax.invert_yaxis()
+    PA_ax_ = PA_ax.pcolor(x,y,PA_Gr, vmin=-np.pi, vmax=np.pi, cmap='gist_rainbow')
+    PA_ax.set_title('low-freq oscillation Phase with Maximum high-freq oscillation Amplitude')
+    PA_ax.invert_xaxis()
     fig1.colorbar(PA_ax_,ax = PA_ax,ticks=[-np.pi, -np.pi/2, 0, np.pi/2, np.pi],label='Phase of low-frequency oscillation')
+    PA_ax.set_xlabel('AP(ms)')
+    PA_ax.set_ylabel('ML(ms)')
     
     if show_flag:
         plt.show()
     return fig,fig1
 
 # # Spacial wave length and speed
-def waveLen_waveSpeed(ct_sig_low, ct_sig_high, fs, stim_start, channel_list, pixel_spacing_x, pixel_spacing_y, Thresh, gridshape, n_mode, tt, fig=None, show_flag=True):  
+def waveLen_waveSpeed(ct_sig_low, ct_sig_high, fs, stim_start, channel_list, pixel_spacing_x, pixel_spacing_y, Thresh, gridshape, n_mode, tt, fig1=None, fig2=None, show_flag=True):  
     
     # INPUT:
     # tt: 取信号比较明显的时刻作为计算时间相位的时间点
     
     SVD_tc_data = ct_sig_low.swapaxes(0,1)
     SVD_tc_data1 = ct_sig_high.swapaxes(0,1)
     
@@ -299,30 +380,33 @@
         ft_rct = reorgChannels(ft,channel_list,gridshape)
         
         high_waveLength_trials[trial] = 1/pm
         high_waveVelocity_trials[trial] = ft_rct/pm
 
 
     # 绘制波长波速直方图
-    fig = plt.figure(1)
-    f1_ax1 = fig.add_subplot(121)
+    if fig1 == None:
+        fig1 = plt.figure()
+    if fig2 == None:
+        fig2 = plt.figure()
+    f1_ax1 = fig1.add_subplot(111)
     low_wl = low_waveLength_trials[:,:,:,tt].reshape(-1)
     low_wl = low_wl[low_wl<10]
     high_wl = high_waveLength_trials[:,:,:,tt].reshape(-1)
     high_wl = high_wl[high_wl<10]
     num_bins = 100
     n, bins, patches = f1_ax1.hist(low_wl,num_bins, density=True,facecolor='blue', alpha=0.5) 
     n, bins, patches = f1_ax1.hist(high_wl,num_bins, density=True,facecolor='red', alpha=0.5) 
     # f1_ax1.set_xscale('log')
     f1_ax1.legend(['low-freq wave','high-freq wave'])
     f1_ax1.set_xlabel('WaveLength(mm/cycle)') 
     f1_ax1.set_ylabel('Probability') 
     f1_ax1.set_title('Histogram of WaveLength') 
 
-    f1_ax2 = fig.add_subplot(122)
+    f1_ax2 = fig2.add_subplot(111)
     low_wv = low_waveVelocity_trials[:,:,:,tt].reshape(-1)
     low_wv = low_wv[low_wv<200]
     low_wv = low_wv[low_wv>0]/1000
     high_wv = high_waveVelocity_trials[:,:,:,tt].reshape(-1)
     high_wv = high_wv[high_wv<200]
     high_wv = high_wv[high_wv>0]/1000
     # print(low_waveLength_trials[1,:,:,tt])
@@ -330,22 +414,23 @@
     n, bins, patches = f1_ax2.hist(low_wv,num_bins, density=True,facecolor='blue', alpha=0.5) 
     n, bins, patches = f1_ax2.hist(high_wv,num_bins, density=True,facecolor='red', alpha=0.5) 
     # f1_ax2.set_xscale('log')
     f1_ax2.legend(['low-freq wave','high-freq wave'])
     f1_ax2.set_xlabel('WaveVelocity(m/s)') 
     f1_ax2.set_ylabel('Probability') 
     f1_ax2.set_title('Histogram of WaveVelocity') 
-
+    fig1.subplots_adjust(bottom=0.2)
+    fig2.subplots_adjust(bottom=0.2)
     if show_flag:
         plt.show()
-    return fig
+    return fig1, fig2
 
 
     # Spacial PhaseDiff and gradient
-def spacial_phase_gradient(ct_sig, fs, stim_start, fast_response_channel, channel_list, bad_channel_list, pixel_spacing_x, pixel_spacing_y, Thresh, gridshape, n_mode, tt, fig=None, show_flag=True):
+def spacial_phase_gradient(x,y,ct_sig, fs, band, stim_start, fast_response_channel, channel_list, bad_channel_list, pixel_spacing_x, pixel_spacing_y, Thresh, gridshape, n_mode, tt, show_gdirection=True, fig=None, show_flag=True):
     SVD_tc_data = ct_sig.swapaxes(0,1)
     period = SVD_tc_data.shape[2]
 
     Tamp = np.zeros((SVD_tc_data.shape[0],SVD_tc_data.shape[2],n_mode))
     sig = np.zeros((SVD_tc_data.shape[0],n_mode))
     most_resp_mode = np.zeros((SVD_tc_data.shape[0],),dtype=int)
     mostRespSPhase = np.zeros((SVD_tc_data.shape[0],SVD_tc_data.shape[1]))
@@ -394,29 +479,33 @@
     AlignedVar_Gr = AlignedVar_Gr.reshape(gridshape)
     Pvals_Gr = Pvals_Gr.reshape(gridshape)
     # print(Pvals_Gr)
     # levels = np.arange(-np.pi, np.pi, 0.001)
     if fig==None:
         fig = plt.figure()
     ax = fig.add_subplot(111)
-    ax_ = ax.pcolor(AlignedAngles_Gr,vmin=-np.pi, vmax=np.pi ,cmap='rainbow')
-    ax.set_title('Phase Gridient')
+    ax_ = ax.pcolor(x-pixel_spacing_x/2,y-pixel_spacing_y/2,AlignedAngles_Gr,vmin=-np.pi, vmax=np.pi ,cmap='rainbow')
+    ax.set_title(f'{band[0]}-{band[1]}Hz Phase Gridient')
     # ax.set_title('high-frequency Phase Gridient')
     fig.colorbar(ax_,ax = ax,ticks=[-np.pi, -np.pi/2, 0, np.pi/2, np.pi],label='Phase')
-    _, ax = plot_vector_field(vec,norm=True,ax=ax,show_flag=False)
+    if show_gdirection:
+        _, ax = plot_vector_field(x,y,vec,pixel_spacing_x,pixel_spacing_y,norm=True,ax=ax,show_flag=False)
+    ax.invert_xaxis()
+    ax.set_xlabel('AP(ms)')
+    ax.set_ylabel('ML(ms)')
 
     if show_flag:
         plt.show()
     return fig, Pvals_Gr
     # # p值显示
     # plt.matshow(Pvals_Gr)
     # plt.title('Pvals')
     # plt.show()
 
-def spacial_phase_diff(ct_sig, stim_start, channel_diff,Thresh,n_mode,fig=None,show_flag=True):
+def spacial_phase_diff(ct_sig, stim_start, channel_diff,Thresh,n_mode,band,fig=None,show_flag=True):
     # # spacial phase difference
     if fig==None:
         fig=plt.figure()
     
     SVD_tc_data = ct_sig.swapaxes(0,1)
     period = SVD_tc_data.shape[2]
     mostRespSPhase = np.zeros((SVD_tc_data.shape[0],SVD_tc_data.shape[1]))
@@ -431,14 +520,37 @@
 
     bin_num = 20
     ph_dif = (mostRespSPhase[:,channel_diff[0]]-mostRespSPhase[:,channel_diff[1]])
     ph_dif[ph_dif<0] = ph_dif[ph_dif<0]+2*np.pi
     
     phaseDiff_pl_ax = fig.add_subplot(111,projection='polar')
     bars = phaseDiff_pl_ax.hist(ph_dif,bin_num,(0,2*np.pi))
-    phaseDiff_pl_ax.set_title('Phase difference(low-frequency)')
+    phaseDiff_pl_ax.set_title(f'{band[0]}-{band[1]}Hz Phase difference')
+    fig.subplots_adjust(top=0.8)
     # phaseDiff_pl_ax.set_title('Phase difference(high-frequency)')
     if show_flag:
         plt.show()
     return fig
 
+def SNR_plotting(x,y,SNR,chan_list,gridshape,fig=None,show_flag=True):
+    SNR_Gr = np.zeros(SNR.shape)
+    for loc,id in enumerate(chan_list):
+        SNR_Gr[loc] = SNR[id]
+    SNR_Gr = SNR_Gr.reshape(gridshape)
+    # print(SNR_Gr)
+    if fig==None:
+        fig = plt.figure()
+    ax = fig.add_subplot(111)
+    ax_ = ax.pcolor(x,y,SNR_Gr,cmap='rainbow')
+    ax.set_title(f'SNR(dB)')
+    # ax.set_title('high-frequency Phase Gridient')
+    fig.colorbar(ax_,ax = ax)
+    ax.invert_xaxis()
+    ax.set_xlabel('AP(ms)')
+    ax.set_ylabel('ML(ms)')
+    if show_flag:
+        plt.show()
+    return fig
+
+
+
```

### Comparing `brainanalysistool-0.0.3/brainanalysistool/preprocessing.py` & `brainanalysistool-0.0.4/brainanalysistool/preprocessing.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,27 +28,33 @@
     elif mod == 'highpass':
         b, a = signal.butter(4, 2*band/fs, 'highpass')
     elif mod == 'bandstop':
         b, a = signal.butter(4, [2*band[0]/fs,2*band[1]/fs], 'bandstop')
     filted_sig = signal.filtfilt(b, a, sig)
     return filted_sig
 
+def re_reference(sig,ref_chan):
+    # raw_sig removed powerline (chans*totaltime)
+    sig = sig-sig[ref_chan]
+    return sig
+
 def powerline_interference_filt(sig, fs, pl_freq=50):
-    sig = butter_filt(sig,fs,[2*(pl_freq-0.5)/fs,2*(pl_freq+0.5)/fs],'bandstop')
-    sig = butter_filt(sig,fs,[2*(2*pl_freq-0.5)/fs,2*(2*pl_freq+0.5)/fs],'bandstop')
-    sig = butter_filt(sig,fs,[2*(3*pl_freq-0.5)/fs,2*(3*pl_freq+0.5)/fs],'bandstop')
-    sig = butter_filt(sig,fs,[2*(4*pl_freq-0.5)/fs,2*(4*pl_freq+0.5)/fs],'bandstop')
+    sig = butter_filt(sig,fs,[pl_freq-0.5,pl_freq+0.5],'bandstop')
+    sig = butter_filt(sig,fs,[2*pl_freq-0.5,2*pl_freq+0.5],'bandstop')
+    sig = butter_filt(sig,fs,[3*pl_freq-0.5,3*pl_freq+0.5],'bandstop')
+    sig = butter_filt(sig,fs,[4*pl_freq-0.5,4*pl_freq+0.5],'bandstop')
     return sig
 
-def default_preprocess(sig,fs,band=[1,100],pl_freq=50):
-    sig = butter_filt(sig,fs,[2*band[0]/fs,2*band[1]/fs],'bandpass')
-    sig = powerline_interference_filt(sig,fs,pl_freq)
+def default_preprocess(sig,fs,band=[1,100],normed=False):
+    sig = butter_filt(sig,fs,band,'bandpass')
+    
     sig[np.isnan(sig)]=0
-    normed_filted_sig = (sig-np.mean(sig))/np.std(sig)
-    return normed_filted_sig
+    if normed:
+        sig = (sig-np.mean(sig))/np.std(sig)
+    return sig
 
 def sig_slice(sig, fs, start, end, time_array):
     #######
     # input:
     # sig.shape = (channels,long_time)
     # output:
     # sig.shape = (channels,trials,trial_time)
@@ -59,9 +65,30 @@
     channel_trial_data = np.zeros((sig.shape[0],time_array.shape[0],period))
     for id in range(sig.shape[0]):
         for trial,evoke in enumerate(time_array[:,0]):
             channel_trial_data_[id][trial] = sig[id][evoke+start:evoke+end]
             channel_trial_data[id][trial] = sig[id][evoke:evoke+period]
     return channel_trial_data_,channel_trial_data,time_points
 
+def gen_time_array(time_stamp,start_time):
+    evoke_time_array = time_stamp[:,0]
+    stim_end_array = time_stamp[:,1]
+    end_time_array = time_stamp[:,2]
+    evoke_time = np.zeros((time_stamp.shape[0],1),int)
+    stim_end = np.zeros((time_stamp.shape[0],1),int)
+    end_time = np.zeros((time_stamp.shape[0],1),int)
+    # print(evoke_time.shape[0])
+    for i in range(evoke_time_array.shape[0]):
+        evoke_time[i] = (evoke_time_array[i][0,-2]*60+evoke_time_array[i][0,-1])*1000 - start_time
+        stim_end[i] = (stim_end_array[i][0,-2]*60+stim_end_array[i][0,-1])*1000 - start_time
+        end_time[i] = (end_time_array[i][0,-2]*60+end_time_array[i][0,-1])*1000 - start_time
+
+    time_array = np.concatenate((evoke_time,stim_end,end_time),1)
+    return time_array
+
+def minus_baseline_ave(ct_sig,stim_start_pnt):
+    ct_sig = ct_sig[:,:]-np.mean(ct_sig[:,:,:stim_start_pnt],-1).reshape(ct_sig.shape[0],ct_sig.shape[1],1)
+    return ct_sig
+
+
 if __name__ == '__main__':
     fir_filt_bp()
```

### Comparing `brainanalysistool-0.0.3/setup.py` & `brainanalysistool-0.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 #!/usr/bin/env python
 from __future__ import print_function
 from setuptools import setup, find_packages
 import sys
  
 setup(
     name="brainanalysistool",
-    version="0.0.3",
+    version="0.0.4",
     author="Runmin Gan",
     author_email="354613146@qq.com",
-    description="Ecog analysis tool",
+    description="Brain/Neuron/Ecog analysis tool",
     long_description=open("README.md").read(),
+    long_description_content_type='text/plain',
     license="MIT",
-    url="https://github.com/RunminGan1218/Ecog-analysis-tool",
+    url="https://github.com/RunminGan1218/Brain-analysis-tool",
     packages=['brainanalysistool'],
     install_requires=[
         "matplotlib>=3.6.2",
         "numpy>=1.23.5",
         "PyWavelets>=1.4.1",
         "scipy>=1.9.3",
         "pactools>= 0.3.1",
         "pycwt>=0.3.0a22"
+        "PyWavelets>=1.4.1"
         ],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

