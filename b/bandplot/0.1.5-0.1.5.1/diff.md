# Comparing `tmp/bandplot-0.1.5-py3-none-any.whl.zip` & `tmp/bandplot-0.1.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 13124 bytes, number of entries: 10
--rw-rw-r--  2.0 unx       24 b- defN 23-May-15 02:20 bandplot/__init__.py
--rw-rw-r--  2.0 unx     6896 b- defN 23-May-15 02:20 bandplot/mass.py
--rw-rw-r--  2.0 unx    36761 b- defN 23-May-15 02:20 bandplot/plots.py
--rw-rw-r--  2.0 unx     6111 b- defN 23-May-15 02:20 bandplot/readdata.py
--rw-rw-r--  2.0 unx    20407 b- defN 23-May-15 02:20 bandplot/wrapper.py
--rw-rw-r--  2.0 unx     2951 b- defN 23-May-15 02:20 bandplot-0.1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-15 02:20 bandplot-0.1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       86 b- defN 23-May-15 02:20 bandplot-0.1.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-May-15 02:20 bandplot-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      774 b- defN 23-May-15 02:20 bandplot-0.1.5.dist-info/RECORD
-10 files, 74111 bytes uncompressed, 11812 bytes compressed:  84.1%
+Zip file size: 15058 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx       26 b- defN 23-May-16 03:55 bandplot/__init__.py
+-rw-rw-r--  2.0 unx     6905 b- defN 23-May-16 03:55 bandplot/mass.py
+-rw-rw-r--  2.0 unx    25472 b- defN 23-May-16 03:55 bandplot/plots.py
+-rw-rw-r--  2.0 unx    22228 b- defN 23-May-16 03:55 bandplot/pplots.py
+-rw-rw-r--  2.0 unx     6349 b- defN 23-May-16 03:55 bandplot/readdata.py
+-rw-rw-r--  2.0 unx    22112 b- defN 23-May-16 03:55 bandplot/wrapper.py
+-rw-rw-r--  2.0 unx     2996 b- defN 23-May-16 03:55 bandplot-0.1.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-16 03:55 bandplot-0.1.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-16 03:55 bandplot-0.1.5.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-16 03:55 bandplot-0.1.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      860 b- defN 23-May-16 03:55 bandplot-0.1.5.1.dist-info/RECORD
+11 files, 87135 bytes uncompressed, 13614 bytes compressed:  84.4%
```

## zipnote {}

```diff
@@ -3,29 +3,32 @@
 
 Filename: bandplot/mass.py
 Comment: 
 
 Filename: bandplot/plots.py
 Comment: 
 
+Filename: bandplot/pplots.py
+Comment: 
+
 Filename: bandplot/readdata.py
 Comment: 
 
 Filename: bandplot/wrapper.py
 Comment: 
 
-Filename: bandplot-0.1.5.dist-info/METADATA
+Filename: bandplot-0.1.5.1.dist-info/METADATA
 Comment: 
 
-Filename: bandplot-0.1.5.dist-info/WHEEL
+Filename: bandplot-0.1.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: bandplot-0.1.5.dist-info/entry_points.txt
+Filename: bandplot-0.1.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: bandplot-0.1.5.dist-info/top_level.txt
+Filename: bandplot-0.1.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bandplot-0.1.5.dist-info/RECORD
+Filename: bandplot-0.1.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bandplot/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.5"
+__version__ = "0.1.5.1"
```

## bandplot/mass.py

```diff
@@ -43,15 +43,15 @@
             points[i*2] = p_range
         elif data[points[i*2],0]==data[points[i*2]-1,0]:
             points[i*2] += -1
         if points[i*2+1] == p_range:
             points[i*2+1] = 0
         elif data[points[i*2+1],0]==data[points[i*2+1]+1,0]:
             points[i*2+1] += 1
-    calM = ['']*4 if abs(data_s[points[3],1]-data_s[points[5],2]) > 0.1 else ['']*6
+    calM = [''] * 4 if abs(data_s[points[3],1]-data_s[points[5],2]) > 0.1 else [''] * 6
     for i in range(len(calM)):
         if i%2 == 0:
             calM[i]=[data[points[i]-N+1:points[i]+1,0].copy(), data_s[points[i]-N+1:points[i]+1,int(i/2)].copy()]
         else:
             calM[i]=[data[points[i]:points[i]+N,0].copy(), data_s[points[i]:points[i]+N,int(i/2)].copy()]
     calM = np.array(calM)
     if len(calM) > 4:
@@ -66,18 +66,18 @@
         fun2 = np.polyfit(A_b[0,i-5:i], A_b[1,i-5:i], 2)
         p1 = np.poly1d(fun1)
         p2 = np.poly1d(fun2)
         if abs(p1(A_a[0,i]) - A_a[1,i]) > abs(p1(A_a[0,i]) - A_b[1,i]) or abs(p2(A_b[0,i]) - A_b[1,i]) > abs(p2(A_b[0,i]) - A_a[1,i]):
             A_a[1,i], A_b[1,i] = A_b[1,i], A_a[1,i]
 
 def npfit(calM):
-    pltlabel=['']*6
+    pltlabel=[''] * 6
     for i in range(len(calM)):
-        if abs(np.corrcoef(calM[i,0], calM[i,1])[0,1]) > 0.9:
-            pltlabel[i] = 0
+        if abs(np.corrcoef(calM[i,0], calM[i,1])[0,1]) > 0.99:
+            pltlabel[i] = 0.0
         else:
             fun = np.polyfit(calM[i,0], calM[i,1], 4)
             x = calM[i,0,-1] if i%2 == 0 else calM[i,0,0]
             le = 12*fun[0]*x**2 + 6*fun[1]*x + 2*fun[2]
             pltlabel[i] = (hp**2/(le*e*1e-20))/me
     if len(calM) > 4:
         if pltlabel[2] > pltlabel[4]:
```

## bandplot/plots.py

```diff
@@ -11,15 +11,15 @@
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
     plt.xticks(ticks,labels)
