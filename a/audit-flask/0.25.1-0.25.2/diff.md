# Comparing `tmp/audit_flask-0.25.1-py3-none-any.whl.zip` & `tmp/audit_flask-0.25.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 7536 bytes, number of entries: 18
+Zip file size: 7669 bytes, number of entries: 18
 -rw-r--r--  2.0 unx       49 b- defN 23-May-07 16:32 audit_flask/__init__.py
 -rw-r--r--  2.0 unx      489 b- defN 23-May-07 17:11 audit_flask/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-07 16:39 audit_flask/main.py
 -rw-r--r--  2.0 unx       79 b- defN 23-May-07 17:10 audit_flask/audit/__init__.py
 -rw-r--r--  2.0 unx      233 b- defN 23-May-07 17:20 audit_flask/audit/kwargs.py
 -rw-r--r--  2.0 unx     2240 b- defN 23-May-07 22:36 audit_flask/audit/mongoengine.py
--rw-r--r--  2.0 unx     1899 b- defN 23-May-07 19:19 audit_flask/audit/sqlalchemy.py
+-rw-r--r--  2.0 unx     2068 b- defN 23-May-16 17:36 audit_flask/audit/sqlalchemy.py
 -rw-r--r--  2.0 unx        1 b- defN 23-May-07 17:19 audit_flask/utils/__init__.py
 -rw-r--r--  2.0 unx      788 b- defN 23-May-07 17:35 audit_flask/utils/flask.py
 -rw-r--r--  2.0 unx      558 b- defN 23-May-07 17:13 audit_flask/utils/json.py
 -rw-r--r--  2.0 unx       45 b- defN 23-May-07 16:58 test/__init__.py
 -rw-r--r--  2.0 unx      217 b- defN 23-May-07 17:00 test/config.py
 -rw-r--r--  2.0 unx     1433 b- defN 23-May-07 17:23 test/test_mongoengine.py
--rw-r--r--  2.0 unx     1990 b- defN 23-May-07 17:10 test/test_sqlalchemy.py
--rw-r--r--  2.0 unx      396 b- defN 23-May-07 22:37 audit_flask-0.25.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-07 22:37 audit_flask-0.25.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-07 22:37 audit_flask-0.25.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1437 b- defN 23-May-07 22:37 audit_flask-0.25.1.dist-info/RECORD
-18 files, 11963 bytes uncompressed, 5172 bytes compressed:  56.8%
+-rw-r--r--  2.0 unx     2227 b- defN 23-May-16 17:34 test/test_sqlalchemy.py
+-rw-r--r--  2.0 unx      396 b- defN 23-May-16 19:22 audit_flask-0.25.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-16 19:22 audit_flask-0.25.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-16 19:22 audit_flask-0.25.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1437 b- defN 23-May-16 19:22 audit_flask-0.25.2.dist-info/RECORD
+18 files, 12369 bytes uncompressed, 5305 bytes compressed:  57.1%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: test/test_mongoengine.py
 Comment: 
 
 Filename: test/test_sqlalchemy.py
 Comment: 
 
-Filename: audit_flask-0.25.1.dist-info/METADATA
+Filename: audit_flask-0.25.2.dist-info/METADATA
 Comment: 
 
-Filename: audit_flask-0.25.1.dist-info/WHEEL
+Filename: audit_flask-0.25.2.dist-info/WHEEL
 Comment: 
 
-Filename: audit_flask-0.25.1.dist-info/top_level.txt
+Filename: audit_flask-0.25.2.dist-info/top_level.txt
 Comment: 
 
-Filename: audit_flask-0.25.1.dist-info/RECORD
+Filename: audit_flask-0.25.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## audit_flask/audit/sqlalchemy.py

```diff
@@ -27,29 +27,32 @@
             if len(hist_attr) > 0:
                 object_before_changed[attr.key] = hist_attr[0]
             else:
                 object_before_changed[attr.key] = None
             if not hist.has_changes():
                 continue
             changes[attr.key] = hist.added
-        __audit((cls, target), 'update', changes, object_before_changed)
+        if len(changes) > 0:
+            __audit((cls, target), 'update', changes, object_before_changed)
 
     @event.listens_for(cls, 'after_delete')
     def after_delete(mapper, connection, target):
         __audit((cls, target), 'delete', None)
 
     def __audit(cls_target, method, changes: dict, object_before_changed=None):
         if changes is not None:
             changes = {key: value[0] for key, value in changes.items()}
 
         cls, target = cls_target
+        target_dictionary = target.__dict__
+        columns = dict(map(lambda x: (x.name, None), inspect(cls).columns))
+        object_repr = {column: target_dictionary[column] for column in columns}
 
         args = {
             'object_pk': getattr(target, cls.__mapper__.primary_key[0].name),
             'content_type': cls.__tablename__,
-            'object_repr': serializar_dict(target.__dict__),
+            'object_repr': serializar_dict(object_repr),
             'action': method,
             'changes': serializar_dict(changes),
             'object_before_changed': serializar_dict(object_before_changed)
         }
-        args['object_repr'].pop('_sa_instance_state', None)
         signal.send(None, **create_kwargs(args))
```

## test/test_sqlalchemy.py

