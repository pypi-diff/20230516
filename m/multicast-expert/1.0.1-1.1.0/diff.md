# Comparing `tmp/multicast_expert-1.0.1.tar.gz` & `tmp/multicast_expert-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicast_expert-1.0.1.tar", max compression
+gzip compressed data, was "multicast_expert-1.1.0.tar", max compression
```

## Comparing `multicast_expert-1.0.1.tar` & `multicast_expert-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2022-07-31 02:40:01.128195 multicast_expert-1.0.1/LICENSE
--rw-r--r--   0        0        0     1781 2022-08-14 00:56:27.095503 multicast_expert-1.0.1/multicast_expert/__init__.py
--rw-r--r--   0        0        0     8915 2022-08-14 01:14:25.564011 multicast_expert-1.0.1/multicast_expert/os_multicast.py
--rw-r--r--   0        0        0     8678 2022-08-14 02:27:13.573668 multicast_expert-1.0.1/multicast_expert/rx_socket.py
--rw-r--r--   0        0        0     5109 2022-08-14 01:53:52.433316 multicast_expert-1.0.1/multicast_expert/tx_socket.py
--rw-r--r--   0        0        0     3881 2022-08-08 04:56:03.023208 multicast_expert-1.0.1/multicast_expert/utils.py
--rw-r--r--   0        0        0      552 2022-08-14 02:02:05.932815 multicast_expert-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    17128 2022-08-14 02:29:08.542970 multicast_expert-1.0.1/README.rst
--rw-r--r--   0        0        0    18044 2022-08-14 02:29:46.383705 multicast_expert-1.0.1/setup.py
--rw-r--r--   0        0        0    17838 2022-08-14 02:29:46.384703 multicast_expert-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-07-31 02:40:01.128195 multicast_expert-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1781 2022-08-14 00:56:27.095503 multicast_expert-1.1.0/multicast_expert/__init__.py
+-rw-r--r--   0        0        0     9404 2023-05-16 04:15:49.630556 multicast_expert-1.1.0/multicast_expert/os_multicast.py
+-rw-r--r--   0        0        0     8653 2023-05-16 04:15:49.645516 multicast_expert-1.1.0/multicast_expert/rx_socket.py
+-rw-r--r--   0        0        0     5355 2023-05-16 04:15:49.658481 multicast_expert-1.1.0/multicast_expert/tx_socket.py
+-rw-r--r--   0        0        0     3964 2023-05-16 04:15:49.675436 multicast_expert-1.1.0/multicast_expert/utils.py
+-rw-r--r--   0        0        0      552 2023-05-16 04:17:50.736209 multicast_expert-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    17128 2022-08-14 02:29:08.542970 multicast_expert-1.1.0/README.rst
+-rw-r--r--   0        0        0    18044 2023-05-16 04:20:07.796057 multicast_expert-1.1.0/setup.py
+-rw-r--r--   0        0        0    17838 2023-05-16 04:20:07.796057 multicast_expert-1.1.0/PKG-INFO
```

### Comparing `multicast_expert-1.0.1/LICENSE` & `multicast_expert-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multicast_expert-1.0.1/multicast_expert/__init__.py` & `multicast_expert-1.1.0/multicast_expert/__init__.py`

 * *Files identical despite different names*

### Comparing `multicast_expert-1.0.1/multicast_expert/os_multicast.py` & `multicast_expert-1.1.0/multicast_expert/os_multicast.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 import struct
 import ctypes
 from typing import List
 from dataclasses import dataclass
 
 import netifaces
 
-
-is_windows = platform.system() == "Windows"
-
 # Import needed Win32 DLL functions
 if is_windows:
     iphlpapi = ctypes.WinDLL('iphlpapi')
     win32_GetAdapterIndex = iphlpapi.GetAdapterIndex
     win32_GetAdapterIndex.argtypes = [ctypes.c_wchar_p, ctypes.POINTER(ctypes.c_ulong)]
 
 
@@ -176,21 +173,29 @@
     """
     Add a source-specific membership for the given multicast IPs on the given socket, with the given sources.
     Currently only supports IPv6.
     """
     for mcast_ip in mcast_ips:
         for source_ip in source_ips:
             if is_windows:
-                # Struct documented here: https://docs.microsoft.com/en-us/windows/win32/api/ws2ipdef/ns-ws2ipdef-ip_mreq_source
+                # Struct documented here:
+                # https://docs.microsoft.com/en-us/windows/win32/api/ws2ipdef/ns-ws2ipdef-ip_mreq_source
                 # Note: imr_interface is in network byte order
                 mreq_source_bytes = struct.pack("!4s4sI",
                                                 socket.inet_aton(mcast_ip), # imr_multiaddr
                                                 socket.inet_aton(source_ip), # imr_sourceaddr
                                                 iface_info.iface_idx) # imr_interface
 
+            elif is_mac:
+                # Struct documented here:
+                # https://opensource.apple.com/source/xnu/xnu-4570.1.46/bsd/netinet/in.h.auto.html
+                mreq_source_bytes = struct.pack("@4s4s4s",
+                                                socket.inet_aton(mcast_ip),  # imr_multiaddr
+                                                socket.inet_aton(source_ip),  # imr_sourceaddr
+                                                socket.inet_aton(iface_info.iface_ip))  # imr_interface
             else:
                 # Struct documented here: https://linux.die.net/man/7/ip
                 mreq_source_bytes = struct.pack("@4s4s4s",
                                                 socket.inet_aton(mcast_ip), # imr_multiaddr
                                                 socket.inet_aton(iface_info.iface_ip), # imr_interface
                                                 socket.inet_aton(source_ip)) # imr_sourceaddr
```

### Comparing `multicast_expert-1.0.1/multicast_expert/rx_socket.py` & `multicast_expert-1.1.0/multicast_expert/rx_socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import platform
 import select
 import socket
 import struct
 from typing import List, Tuple, Optional
 import ctypes
 
-from .utils import get_interface_ips, get_default_gateway_iface_ip, validate_mcast_ip, MulticastExpertError
+from .utils import get_interface_ips, get_default_gateway_iface_ip, validate_mcast_ip, MulticastExpertError, is_mac, is_windows
 from . import os_multicast, LOCALHOST_IPV6, LOCALHOST_IPV4
 
-is_windows = platform.system() == "Windows"
-
 class McastRxSocket:
     """
     Class to wrap a socket that receives from one or more multicast groups.
     """
 
     def __init__(self, addr_family: int, mcast_ips: List[str], port: int, iface_ip: str=None, source_ips: List[str]=None, blocking=True):
         """
```

### Comparing `multicast_expert-1.0.1/multicast_expert/tx_socket.py` & `multicast_expert-1.1.0/multicast_expert/tx_socket.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import platform
 import socket
 import struct
 from typing import List, Tuple
 import ctypes
 
-from .utils import get_interface_ips, validate_mcast_ip, get_default_gateway_iface_ip, MulticastExpertError
+from .utils import get_interface_ips, validate_mcast_ip, get_default_gateway_iface_ip, MulticastExpertError, is_mac, is_windows
 from . import os_multicast, LOCALHOST_IPV4, LOCALHOST_IPV6
 
-is_windows = platform.system() == "Windows"
-
 class McastTxSocket:
     """
     Class to wrap a socket that sends to one or more multicast groups.
     """
 
     def __init__(self, addr_family: int, mcast_ips: List[str], iface_ip: str=None, ttl: int=1):
         """
@@ -70,18 +68,23 @@
             self.socket.setsockopt(socket.IPPROTO_IP, socket.IP_MULTICAST_TTL, self.ttl)
         else: # IPv6
             self.socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_MULTICAST_HOPS, self.ttl)
 
         # On Unix, we need to disable multicast loop here.  Otherwise, sent packets will get looped back to local
         # sockets on the same interface.
         if not is_windows:
+
+            # On Mac, we do want to keep loopback enabled but only on the loopback interface.
+            # On Linux, always disable it.
+            enable_loopback = is_mac() and (self.iface_ip == LOCALHOST_IPV4 or self.iface_ip == LOCALHOST_IPV6)
+
             if self.addr_family == socket.AF_INET:
-                self.socket.setsockopt(socket.IPPROTO_IP, socket.IP_MULTICAST_LOOP, False)
+                self.socket.setsockopt(socket.IPPROTO_IP, socket.IP_MULTICAST_LOOP, enable_loopback)
             else:
-                self.socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_MULTICAST_LOOP, False)
+                self.socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_MULTICAST_LOOP, enable_loopback)
 
         self.is_opened = True
 
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `multicast_expert-1.0.1/multicast_expert/utils.py` & `multicast_expert-1.1.0/multicast_expert/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import socket
 from typing import List, Dict, Optional
 import ipaddress
 
 import netifaces
 
+is_windows = platform.system() == "Windows"
+is_mac = platform.system() == "Darwin"
 
 # Exception class for this library
 class MulticastExpertError(RuntimeError):
     pass
 
 
 def get_interface_ips(include_ipv4=True, include_ipv6=True) -> List[str]:
```

### Comparing `multicast_expert-1.0.1/pyproject.toml` & `multicast_expert-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multicast_expert"
-version = "1.0.1"
+version = "1.1.0"
 description = "A library to take the fiddly parts out of multicast networking!"
 authors = ["Jamie Smith <jsmith@crackofdawn.onmicrosoft.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/multiplemonomials/multicast_expert"
 
 [tool.poetry.dependencies]
```

### Comparing `multicast_expert-1.0.1/README.rst` & `multicast_expert-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `multicast_expert-1.0.1/setup.py` & `multicast_expert-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['netifaces<1.0.0']
 
 setup_kwargs = {
     'name': 'multicast-expert',
-    'version': '1.0.1',
+    'version': '1.1.0',
     'description': 'A library to take the fiddly parts out of multicast networking!',
     'long_description': '###########################\nMulticast Expert for Python\n###########################\n\nMulticasting is one of the cooler features of Internet Protocol (IP).  It allows a single source to send out IP packets (usually UDP) which are then received by multiple other devices on the network.  No configuration in advance is needed -- the sender just sends packets, and other devices may subscribe to these packets at their leisure.  Using a protocol called IGMP, computers and network switches communicate to ensure that the multicasts are only sent where they are needed, and not anywhere else.  It\'s great for applications such as audio/video transmission or distributed systems where you need to send out data to many different machines on a network.\n\nIdeally, multicasting is as simple as sending a packet to a specific multicast address, and then having certain other machines receive it.  It looks a bit like this:\n\n.. image:: https://app.box.com/shared/static/ftsh3tq2gvrzibhqwr26n1nvwqazcmlu.png\n    :alt: Diagram of a multicast packet being sent on a network\n\nOf course, in practice, things are a bit more complicated -- chiefly because using multicast requires setting additional socket options whose values and formats often differ by OS.  To that end, this library was created, so that you can use multicast networking without having to mess around with low level OS stuff.  Multicast Expert includes all the required pieces to create and use IPv4 and IPv6 multicast sockets on Windows, Mac, and Linux.\n\n*******************\nMulticasting Basics\n*******************\n\nBefore I can explain how to use this library, I first need to explain the basics of multicasting itself.  There\'s not a lot of info out there on the net about how to do multicasting right, and much of what there is is buried deep in OS documentation.  So let\'s go over some of the basic concepts first.\n\nFirst and foremost, there is one principle that I need to make clear, or you will not have a good time trying to use multicast.  **Multicasting happens at the network interface level, not the machine level**.  Almost every machine has at least two network interfaces: the loopback interface to itself and the Ethernet/WiFi connection it uses to access the the Internet.  Many machines also have additional interfaces such as bridges to Docker containers/virtual machines, VPNs, or additional private LANs.  With normal (unicast) networking, you simply tell the OS what IP address you want to send a packet to, and it will select the appropriate interface automatically (using a structure called the routing table).  This is not so with multicast!  Every multicast socket needs to be bound to one specific network interface that it will use.  There is no such thing as "bind to 0.0.0.0" or "listen on all addresses"!\n\nNow that we\'ve gotten that out of the way, we can cover the four essential topics for multicast: multicast addresses, understanding network routing, creating a transmitter, and creating a receiver.\n\nMulticast Addresses\n===================\nA multicast IPv4 address is defined as any IPv4 address whose most significant four bits are "1110".  This means any IP address whose first number is in the range of 224 through 239 (0xE0-0xEF) is a multicast address.  Similarly, for IPv6, any address whose first byte is 0xFF is a multicast address.\n\nWhen a network interface (e.g. your Ethernet card) sees a packet going to a multicast IP address, it processes it differently.  The exact specifics are outside of the scope of this document and depend on the specific medium, but often it will mark that packet as multicast at the link layer too, e.g. by giving it a special destination MAC address.  This ensures that the packet is delivered correctly by the link layer.\n\nIf you are simply trying to receive existing multicast packets, all you need to know is the group address that the multicasts are being sent on.  But if you\'re trying to build your own application that communicates via multicast, you\'ll need to select an IPv4 or IPv6 multicast address to use for it.  Many of these addresses have to be officially assigned by IANA (the `wikipedia page on multicast addresses <https://en.wikipedia.org/wiki/Multicast_address#IPv4>`_ has the full details), though IP addresses in the 239.x.x.x range are "administratively scoped" and available for private use on LANs.\n\nMulticast Routing in Networks\n=============================\nCompared to regular IP packets, multicast packets are handled differently by networking devices such as Ethernet switches and routers.  It\'s all too easy to forget to take this into account, and then find yourself asking "wait, why am I not receiving any multicast traffic", or even "wait, why am I receiving *all of the multicasts* that I didn\'t ask for?"  This section will go over some basics of how multicast packets move through Ethernet networks.  Other networks may differ in the specifics, but the basic concepts should be similar.\n\nFor a simple ("unmanaged") Ethernet switch, its handling of multicast packets is very simple.  It simply treats them like broadcasts, and forwards them to every other port of the switch.\n\nAs you might imagine, if you have a large network full of multicast users, and switches are broadcasting every message everywhere, you could get some pretty awful network congestion.  To combat this, more complex ("managed") Ethernet switches often have a feature called "IGMP snooping".  When a switch has this setting enabled, it listens for what\'s called an "IGMP join message" to be sent by a host.  This message is automatically sent by your OS whenever you open a multicast receive socket, and indicates that host X wants to receive traffic going to multicast address Y.  When the switch sees one of these messages, it automatically begins routing traffic going to multicast address Y into host X\'s network link.  No IGMP join message?  No multicasts for you.\n\nNote: for IPv6, MLD messages are used instead of IGMP, but they do pretty much the same thing.\n\nLast but not least, routers.  In contrast to Ethernet switches, which connect individual hosts together, routers connect entire networks together.  They have quite a bit more logic and generally require at least some manual configuration of what packets are routed where.  Often, multicasts are just used within the local network and are dropped by routers (you can guarantee this by setting the Time To Live to 1, forcing them to be dropped by any router).  However, the specifics depend on the router configuration, and often individual multicast addresses are treated differently.  If you really do need to pass multicasts through a router, you should contact your ISP or your network admin to verify the router settings.\n\nIn conclusion, here\'s a table of how different boxes handle multicasts:\n\n========================================= ============================================\nBox                                       What does it do with multicast packets?\n========================================= ============================================\nEthernet Switch (No IGMP Snooping)        Forwards to all hosts\nEthernet Switch (IGMP Snooping Enabled)   Forwards to any hosts that have subscribed\nRouter                                    Depends on configuration.\n========================================= ============================================\n\n**NOTE:** Be careful of boxes with unexpected behavior!  Multicast is one of the more rarely used features of IP and often does not seem to be well tested.  In my time working with multicast, I\'ve seen a number of devices that do not implement the standard as I\'ve written it here.  For instance, some switches can individually have IGMP snooping enabled/disabled on each port, producing unexpected behavior.  I think the worst was a desktop switch which worked fine out of the box but started dropping most multicast traffic when IGMP snooping was enabled!\n\nSince lots of devices come with weird multicast settings out of the box, prepare to have to check and fix the configuration on each switch/device when you start using multicast on your network.\n\nSending Multicasts\n===================\n\nTo send multicasts, an application can pretty much just create a normal UDP socket and have it send packets to a multicast IP address.  However, there is one additional piece needed, which is that the OS needs to be told which interface to send the multicasts on.  This is always done using the IP_MULTICAST_IF setsockopt() option, but the exact syntax and procedure for using this option differs by OS.  Luckily, Multicast Expert takes care of that for you!\n\nReceiving Multicasts\n====================\n\nTo receive multicasts, essentially two things need to happen.  First, your OS needs to be told to send out an IGMP join message, telling other devices on the network to send multicast packets your way.  This generally happens as a side effect of enabling the IP_ADD_MEMBERSHIP socket option (or one of its variants) on a socket.  Then, the OS network stack needs to be configured to forward multicast packets which arrive on the given interface to your application.  This process is pretty different on Windows and Unix.\n\nOn Windows, multicast sockets are bound to a given port and interface (using bind()) when they are initially created.  Then, IP_ADD_MEMBERSHIP commands are used to further associate them with individual multicast addresses, so that when a packet is received to that multicast addr, it goes to the correct socket.  This is convenient as it means one socket can use multiple multicast groups and still not receive unwanted traffic from other groups that use the same port.  However, there\'s no way to block unicast traffic going to that interface and port from also being received by the multicast socket.\n\nBut on Unix, the situation is a bit different.  The IP_ADD_MEMBERSHIP command does not directly set up filtering by multicast address, it pretty much just sends the IGMP join message and opens the interface to receive packets going to the multicast address.  It does not directly associate the socket with the multicast address, it\'s still a "regular" UDP socket.  So, if you were to take a multicast socket and bind it to 0.0.0.0, it would end up receiving all UDP traffic on the port number, even traffic to other multicast addresses or to the unicast address.  The only way to fix this is to bind the socket to the specific multicast address instead, causing any traffic with a different destination address to not be accepted by the socket.  Unfortunately, a socket can only be bound to one destination address at a time, so this means multicast expert needs to create a different socket under the hood for each multicast address you want to listen on.\n\n**********************\nUsing Multicast Expert\n**********************\n\nNow let\'s get into some actual code examples.  Now first, before we can create any sockets, we need to find the interface address we want to use (see above).  Luckily, Multicast Expert comes with a convenient function to list all available network interfaces:\n\n>>> import multicast_expert\n>>> multicast_expert.get_interface_ips(include_ipv4=True, include_ipv6=False)\n[\'192.168.0.248\', \'192.168.153.1\', \'127.0.0.1\']\n\n(note that this function is a wrapper around the netifaces library, which provides quite a bit more functionality if you need it)\n\nBut which of those is the interface we actually want to use?  Well, that depends on your specific nework setup, but to make an educated guess, we also have a function to get the interface your machine uses to contact the internet.  This is not always correct but will work for many network setups.\n\n>>> multicast_expert.get_default_gateway_iface_ip_v4()\n\'192.168.0.248\'\n\nTransmitting Multicasts\n=======================\n\nTo send some data to a multicast, use the McastTxSocket class.  This wraps a socket internally, and does all the hard work of configuring it correctly for multicast.  For now we will use \'239.1.2.3\' as our multicast address since it\'s in the administratively scoped block.\n\nThe following block shows how to create a Tx socket and send some data:\n\n>>> import socket\n>>> with multicast_expert.McastTxSocket(socket.AF_INET, mcast_ips=[\'239.1.2.3\'], iface_ip=\'192.168.0.248\') as mcast_tx_sock:\n...     mcast_tx_sock.sendto(b\'Hello World\', (\'239.1.2.3\', 12345))\n\nNote: when you construct the socket, you have to pass in all of the multicast IPs that you will want to use the socket to send to.  These must be known in advance in order to configure socket options correctly.\n\nNote 2: If you omitted the iface_ip= argument, the get_default_gateway_iface_ip_v4() function would have been called to guess the iface ip.  So, we could have omitted this argument for the same result.\n\nReceiving Multicasts\n====================\n\nTo receive from one or more multicast addresses, use the McastRxSocket class.  For example:\n\n>>> with multicast_expert.McastRxSocket(socket.AF_INET, mcast_ips=[\'239.1.2.3\'], port=12345, iface_ip=\'192.168.0.248\') as mcast_rx_sock:\n...     bytes, src_address = mcast_rx_sock.recvfrom()\n\nThe above code will listen on the 239.1.2.3 multicast address, and will block until a packet is received.  To change the blocking behavior, use the settimeout() function.\n\nFull Example\n============\nFor a complete example of how to use this library, see the system test script `here <https://github.com/multiplemonomials/multicast_expert/blob/main/examples/mcast_communicator.py>`_.\n\nFAQ\n===\nQ: What happens if an interface changes IP address (e.g. due to the user modifying a static IP) after I create a multicast socket on that interface?\n    A: On all machines tested so far, multicast sockets will stick with their assigned interface once created, even if the IP of that interface changes or it is brought down.\n\nQ: Do McastRxSockets receive regular (unicast) UDP packets going to the same interface and port?\n    A: On Windows, yes.  On Unix, no.  Unfortunately, this is a platform difference that I haven\'t found an easy way to work around.\n\nQ: Can I create multiple McastRxSockets on the same port and interface?\n    A: As long as they have different mcast addresses, then yes, this works how you\'d expect.\n\nQ: Is it possible to receive multicasts on all interfaces with a single socket?\n    A: For reception, this should be possible; it may be implemented in a future version of the library.\n\nQ: Why are my multicasts to the loopback device not going through in Linux?\n    A: Linux seems to be very picky about what it allows through loopback.  First of all, you need to use ``ip route`` to add a route directing your multicast address to the ``lo`` interface.  For example, the command ``sudo ip route add 239.2.2.0/24 dev lo`` would allow any multicasts in the 239.2.2.x range through loopback.\n\n    Additionally, for IPv6, I have found that multicasts to addresses that don\'t start with ``ffx1`` (i.e. non-interface-local addresses) do not seem to be sent on loopback.  Still trying to find any document explaining this behavior...\n\nQ: My multicasts aren\'t being received in Linux, even though I see them coming in in packet dumps.\n    A: On Linux, you must also be careful of a kernel feature called Reverse Path Filtering (RPF).  You see, in most cases, multicast doesn\'t care about unicast IPs or subnets -- you can quite easily have a machine with IP 10.0.0.1 send multicasts to 192.168.1.2, even though those are on different subnets so they can\'t normally communicate.  However, RPF throws a wrench in this.  In its default "loose" mode (setting 2), it blocks reception of IP packets if they come from an IP address not reachable by any interface.  So, for example, if you receive a multicast from 10.0.0.1 but you only have routes in your routing table for 192.168.x.x IP addresses, the kernel will summarily drop the packet.  The easiest fix is to label one of your network interfaces as a default route.  This makes all IP addresses reachable from an interface, so all packets will be able to get by the check.\n\n    RPF\'s "strict" mode (setting 1) is even worse.  It applies the same check, but on a per-interface level.  So, in order to receive packets from multicast address X, each individual interface must have a routing rule permitting it to send packets to X.  If this is too much of a pain to set up, you can turn RPF off using sysctl (`this seems like a decent guide <https://access.redhat.com/solutions/53031#:~:text=rp_filter%20parameter%20only%20has%20two,default%20is%201%20(loose).>`_).  Just remember to change it both for the "all" interface and for whichever interfaces you want to affect -- the kernel takes the stricter of the two values.\n\n    If RPF isn\'t the problem, you may also want to check any firewalls (firewalld/iptables) and see if those are blocking multicast packets.\n\nQ: If I have a socket that receives from multiple mcast addresses, say A and B, and I receive a packet, how do I tell whether the packet was sent to multicast address A or B?\n    A: You can\'t, or at least I haven\'t found a way to do this from Python.  You\'ll need to create multiple sockets if you need this information.',
     'author': 'Jamie Smith',
     'author_email': 'jsmith@crackofdawn.onmicrosoft.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/multiplemonomials/multicast_expert',
```

### Comparing `multicast_expert-1.0.1/PKG-INFO` & `multicast_expert-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicast-expert
-Version: 1.0.1
+Version: 1.1.0
 Summary: A library to take the fiddly parts out of multicast networking!
 Home-page: https://github.com/multiplemonomials/multicast_expert
 License: MIT
 Author: Jamie Smith
 Author-email: jsmith@crackofdawn.onmicrosoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

