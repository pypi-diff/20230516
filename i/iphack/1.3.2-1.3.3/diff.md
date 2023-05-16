# Comparing `tmp/iphack-1.3.2.tar.gz` & `tmp/iphack-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iphack-1.3.2.tar", last modified: Mon May 15 15:01:19 2023, max compression
+gzip compressed data, was "iphack-1.3.3.tar", last modified: Tue May 16 19:38:55 2023, max compression
```

## Comparing `iphack-1.3.2.tar` & `iphack-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-15 15:01:19.023262 iphack-1.3.2/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     7222 2023-05-15 15:01:19.023262 iphack-1.3.2/PKG-INFO
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     5702 2023-01-30 09:48:18.000000 iphack-1.3.2/README.md
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-15 15:01:19.019262 iphack-1.3.2/iphack/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       95 2023-01-30 09:40:16.000000 iphack-1.3.2/iphack/__init__.py
--rw-------   0 u0_a314  (10314) u0_a314  (10314)    42871 2023-05-15 14:51:46.000000 iphack-1.3.2/iphack/iphack.py
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-15 15:01:19.023262 iphack-1.3.2/iphack.egg-info/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     7222 2023-05-15 15:01:18.000000 iphack-1.3.2/iphack.egg-info/PKG-INFO
--rw-------   0 u0_a314  (10314) u0_a314  (10314)      213 2023-05-15 15:01:18.000000 iphack-1.3.2/iphack.egg-info/SOURCES.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)        1 2023-05-15 15:01:18.000000 iphack-1.3.2/iphack.egg-info/dependency_links.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       65 2023-05-15 15:01:18.000000 iphack-1.3.2/iphack.egg-info/requires.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)        7 2023-05-15 15:01:18.000000 iphack-1.3.2/iphack.egg-info/top_level.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       79 2023-05-15 15:01:19.023262 iphack-1.3.2/setup.cfg
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     2293 2023-05-15 14:42:53.000000 iphack-1.3.2/setup.py
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-16 19:38:55.645628 iphack-1.3.3/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     7306 2023-05-16 19:38:55.645628 iphack-1.3.3/PKG-INFO
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     5786 2023-05-16 19:38:47.000000 iphack-1.3.3/README.md
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-16 19:38:55.645628 iphack-1.3.3/iphack/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       95 2023-01-30 09:40:16.000000 iphack-1.3.3/iphack/__init__.py
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)    43501 2023-05-16 19:33:51.000000 iphack-1.3.3/iphack/iphack.py
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-16 19:38:55.645628 iphack-1.3.3/iphack.egg-info/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     7306 2023-05-16 19:38:55.000000 iphack-1.3.3/iphack.egg-info/PKG-INFO
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)      213 2023-05-16 19:38:55.000000 iphack-1.3.3/iphack.egg-info/SOURCES.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)        1 2023-05-16 19:38:55.000000 iphack-1.3.3/iphack.egg-info/dependency_links.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       65 2023-05-16 19:38:55.000000 iphack-1.3.3/iphack.egg-info/requires.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)        7 2023-05-16 19:38:55.000000 iphack-1.3.3/iphack.egg-info/top_level.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       79 2023-05-16 19:38:55.645628 iphack-1.3.3/setup.cfg
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     2293 2023-05-16 19:37:39.000000 iphack-1.3.3/setup.py
```

### Comparing `iphack-1.3.2/PKG-INFO` & `iphack-1.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphack
-Version: 1.3.2
+Version: 1.3.3
 Summary: the most ideal tool for finding out information about IP, etc.
 Home-page: https://github.com/mishakorzik/IpHack
 Author: MishaKorzhik_He1Zen
 Author-email: developer.mishakorzhik@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/mishakorzik/IpHack/issues
 Project-URL: Sponsor, https://www.buymeacoffee.com/misakorzik
@@ -110,14 +110,20 @@
 ip.proxy(False)
 
 # get proxy list for api
 >>> from iphack import ip
 >>> ip.proxy(True)
 ['3.66.38.117:10882', '130.41.47.235:8080', '130.41.55.190:8080']
 >>>