```diff
@@ -1,12 +1,12 @@
-
+import datetime
 from sqlalchemy import create_engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import Session
-from sqlalchemy import (Column, String, Integer, Boolean)
+from sqlalchemy import (Column, String, Integer, Boolean, DateTime)
 
 from audit_flask.audit import sqlalchemy as sqlalchemy_audit_flask
 
 
 SQLALCHEMY_DATABASE_URL = "postgresql://{}:{}@{}/{}".format('Finkargo', 'Finkargo', 'localhost:5432', 'Testing')
 engine = create_engine(
     SQLALCHEMY_DATABASE_URL,
@@ -15,25 +15,28 @@
 Base = declarative_base()
 session = Session(autocommit=False, autoflush=False, bind=engine)
 
 
 def signal_sqlalchemy(*args, **kwargs):
     print('CHANGES LIBRARY SQLALCHEMY')
     print(kwargs)
+    print(len(kwargs['object_repr']) == len(kwargs['object_before_changed'] or []))
 
 
 class User(Base):
     __tablename__ = 'User'
     id_user = Column(Integer, primary_key=True, comment='id único')
     name = Column(String, comment='Nombre del usuario')
     surname = Column(String, comment='Apellido del usuario')
     email = Column(String, unique=False, comment='correo electrónico del usuario')
     status = Column(Boolean, comment='Si el usaurio está activo')
     generic = Column(Boolean, default=True, comment='Si es usuario generico')
     cellphone_number = Column(String, comment='Número celular del usuario')
+    created_at = Column(DateTime, default=datetime.datetime.now)
+    updated_at = Column(DateTime, default=datetime.datetime.now)
 
 
 Base.metadata.create_all(engine)
 
 sqlalchemy_audit_flask.keep_logs_models(User)
 
 sqlalchemy_audit_flask.signal.connect(signal_sqlalchemy)
@@ -63,9 +66,9 @@
 def test_delete_row():
     user = session.query(User).filter(User.id_user == 1).first()
     session.delete(user)
     session.commit()
 
 
 # test_create_row()
-# test_change_row()
+test_change_row()
 # test_delete_row()
```

## Comparing `audit_flask-0.25.1.dist-info/RECORD` & `audit_flask-0.25.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 audit_flask/__init__.py,sha256=gXThpjrk5OnqdQRuSRD0l3DyOn66eEuF0kQPePaF4sQ,49
 audit_flask/config.py,sha256=94KYLsr8p--fTi-Egm_8cRpJMtytFybHEmcS_-wIeqw,489
 audit_flask/main.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 audit_flask/audit/__init__.py,sha256=aNCr6aPAmOKm1hASiH-qnAG8726WKHYmXamTRkp3mDY,79
 audit_flask/audit/kwargs.py,sha256=Lv_5vafyyi-zDkvfEv-bsY7hWPejNJIz24drsTHhQj8,233
 audit_flask/audit/mongoengine.py,sha256=OfLtA05v7a5UxwxVlhqyH2ECUSbHTFjGxr60osWA8os,2240
-audit_flask/audit/sqlalchemy.py,sha256=dgbQHBHpslX45FIr_UKT00GzwFFz305wr2j3XwpTevo,1899
+audit_flask/audit/sqlalchemy.py,sha256=uqhuOhTq5aHoaCysC2MBYyW-dY2NnRKoSMFTfuQYSYw,2068
 audit_flask/utils/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 audit_flask/utils/flask.py,sha256=VMFKl0Cj9x06KnYU_owteST7qcYF8nWJGCKSrXNqkWQ,788
 audit_flask/utils/json.py,sha256=DX2KiAD4xI5FKxA15SXaagaFTzil8uqwkwMcVgavwRw,558
 test/__init__.py,sha256=rietiseBKDBp2H2-xOZviKdWmnacQnEqzQQ0Y6Ej8CY,45
 test/config.py,sha256=vP45_qCTy55AjqPx_M-o6qZBRHq2QcST1bDghZwPxXI,217
 test/test_mongoengine.py,sha256=72Yz5OfX7zDuFZucuTW2xmvt5yGf1w7GNtRV_3dIWw4,1433
-test/test_sqlalchemy.py,sha256=OGMkHKbqgv8BBtNbSOh-Jey77ljxKkOF2S9zlZM98-A,1990
-audit_flask-0.25.1.dist-info/METADATA,sha256=7Sq1Fxd3ULW7gPSrLaLdarmEn3uK9SNb4kwCPDcCjZI,396
-audit_flask-0.25.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-audit_flask-0.25.1.dist-info/top_level.txt,sha256=vnGYiKEEfaT1zXkdI7u5w5e93ymHk2o0gj35p8UKU8Q,17
-audit_flask-0.25.1.dist-info/RECORD,,
+test/test_sqlalchemy.py,sha256=6v9u0Vuif9VWlsutD_8Sv2-AAK6YcCdUlHr44OyJbBI,2227
+audit_flask-0.25.2.dist-info/METADATA,sha256=mS8qqbeGQiw6-mXo4H6eYvjKCz3P8SZSkpi5px2sStk,396
+audit_flask-0.25.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+audit_flask-0.25.2.dist-info/top_level.txt,sha256=vnGYiKEEfaT1zXkdI7u5w5e93ymHk2o0gj35p8UKU8Q,17
+audit_flask-0.25.2.dist-info/RECORD,,
```