-    plt.legend(legend, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    plt.legend([legend[0]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.xlim(arr[0], arr[-1])
     plt.ylim(fig_p.vertical)
     plt.ylabel('Energy (eV)')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Noneispin2(arr, bands, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
@@ -44,15 +44,54 @@
     plt.ylim(fig_p.vertical)
     plt.ylabel('Energy (eV)')
     ax = plt.axes()
     g = ax.plot(arr[1], bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     ax.set_xlim(arr[1][0], arr[1][-1])
     ax.set_ylim(fig_p.vertical)
     ax.axis('off')
-    plt.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'medium'})
+    plt.gca().add_artist(L)
+    plt.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
+
+def Noneispin3(arr, bands, ticks, labels, legend, fig_p):
+    plt.figure(figsize=fig_p.size)
+    color = fig_p.color or ['r', 'k', 'b']
+    linestyle = fig_p.linestyle or ['-', '-.', ':']
+    linewidth = fig_p.linewidth or [0.8, 0.8, 0.8]
+    if len(color) < 3:
+        color = color + [''] * (3 - len(color))
+    if len(linestyle) < 3:
+        linestyle = linestyle + ['-'] * (3 - len(linestyle))
+    if len(linewidth) < 3:
+        linewidth = linewidth + [0.8] * (3 - len(linewidth))
+    f = plt.plot(arr[0], bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
+    plt.tick_params(axis='y', which='minor', color='gray')
+    plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
+    if len(ticks) > 2:
+        ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
+        for i in ticks[1:-1]:
+            plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
+    plt.xticks(ticks,labels)
+    plt.xlim(arr[0][0], arr[0][-1])
+    plt.ylim(fig_p.vertical)
+    plt.ylabel('Energy (eV)')
+    ax = plt.axes()
+    g = ax.plot(arr[1], bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
+    ax.set_xlim(arr[1][0], arr[1][-1])
+    ax.set_ylim(fig_p.vertical)
+    ax.axis('off')
+    af = plt.axes()
+    h = ax.plot(arr[2], bands[2].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
+    af.set_xlim(arr[2][0], arr[2][-1])
+    af.set_ylim(fig_p.vertical)
+    af.axis('off')
+    L = plt.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'medium'})
+    plt.gca().add_artist(L)
+    plt.legend([f[0], g[0], h[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Ispin(arr, bands, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
     linewidth = fig_p.linewidth or [0.8, 0.8]
@@ -60,15 +99,16 @@
         color = [color[0], 'k']
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
     if len(linewidth) == 1:
         linewidth = [linewidth[0], 0.8]
     p_up = plt.plot(arr, bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     p_do = plt.plot(arr, bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    plt.legend([p_up[0], p_do[0]], ['up', 'down'], frameon=False, prop={'style':'italic', 'size':'medium'}, loc=fig_p.location, alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
+    plt.legend([p_up[0], p_do[0]], ['up', 'down'], frameon=False, prop={'style':'italic', 'size':'medium'}, loc=fig_p.location,
+                alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
 
@@ -154,30 +194,100 @@
     ax2.set_ylim(fig_p.vertical)
     if len(labels) > 0:
         ax1.set_xticks(ticks,labels[:-1]+[''])
     else:
         ax1.set_xticks(ticks,labels)
     ax2.set_xticks(ticks,labels)
     ax1.set_ylabel('Energy (eV)')
+
+    ax1_f = fig.add_subplot(1,2,1)
+    g1 = ax1_f.plot(arr[1], bands[1][0].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
+    ax1_f.set_xlim(arr[1][0], arr[1][-1])
+    ax1_f.set_ylim(fig_p.vertical)
+    ax1_f.axis('off')
+    ax2_f = fig.add_subplot(1,2,2)
+    g2 = ax2_f.plot(arr[1], bands[1][1].T, color=color[3], linewidth=linewidth[3], linestyle=linestyle[3])
+    ax2_f.set_xlim(arr[1][0], arr[1][-1])
+    ax2_f.set_ylim(fig_p.vertical)
+    ax2_f.axis('off')
+
+    ax1.legend([f1[0], g1[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location,
+                alignment='left', title='up', title_fontproperties={'style':'italic', 'size':'medium'})
+    ax2.legend([f2[0], g2[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location,
+                alignment='left', title='down', title_fontproperties={'style':'italic', 'size':'medium'})
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
+
+def Dispin3(arr, bands, ticks, labels, legend, fig_p):
+    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=fig_p.size)
+    fig.subplots_adjust(wspace=0.0)
+    color = fig_p.color or ['r', 'r', 'k', 'k', 'b', 'b']
+    linestyle = fig_p.linestyle or ['-', '-', '-.', '-.', ':', ':']
+    linewidth = fig_p.linewidth or [0.8] * 6
+    if len(color) < 6:
+        color = color + [''] * (6 - len(color))
+    if len(linestyle) < 6:
+        linestyle = linestyle + ['-'] * (6 - len(linestyle))
+    if len(linewidth) < 6:
+        linewidth = linewidth + [0.8] * (6 - len(linewidth))
+    f1 = ax1.plot(arr[0], bands[0][0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
+    f2 = ax2.plot(arr[0], bands[0][1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
+    L = ax1.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'medium'})
+    ax1.add_artist(L)
+    ax1.tick_params(axis='y', which='minor', color='gray')
+    ax2.tick_params(axis='y', which='minor', color='gray')
+
+    ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
+    ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
+    ax2.set_yticklabels([])
+    if len(ticks) > 2:
+        ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
+        for i in ticks[1:-1]:
+            ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
+            ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
+
+    ax1.set_xlim(arr[0][0], arr[0][-1])
+    ax1.set_ylim(fig_p.vertical)
+    ax2.set_xlim(arr[0][0], arr[0][-1])
+    ax2.set_ylim(fig_p.vertical)
+    if len(labels) > 0:
+        ax1.set_xticks(ticks,labels[:-1]+[''])
+    else:
+        ax1.set_xticks(ticks,labels)
+    ax2.set_xticks(ticks,labels)
+    ax1.set_ylabel('Energy (eV)')
+
     ax1_f = fig.add_subplot(1,2,1)
     g1 = ax1_f.plot(arr[1], bands[1][0].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
     ax1_f.set_xlim(arr[1][0], arr[1][-1])
     ax1_f.set_ylim(fig_p.vertical)
     ax1_f.axis('off')
     ax2_f = fig.add_subplot(1,2,2)
     g2 = ax2_f.plot(arr[1], bands[1][1].T, color=color[3], linewidth=linewidth[3], linestyle=linestyle[3])
     ax2_f.set_xlim(arr[1][0], arr[1][-1])
     ax2_f.set_ylim(fig_p.vertical)
     ax2_f.axis('off')
-    ax1.legend([f1[0], g1[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title='up', title_fontproperties={'style':'italic', 'size':'medium'})
-    ax2.legend([f2[0], g2[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title='down', title_fontproperties={'style':'italic', 'size':'medium'})
+
+    ax1_g = fig.add_subplot(1,2,1)
+    h1 = ax1_f.plot(arr[2], bands[2][0].T, color=color[4], linewidth=linewidth[4], linestyle=linestyle[4])
+    ax1_g.set_xlim(arr[2][0], arr[2][-1])
+    ax1_g.set_ylim(fig_p.vertical)
+    ax1_g.axis('off')
+    ax2_g = fig.add_subplot(1,2,2)
+    h2 = ax2_f.plot(arr[2], bands[2][1].T, color=color[5], linewidth=linewidth[5], linestyle=linestyle[5])
+    ax2_g.set_xlim(arr[2][0], arr[2][-1])
+    ax2_g.set_ylim(fig_p.vertical)
+    ax2_g.axis('off')
+    ax1.legend([f1[0], g1[0], h1[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=fig_p.location,
+                alignment='left', title='up', title_fontproperties={'style':'italic', 'size':'medium'})
+    ax2.legend([f2[0], g2[0], h2[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=fig_p.location,
+                alignment='left', title='down', title_fontproperties={'style':'italic', 'size':'medium'})
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def NoneispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, width_ratios, legend, fig_p):
-    fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-width_ratios, width_ratios], figsize=fig_p.size)
+def NoneispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p):
+    fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-fig_p.width_ratios, fig_p.width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
 
     ax1.plot(arr, bands.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     num = len(index_f)
@@ -197,15 +307,15 @@
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=fig_p.fill)
         else:
             ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+1], linestyle=linestyle[i+1])
             if fig_p.fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
 
-    ax1.legend(legend, frameon=False, prop={'size':'small'}, loc=fig_p.location)
+    ax1.legend([legend[0]], frameon=False, prop={'size':'small'}, loc=fig_p.location)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.minorticks_on()
     ax2.tick_params(axis='both', which='minor', color='gray')
     ax2.set_yticklabels([])
     ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location, alignment='left', title="Density of states", title_fontproperties={'size':'small'})
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
@@ -220,16 +330,16 @@
     ax2.set_xlim(fig_p.horizontal)
     ax2.set_ylim(fig_p.vertical)
     ax1.set_xticks(ticks,labels)
     ax2.tick_params(axis='x', labelsize='x-small', labelcolor='dimgray', labelrotation=-90, pad=1.5)
     ax1.set_ylabel('Energy (eV)')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def IspinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, width_ratios, legend, fig_p):
-    fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-width_ratios, width_ratios], figsize=fig_p.size)
+def IspinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p):
+    fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-fig_p.width_ratios, fig_p.width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
     linewidth = fig_p.linewidth or [0.8, 0.8]
     if len(color) == 1:
         color = [color[0], 'k']
     if len(linestyle) == 1:
@@ -278,16 +388,16 @@
     ax2.set_xlim(fig_p.horizontal)
     ax2.set_ylim(fig_p.vertical)
     ax1.set_xticks(ticks,labels)
     ax2.tick_params(axis='x', labelsize='x-small', labelcolor='dimgray', labelrotation=-90, pad=1.5)
     ax1.set_ylabel('Energy (eV)')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def DispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, width_ratios, legend, fig_p):
-    fig, (ax1, ax2, ax3) = plt.subplots(1, 3, width_ratios=[0.4*(1-width_ratios), 0.4*(1-width_ratios), width_ratios], figsize=fig_p.size)
+def DispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p):
+    fig, (ax1, ax2, ax3) = plt.subplots(1, 3, width_ratios=[0.5*(1-fig_p.width_ratios), 0.5*(1-fig_p.width_ratios), fig_p.width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
     linewidth = fig_p.linewidth or [0.8, 0.8]
     if len(color) == 1:
         color = [color[0], 'k']
     if len(linestyle) == 1:
@@ -401,361 +511,14 @@
 
         plt.tick_params(axis='x', labelsize='medium', labelcolor='dimgray')
         plt.ylim(fig_p.vertical)
         plt.xlim(fig_p.horizontal)
         plt.ylabel('Energy (eV)')
         plt.xlabel('Density of states, electrons/eV')
 
+    L = plt.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'medium'})
+    plt.gca().add_artist(L)
     plt.axvline(linewidth=0.4, linestyle='-.', c='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
-    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
-
-# pbandplot
-def Broken(arr, fre, ticks, labels, broken, height_ratio, legend, fig_p):
-    fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True, height_ratios=[height_ratio, 1-height_ratio], figsize=fig_p.size)
-    fig.subplots_adjust(hspace=0.0)
-    color = fig_p.color or ['r']
-    linestyle = fig_p.linestyle or ['-']
-    linewidth = fig_p.linewidth or [0.8]
-    ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    ax2.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    plt.xlim(arr[0], arr[-1])
-    vertical = fig_p.vertical or plt.ylim()
-    ax1.set_ylim(broken[1], vertical[1])
-    ax2.set_ylim(vertical[0], broken[0])
-    ax1.spines['bottom'].set_visible(False)
-    ax2.spines['top'].set_visible(False)
-    ax1.xaxis.set_ticks_position(position='none')
-    ax1.tick_params(axis='y', which='minor', color='darkgray')
-    ax1.tick_params(axis='y', labelsize='small', labelcolor='dimgray', labelrotation=-60)
-    ax2.tick_params(axis='y', which='minor', color='gray')
-    ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    if len(ticks) > 2:
-        ticks[0],ticks[-1] = arr[0],arr[-1]
-        for i in ticks[1:-1]:
-            ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-            ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
-    ax2.legend(legend, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
-    plt.xticks(ticks,labels)
-    plt.suptitle('Frequency (THz)', rotation=90, x=0.06, y=0.6, size='medium')
-    kwargs = dict(marker=[(-1, -1), (1, 1)], markersize=6,
-                  linestyle='', color='k', mec='k', mew=1, clip_on=False)
-    ax1.plot([0, 1], [0.02, 0.02], transform=ax1.transAxes, **kwargs)
-    ax2.plot([0, 1], [0.98, 0.98], transform=ax2.transAxes, **kwargs)
-    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
-
-def Broken2(arr, fre, ticks, labels, broken, height_ratio, legend, fig_p):
-    fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True, height_ratios=[height_ratio, 1-height_ratio], figsize=fig_p.size)
-    fig.subplots_adjust(hspace=0.0)
-    color = fig_p.color or ['r', 'k']
-    linestyle = fig_p.linestyle or ['-', '-.']
-    linewidth = fig_p.linewidth or [0.8, 0.8]
-    if len(color) == 1:
-        color = [color[0], 'k']
-    if len(linestyle) == 1:
-        linestyle = [linestyle[0], '-.']
-    if len(linewidth) == 1:
-        linewidth = [linewidth[0], 0.8]
-    ax1.plot(arr[0], fre[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    f = ax2.plot(arr[0], fre[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    plt.xlim(arr[0][0], arr[0][-1])
-    vertical = fig_p.vertical or plt.ylim()
-    ax1.set_ylim(broken[1], vertical[1])
-    ax2.set_ylim(vertical[0], broken[0])
-    ax1.spines['bottom'].set_visible(False)
-    ax2.spines['top'].set_visible(False)
-    ax1.xaxis.set_ticks_position(position='none')
-    ax1.tick_params(axis='y', which='minor', color='darkgray')
-    ax1.tick_params(axis='y', labelsize='small', labelcolor='dimgray', labelrotation=-60)
-    ax2.tick_params(axis='y', which='minor', color='gray')
-    ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    if len(ticks) > 2:
-        ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
-        for i in ticks[1:-1]:
-            ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-            ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
-    plt.xticks(ticks,labels)
-    plt.suptitle('Frequency (THz)', rotation=90, x=0.06, y=0.6, size='medium')
-    kwargs = dict(marker=[(-1, -1), (1, 1)], markersize=6,
-                  linestyle='', color='k', mec='k', mew=1, clip_on=False)
-    ax1.plot([0, 1], [0.02, 0.02], transform=ax1.transAxes, **kwargs)
-    ax2.plot([0, 1], [0.98, 0.98], transform=ax2.transAxes, **kwargs)
-    ax1_f = fig.add_subplot(2,1,1)
-    ax1_f.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    ax1_f.set_xlim(arr[1][0], arr[1][-1])
-    ax1_f.set_ylim(broken[1], vertical[1])
-    ax1_f.axis('off')
-    ax2_f = fig.add_subplot(2,1,2)
-    g = ax2_f.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    ax2_f.set_xlim(arr[1][0], arr[1][-1])
-    ax2_f.set_ylim(vertical[0], broken[0])
-    ax2_f.axis('off')
-    ax2.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
-    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
-
-def Nobroken(arr, fre, ticks, labels, legend, fig_p):
-    plt.figure(figsize=fig_p.size)
-    color = fig_p.color or ['r']
-    linestyle = fig_p.linestyle or ['-']
-    linewidth = fig_p.linewidth or [0.8]
-    plt.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    plt.tick_params(axis='y', which='minor', color='gray')
-    plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    if len(ticks) > 2:
-        ticks[0],ticks[-1] = arr[0],arr[-1]
-        for i in ticks[1:-1]:
-            plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
-    plt.legend(legend, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
-    plt.xticks(ticks,labels)
-    plt.xlim(arr[0], arr[-1])
-    plt.ylim(fig_p.vertical)
-    plt.ylabel('Frequency (THz)')
-    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
-
-def Nobroken2(arr, fre, ticks, labels, legend, fig_p):
-    plt.figure(figsize=fig_p.size)
-    color = fig_p.color or ['r', 'k']
-    linestyle = fig_p.linestyle or ['-', '-.']
-    linewidth = fig_p.linewidth or [0.8, 0.8]
-    if len(color) == 1:
-        color = [color[0], 'k']
-    if len(linestyle) == 1:
-        linestyle = [linestyle[0], '-.']
-    if len(linewidth) == 1:
-        linewidth = [linewidth[0], 0.8]
-    f = plt.plot(arr[0], fre[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    plt.tick_params(axis='y', which='minor', color='gray')
-    plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    if len(ticks) > 2:
-        ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
-        for i in ticks[1:-1]:
-            plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
-    plt.xticks(ticks,labels)
-    plt.xlim(arr[0][0], arr[0][-1])
-    ylim=plt.ylim(fig_p.vertical)
-    plt.ylabel('Frequency (THz)')
-    ax = plt.axes()
-    g = ax.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    ax.set_xlim(arr[1][0], arr[1][-1])
-    ax.set_ylim(ylim)
-    ax.axis('off')
-    plt.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
-    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
-
-def BrokenWd(arr, fre, ticks, labels, broken, height_ratio, darr, dele, elements, width_ratios, legend, fig_p):
-    fig, ((ax1, ax2), (ax3, ax4)) = plt.subplots(2, 2, height_ratios=[height_ratio, 1-height_ratio], width_ratios=[1-width_ratios, width_ratios], figsize=fig_p.size)
-    fig.subplots_adjust(wspace=0.0, hspace=0.0)
-    color = fig_p.color or ['r']
-    linestyle = fig_p.linestyle or ['-']
-    linewidth = fig_p.linewidth or [0.8]
-    ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    ax3.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    num = dele.shape[-1]
-    p_dos = []
-    if num + 1 > len(color):
-        color = color + [''] * (num - len(color) + 1)
-
-    if num + 1 > len(linestyle):
-        linestyle = linestyle + ['-'] * (num - len(linestyle) + 1)
-
-    if num + 1 > len(linewidth):
-        linewidth = linewidth + [0.8] * (num - len(linewidth) + 1)
-
-    for i in range(num):
-        if color[i+1]:
-            ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
-            p_dos = p_dos + ax4.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
-            if fig_p.fill:
-                plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=fig_p.fill)
-        else:
-            ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1])
-            p_dos = p_dos + ax4.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1])
-            if fig_p.fill:
-                plt.fill_between(dele[:,i], darr, 0, alpha=fig_p.fill)
-
-    ax1.set_xlim(arr[0], arr[-1])
-    ax3.set_xlim(arr[0], arr[-1])
-    vertical = fig_p.vertical or ax1.get_ylim()
-
-    ax1.set_ylim(broken[1], vertical[1])
-    ax2.set_ylim(broken[1], vertical[1])
-    ax3.set_ylim(vertical[0], broken[0])
-    ax4.set_ylim(vertical[0], broken[0])
-    ax2.set_xlim(fig_p.horizontal)
-    ax4.set_xlim(fig_p.horizontal)
-    ax1.spines['bottom'].set_visible(False)
-    ax2.spines['bottom'].set_visible(False)
-    ax3.spines['top'].set_visible(False)
-    ax4.spines['top'].set_visible(False)
-    ax1.xaxis.set_ticks_position('none')
-    ax2.xaxis.set_ticks_position('none')
-    ax1.tick_params(axis='y', which='minor', color='darkgray')
-    ax1.tick_params(axis='y', labelsize='small', labelcolor='dimgray', labelrotation=-60)
-    ax3.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    ax4.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    ax2.tick_params(axis='y', which='minor', color='darkgray')
-    ax3.tick_params(axis='y', which='minor', color='gray')
-    ax4.minorticks_on()
-    ax4.tick_params(axis='x', labelsize='small', labelcolor='dimgray', labelrotation=-90, pad=3)
-    ax4.tick_params(axis='both', which='minor', color='gray')
-    ax1.set_xticklabels([])
-    ax2.set_xticklabels([])
-    ax2.set_yticklabels([])
-    ax4.set_yticklabels([])
-    ax2.axvline(linewidth=0.4, linestyle='-.', c='gray')
-    ax4.axvline(linewidth=0.4, linestyle='-.', c='gray')
-    if num > len(elements):
-        elements = elements + [''] * (num - len(elements))
-    elif num < len(elements):
-        if num == 1:
-            elements = ['$tdos$']
-        else:
-            elements = elements[:num]
-
-    ax3.legend(legend, frameon=False, prop={'size':'small'}, loc=fig_p.location)
-    ax4.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location, alignment='left', title="Phonon DOS", title_fontproperties={'size':'small'})
-    if len(ticks) > 2:
-        ticks[0],ticks[-1] = arr[0],arr[-1]
-        for i in ticks[1:-1]:
-            ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-            ax3.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
-    ax3.set_xticks(ticks,labels)
-    plt.suptitle('Frequency (THz)', rotation=90, x=0.06, y=0.6, size='medium')
-    kwargs = dict(marker=[(-1, -1), (1, 1)], markersize=6,
-                  linestyle='', color='k', mec='k', mew=1, clip_on=False)
-    ax1.plot([0, 1], [0.02, 0.02], transform=ax1.transAxes, **kwargs)
-    ax3.plot([0, 1], [0.98, 0.98], transform=ax3.transAxes, **kwargs)
-    ax2.plot(1, 0.02, transform=ax2.transAxes, **kwargs)
-    ax4.plot(1, 0.98, transform=ax4.transAxes, **kwargs)
-    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
-
-def NobrokenWd(arr, fre, ticks, labels, darr, dele, elements, width_ratios, legend, fig_p):
-    fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-width_ratios, width_ratios], figsize=fig_p.size)
-    fig.subplots_adjust(wspace=0.0)
-    color = fig_p.color or ['r']
-    linestyle = fig_p.linestyle or ['-']
-    linewidth = fig_p.linewidth or [0.8]
-    ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    num = dele.shape[-1]
-    p_dos = []
-    if num + 1 > len(color):
-        color = color + [''] * (num - len(color) + 1)
-
-    if num + 1 > len(linestyle):
-        linestyle = linestyle + ['-'] * (num - len(linestyle) + 1)
-
-    if num + 1 > len(linewidth):
-        linewidth = linewidth + [0.8] * (num - len(linewidth) + 1)
-
-    for i in range(num):
-        if color[i+1]:
-            p_dos = p_dos + ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
-            if fig_p.fill:
-                plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=fig_p.fill)
-        else:
-            p_dos = p_dos + ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1])
-            if fig_p.fill:
-                plt.fill_between(dele[:,i], darr, 0, alpha=fig_p.fill)
-
-    ax1.set_xlim(arr[0], arr[-1])
-    vertical = fig_p.vertical or ax1.get_ylim()
-
-    ax1.set_ylim(vertical)
-    ax2.set_ylim(vertical)
-    ax2.set_xlim(fig_p.horizontal)
-    ax1.tick_params(axis='y', which='minor', color='gray')
-    ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    ax2.minorticks_on()
-    ax2.tick_params(axis='x', labelsize='small', labelcolor='dimgray', labelrotation=-90, pad=3)
-    ax2.tick_params(axis='both', which='minor', color='gray')
-    ax2.set_yticklabels([])
-    ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    if num > len(elements):
-        elements = elements + [''] * (num - len(elements))
-    elif num < len(elements):
-        if num == 1:
-            elements = ['$tdos$']
-        else:
-            elements = elements[:num]
-
-    ax1.legend(legend, frameon=False, prop={'size':'small'}, loc=fig_p.location)
-    ax2.axvline(linewidth=0.4,linestyle='-.',c='dimgray')
-    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location, alignment='left', title="Phonon DOS", title_fontproperties={'size':'small'})
-    if len(ticks) > 2:
-        ticks[0],ticks[-1] = arr[0],arr[-1]
-        for i in ticks[1:-1]:
-            ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
-    ax1.set_xticks(ticks,labels)
-    ax1.set_ylabel('Frequency (THz)')
-    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
-
-def dosfile(darr, dele, elements, legend, fig_p):
-    plt.figure(figsize=fig_p.size)
-    plt.minorticks_on()
-    plt.tick_params(axis='both', which='minor', color='gray')
-    num = dele.shape[-1]
-    color = fig_p.color
-    linestyle = fig_p.linestyle
-    linewidth = fig_p.linewidth
-    p_dos = []
-    if num > len(color):
-        color = color + [''] * (num - len(color))
-
-    if num > len(linestyle):
-        linestyle = linestyle + ['-'] * (num - len(linestyle))
-
-    if num > len(linewidth):
-        linewidth = linewidth + [0.8] * (num - len(linewidth))
-
-    if fig_p.exchange:
-        for i in range(num):
-            if color[i]:
-                p_dos = p_dos + plt.plot(darr, dele[:,i], linewidth=linewidth[i], linestyle=linestyle[i], color=color[i])
-                if fig_p.fill:
-                    plt.fill_between(darr, dele[:,i], 0, color=color[i], alpha=fig_p.fill)
-            else:
-                p_dos = p_dos + plt.plot(darr, dele[:,i], linewidth=linewidth[i], linestyle=linestyle[i])
-                if fig_p.fill:
-                    plt.fill_between(darr, dele[:,i], 0, alpha=fig_p.fill)
-
-        plt.xlim(fig_p.vertical)
-        plt.ylim(fig_p.horizontal)
-        plt.xlabel('Frequency (THz)')
-        plt.ylabel('Phonon DOS')
-        plt.tick_params(axis='y', labelsize='medium', labelcolor='dimgray')
-    else:
-        for i in range(num):
-            if color[i]:
-                p_dos = p_dos + plt.plot(dele[:,i], darr, linewidth=linewidth[i], linestyle=linestyle[i], color=color[i])
-                if fig_p.fill:
-                    plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=fig_p.fill)
-            else:
-                p_dos = p_dos + plt.plot(dele[:,i], darr, linewidth=linewidth[i], linestyle=linestyle[i])
-                if fig_p.fill:
-                    plt.fill_between(dele[:,i], darr, 0, alpha=fig_p.fill)
-
-        plt.ylim(fig_p.vertical)
-        plt.xlim(fig_p.horizontal)
-        plt.ylabel('Frequency (THz)')
-        plt.xlabel('Phonon DOS')
-        plt.tick_params(axis='x', labelsize='medium', labelcolor='dimgray')
-
-    plt.axvline(linewidth=0.4, linestyle='-.', c='gray')
-    plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    if num > len(elements):
-        elements = elements + [''] * (num - len(elements))
-    elif num < len(elements):
-        if num == 1:
-            elements = ['$tdos$']
-        else:
-            elements = elements[:num]
-
-    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
+    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
```

## bandplot/readdata.py

```diff
@@ -19,25 +19,21 @@
 
 def dos(DOS):
     ARR = []
     ELE = []
     s_elements = []
     for pdos in DOS:
         with open(pdos, "r") as main_file:
-            lines = main_file.readlines()
-        arr = []
-        ele = []
-        for line in lines[1:]:
-            values = [float(val) for val in line.split() if val]
-            if values:
-                arr.append(values[0])
-                ele.append(values[1:])
-        ARR.append(np.array(arr))
-        ELE.append(np.array(ele))
-        s_elements.append([re.sub('.dat|^[A-Za-z]+_', '', pdos)] + lines[0].split()[1:])
+            first_line = next(main_file)
+        data = np.loadtxt(pdos)
+        arr = data[:, 0]
+        ele = data[:, 1:]
+        ARR.append(arr)
+        ELE.append(ele)
+        s_elements.append([re.sub('.dat|^[A-Za-z]+_', '', pdos)] + first_line.split()[1:])
     return ARR, ELE, s_elements
 
 def select(s_elements, partial):
     partial = [i for i in partial if i.strip()]
     num = len(s_elements)
     if not partial:
         index = [(i, -1) for i in range(num)]
@@ -53,22 +49,24 @@
                         if j == 0 or sub_elem not in str_list:
                             continue
                         index.append((i, j))
             else:
                 str_list = [i.strip() for i in str0.split('-') if i.strip()]
                 if len(str_list) == 1:
                     for i, elem in enumerate(s_elements):
-                        if elem[0] == str_list[0]:
+                        if elem[0] == str_list[0] or elem[0] == str_list[0]+'_UP' or elem[0] == str_list[0]+'_DW':
                             index += [(i, j) for j in range(1, len(elem))]
                 elif len(str_list) == 2:
                     for i, elem in enumerate(s_elements):
-                        if elem[0] == str_list[0]:
+                        if elem[0] == str_list[0] or elem[0] == str_list[0]+'_UP' or elem[0] == str_list[0]+'_DW':
                             index += [(i, j) for j, sub_elem in enumerate(elem)
                                       if j > 0 and sub_elem in str_list[1].split(',')]
-    labels_elements = [s_elements[i[0]][0] + '-$' + s_elements[i[0]][i[1]] + '$' for i in index]
+    labels_elements = [s_elements[i[0]][0].replace('_DW','')+'-$'+s_elements[i[0]][i[1]]+'$'+' ($dw$)' if s_elements[i[0]][0].endswith('_DW')
+                  else s_elements[i[0]][0].replace('_UP','')+'-$'+s_elements[i[0]][i[1]]+'$'+' ($up$)' if s_elements[i[0]][0].endswith('_UP')
+                  else s_elements[i[0]][0]+'-$'+s_elements[i[0]][i[1]]+'$' for i in index]
     index_f = [(i, j-1) if j > 0 else (i, j) for i, j in index]
     return index_f, labels_elements
 
 def bands(PLOT):
     with open(PLOT, "r") as main_file:
         lines = main_file.readlines()
     str0 = lines[0].split()
```

## bandplot/wrapper.py

```diff
@@ -1,10 +1,10 @@
 import argparse, os, re, platform, glob
 import matplotlib.pyplot as plt
-from bandplot import plots, readdata
+from bandplot import plots, pplots, readdata
 from bandplot import __version__
 
 plt.rcParams['xtick.direction'] = 'in'
 plt.rcParams['ytick.direction'] = 'in'
 plt.rcParams['ytick.minor.visible'] = True
 plt.rcParams["mathtext.fontset"] = 'cm'
 
@@ -12,21 +12,22 @@
     def __init__(self, **kwargs):
         for key, value in kwargs.items():
             if isinstance(value, str):
                 exec('self.%s = "%s"' %(key, value))
             else:
                 exec('self.%s = %s' %(key, value))
 
+# bandplot
 def main():
     parser = argparse.ArgumentParser(description='Plot the band structure or DOS from vaspkit result.',
                                      epilog='''
 Example:
-bandplot -i BAND.dat -o BAND.png -l g m k g -d PDOS* -z
+bandplot -i BAND.dat -o BAND.png -l g m k g -d PDOS* -z -p C-s,p Ti-d
 ''',
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
+    formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('-v', "--version",    action="version",     version="bandplot "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
     parser.add_argument('-s', "--size",       type=int,   nargs=2,  help='figure size: width, height')
     parser.add_argument('-b', "--divided",    action='store_true',  help="plot the up and down spin in divided subplot")
     parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="energy (eV) range, default: [-5.0, 5.0]")
     parser.add_argument('-g', "--legend",     type=str,             nargs='+', help="legend labels", default=[])
     parser.add_argument('-L', "--location",   type=str.lower,       choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right',
                                                                              'center left', 'center right', 'lower center', 'upper center', 'center'],
@@ -42,17 +43,17 @@
     parser.add_argument('-o', "--output",     type=str,             help="plot figure filename, default: BAND.png", default="BAND.png")
     parser.add_argument('-q', "--dpi",        type=int,             help="dpi of the figure, default: 500", default=500)
     parser.add_argument('-j', "--klabels",    type=str,             help="filename of KLABELS, default: KLABELS", default="KLABELS")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             nargs='+', default=[], help="plot DOS from .dat file, or file list")
     parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Density of states, electrons/eV range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of DOS")
-    parser.add_argument('-p', "--partial",    type=str,             nargs='+', default=[], help='the partial DOS to plot, s p d')
+    parser.add_argument('-p', "--partial",    type=str,             nargs='+', default=[], help='the partial DOS to plot, s p d, or symbol-s,p,d')
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
-    parser.add_argument('-r', "--wratios",    type=float,           help='width ratio for DOS subplot')
+    parser.add_argument('-W', "--wratios",    type=float,           help='width ratio for DOS subplot')
     parser.add_argument('-z', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
     parser.add_argument('-Z', "--alpha",      type=float,           help='alpha value for filling region, default=0.2', default=0.2)
     parser.add_argument('-f', "--font",       type=str,             help="font to use", default='STIXGeneral')
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
@@ -110,45 +111,68 @@
         labels=[re.sub('GAMMA|Gamma|G', 'Γ', re.sub('Undefined|Un|[0-9]', '', i)) for i in klabels]
 
     if len(ticks) > len(labels):
         labels = labels + [''] * (len(ticks) - len(labels))
     elif len(ticks) < len(labels):
         labels = labels[:len(ticks)]
 
+    width_ratios = args.wratios or (0.3 if args.divided else 0.5)
+
     fig_p = cla_fig(output=args.output, size=args.size, vertical=args.vertical, horizontal=args.horizontal,
                     color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi,
-                    exchange=args.exchange, fill=args.fill)
+                    width_ratios=width_ratios, exchange=args.exchange, fill=args.fill)
 # calculate the effective masses
     if args.mass:
         if not fig_p.vertical:
             fig_p.vertical = [-5.0, 5.0]
         from bandplot import mass
         if os.path.exists("BAND_GAP"):
             lumo, homo, homo_c, filename = mass.get_vbm_cbm("BAND_GAP")
             Extension = [len(lumo), len(homo), len(homo_c), len(filename)]
             if all(x == 1 for x in Extension):
                 data = mass.bs_dat_read(filename)
                 calM = mass.dat_read(data[0], lumo[0], homo[0], homo_c[0], args.scale)
                 pltlabel = mass.npfit(calM)
                 mass.plot(data[0], calM, pltlabel, ticks, labels, legend, fig_p)
+                print("{:<8}{:<8}{:<8}{:<8}{:<8}{:<8}".format("e_x","e_y","h1_x","h1_y","h2_x","h2_y"))
+                for i in pltlabel:
+                    if isinstance(i, float):
+                        print("{:<8.3f}".format(i), end='')
+                    else:
+                        print("{:<8s}".format('-'), end='')
+                print()
             elif all(x == 2 for x in Extension):
                 data = mass.bs_dat_read(filename)
                 calM_u = mass.dat_read(data[0], lumo[0], homo[0], homo_c[0], args.scale)
                 calM_d = mass.dat_read(data[1], lumo[1], homo[1], homo_c[1], args.scale)
                 pltlabel_u = mass.npfit(calM_u)
                 pltlabel_d = mass.npfit(calM_d)
                 mass.plot2(data, calM_u, pltlabel_u, calM_d, pltlabel_d, ticks, labels, legend, fig_p)
+                print("{:<8}{:<8}{:<8}{:<8}{:<8}{:<8}".format("e_x","e_y","h1_x","h1_y","h2_x","h2_y"))
+                for i in pltlabel_u:
+                    if isinstance(i, float):
+                        print("{:<8.3f}".format(i), end='')
+                    else:
+                        print("{:<8s}".format('-'), end='')
+                print()
+                for i in pltlabel_d:
+                    if isinstance(i, float):
+                        print("{:<8.3f}".format(i), end='')
+                    else:
+                        print("{:<8s}".format('-'), end='')
+                print()
             else:
                 print("ERROR: Input file mismatch.")
         else:
             print("ERROR: BAND_GAP file does not exist.")
 # plot Band Structure
     else:
         bandfile = [f for i in args.input for f in glob.glob(i)]
-        if len(bandfile) == 1:
+        len_bandfile = len(bandfile)
+        if len_bandfile == 1:
             if not fig_p.vertical:
                 fig_p.vertical = [-5.0, 5.0]
             arr, bands, ispin = readdata.bands(bandfile[0])
             if not dosfiles:
                 if ispin == "Noneispin":
                     plots.Noneispin(arr, bands, ticks, labels, legend, fig_p)
                 elif ispin == "Ispin" and not args.divided:
@@ -156,88 +180,86 @@
                 elif ispin == "Ispin" and args.divided:
                     plots.Dispin(arr, bands, ticks, labels, legend, fig_p)
             else:
                 darr, dele, s_elements = readdata.dos(args.dos)
                 index_f, labels_elements = readdata.select(s_elements, args.partial)
                 if not elements:
                     elements = labels_elements
-                if not args.wratios:
-                    if not args.divided:
-                        width_ratios = 0.5
-                    else:
-                        width_ratios = 0.3
-                else:
-                    width_ratios = args.wratios
                 if fig_p.fill:
                     fig_p.fill = args.alpha
 
                 if ispin == "Noneispin":
-                    plots.NoneispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, width_ratios, legend, fig_p)
+                    plots.NoneispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p)
                 elif ispin == "Ispin" and not args.divided:
-                    plots.IspinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, width_ratios, legend, fig_p)
+                    plots.IspinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p)
                 elif ispin == "Ispin" and args.divided:
-                    plots.DispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, width_ratios, legend, fig_p)
+                    plots.DispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p)
 # plot DOS
-        elif len(bandfile) == 0:
+        elif len_bandfile == 0:
             if dosfiles:
                 if fig_p.output == "BAND.png":
                     fig_p.output = "DOS.png"
                 darr, dele, s_elements = readdata.dos(dosfiles)
                 index_f, labels_elements = readdata.select(s_elements, args.partial)
                 if not elements:
                     elements = labels_elements
                 if fig_p.fill:
                     fig_p.fill = args.alpha
 
                 plots.pdosfiles(darr, dele, index_f, elements, legend, fig_p)
             else:
                 print("ERROR: No *.dat file.")
-# compare two band structures
-        elif len(bandfile) == 2:
+# compare two Band structures
+        elif len_bandfile == 2:
             if not fig_p.vertical:
                 fig_p.vertical = [-5.0, 5.0]
-            arr = [''] * 2
+            arr =   [''] * 2
             bands = [''] * 2
             ispin = [''] * 2
             arr[0], bands[0], ispin[0] = readdata.bands(bandfile[0])
             arr[1], bands[1], ispin[1] = readdata.bands(bandfile[1])
-            ticks   = []
-            klabels = []
-            if os.path.exists(args.klabels):
-                ticks, klabels = readdata.klabels(args.klabels)
-
-            if len(labels) == 0:
-                labels=[re.sub('GAMMA|Gamma|G', 'Γ', re.sub('Undefined|Un|[0-9]', '', i)) for i in klabels]
-
-            if len(ticks) > len(labels):
-                labels = labels + [''] * (len(ticks) - len(labels))
-            elif len(ticks) < len(labels):
-                labels = labels[:len(ticks)]
-
             if len(legend) < 3:
                 legend = legend + [''] * (3 - len(legend))
 
             if all(x == "Noneispin" for x in ispin):
                 plots.Noneispin2(arr, bands, ticks, labels, legend, fig_p)
             elif all(x == "Ispin" for x in ispin):
                 plots.Dispin2(arr, bands, ticks, labels, legend, fig_p)
+# compare three Band structures
+        elif len_bandfile == 3:
+            if not fig_p.vertical:
+                fig_p.vertical = [-5.0, 5.0]
+            arr =   [''] * 3
+            bands = [''] * 3
+            ispin = [''] * 3
+            arr[0], bands[0], ispin[0] = readdata.bands(bandfile[0])
+            arr[1], bands[1], ispin[1] = readdata.bands(bandfile[1])
+            arr[2], bands[2], ispin[2] = readdata.bands(bandfile[2])
+            if len(legend) < 4:
+                legend = legend + [''] * (4 - len(legend))
+
+            if all(x == "Noneispin" for x in ispin):
+                plots.Noneispin3(arr, bands, ticks, labels, legend, fig_p)
+            elif all(x == "Ispin" for x in ispin):
+                plots.Dispin3(arr, bands, ticks, labels, legend, fig_p)
         else:
             print("Input file mismatch.")
 
+# bandplot
 def pmain():
     parser = argparse.ArgumentParser(description='Plot the phonon band structure or DOS from phonopy results.',
                                      epilog='''
 Example:
 pbandplot -i BAND.dat -o BAND.png -l g m k g -d projected_dos.dat -g \$\\pi^2_4\$ -e Si C O
 ''',
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
+    formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('-v', "--version",    action="version",     version="bandplot "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
     parser.add_argument('-s', "--size",       type=float, nargs=2,  help='figure size: width, height')
     parser.add_argument('-b', "--broken",     type=float, nargs=2,  help='broken axis: start, end')
-    parser.add_argument('-r', "--hratios",    type=float,           help='height ratio for broken axis, default: 0.2', default=0.2)
+    parser.add_argument('-H', "--hratios",    type=float,           help='height ratio for broken axis, default: 0.2', default=0.2)
     parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="frequency (THz) range")
     parser.add_argument('-g', "--legend",     type=str,             nargs='+', help="legend labels", default=[])
     parser.add_argument('-L', "--location",   type=str.lower,       choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right',
                                                                              'center left', 'center right', 'lower center', 'upper center', 'center'],
                                                                     help="arrange the legend location, default: best", default='best')
     parser.add_argument('-c', "--color",      type=str,             nargs='+', help="line color: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow;"+
                                                                                     "k, black; w, white", default=[])
@@ -249,15 +271,15 @@
     parser.add_argument('-q', "--dpi",        type=int,             help="dpi of the figure, default: 500", default=500)
     parser.add_argument('-j', "--bandconf",   type=str,             help="filename of band setting file, default: band.conf", default="band.conf")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             help="plot Phonon DOS from .dat file")
     parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Phonon density of states range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of Phonon DOS")
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
-    parser.add_argument('-p', "--wratios",    type=float,           help='width ratio for DOS subplot, default 0.5', default=0.5)
+    parser.add_argument('-W', "--wratios",    type=float,           help='width ratio for DOS subplot, default 0.5', default=0.5)
     parser.add_argument('-z', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
     parser.add_argument('-Z', "--alpha",      type=float,           help='alpha value for filling region, default=0.2', default=0.2)
     parser.add_argument('-f', "--font",       type=str,             help="font to use", default='STIXGeneral')
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
@@ -305,78 +327,93 @@
                 formula = formula + symbol[i]
 
     if not elements and s_ele:
         elements = s_ele
 
     legend = args.legend or [formula] or [pltname]
 
+    klabels = []
+    if os.path.exists(args.bandconf):
+        klabels = readdata.bandset(args.bandconf)
+    if len(labels) == 0:
+        labels=[re.sub('^GA[A-Z]+$|^G$', 'Γ', i) for i in klabels]
+
     broken = args.broken
-    height_ratio = args.hratios
-    if height_ratio >= 1 or height_ratio <= 0:
-        height_ratio = 0.2
-
-    width_ratios = args.wratios
-    if width_ratios >= 1 or width_ratios <= 0:
-        width_ratios = 0.5
+    height_ratio = args.hratios if 0 < args.hratios < 1 else 0.2
+    width_ratios = args.wratios if 0 < args.wratios < 1 else 0.5
 
     fig_p = cla_fig(output=args.output, size=args.size, vertical=args.vertical, horizontal=args.horizontal,
                     color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi,
-                    exchange=args.exchange, fill=args.fill)
+                    height_ratio=height_ratio, width_ratios=width_ratios, exchange=args.exchange, fill=args.fill)
 # plot Phonon Band Structure
     bandfile = [f for i in args.input for f in glob.glob(i)]
-    if len(bandfile) == 1:
+    len_bandfile = len(bandfile)
+    if len_bandfile == 1:
         arr, fre, ticks = readdata.pbands(bandfile[0])
-        klabels = []
-        if os.path.exists(args.bandconf):
-            klabels = readdata.bandset(args.bandconf)
-        if len(labels) == 0:
-            labels=[re.sub('^GA[A-Z]+$|^G$', 'Γ', i) for i in klabels]
         if len(ticks) > len(labels):
             labels = labels + [''] * (len(ticks) - len(labels))
         elif len(ticks) < len(labels):
             labels = labels[:len(ticks)]
         if args.dos is None:
             if args.broken is None:
-                plots.Nobroken(arr, fre, ticks, labels, legend, fig_p)
+                pplots.Nobroken(arr, fre, ticks, labels, legend, fig_p)
             else:
-                plots.Broken(arr, fre, ticks, labels, broken, height_ratio, legend, fig_p)
+                pplots.Broken(arr, fre, ticks, labels, broken, legend, fig_p)
         elif os.path.exists(args.dos):
             darr, dele = readdata.pdos(args.dos)
             if fig_p.fill:
                 fig_p.fill = args.alpha
             if args.broken is None:
-                plots.NobrokenWd(arr, fre, ticks, labels, darr, dele, elements, width_ratios, legend, fig_p)
+                pplots.NobrokenWd(arr, fre, ticks, labels, darr, dele, elements, legend, fig_p)
             else:
-                plots.BrokenWd(arr, fre, ticks, labels, broken, height_ratio, darr, dele, elements, width_ratios, legend, fig_p)
+                pplots.BrokenWd(arr, fre, ticks, labels, broken, darr, dele, elements, legend, fig_p)
 # plot Phonon DOS
-    elif len(bandfile) == 0:
+    elif len_bandfile == 0:
         if args.dos and os.path.exists(args.dos):
+            if fig_p.output == "BAND.png":
+                    fig_p.output = "DOS.png"
             darr, dele = readdata.pdos(args.dos)
             if fig_p.fill:
                 fig_p.fill = args.alpha
-            plots.dosfile(darr, dele, elements, legend, fig_p)
+            pplots.dosfile(darr, dele, elements, legend, fig_p)
         else:
             print('No *.dat file.')
-# compare two Phonon band structures
-    elif len(bandfile) == 2:
+# compare two Phonon Band structures
+    elif len_bandfile == 2:
         arr = [''] * 2
         fre = [''] * 2
         ticks = [''] * 2
         arr[0], fre[0], ticks[0] = readdata.pbands(bandfile[0])
         arr[1], fre[1], ticks[1] = readdata.pbands(bandfile[1])
-        klabels = []
-        if os.path.exists(args.bandconf):
-            klabels = readdata.bandset(args.bandconf)
-        if len(labels) == 0:
-            labels=[re.sub('^GA[A-Z]+$|^G$', 'Γ', i) for i in klabels]
         if len(ticks[0]) > len(labels):
             labels = labels + [''] * (len(ticks[0]) - len(labels))
         elif len(ticks[0]) < len(labels):
             labels = labels[:len(ticks[0])]
         if len(legend) < 3:
             legend = legend + [''] * (3 - len(legend))
 
         if args.broken is None:
-            plots.Nobroken2(arr, fre, ticks[0], labels, legend, fig_p)
+            pplots.Nobroken2(arr, fre, ticks[0], labels, legend, fig_p)
         else:
-            plots.Broken2(arr, fre, ticks[0], labels, broken, height_ratio, legend, fig_p)
+            pplots.Broken2(arr, fre, ticks[0], labels, broken, legend, fig_p)
+# compare three Phonon Band structures
+    elif len_bandfile == 3:
+        arr = [''] * 3
+        fre = [''] * 3
+        ticks = [''] * 3
+        arr[0], fre[0], ticks[0] = readdata.pbands(bandfile[0])
+        arr[1], fre[1], ticks[1] = readdata.pbands(bandfile[1])
+        arr[2], fre[2], ticks[2] = readdata.pbands(bandfile[2])
+        if len(ticks[0]) > len(labels):
+            labels = labels + [''] * (len(ticks[0]) - len(labels))
+        elif len(ticks[0]) < len(labels):
+            labels = labels[:len(ticks[0])]
+        if len(legend) < 4:
+            legend = legend + [''] * (4 - len(legend))
+
+        if args.broken is None:
+            pplots.Nobroken3(arr, fre, ticks[0], labels, legend, fig_p)
+        else:
+            pplots.Broken3(arr, fre, ticks[0], labels, broken, legend, fig_p)
+    else:
+        print("Input file mismatch.")
```

## Comparing `bandplot-0.1.5.dist-info/METADATA` & `bandplot-0.1.5.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandplot
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: Band structure, DOS or phonon band structure plot from vaspkit or phonopy result.
 Home-page: https://github.com/lkccrr/bandplot
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT VASP DOS band plot Phonon
 Platform: Unix
@@ -49,9 +49,10 @@
 <b style="color:blue;"><i>pbandplot</b></i>
 * To execute <b style="color:blue;"><i>pbandplot</b></i> <b style="color:red;"><i>\-h</b></i> for the parameters to use.
 * Example:
 ```bash
 pbandplot -h
 pbandplot -i BAND.dat -o BAND.png -l g m k g -d projected_dos.dat -z
 pbandplot -b 23 100 -l g m k g -y -2 110
+pbandplot -i BAND1.dat BAND2.dat -b 20 100
 ```
```

## Comparing `bandplot-0.1.5.dist-info/RECORD` & `bandplot-0.1.5.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-bandplot/__init__.py,sha256=tHy0AYzeXxkaLmGY3UQY9VEGpL3XoCQFL6d2NqLyyC0,24
-bandplot/mass.py,sha256=1s1tBdlNVPh_ZwgF6mz43EiBvsMSeyF-tzCDOz-Rva8,6896
-bandplot/plots.py,sha256=9R5p0X3yaBjIH-WYPwJJq8Hv6zHTO21RaI9TMcDn3iM,36761
-bandplot/readdata.py,sha256=sW5TZ9oGXoWKlHkV-A8uTM2lQLzl8f1iia2GosxYGzs,6111
-bandplot/wrapper.py,sha256=h3TyRvGeUCNkevBeapoftJ9VyFGLsJPwNQbyWz2oi3Y,20407
-bandplot-0.1.5.dist-info/METADATA,sha256=fW-4WWGLH6SQQm3Ww9ooWDtBFJPqJcuTsO-in8jNRLU,2951
-bandplot-0.1.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bandplot-0.1.5.dist-info/entry_points.txt,sha256=1iTM_knGcHWOG7xxwvloJo_nbjS8WKTPOHP_HIKQr7k,86
-bandplot-0.1.5.dist-info/top_level.txt,sha256=SMQlf9lMS_nlhnQduityQVcU231XkEEvM7Z0n9gB0JE,9
-bandplot-0.1.5.dist-info/RECORD,,
+bandplot/__init__.py,sha256=w-haw8VvOBV0REEpDEA3YYkEW0r9HaXZ_YHjJvhLyj4,26
+bandplot/mass.py,sha256=R43Y-sUbzwgOfkQCp-rjnGwB8_eG30y111pYAlIRCJM,6905
+bandplot/plots.py,sha256=F90OAHVCLQBPFkFsY-Gsetr62hZaM-jd1Ct9gLF-jeg,25472
+bandplot/pplots.py,sha256=tb50x0RYG_Vmj7G3ftMmcXCbRESUqkEfHU0VsqKljXI,22228
+bandplot/readdata.py,sha256=eBmorJzcS-IwyoZlHg1INsHGXY3EYPgV04_4R-F_Xvk,6349
+bandplot/wrapper.py,sha256=XXpD1qNy_mLN5rOrqjb0iYapPkoP1KaZLh9gIPY0Aow,22112
+bandplot-0.1.5.1.dist-info/METADATA,sha256=S2sEslpOaMecXVzXRQO4bn3RsjC22nO2ZdZX9TvZXpY,2996
+bandplot-0.1.5.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bandplot-0.1.5.1.dist-info/entry_points.txt,sha256=1iTM_knGcHWOG7xxwvloJo_nbjS8WKTPOHP_HIKQr7k,86
+bandplot-0.1.5.1.dist-info/top_level.txt,sha256=SMQlf9lMS_nlhnQduityQVcU231XkEEvM7Z0n9gB0JE,9
+bandplot-0.1.5.1.dist-info/RECORD,,
```