+
+# using shodan
+>>> from iphack import *
+>>> iphack.shodan.find("google.com")
+>>> 
+
 ```
 
 **Check Proxy**
 
 ```python
 # check proxy 
 >>> from iphack import check
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iphack Version: 1.3.2 Summary: the most ideal tool
+Metadata-Version: 2.1 Name: iphack Version: 1.3.3 Summary: the most ideal tool
 for finding out information about IP, etc. Home-page: https://github.com/
 mishakorzik/IpHack Author: MishaKorzhik_He1Zen Author-email:
 developer.mishakorzhik@gmail.com License: Apache 2.0 Project-URL: Bug Tracker,
 https://github.com/mishakorzik/IpHack/issues Project-URL: Sponsor, https://
 www.buymeacoffee.com/misakorzik Keywords:
 ip,address,iphack,ips,pypi,pip,dns,router,ipv4,ipv6,public,ip-
 address,isp,location,lookup,iplookup,inquiry,tor,anon Classifier: Development
@@ -43,28 +43,29 @@
 requests pip install torpy==1.1.6 wget --no-check-certificate "https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/install.sh" bash install.sh
 ``` ## Usage **Ip Address** ```python # ip address tracking from iphack import
 ip ip.address("ip") # domain ip address tracking from iphack import ip
 ip.domain("google.com") # my ip address from iphack import ip ip.my() # get
 proxy from iphack import ip ip.proxy(False) # get proxy list for api >>> from
 iphack import ip >>> ip.proxy(True) ['3.66.38.117:10882', '130.41.47.235:8080',
-'130.41.55.190:8080'] >>> ``` **Check Proxy** ```python # check proxy >>> from
-iphack import check >>> check.proxy("130.41.55.190", "8080") Proxy : Online
-#Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM City : Los
-Angeles Country : United States Region : California Network : 130.41.52.0/22
-Version : IPv4 >>> ``` **Websites** ```python # Check amazon subdomains from
-iphack import ip ip.subdomains("amazon.com") # Check amazon directories from
-iphack import ip ip.directory("amazon.com") ``` **Inquiry** ```python #
-anonymous request from iphack import inquiry # request from url, using tor &
-fake user-agent >>> get = inquiry.get("https://api.ipify.org/") #method get >>>
-print(get.text) 199.249.230.102 >>> post = inquiry.post("https://example.com")
-#method post put = inquiry.put("https://example.com") #method put delete =
-inquiry.delete("https://example.com") #method delete head = inquiry.head
-("https://example.com") #method head # inquiry logs inquiry.debug() #enable log
-inquiry.debug() #disable log # inquiry anon method (default: web)
+'130.41.55.190:8080'] >>> # using shodan >>> from iphack import * >>>
+iphack.shodan.find("google.com") >>> ``` **Check Proxy** ```python # check
+proxy >>> from iphack import check >>> check.proxy("130.41.55.190", "8080")
+Proxy : Online #Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM
+City : Los Angeles Country : United States Region : California Network :
+130.41.52.0/22 Version : IPv4 >>> ``` **Websites** ```python # Check amazon
+subdomains from iphack import ip ip.subdomains("amazon.com") # Check amazon
+directories from iphack import ip ip.directory("amazon.com") ``` **Inquiry**
+```python # anonymous request from iphack import inquiry # request from url,
+using tor & fake user-agent >>> get = inquiry.get("https://api.ipify.org/")
+#method get >>> print(get.text) 199.249.230.102 >>> post = inquiry.post("https:
+//example.com") #method post put = inquiry.put("https://example.com") #method
+put delete = inquiry.delete("https://example.com") #method delete head =
+inquiry.head("https://example.com") #method head # inquiry logs inquiry.debug()
+#enable log inquiry.debug() #disable log # inquiry anon method (default: web)
 inquiry.rechange("tor") #use tor inquiry.rechange("web") #use web
 inquiry.rechange("vpn") #use vpn ``` ## Screenshot **Repository Views** !
 [Views](https://profile-counter.glitch.me/IpHack/count.svg) **Without logs**
 [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
 IMG_20220822_110928.jpg] **With logs & tor** [https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/IMG_20220824_150950.jpg]
 **With logs & web** [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
```

### Comparing `iphack-1.3.2/README.md` & `iphack-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,20 @@
 ip.proxy(False)
 
 # get proxy list for api
 >>> from iphack import ip
 >>> ip.proxy(True)
 ['3.66.38.117:10882', '130.41.47.235:8080', '130.41.55.190:8080']
 >>>
+
+# using shodan
+>>> from iphack import *
+>>> iphack.shodan.find("google.com")
+>>> 
+
 ```
 
 **Check Proxy**
 
 ```python
 # check proxy 
 >>> from iphack import check
```

#### html2text {}

```diff
@@ -22,28 +22,29 @@
 requests pip install torpy==1.1.6 wget --no-check-certificate "https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/install.sh" bash install.sh
 ``` ## Usage **Ip Address** ```python # ip address tracking from iphack import
 ip ip.address("ip") # domain ip address tracking from iphack import ip
 ip.domain("google.com") # my ip address from iphack import ip ip.my() # get
 proxy from iphack import ip ip.proxy(False) # get proxy list for api >>> from
 iphack import ip >>> ip.proxy(True) ['3.66.38.117:10882', '130.41.47.235:8080',
-'130.41.55.190:8080'] >>> ``` **Check Proxy** ```python # check proxy >>> from
-iphack import check >>> check.proxy("130.41.55.190", "8080") Proxy : Online
-#Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM City : Los
-Angeles Country : United States Region : California Network : 130.41.52.0/22
-Version : IPv4 >>> ``` **Websites** ```python # Check amazon subdomains from
-iphack import ip ip.subdomains("amazon.com") # Check amazon directories from
-iphack import ip ip.directory("amazon.com") ``` **Inquiry** ```python #
-anonymous request from iphack import inquiry # request from url, using tor &
-fake user-agent >>> get = inquiry.get("https://api.ipify.org/") #method get >>>
-print(get.text) 199.249.230.102 >>> post = inquiry.post("https://example.com")
-#method post put = inquiry.put("https://example.com") #method put delete =
-inquiry.delete("https://example.com") #method delete head = inquiry.head
-("https://example.com") #method head # inquiry logs inquiry.debug() #enable log
-inquiry.debug() #disable log # inquiry anon method (default: web)
+'130.41.55.190:8080'] >>> # using shodan >>> from iphack import * >>>
+iphack.shodan.find("google.com") >>> ``` **Check Proxy** ```python # check
+proxy >>> from iphack import check >>> check.proxy("130.41.55.190", "8080")
+Proxy : Online #Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM
+City : Los Angeles Country : United States Region : California Network :
+130.41.52.0/22 Version : IPv4 >>> ``` **Websites** ```python # Check amazon
+subdomains from iphack import ip ip.subdomains("amazon.com") # Check amazon
+directories from iphack import ip ip.directory("amazon.com") ``` **Inquiry**
+```python # anonymous request from iphack import inquiry # request from url,
+using tor & fake user-agent >>> get = inquiry.get("https://api.ipify.org/")
+#method get >>> print(get.text) 199.249.230.102 >>> post = inquiry.post("https:
+//example.com") #method post put = inquiry.put("https://example.com") #method
+put delete = inquiry.delete("https://example.com") #method delete head =
+inquiry.head("https://example.com") #method head # inquiry logs inquiry.debug()
+#enable log inquiry.debug() #disable log # inquiry anon method (default: web)
 inquiry.rechange("tor") #use tor inquiry.rechange("web") #use web
 inquiry.rechange("vpn") #use vpn ``` ## Screenshot **Repository Views** !
 [Views](https://profile-counter.glitch.me/IpHack/count.svg) **Without logs**
 [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
 IMG_20220822_110928.jpg] **With logs & tor** [https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/IMG_20220824_150950.jpg]
 **With logs & web** [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
```

### Comparing `iphack-1.3.2/iphack/iphack.py` & `iphack-1.3.3/iphack/iphack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os, sys, json, random, platform, time, re, pyproxify
 #from scapy.all import *
 import itertools
-import threading
+import threading, bs4
 from ua_headers import ua
 
 r = "\033[31m"
 g = "\033[32m"
 y = "\033[33m"
 b = "\033[34m"
 p = "\033[35m"
@@ -65,14 +65,21 @@
             ipdata_list = ['?api-key=6818a70bf0dcdbf1dd6bf89e62299740a49725ac65ff8e4056e3b343', '?api-key=7d9bf69a54c63b6f9274c6074b2f50aee46208d10a33533452add840', '?api-key=6453632fcabd2a4c2de4bb45ab35254594fd719e61d58bacde4429f0']
             ipdata = random.choice(ipdata_list)
             paste = "https://api.ipdata.co/"+ipaddr+ipdata
             data1 = requests.get(paste, headers=headers).json()
             data6 = requests.get("http://ip-api.com/json/"+ipaddr+"?fields=status,message,isp,org,as,reverse,mobile,proxy,hosting,query,district", headers=headers, timeout=10).json()
             data7 = requests.get("https://api.ipregistry.co/"+ipaddr+"?key=g54hjdzjnudhhsp4", headers=headers, timeout=10).json()
             he1zen = requests.get("https://raw.githubusercontent.com/mishakorzik/mishakorzik.menu.io/master/%D0%A1%D0%B5%D1%80%D0%B2%D0%B5%D1%80/iphack.json", timeout=15).json()
+            html = bs4.BeautifulSoup(requests.get("https://spur.us/context/"+ipaddr, headers={"User-Agent": ua.windows()}).text, features="lxml")
+            title = str(html.title)
+            title = title.replace("IP Context - Spur</title>", "")
+            title = title.replace("<title>", "")
+            title = title.replace("(", "")
+            title = title.replace(")", "")
+            title = title.replace(ipaddr, "")
             try:
                 he1zen = he1zen[ipaddr]
             except:
                 he1zen = " "
             a = lgreen+bold+"["+clear+"+"+lgreen+bold+"]"+clear
             r = lgreen+bold+"["+red+bold+"!"+lgreen+bold+"]"+clear
             data9 = data7['location']
@@ -141,24 +148,25 @@
             threat = data4['is_threat']
             if tor == True or vpn == True or proxy == True or anon == True or cloud == True or attacker == True or threat == True:
                 spur = "spur.us/context/"+ipaddr
             else:
                 spur = " "
             print(a, "┌──────────[Information]")
             print(a, "┼ spur.us            : "+spur)
+            print(a, "├ other info         : "+str(title))
             print(a, "└ he1zen info        : "+he1zen)
         except KeyboardInterrupt:
             print('Quiting Utility! Bye Bye, Have a nice day!'+lgreen)
             sys.exit(0)
         except requests.exceptions.ConnectionError as e:
             print (red+"[-]"+" Please check your internet connection!"+clear)
             print (red+"[-]"+" Error code: 106 DNS server refused to connect!"+clear)
-        except:
-            b = red+bold+"["+clear+"-"+red+bold+"]"+clear
-            print(b, "[-] Unknown Error")
+        #except:
+        #    b = red+bold+"["+clear+"-"+red+bold+"]"+clear
+        #    print(b, " Unknown Error")
     def my():
         import requests
         headers = {
                 'User-Agent' : ua.linux()
         }
         print(red+"""
 ██╗██████╗░██╗░░██╗░█████╗░░█████╗░██╗░░██╗
@@ -354,14 +362,19 @@
                print("Https      : False")
                print("Google     : True")
                print("Country    : "+c_name)
                print("Checked    : "+last)
                print("Anonymity  : "+anonymity)
                print(" ")
 
+class shodan:
+    def find(*text:str):
+        find = " ".join([str(m) for m in text])
+        os.system("shodan search "+str(find))
+
 class check:
     def proxy(ip, port):
         import requests
         proxies = {"http":"http://"+ip+":"+port}
         headers = {"User-Agent": ua.windows()}
         info = requests.get("https://ipapi.co/"+ip+"/json/", headers=headers).json()
         try:
```

### Comparing `iphack-1.3.2/iphack.egg-info/PKG-INFO` & `iphack-1.3.3/iphack.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphack
-Version: 1.3.2
+Version: 1.3.3
 Summary: the most ideal tool for finding out information about IP, etc.
 Home-page: https://github.com/mishakorzik/IpHack
 Author: MishaKorzhik_He1Zen
 Author-email: developer.mishakorzhik@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/mishakorzik/IpHack/issues
 Project-URL: Sponsor, https://www.buymeacoffee.com/misakorzik
@@ -110,14 +110,20 @@
 ip.proxy(False)
 
 # get proxy list for api
 >>> from iphack import ip
 >>> ip.proxy(True)
 ['3.66.38.117:10882', '130.41.47.235:8080', '130.41.55.190:8080']
 >>>
+
+# using shodan
+>>> from iphack import *
+>>> iphack.shodan.find("google.com")
+>>> 
+
 ```
 
 **Check Proxy**
 
 ```python
 # check proxy 
 >>> from iphack import check
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iphack Version: 1.3.2 Summary: the most ideal tool
+Metadata-Version: 2.1 Name: iphack Version: 1.3.3 Summary: the most ideal tool
 for finding out information about IP, etc. Home-page: https://github.com/
 mishakorzik/IpHack Author: MishaKorzhik_He1Zen Author-email:
 developer.mishakorzhik@gmail.com License: Apache 2.0 Project-URL: Bug Tracker,
 https://github.com/mishakorzik/IpHack/issues Project-URL: Sponsor, https://
 www.buymeacoffee.com/misakorzik Keywords:
 ip,address,iphack,ips,pypi,pip,dns,router,ipv4,ipv6,public,ip-
 address,isp,location,lookup,iplookup,inquiry,tor,anon Classifier: Development
@@ -43,28 +43,29 @@
 requests pip install torpy==1.1.6 wget --no-check-certificate "https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/install.sh" bash install.sh
 ``` ## Usage **Ip Address** ```python # ip address tracking from iphack import
 ip ip.address("ip") # domain ip address tracking from iphack import ip
 ip.domain("google.com") # my ip address from iphack import ip ip.my() # get
 proxy from iphack import ip ip.proxy(False) # get proxy list for api >>> from
 iphack import ip >>> ip.proxy(True) ['3.66.38.117:10882', '130.41.47.235:8080',
-'130.41.55.190:8080'] >>> ``` **Check Proxy** ```python # check proxy >>> from
-iphack import check >>> check.proxy("130.41.55.190", "8080") Proxy : Online
-#Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM City : Los
-Angeles Country : United States Region : California Network : 130.41.52.0/22
-Version : IPv4 >>> ``` **Websites** ```python # Check amazon subdomains from
-iphack import ip ip.subdomains("amazon.com") # Check amazon directories from
-iphack import ip ip.directory("amazon.com") ``` **Inquiry** ```python #
-anonymous request from iphack import inquiry # request from url, using tor &
-fake user-agent >>> get = inquiry.get("https://api.ipify.org/") #method get >>>
-print(get.text) 199.249.230.102 >>> post = inquiry.post("https://example.com")
-#method post put = inquiry.put("https://example.com") #method put delete =
-inquiry.delete("https://example.com") #method delete head = inquiry.head
-("https://example.com") #method head # inquiry logs inquiry.debug() #enable log
-inquiry.debug() #disable log # inquiry anon method (default: web)
+'130.41.55.190:8080'] >>> # using shodan >>> from iphack import * >>>
+iphack.shodan.find("google.com") >>> ``` **Check Proxy** ```python # check
+proxy >>> from iphack import check >>> check.proxy("130.41.55.190", "8080")
+Proxy : Online #Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM
+City : Los Angeles Country : United States Region : California Network :
+130.41.52.0/22 Version : IPv4 >>> ``` **Websites** ```python # Check amazon
+subdomains from iphack import ip ip.subdomains("amazon.com") # Check amazon
+directories from iphack import ip ip.directory("amazon.com") ``` **Inquiry**
+```python # anonymous request from iphack import inquiry # request from url,
+using tor & fake user-agent >>> get = inquiry.get("https://api.ipify.org/")
+#method get >>> print(get.text) 199.249.230.102 >>> post = inquiry.post("https:
+//example.com") #method post put = inquiry.put("https://example.com") #method
+put delete = inquiry.delete("https://example.com") #method delete head =
+inquiry.head("https://example.com") #method head # inquiry logs inquiry.debug()
+#enable log inquiry.debug() #disable log # inquiry anon method (default: web)
 inquiry.rechange("tor") #use tor inquiry.rechange("web") #use web
 inquiry.rechange("vpn") #use vpn ``` ## Screenshot **Repository Views** !
 [Views](https://profile-counter.glitch.me/IpHack/count.svg) **Without logs**
 [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
 IMG_20220822_110928.jpg] **With logs & tor** [https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/IMG_20220824_150950.jpg]
 **With logs & web** [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
```

### Comparing `iphack-1.3.2/setup.py` & `iphack-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='iphack',  # should match the package folder
     packages=['iphack'],  # should match the package folder
-    version='1.3.2',  # important for updates
+    version='1.3.3',  # important for updates
     python_requires=">=3.4",
     license='Apache 2.0',  # should match your chosen license
     description='the most ideal tool for finding out information about IP, etc.',
     long_description=long_description,  # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='MishaKorzhik_He1Zen',
     author_email='developer.mishakorzhik@gmail.com',
```

