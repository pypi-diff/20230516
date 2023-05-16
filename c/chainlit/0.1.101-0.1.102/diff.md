# Comparing `tmp/chainlit-0.1.101.tar.gz` & `tmp/chainlit-0.1.102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlit-0.1.101.tar", max compression
+gzip compressed data, was "chainlit-0.1.102.tar", max compression
```

## Comparing `chainlit-0.1.101.tar` & `chainlit-0.1.102.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2349 2023-05-15 15:39:42.757523 chainlit-0.1.101/README.md
--rw-r--r--   0        0        0    13853 2023-05-15 15:38:57.288268 chainlit-0.1.101/chainlit/__init__.py
--rw-r--r--   0        0        0       87 2023-05-15 15:38:57.288268 chainlit-0.1.101/chainlit/__main__.py
--rw-r--r--   0        0        0     3527 2023-05-15 15:38:57.288268 chainlit-0.1.101/chainlit/cli/__init__.py
--rw-r--r--   0        0        0     4093 2023-05-15 15:38:57.288268 chainlit-0.1.101/chainlit/cli/auth.py
--rw-r--r--   0        0        0     2594 2023-05-15 15:38:57.288268 chainlit-0.1.101/chainlit/cli/deploy.py
--rw-r--r--   0        0        0      716 2023-05-15 15:38:57.288268 chainlit-0.1.101/chainlit/cli/utils.py
--rw-r--r--   0        0        0     5150 2023-05-15 15:38:57.288268 chainlit-0.1.101/chainlit/client.py
--rw-r--r--   0        0        0     6385 2023-05-15 15:38:57.288268 chainlit-0.1.101/chainlit/config.py
--rw-r--r--   0        0        0  2070264 2023-05-15 15:40:14.958394 chainlit-0.1.101/chainlit/frontend/dist/assets/index-10932891.js
--rw-r--r--   0        0        0     4317 2023-05-15 15:40:14.958394 chainlit-0.1.101/chainlit/frontend/dist/assets/index-bdffdaa0.css
--rw-r--r--   0        0        0     8889 2023-05-15 15:40:14.950394 chainlit-0.1.101/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
--rw-r--r--   0        0        0     8891 2023-05-15 15:40:14.958394 chainlit-0.1.101/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
--rw-r--r--   0        0        0     6455 2023-05-15 15:40:13.434353 chainlit-0.1.101/chainlit/frontend/dist/favicon.svg
--rw-r--r--   0        0        0      772 2023-05-15 15:40:14.958394 chainlit-0.1.101/chainlit/frontend/dist/index.html
--rw-r--r--   0        0        0      344 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/hello.py
--rw-r--r--   0        0        0        0 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/lc/__init__.py
--rw-r--r--   0        0        0     8077 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/lc/chainlit_handler.py
--rw-r--r--   0        0        0      863 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/lc/monkey.py
--rw-r--r--   0        0        0     5388 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/lc/new_monkey.py
--rw-r--r--   0        0        0     4129 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/lc/old_monkey.py
--rw-r--r--   0        0        0     1117 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/lc/utils.py
--rw-r--r--   0        0        0      398 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/logger.py
--rw-r--r--   0        0        0     1618 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/markdown.py
--rw-r--r--   0        0        0     8217 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/sdk.py
--rw-r--r--   0        0        0     9948 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/server.py
--rw-r--r--   0        0        0      813 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/session.py
--rw-r--r--   0        0        0     2017 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/telemetry.py
--rw-r--r--   0        0        0     1044 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/types.py
--rw-r--r--   0        0        0     1145 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/user_session.py
--rw-r--r--   0        0        0      196 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/version.py
--rw-r--r--   0        0        0     1551 2023-05-15 15:38:57.292268 chainlit-0.1.101/chainlit/watch.py
--rw-r--r--   0        0        0     1020 2023-05-15 15:38:57.292268 chainlit-0.1.101/pyproject.toml
--rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 chainlit-0.1.101/PKG-INFO
+-rw-r--r--   0        0        0     2349 2023-05-16 08:27:26.148519 chainlit-0.1.102/README.md
+-rw-r--r--   0        0        0    13853 2023-05-16 08:26:51.760142 chainlit-0.1.102/chainlit/__init__.py
+-rw-r--r--   0        0        0       87 2023-05-16 08:26:51.760142 chainlit-0.1.102/chainlit/__main__.py
+-rw-r--r--   0        0        0     3527 2023-05-16 08:26:51.760142 chainlit-0.1.102/chainlit/cli/__init__.py
+-rw-r--r--   0        0        0     4093 2023-05-16 08:26:51.760142 chainlit-0.1.102/chainlit/cli/auth.py
+-rw-r--r--   0        0        0     2594 2023-05-16 08:26:51.760142 chainlit-0.1.102/chainlit/cli/deploy.py
+-rw-r--r--   0        0        0      716 2023-05-16 08:26:51.760142 chainlit-0.1.102/chainlit/cli/utils.py
+-rw-r--r--   0        0        0     5150 2023-05-16 08:26:51.760142 chainlit-0.1.102/chainlit/client.py
+-rw-r--r--   0        0        0     6385 2023-05-16 08:26:51.760142 chainlit-0.1.102/chainlit/config.py
+-rw-r--r--   0        0        0  2070332 2023-05-16 08:27:52.440807 chainlit-0.1.102/chainlit/frontend/dist/assets/index-70c66596.js
+-rw-r--r--   0        0        0     4317 2023-05-16 08:27:52.440807 chainlit-0.1.102/chainlit/frontend/dist/assets/index-bdffdaa0.css
+-rw-r--r--   0        0        0     8889 2023-05-16 08:27:52.436807 chainlit-0.1.102/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
+-rw-r--r--   0        0        0     8891 2023-05-16 08:27:52.440807 chainlit-0.1.102/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
+-rw-r--r--   0        0        0     6455 2023-05-16 08:27:51.144793 chainlit-0.1.102/chainlit/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0      772 2023-05-16 08:27:52.440807 chainlit-0.1.102/chainlit/frontend/dist/index.html
+-rw-r--r--   0        0        0      344 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/hello.py
+-rw-r--r--   0        0        0        0 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/lc/__init__.py
+-rw-r--r--   0        0        0     8077 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/lc/chainlit_handler.py
+-rw-r--r--   0        0        0      863 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/lc/monkey.py
+-rw-r--r--   0        0        0     5388 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/lc/new_monkey.py
+-rw-r--r--   0        0        0     4129 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/lc/old_monkey.py
+-rw-r--r--   0        0        0     1117 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/lc/utils.py
+-rw-r--r--   0        0        0      398 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/logger.py
+-rw-r--r--   0        0        0     1618 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/markdown.py
+-rw-r--r--   0        0        0     8217 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/sdk.py
+-rw-r--r--   0        0        0     9948 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/server.py
+-rw-r--r--   0        0        0      813 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/session.py
+-rw-r--r--   0        0        0     2017 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/telemetry.py
+-rw-r--r--   0        0        0     1044 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/types.py
+-rw-r--r--   0        0        0     1145 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/user_session.py
+-rw-r--r--   0        0        0      196 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/version.py
+-rw-r--r--   0        0        0     1551 2023-05-16 08:26:51.764143 chainlit-0.1.102/chainlit/watch.py
+-rw-r--r--   0        0        0     1020 2023-05-16 08:26:51.764143 chainlit-0.1.102/pyproject.toml
+-rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 chainlit-0.1.102/PKG-INFO
```

### Comparing `chainlit-0.1.101/README.md` & `chainlit-0.1.102/README.md`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/__init__.py` & `chainlit-0.1.102/chainlit/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/cli/__init__.py` & `chainlit-0.1.102/chainlit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/cli/auth.py` & `chainlit-0.1.102/chainlit/cli/auth.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/cli/deploy.py` & `chainlit-0.1.102/chainlit/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/cli/utils.py` & `chainlit-0.1.102/chainlit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/client.py` & `chainlit-0.1.102/chainlit/client.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/config.py` & `chainlit-0.1.102/chainlit/config.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/frontend/dist/assets/index-10932891.js` & `chainlit-0.1.102/chainlit/frontend/dist/assets/index-70c66596.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -82478,14 +82478,15 @@
                     alignItems: "center"
                 },
                 children: [O.jsx(Mn, {
                     fontSize: "18px",
                     fontWeight: 700,
                     children: "Prompt playground"
                 }), O.jsx(ai, {
+                    edge: "end",
                     id: "close-playground",
                     sx: {
                         ml: "auto"
                     },
                     onClick: p,
                     children: O.jsx(Lp, {})
                 })]
@@ -82494,15 +82495,16 @@
                     display: "flex",
                     flexDirection: "column"
                 },
                 children: [O.jsxs(rr, {
                     direction: "row",
                     spacing: 2,
                     sx: {
-                        overflowY: "scroll",
+                        overflowY: "auto",
+                        overflowX: "hidden",
                         flexGrow: 1
                     },
                     children: [O.jsx(Pt, {
                         sx: {
                             fontFamily: "Inter",
                             fontSize: "16px",
                             lineHeight: "24px",
@@ -82802,27 +82804,29 @@
                         fontSize: "14px",
                         fontWeight: 700
                     },
                     children: "Last messages"
                 }), O.jsx(oie, {})]
             }, "title"),
             u = (n == null ? void 0 : n.length) === 0 ? O.jsx("div", {
+                id: "history-empty",
                 disabled: !0,
                 children: O.jsx(Mn, {
                     color: "text.secondary",
                     sx: {
                         fontSize: "12px",
                         fontWeight: 700,
                         padding: "16px 12px",
                         textTransform: "uppercase"
                     },
                     children: "Such empty..."
                 })
             }, "empty") : null,
             p = [l, u, n ? null : O.jsx("div", {
+                id: "history-loading",
                 disabled: !0,
                 children: O.jsx(Mn, {
                     color: "text.secondary",
                     sx: {
                         fontSize: "12px",
                         fontWeight: 700,
                         padding: "16px 12px",
@@ -82846,14 +82850,15 @@
                         },
                         children: v
                     })
                 }, v));
                 let y = "";
                 g[v].forEach(_ => {
                     y !== _.content && (y = _.content, p.push(O.jsx(lu, {
+                        className: "history-item",
                         onClick: E => {
                             E.stopPropagation(), E.preventDefault(), i(!1), e(_.content)
                         },
                         disableRipple: !0,
                         sx: {
                             p: 1,
                             alignItems: "baseline",
@@ -82878,27 +82883,26 @@
                     }, _.key)))
                 })
             })
         }
         const f = O.jsx(GF, {
             autoFocus: !0,
             anchorEl: o,
-            id: "account-menu",
             open: r,
             onClose: () => i(!1),
             PaperProps: {
                 sx: {
                     p: 1,
                     backgroundImage: "none",
                     mt: -2,
                     ml: -1,
                     overflow: "visible",
                     maxHeight: "314px",
                     width: "334px",
-                    overflowY: "scroll",
+                    overflowY: "auto",
                     border: g => `1px solid ${g.palette.divider}`,
                     boxShadow: g => g.palette.mode === "light" ? "0px 2px 4px 0px #0000000D" : "0px 10px 10px 0px #0000000D"
                 }
             },
             anchorOrigin: {
                 vertical: "top",
                 horizontal: "left"
@@ -82923,15 +82927,15 @@
     }
     const WI = "chatHistory",
         s9 = 50;
 
     function lie() {
         const e = k.useCallback(() => {
             const n = localStorage.getItem(WI);
-            if (n) return JSON.parse(n)
+            return n ? JSON.parse(n) : []
         }, []);
         return {
             persistChatLocally: k.useCallback(n => {
                 const r = {
                         createdAt: new Date().getTime(),
                         messages: [{
                             content: n
@@ -82950,18 +82954,18 @@
     }
 
     function Lpt({
         onClick: e
     }) {
         const {
             getLocalChatHistory: t
-        } = lie(), n = t(), r = k.useCallback(() => t(), []);
+        } = lie(), [n, r] = k.useState(t());
         return O.jsx(sie, {
             onClick: e,
-            onOpen: r,
+            onOpen: () => r(t()),
             chats: n
         })
     }
     const Fpt = Oo`
   query ($first: Int, $projectId: String!, $authorEmail: String) {
     conversations(
       first: $first
@@ -83097,15 +83101,15 @@
                     backgroundColor: "background.paper",
                     borderRadius: 1,
                     border: y => `1px solid ${y.palette.divider}`,
                     boxShadow: "box-shadow: 0px 2px 4px 0px #0000000D",
                     textarea: {
                         height: "34px",
                         maxHeight: "30vh",
-                        overflowY: "scroll !important",
+                        overflowY: "auto !important",
                         resize: "none",
                         paddingBottom: "0.75rem",
                         paddingTop: "0.75rem",
                         color: "text.primary",
                         lineHeight: "24px"
                     }
                 }
```

### Comparing `chainlit-0.1.101/chainlit/frontend/dist/assets/index-bdffdaa0.css` & `chainlit-0.1.102/chainlit/frontend/dist/assets/index-bdffdaa0.css`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg` & `chainlit-0.1.102/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg` & `chainlit-0.1.102/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/frontend/dist/favicon.svg` & `chainlit-0.1.102/chainlit/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/frontend/dist/index.html` & `chainlit-0.1.102/chainlit/frontend/dist/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     <link
       href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap"
       rel="stylesheet"
     />
     <script>
       const global = globalThis;
     </script>
-    <script type="module" crossorigin src="/assets/index-10932891.js"></script>
+    <script type="module" crossorigin src="/assets/index-70c66596.js"></script>
     <link rel="stylesheet" href="/assets/index-bdffdaa0.css">
   </head>
   <body>
     <div id="root"></div>
     
   </body>
 </html>
```

### Comparing `chainlit-0.1.101/chainlit/lc/chainlit_handler.py` & `chainlit-0.1.102/chainlit/lc/chainlit_handler.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/lc/monkey.py` & `chainlit-0.1.102/chainlit/lc/monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/lc/new_monkey.py` & `chainlit-0.1.102/chainlit/lc/new_monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/lc/old_monkey.py` & `chainlit-0.1.102/chainlit/lc/old_monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/lc/utils.py` & `chainlit-0.1.102/chainlit/lc/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/markdown.py` & `chainlit-0.1.102/chainlit/markdown.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/sdk.py` & `chainlit-0.1.102/chainlit/sdk.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/server.py` & `chainlit-0.1.102/chainlit/server.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/session.py` & `chainlit-0.1.102/chainlit/session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/telemetry.py` & `chainlit-0.1.102/chainlit/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/types.py` & `chainlit-0.1.102/chainlit/types.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/user_session.py` & `chainlit-0.1.102/chainlit/user_session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/chainlit/watch.py` & `chainlit-0.1.102/chainlit/watch.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.1.101/pyproject.toml` & `chainlit-0.1.102/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainlit"
-version = "0.1.101"
+version = "0.1.102"
 keywords = ['LLM', 'Agents', 'gen ai', 'chat ui', 'chatbot ui', 'langchain']
 description = "A faster way to build chatbot UIs."
 authors = ["Chainlit"]
 license = "Apache-2.0 license"
 repository = "https://github.com/Chainlit/chainlit"
 readme = "README.md"
 exclude = [
```

### Comparing `chainlit-0.1.101/PKG-INFO` & `chainlit-0.1.102/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlit
-Version: 0.1.101
+Version: 0.1.102
 Summary: A faster way to build chatbot UIs.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,langchain
 Author: Chainlit
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

