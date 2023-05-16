# Comparing `tmp/dmbiolib-0.3.9.tar.gz` & `tmp/dmbiolib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmbiolib-0.3.9.tar", last modified: Thu Mar  2 07:14:28 2023, max compression
+gzip compressed data, was "dmbiolib-0.4.0.tar", last modified: Tue May 16 05:25:41 2023, max compression
```

## Comparing `dmbiolib-0.3.9.tar` & `dmbiolib-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 07:14:28.830592 dmbiolib-0.3.9/
--rw-rw-rw-   0        0        0    35802 2022-04-11 07:19:36.000000 dmbiolib-0.3.9/LICENSE
--rw-rw-rw-   0        0        0     1261 2023-03-02 07:14:28.828593 dmbiolib-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0      649 2023-02-08 06:46:06.000000 dmbiolib-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 07:14:28.819592 dmbiolib-0.3.9/dmbiolib/
-drwxrwxrwx   0        0        0        0 2023-03-02 07:14:28.826591 dmbiolib-0.3.9/dmbiolib/dmbiolib.egg-info/
--rw-rw-rw-   0        0        0     1261 2023-03-02 07:14:28.000000 dmbiolib-0.3.9/dmbiolib/dmbiolib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-03-02 07:14:28.000000 dmbiolib-0.3.9/dmbiolib/dmbiolib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 07:14:28.000000 dmbiolib-0.3.9/dmbiolib/dmbiolib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-02 07:14:28.000000 dmbiolib-0.3.9/dmbiolib/dmbiolib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18114 2023-03-02 07:02:47.000000 dmbiolib-0.3.9/dmbiolib/dmbiolib.py
--rw-rw-rw-   0        0        0       42 2023-03-02 07:14:28.830592 dmbiolib-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-03-02 07:03:29.000000 dmbiolib-0.3.9/setup.py
+drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 05:25:38.723748 dmbiolib-0.4.0/
+-rwxrwxrwx   0 daming    (1000) daming    (1000)    35802 2022-04-11 07:19:36.000000 dmbiolib-0.4.0/LICENSE
+-rwxrwxrwx   0 daming    (1000) daming    (1000)     1224 2023-05-16 05:25:38.720747 dmbiolib-0.4.0/PKG-INFO
+-rwxrwxrwx   0 daming    (1000) daming    (1000)      649 2023-02-08 06:46:06.000000 dmbiolib-0.4.0/README.md
+drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 05:25:38.617753 dmbiolib-0.4.0/dmbiolib/
+drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 05:25:38.700751 dmbiolib-0.4.0/dmbiolib/dmbiolib.egg-info/
+-rwxrwxrwx   0 daming    (1000) daming    (1000)     1224 2023-05-16 05:25:38.000000 dmbiolib-0.4.0/dmbiolib/dmbiolib.egg-info/PKG-INFO
+-rwxrwxrwx   0 daming    (1000) daming    (1000)      211 2023-05-16 05:25:38.000000 dmbiolib-0.4.0/dmbiolib/dmbiolib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daming    (1000) daming    (1000)        1 2023-05-16 05:25:38.000000 dmbiolib-0.4.0/dmbiolib/dmbiolib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daming    (1000) daming    (1000)        9 2023-05-16 05:25:38.000000 dmbiolib-0.4.0/dmbiolib/dmbiolib.egg-info/top_level.txt
+-rwxrwxrwx   0 daming    (1000) daming    (1000)    23165 2023-05-16 03:03:41.000000 dmbiolib-0.4.0/dmbiolib/dmbiolib.py
+-rwxrwxrwx   0 daming    (1000) daming    (1000)       38 2023-05-16 05:25:38.724749 dmbiolib-0.4.0/setup.cfg
+-rwxrwxrwx   0 daming    (1000) daming    (1000)      928 2023-05-16 03:15:01.000000 dmbiolib-0.4.0/setup.py
```

### Comparing `dmbiolib-0.3.9/LICENSE` & `dmbiolib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dmbiolib-0.3.9/PKG-INFO` & `dmbiolib-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-Metadata-Version: 2.1
-Name: dmbiolib
-Version: 0.3.9
-Summary: Library of Python functions used in other projects
-Home-page: https://github.com/damienmarsic/dmbiolib
-Author: Damien Marsic
-Author-email: damien.marsic@aliyun.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# dmbiolib
-
-Library of Python functions for bioinformatics
-
-Install from Bioconda:
-````
-conda install -c bioconda dmbiolib
-````
-Install from PyPI:
-````
-pip install dmbiolib
-````
-Full documentation: https://dmbiolib.readthedocs.io/
-
-GitHub issues (bug reports, feature requests): https://github.com/damienmarsic/dmbiolib/issues/new/choose
-
-[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/dmbiolib/README.html)
-
-[![dmbiolib documentation](https://img.shields.io/badge/dmbiolib-Documentation-yellow)](https://dmbiolib.readthedocs.io/)
-
-
+Metadata-Version: 2.1
+Name: dmbiolib
+Version: 0.4.0
+Summary: Library of Python functions used in other projects
+Home-page: https://github.com/damienmarsic/dmbiolib
+Author: Damien Marsic
+Author-email: damien.marsic@aliyun.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dmbiolib
+
+Library of Python functions for bioinformatics
+
+Install from Bioconda:
+````
+conda install -c bioconda dmbiolib
+````
+Install from PyPI:
+````
+pip install dmbiolib
+````
+Full documentation: https://dmbiolib.readthedocs.io/
+
+GitHub issues (bug reports, feature requests): https://github.com/damienmarsic/dmbiolib/issues/new/choose
+
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/dmbiolib/README.html)
+
+[![dmbiolib documentation](https://img.shields.io/badge/dmbiolib-Documentation-yellow)](https://dmbiolib.readthedocs.io/)
+
+
```

### Comparing `dmbiolib-0.3.9/README.md` & `dmbiolib-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dmbiolib-0.3.9/dmbiolib/dmbiolib.egg-info/PKG-INFO` & `dmbiolib-0.4.0/dmbiolib/dmbiolib.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-Metadata-Version: 2.1
-Name: dmbiolib
-Version: 0.3.9
-Summary: Library of Python functions used in other projects
-Home-page: https://github.com/damienmarsic/dmbiolib
-Author: Damien Marsic
-Author-email: damien.marsic@aliyun.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# dmbiolib
-
-Library of Python functions for bioinformatics
-
-Install from Bioconda:
-````
-conda install -c bioconda dmbiolib
-````
-Install from PyPI:
-````
-pip install dmbiolib
-````
-Full documentation: https://dmbiolib.readthedocs.io/
-
-GitHub issues (bug reports, feature requests): https://github.com/damienmarsic/dmbiolib/issues/new/choose
-
-[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/dmbiolib/README.html)
-
-[![dmbiolib documentation](https://img.shields.io/badge/dmbiolib-Documentation-yellow)](https://dmbiolib.readthedocs.io/)
-
-
+Metadata-Version: 2.1
+Name: dmbiolib
+Version: 0.4.0
+Summary: Library of Python functions used in other projects
+Home-page: https://github.com/damienmarsic/dmbiolib
+Author: Damien Marsic
+Author-email: damien.marsic@aliyun.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dmbiolib
+
+Library of Python functions for bioinformatics
+
+Install from Bioconda:
+````
+conda install -c bioconda dmbiolib
+````
+Install from PyPI:
+````
+pip install dmbiolib
+````
+Full documentation: https://dmbiolib.readthedocs.io/
+
+GitHub issues (bug reports, feature requests): https://github.com/damienmarsic/dmbiolib/issues/new/choose
+
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/dmbiolib/README.html)
+
+[![dmbiolib documentation](https://img.shields.io/badge/dmbiolib-Documentation-yellow)](https://dmbiolib.readthedocs.io/)
+
+
```

### Comparing `dmbiolib-0.3.9/dmbiolib/dmbiolib.py` & `dmbiolib-0.4.0/dmbiolib/dmbiolib.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
-__version__='0.3.9'
-last_update='2023-03-02'
+__version__='0.4.0'
+last_update='2023-05-16'
 author='Damien Marsic, damien.marsic@aliyun.com'
 license='GNU General Public v3 (GPLv3)'
 docs='https://dmbiolib.readthedocs.io'
 
 import sys,os,gzip,time,math
 from glob import glob
 from collections import defaultdict
@@ -19,14 +19,53 @@
 gcode={
 'ggg':'G','gga':'G','ggc':'G','ggt':'G','gag':'E','gaa':'E','gac':'D','gat':'D','gcg':'A', 'gca':'A', 'gcc':'A', 'gct':'A', 'gtg':'V', 'gta':'V', 'gtc':'V', 'gtt':'V',
 'agg':'R','aga':'R','agc':'S','agt':'S','aag':'K','aaa':'K','aac':'N','aat':'N','acg':'T', 'aca':'T', 'acc':'T', 'act':'T', 'atg':'M', 'ata':'I', 'atc':'I', 'att':'I',
 'cgg':'R','cga':'R','cgc':'R','cgt':'R','cag':'Q','caa':'Q','cac':'H','cat':'H','ccg':'P', 'cca':'P', 'ccc':'P', 'cct':'P', 'ctg':'L', 'cta':'L', 'ctc':'L', 'ctt':'L',
 'tgg':'W','tga':'*','tgc':'C','tgt':'C','tag':'*','taa':'*','tac':'Y','tat':'Y','tcg':'S', 'tca':'S', 'tcc':'S', 'tct':'S', 'ttg':'L', 'tta':'L', 'ttc':'F', 'ttt':'F'}
 bpairs={'a':'t','c':'g','g':'c','t':'a','n':'n','r':'y','y':'r','s':'s','w':'w','k':'m','m':'k','b':'v','d':'h','h':'d','v':'b'}
 
+def aa_dist(seqs,parvrs,fname,r):
+    aadist={}
+    mutdist={}
+    for vr in seqs:
+        if parvrs and not vr in parvrs:
+            continue
+        if not seqs[vr]:
+            continue
+        temp={}
+        total=0
+        mut={}
+        name=[]
+        for i in range(len(list(seqs[vr].keys())[0])):
+            if parvrs:
+                name.append(str(parvrs[vr][1]+i))
+                mut[name[i]]=0
+            elif len(seqs)>1:
+                name.append(vr+'-'+str(i+1))
+            else:
+                name.append(str(i+1))
+            temp[name[i]]=defaultdict(int)
+        for seq in seqs[vr]:
+            total+=seqs[vr][seq]
+            for i in range(len(seq)):
+                temp[name[i]][seq[i]]+=seqs[vr][seq]
+                if parvrs and seq[i]!=parvrs[vr][0][i]:
+                    mut[name[i]]+=seqs[vr][seq]
+        for n in temp:
+            aadist[n]={k:0 for k in aa}
+            for m in temp[n]:
+                aadist[n][m]=temp[n][m]/total
+        for n in mut:
+            mutdist[n]=mut[n]/total*100
+    if fname and aadist:
+        csv_write(fname+'_aad.csv',None,aadist,[k for k in aa],'Amino acid distribution was',r)
+        if parvrs and mutdist:
+            csv_write(fname+'_md.csv',None,mutdist,'Position,% mutant','Mutation distribution was',r)
+    return aadist,mutdist
+
 def aln2seq(fn,type,full,ref):
     fail=''
     seq={}
     if ref:
         ref,fail=getfasta(ref,type,type,False)
         if fail:
             return seq,fail
@@ -184,25 +223,24 @@
     x=''
     for n in seq:
         if x and n in 'atgc' and n==x[-1]:
             continue
         x+=n
     return x
 
-def conf_start(fname,title):
-    f=open(fname,'w')
-    f.write('=== '+title.upper()+' CONFIGURATION FILE ===\n\n')
+def conf_start(title):
+    content='=== '+title.upper()+' CONFIGURATION FILE ===\n\n'
     x=dirname()
     y=find_read_files()
-    return f,x,y
+    return content,x,y
 
-def conf_end(f,fname,title):
-    f.write('=== END OF CONFIGURATION FILE ===')
-    f.close()
-    print('\n  Edit the file '+fname+' before running '+title+' again !\n\n')
+def conf_end(fname,content,title):
+    with open(fname,'w') as f:
+        f.write(content+'\n=== END OF CONFIGURATION FILE ===\n')
+    print('\n  Edit the file '+fname+' before running '+title+' again (without arguments)!\n\n')
 
 def csv_read(fname,dic,header):
     with open(fname,'r') as f:
         x=f.read().strip().split('\n')
     x=[n.split(',') for n in x if n]
     if header:
         header=x[0]
@@ -224,54 +262,83 @@
             for j in range(len(x)):
                 x[j][i]=q(x[j][i])
     if dic and len(x[0])>1:
         x={n[0]:n[1:] for n in x}
     return header,x
 
 def csv_write(fname,keys,listordict,header,descr,r):
+    content=''
     if isinstance(listordict,dict):
         if not keys:
             keys=list(listordict.keys())
         x=list(listordict.values())[0]
     else:
         x=listordict[0]
-    if isinstance(x,list) or isinstance(x,tuple):
+    if isinstance(x,list) or isinstance(x,tuple) or isinstance(x,dict):
         x=len(x)
-        if keys:
-            x+=1
+        if keys: x+=1
     else:
         x=str(x).count(',')+2
-    f=open(fname,'w')
     if header:
         if isinstance(header,list) or isinstance(header,tuple):
-            header=','.join(header)
-        if header.count(',')+1==x-1:
-            header=','+header
-        f.write(str(header)+'\n')
+            y=','.join(header)
+        else:
+            y=header
+            header=header.split(',')
+        if y.count(',')+1==x-1:
+            y=','+y
+        content+=str(y)+'\n'
     for i in range(len(listordict)):
         a=''
         if keys:
             if i>=len(keys):
                 break
             a=keys[i]
         if isinstance(listordict,dict):
-            b=listordict[a]
+            x=listordict[a]
         else:
-            b=listordict[i]
-        if isinstance(b,list) or isinstance(b,tuple):
-            b=','.join([str(k) for k in b])
+            x=listordict[i]
+        if isinstance(x,list) or isinstance(x,tuple):
+            b=','.join([str(k) if k!=None else '' for k in x])
+        elif isinstance(x,dict):
+            b=','.join([str(x[k]) if x[k]!=None else '' for k in header])
         else:
-            b=str(b)
-        if a!='':
-            a=str(a)+','
-        f.write(a+b+'\n')
-    f.write('\n')
-    f.close()
+            b=str(x)
+        if a: a=str(a)+','
+        content+=a+b+'\n'
+    with open(fname,'w') as f:
+        f.write(content)
     if descr:
-        pr2(r,'\n  '+descr+' was saved into file: '+fname)
+        pr2(r,'\n  '+descr+' saved into file: '+fname)
+
+def detect_vr(libnt,mindist):
+    vrs={}
+    a=0
+    vr=''
+    for n in range(0,len(libnt),3):
+        x=libnt[n:n+3]
+        amb=any([i not in 'atgc' for i in x])
+        if amb and vr:
+            vr+=libnt[a:n+3]
+            a=n+3
+        if vr and (n+len(x)>=len(libnt) or (not amb and n+3-a>mindist)):
+            rprobe=''
+            if a<len(libnt):
+                rprobe=libnt[a:a+15]
+                x=[i for i in rprobe if i not in 'atgc']
+                if x:
+                    rprobe=rprobe[:rprobe.find(x[0])]
+            vrs['VR'+str(len(vrs)+1)]=[lprobe,vr,rprobe]
+            vr=''
+            continue
+        if not vr and amb:
+            vr=x
+            lprobe=libnt[max(0,n-15,a):n]
+            a=n+3
+    return vrs
 
 def diff(seqs):
     z=len(seqs[0])
     x=[(seqs[i],seqs[j]) for i in range(len(seqs)) for j in range(i+1, len(seqs))]
     for (a,b) in x:
         y=0
         for i in range(len(a)):
@@ -312,14 +379,16 @@
                 j+=1
             y[i]=j
     return y
 
 def find_read_files():
     rfiles=glob('*.f*.gz')
     if not rfiles:
+        rfiles=glob('*.f*a')+glob('*.f*q')
+    if not rfiles:
         return {}
     x=defaultdict(int)
     for n in rfiles:
         for m in ('_R1','_R2','_1.','_2.'):
             if m in n:
                 x[m]+=1
     for (a,b) in (('_R1','_R2'),('_1.','_2.')):
@@ -332,14 +401,24 @@
     for i in range(len(y)):
         x=y[i]
         if a and '*' in x:
             x=y[i].replace('*',a)+' '+y[i].replace('*',b)
         y[i]=y[i][:z[i]]+' '+x
     return sortfiles(y,' ')
 
+def findall(probe,seq,start,end,overlap=False):
+    i=seq.find(probe,start,end)
+    while i!=-1:
+        yield i
+        if overlap:
+            i+=1
+        else:
+            i+=len(probe)
+        i=seq.find(probe,i,end)
+
 def format_dna(seq,margin,cpl,cpn):
     x=len(str(len(seq)))
     if cpn<=x:
         cpn=x+1
     c=0
     t=''
     m=' '*margin
@@ -354,14 +433,32 @@
             else:
                 t+=' '*x
         t+='\n'+m+seq[c:c+cpl]+'\n'
         c+=cpl
         i=-(c%cpn)
     return t
 
+def frame(seq,strict):
+    trans={}
+    stop={}
+    for i in range(3):
+        trans[i]=transl(seq[i:3*(len(seq[i:])//3)+i])
+        if seq.startswith('atg') and len(seq)%3==0 and not '*' in trans[i][:-1]: return 0
+        if '*' in trans[i]:
+            stop[i]=trans[i].find('*')
+        elif seq.startswith('atg') and len(seq)%3==0:
+            return 0
+    if len(stop)==2: return [i for i in trans if not i in stop][0]
+    if len(stop)==3 and not strict:
+        x=[i for i in stop if stop[i]==max(stop.values())]
+        if len(x)==1 and stop[x[0]]>=len(seq)/3*.9:
+            return x[0]
+    else:
+        return None
+
 def fsize(filename):
     return os.path.getsize(filename)
 
 def getfasta(fn,type,required,multi):
     fail=''
     seq={}
     if not check_file(fn,False):
@@ -377,15 +474,15 @@
         return seq,fail
     x=x.split('>')
     for n in x:
         if not n:
             continue
         y=n[:n.find('\n')]+' '
         y=y[:y.find(' ')]
-        if not y and multi:
+        if not y:
             fail+='\n  Sequence with no name found in file '+fn+'! All sequences must have a name!'
         z=n[n.find('\n'):]
         if y in seq:
             fail+='\n  Duplicate sequence name '+y+' found in file '+fn+'! All sequences must have a different name!'
         z=z.replace(' ','').replace('\n','')
         if type==aa:
             z=z.upper()
@@ -420,15 +517,15 @@
         while z<y:
             l=f.readline().strip()
             if not z:
                 name=l
             if z==1:
                 seq=l.lower()
             z+=1
-    if seq:
+    if seq and counter:
         counter+=1
     return seq,f,counter,name
 
 def initreadfile(rfile):
     f=rfile_open(rfile)
     l=f.readline().strip()
     if not l or l[0] not in ('>','@'):
@@ -465,14 +562,28 @@
                 return False
         return True
     else:
         return False
 
 def mean(x):
     return sum(x)/len(x)
+    
+def mut_per_read(seqs,parseq,fname,r):
+    mut=defaultdict(int)
+    parseq=''.join(parseq)
+    for n in seqs:
+        x=0
+        m=''.join(n)
+        for i in range(len(m)):
+            if m[i]!=parseq[i]:
+                x+=1
+        mut[x]+=seqs[n]
+    if fname:
+        csv_write(fname,sorted(mut),mut,'Number of mutations,Number of reads','Mutation number distribution was',r)
+    return mut
 
 def nt_match(nt1, nt2):
     if nt1==nt2:
         return True
     elif (nt2 in ambiguous and nt1 in IUPAC[ambiguous.index(nt2)]) or (nt1 in ambiguous and nt2 in IUPAC[ambiguous.index(nt1)]):
         return True
     elif nt1 in ambiguous and nt2 in ambiguous and (not IUPAC[ambiguous.index(nt2)]-IUPAC[ambiguous.index(nt1)] or not IUPAC[ambiguous.index(nt1)]-IUPAC[ambiguous.index(nt2)]):
@@ -508,17 +619,22 @@
         for i in range(len(y)):
             x=len(y[i])
             for n in ('-','_','.','*'):
                 p=y[i].find(n,z[i]+1)
                 if p>0 and p<x:
                     x=p
             z[i]=x
-        if len(set([y[i][:z[i]] for i in range(len(y))]))==len(set(y)):
-            break
-    return z
+        if len(set([y[i][:z[i]] for i in range(len(y))]))==len(set(y)): break
+    return [y[i][:z[i]] for i in range(len(y))]
+
+def prod(x):
+    p=1
+    for n in x:
+        p*=n
+    return p
 
 def progress_check(c,show,t):
     if c in show:
         k=show[c]
         print('\r  '+t+' '*(8-len(k))+k+'%',end='')
 
 def progress_end():
@@ -534,15 +650,18 @@
     return show
 
 def readcount(R):
     if R[-3:]=='.gz':
         f=gzip.open(R,'r')
     else:
         f=open(R,'rb')
-    nr=xcount(f,'\n')//4
+    if R[-1].lower()=='a' or R[-4:].lower()=='a.gz':
+        nr=xcount(f,'>')
+    else:
+        nr=xcount(f,'\n')//4
     f.close()
     return nr
 
 def rename(name):
     if glob(name) and fsize(name):
         t=str(time.time())
         n=name[:name.rfind('.')]+'-'+t[:t.find('.')]+name[name.rfind('.'):]
@@ -564,14 +683,40 @@
 def rfile_open(x):
     if x[-2:]=='gz':
         f=gzip.open(x,'rt')
     else:
         f=open(x,'r')
     return f
 
+def seq_clust_card_dist(seqs,fname,r):
+    if isinstance(seqs,dict):
+        seqs=[seqs[k] for k in seqs]
+    total=sum(seqs)    
+    x=Counter(seqs)
+    sccd={k:x[k]/total for k in x}
+    if fname:
+        csv_write(fname,sorted(sccd),sccd,'Sequence cluster cardinality,Fraction of distinct sequences','Sequence cluster cardinality distribution was',r)
+    return sccd
+
+def seq_write(fname,top,seqs,dic,descr,r):
+    content=''
+    if top:
+        content+=str(top)+'\n'
+    if not seqs:
+        seqs=sorted(dic,key=dic.get,reverse=True)
+    for seq in seqs:
+        x=str(seq).replace(' ','').replace('(','').replace(')','').replace("'","")
+        if dic:
+            x+='\t'+str(dic[seq])
+        content+=x+'\n'
+    with open(fname,'w') as f:
+        f.write(content)
+    if descr:
+        pr2(r,'  '+descr+' saved into file: '+fname)
+
 def shortest_probe(seqs,lim,host,t):
     if lim<1:
         lim=1
     fail=''
     q=-1
     x=min([len(k) for k in seqs])
     y=set([k[-x:] for k in seqs])
@@ -584,14 +729,23 @@
         while True:
             y=set([k[-q:] for k in seqs])
             if len(y)==len(seqs) and max([k.count(p) for k in seqs for p in y])==1 and not len([k for k in y if k in host+host[:q-1]]):
                 break
             q+=1
     return q,fail
 
+def size_dist(seqs,fname,r):
+    sd=defaultdict(int)
+    for n in seqs:
+        sd[len(n)]+=seqs[n]
+    keys=sorted(sd,key=sd.get,reverse=True)
+    if fname:
+        csv_write(fname,keys,sd,'Length (nt),Number of reads','Sequence length distribution was',r)
+    return keys,sd
+
 def sortfiles(x,str):
     x.sort()
     if not str:
         str='.'
     y=[k for k in x if not any(i.isdigit() for i in k[:k.rfind(str)])]
     x=[k for k in x if not k in y]
     z=[(int(''.join([n for n in k if n.isdigit()])),k) for k in x]
```

### Comparing `dmbiolib-0.3.9/setup.py` & `dmbiolib-0.4.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="dmbiolib", # Replace with your own username
-    version="0.3.9",
+    version="0.4.0",
     author="Damien Marsic",
     author_email="damien.marsic@aliyun.com",
     description="Library of Python functions used in other projects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/damienmarsic/dmbiolib",
     package_dir={'': 'dmbiolib'},
```

