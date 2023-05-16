# Comparing `tmp/lowatt-enedis-2.1.0.tar.gz` & `tmp/lowatt-enedis-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lowatt-enedis-2.1.0.tar", last modified: Mon Apr 24 09:14:40 2023, max compression
+gzip compressed data, was "lowatt-enedis-2.2.0.tar", last modified: Tue May 16 15:31:33 2023, max compression
```

## Comparing `lowatt-enedis-2.1.0.tar` & `lowatt-enedis-2.2.0.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.589472 lowatt-enedis-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)    34619 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/lowatt_enedis/
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/certauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    28507 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.589472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    42043 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    45741 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    36631 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    36631 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommandeCollectePublicationMesures-v3.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommanderCollectePublicationMesures-v3.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    38245 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.593472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommandeTransmissionDonneesInfraJ-v1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommanderTransmissionDonneesInfraJ-v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    38416 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsultationDonneesTechniquesContractuelles-v1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsulterDonneesTechniquesContractuelles-v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.605472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ADAM.ConsulterMesuresDetailleesCommun.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ConsultationMesuresDetaillees-v3.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    38452 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    38245 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    40590 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    36163 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.597472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.601472 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-24 09:14:40.000000 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-24 09:14:40.000000 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:14:40.000000 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 09:14:40.000000 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 09:14:40.000000 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 09:14:40.000000 lowatt-enedis-2.1.0/lowatt_enedis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-24 09:14:40.613472 lowatt-enedis-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:40.609472 lowatt-enedis-2.1.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/test/data/consulterMesuresDetailleesResponse.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/test/data/consulterMesuresResponse.xml
--rw-r--r--   0 runner    (1001) docker     (123)    74247 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/test/data/requests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/test/test_lowatt_enedis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/test/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-24 09:14:34.000000 lowatt-enedis-2.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.472520 lowatt-enedis-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.440520 lowatt-enedis-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    34619 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-16 15:31:33.472520 lowatt-enedis-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.444520 lowatt-enedis-2.2.0/lowatt_enedis/
+-rw-r--r--   0 runner    (1001) docker     (123)    12323 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/certauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.448520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    42043 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    45741 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.448520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    36631 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.448520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.448520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.448520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    36631 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommandeCollectePublicationMesures-v3.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommanderCollectePublicationMesures-v3.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38245 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommandeTransmissionDonneesInfraJ-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommanderTransmissionDonneesInfraJ-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.456520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38416 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.456520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.456520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsultationDonneesTechniquesContractuelles-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsulterDonneesTechniquesContractuelles-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.456520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.456520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.460520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.460520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.460520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.460520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ADAM.ConsulterMesuresDetailleesCommun.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ConsultationMesuresDetaillees-v3.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.464520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.464520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38452 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.464520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.464520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38245 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.464520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.464520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.468520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.468520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    40590 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    36163 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.468520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.444520 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-16 15:31:33.000000 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-16 15:31:33.000000 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:31:33.000000 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 15:31:33.000000 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 15:31:33.000000 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 15:31:33.000000 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-16 15:31:33.472520 lowatt-enedis-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.468520 lowatt-enedis-2.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.472520 lowatt-enedis-2.2.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/test/data/consulterMesuresDetailleesResponse.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/test/data/consulterMesuresResponse.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    92977 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/test/data/requests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/test/test_lowatt_enedis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/test/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/tox.ini
```

### Comparing `lowatt-enedis-2.1.0/.flake8` & `lowatt-enedis-2.2.0/.flake8`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/.github/workflows/tox.yml` & `lowatt-enedis-2.2.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/COPYING` & `lowatt-enedis-2.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/PKG-INFO` & `lowatt-enedis-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowatt-enedis
-Version: 2.1.0
+Version: 2.2.0
 Summary: Query Enedis SGE web-service
 Home-page: https://github.com/lowatt/lowatt-enedis
 Author: Lowatt
 Author-email: info@lowatt.fr
 License: GPL3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lowatt-enedis-2.1.0/README.md` & `lowatt-enedis-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/__init__.py` & `lowatt-enedis-2.2.0/lowatt_enedis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,15 +317,17 @@
     xstypes_map = {}
     service_def = client.sd[0]
     for xstype in service_def.types:
         assert xstype[0] is xstype[1]  # duh?!
         xstype = xstype[0]
         ns = xstype.resolve().namespace()[1]
         prefix = service_def.getprefix(ns)
-        assert xstype.name not in xstypes_map
+        # Fix for issue #34
+        if service_def.service.name != "CommanderAccesDonneesMesures-V1.0":
+            assert xstype.name not in xstypes_map
         xstypes_map[xstype.name] = (xstype, prefix)
 
     return xstypes_map
 
 
 def xstype_children_map(
     xstype: suds.xsd.sxbase.SchemaObject,
```

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/__main__.py` & `lowatt-enedis-2.2.0/lowatt_enedis/__main__.py`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/certauth.py` & `lowatt-enedis-2.2.0/lowatt_enedis/certauth.py`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/services.py` & `lowatt-enedis-2.2.0/lowatt_enedis/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -645,14 +645,103 @@
         "ns0:DeclarationConsentementType",
     )
 
     return client.service.commanderTransmissionHistoriqueMesures(demande)
 
 
 @register(
+    "cmdAcces",
+    "CommanderAccesDonneesMesures-V1.0",
+    dict_from_dicts(
+        DONNEES_GENERALES_OPTIONS,
+        {
+            "--from": {
+                "default": (date.today()).isoformat(),
+                "help": "date de début souhaitée (incluse)",
+            },
+            "--to": {
+                "default": (date.today() + timedelta(days=365 * 3)).isoformat(),
+                "help": "date de fin souhaitée (excluse)",
+            },
+            "type": {
+                "choices": ["ENERGIE", "PMAX", "COURBE", "INDEX"],
+                "help": "type de mesure demandé : ENERGIE pour les consommations "
+                "globales quotidiennes, PMAX pour les puissances maximales "
+                "quotidiennes, COURBE pour la courbe de charge.",
+            },
+            "--injection": {
+                "action": "store_true",
+                "help": "demander les données en injection (soutirage par défaut).",
+            },
+        },
+        ACCORD_CLIENT_OPTIONS,
+    ),
+)
+@ws("CommanderAccesDonneesMesures-V1.0")
+def point_cmd_acces(client: Client, args: argparse.Namespace) -> suds.sudsobject.Object:
+    demande = client.factory.create("ns1:DemandeType")
+
+    demande.donneesGenerales = create_from_options(
+        client,
+        args,
+        "DonneesGeneralesType",
+        {
+            # XXX missing: refExterne
+            "prm": "pointId",
+            "login": "initiateurLogin",
+        },
+    )
+    assert demande.donneesGenerales is not None
+
+    demande.donneesGenerales.objetCode = "AME"
+    demande.donneesGenerales.contrat = create_from_options(
+        client,
+        args,
+        "ContratType",
+        {
+            # XXX missing: acteurMarcheCode, contratType
+            "contrat": "contratId",
+        },
+    )
+
+    demande.accesDonnees = create_from_options(
+        client,
+        args,
+        "AccesDonneesType",
+        {
+            "from": "dateDebut",
+            "to": "dateFin",
+            "type": "typeDonnees",
+        },
+    )
+    assert demande.accesDonnees is not None
+
+    # COURBE and INDEX are correct values according to the documentation, but
+    # the error "SGT4Q1: Le type de mesure renseigné n'est pas conforme." is returned.
+    # CDC and IDX do not return this error.
+    if demande.accesDonnees.typeDonnees == "COURBE":
+        demande.accesDonnees.typeDonnees = "CDC"
+    elif demande.accesDonnees.typeDonnees == "INDEX":
+        demande.accesDonnees.typeDonnees = "IDX"
+
+    injection = get_option(args, "injection")
+    demande.accesDonnees.soutirage = _boolean(not injection)
+    demande.accesDonnees.injection = _boolean(injection)
+
+    demande.accesDonnees.declarationAccordClient = _accord_client(
+        client,
+        args,
+        xs_accord_type="ns1:DeclarationAccordClientType",
+        autorisation=not get_option(args, "no_autorisation"),
+    )
+
+    return client.service.commanderAccesDonneesMesures(demande)
+
+
+@register(
     "cmdInfraJ",
     "CommandeTransmissionDonneesInfraJ-v1.0",
     dict_from_dicts(
         DONNEES_GENERALES_OPTIONS,
         {
             "--injection": {
                 "action": "store_true",
```

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.wsdl` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommandeCollectePublicationMesures-v3.0.wsdl` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommandeCollectePublicationMesures-v3.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommanderCollectePublicationMesures-v3.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommanderCollectePublicationMesures-v3.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommandeTransmissionDonneesInfraJ-v1.0.wsdl` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommandeTransmissionDonneesInfraJ-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommanderTransmissionDonneesInfraJ-v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommanderTransmissionDonneesInfraJ-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsultationDonneesTechniquesContractuelles-v1.0.wsdl` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsultationDonneesTechniquesContractuelles-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsulterDonneesTechniquesContractuelles-v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsulterDonneesTechniquesContractuelles-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ADAM.ConsulterMesuresDetailleesCommun.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ADAM.ConsulterMesuresDetailleesCommun.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ConsultationMesuresDetaillees-v3.0.wsdl` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ConsultationMesuresDetaillees-v3.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd` & `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis.egg-info/PKG-INFO` & `lowatt-enedis-2.2.0/lowatt_enedis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowatt-enedis
-Version: 2.1.0
+Version: 2.2.0
 Summary: Query Enedis SGE web-service
 Home-page: https://github.com/lowatt/lowatt-enedis
 Author: Lowatt
 Author-email: info@lowatt.fr
 License: GPL3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lowatt-enedis-2.1.0/lowatt_enedis.egg-info/SOURCES.txt` & `lowatt-enedis-2.2.0/lowatt_enedis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/setup.cfg` & `lowatt-enedis-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/setup.py` & `lowatt-enedis-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/test/data/consulterMesuresDetailleesResponse.xml` & `lowatt-enedis-2.2.0/test/data/consulterMesuresDetailleesResponse.xml`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/test/data/consulterMesuresResponse.xml` & `lowatt-enedis-2.2.0/test/data/consulterMesuresResponse.xml`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/test/data/requests.yaml` & `lowatt-enedis-2.2.0/test/data/requests.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,447 @@
+ACCES-NR1 (C2-C4):
+  data: |
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commanderaccesdonneesmesures/v1.0">
+      <SOAP-ENV:Header>
+        <tec:entete>
+          <version>1.0</version>
+          <infoDemandeur>
+            <loginDemandeur>test@example.com</loginDemandeur>
+          </infoDemandeur>
+        </tec:entete>
+      </SOAP-ENV:Header>
+      <ns0:Body>
+        <ns1:commanderAccesDonneesMesures>
+          <demande>
+            <donneesGenerales>
+              <objetCode>AME</objetCode>
+              <pointId>98800002267746</pointId>
+              <initiateurLogin>test@example.com</initiateurLogin>
+              <contrat>
+                <contratId>1234</contratId>
+              </contrat>
+            </donneesGenerales>
+            <accesDonnees>
+              <dateDebut>2022-02-22</dateDebut>
+              <dateFin>2025-02-21</dateFin>
+              <declarationAccordClient>
+                <accord>false</accord>
+                <personnePhysique>
+                  <nom>DUPONT</nom>
+                </personnePhysique>
+              </declarationAccordClient>
+              <typeDonnees>ENERGIE</typeDonnees>
+              <soutirage>true</soutirage>
+              <injection>false</injection>
+            </accesDonnees>
+          </demande>
+        </ns1:commanderAccesDonneesMesures>
+      </ns0:Body>
+    </SOAP-ENV:Envelope>
+  url: https://sge-homologation-b2b.enedis.fr/CommanderAccesDonneesMesures/v1.0
+ACCES-NR1 (C5):
+  data: |
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commanderaccesdonneesmesures/v1.0">
+      <SOAP-ENV:Header>
+        <tec:entete>
+          <version>1.0</version>
+          <infoDemandeur>
+            <loginDemandeur>test@example.com</loginDemandeur>
+          </infoDemandeur>
+        </tec:entete>
+      </SOAP-ENV:Header>
+      <ns0:Body>
+        <ns1:commanderAccesDonneesMesures>
+          <demande>
+            <donneesGenerales>
+              <objetCode>AME</objetCode>
+              <pointId>24380318190106</pointId>
+              <initiateurLogin>test@example.com</initiateurLogin>
+              <contrat>
+                <contratId>1234</contratId>
+              </contrat>
+            </donneesGenerales>
+            <accesDonnees>
+              <dateDebut>2022-02-22</dateDebut>
+              <dateFin>2025-02-21</dateFin>
+              <declarationAccordClient>
+                <accord>false</accord>
+                <personnePhysique>
+                  <nom>DUPONT</nom>
+                </personnePhysique>
+              </declarationAccordClient>
+              <typeDonnees>ENERGIE</typeDonnees>
+              <soutirage>true</soutirage>
+              <injection>false</injection>
+            </accesDonnees>
+          </demande>
+        </ns1:commanderAccesDonneesMesures>
+      </ns0:Body>
+    </SOAP-ENV:Envelope>
+  url: https://sge-homologation-b2b.enedis.fr/CommanderAccesDonneesMesures/v1.0
+ACCES-NR2 (C2-C4):
+  data: |
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commanderaccesdonneesmesures/v1.0">
+      <SOAP-ENV:Header>
+        <tec:entete>
+          <version>1.0</version>
+          <infoDemandeur>
+            <loginDemandeur>test@example.com</loginDemandeur>
+          </infoDemandeur>
+        </tec:entete>
+      </SOAP-ENV:Header>
+      <ns0:Body>
+        <ns1:commanderAccesDonneesMesures>
+          <demande>
+            <donneesGenerales>
+              <objetCode>AME</objetCode>
+              <pointId>98800002267746</pointId>
+              <initiateurLogin>test@example.com</initiateurLogin>
+              <contrat>
+                <contratId>1234</contratId>
+              </contrat>
+            </donneesGenerales>
+            <accesDonnees>
+              <dateDebut>2022-02-22</dateDebut>
+              <dateFin>2050-04-21</dateFin>
+              <declarationAccordClient>
+                <accord>true</accord>
+                <personnePhysique>
+                  <nom>DUPONT</nom>
+                </personnePhysique>
+              </declarationAccordClient>
+              <typeDonnees>ENERGIE</typeDonnees>
+              <soutirage>true</soutirage>
+              <injection>false</injection>
+            </accesDonnees>
+          </demande>
+        </ns1:commanderAccesDonneesMesures>
+      </ns0:Body>
+    </SOAP-ENV:Envelope>
+  url: https://sge-homologation-b2b.enedis.fr/CommanderAccesDonneesMesures/v1.0
+ACCES-NR2 (C5):
+  data: |
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commanderaccesdonneesmesures/v1.0">
+      <SOAP-ENV:Header>
+        <tec:entete>
+          <version>1.0</version>
+          <infoDemandeur>
+            <loginDemandeur>test@example.com</loginDemandeur>
+          </infoDemandeur>
+        </tec:entete>
+      </SOAP-ENV:Header>
+      <ns0:Body>
+        <ns1:commanderAccesDonneesMesures>
+          <demande>
+            <donneesGenerales>
+              <objetCode>AME</objetCode>
+              <pointId>24380318190106</pointId>
+              <initiateurLogin>test@example.com</initiateurLogin>
+              <contrat>
+                <contratId>1234</contratId>
+              </contrat>
+            </donneesGenerales>
+            <accesDonnees>
+              <dateDebut>2022-02-22</dateDebut>
+              <dateFin>2050-04-21</dateFin>
+              <declarationAccordClient>
+                <accord>true</accord>
+                <personnePhysique>
+                  <nom>DUPONT</nom>
+                </personnePhysique>
+              </declarationAccordClient>
+              <typeDonnees>ENERGIE</typeDonnees>
+              <soutirage>true</soutirage>
+              <injection>false</injection>
+            </accesDonnees>
+          </demande>
+        </ns1:commanderAccesDonneesMesures>
+      </ns0:Body>
+    </SOAP-ENV:Envelope>
+  url: https://sge-homologation-b2b.enedis.fr/CommanderAccesDonneesMesures/v1.0
+ACCES-R1 (C2-C4) \*:
+  data: |
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commanderaccesdonneesmesures/v1.0">
+      <SOAP-ENV:Header>
+        <tec:entete>
+          <version>1.0</version>
+          <infoDemandeur>
+            <loginDemandeur>test@example.com</loginDemandeur>
+          </infoDemandeur>
+        </tec:entete>
+      </SOAP-ENV:Header>
+      <ns0:Body>
+        <ns1:commanderAccesDonneesMesures>
+          <demande>
+            <donneesGenerales>
+              <objetCode>AME</objetCode>
+              <pointId>98800002267746</pointId>
+              <initiateurLogin>test@example.com</initiateurLogin>
+              <contrat>
+                <contratId>1234</contratId>
+              </contrat>
+            </donneesGenerales>
+            <accesDonnees>
+              <dateDebut>2022-02-22</dateDebut>
+              <dateFin>2025-02-21</dateFin>
+              <declarationAccordClient>
+                <accord>true</accord>
+                <personnePhysique>
+                  <nom>DUPONT</nom>
+                </personnePhysique>
+              </declarationAccordClient>
+              <typeDonnees>ENERGIE</typeDonnees>
+              <soutirage>true</soutirage>
+              <injection>false</injection>
+            </accesDonnees>
+          </demande>
+        </ns1:commanderAccesDonneesMesures>
+      </ns0:Body>
+    </SOAP-ENV:Envelope>
+  url: https://sge-homologation-b2b.enedis.fr/CommanderAccesDonneesMesures/v1.0
+ACCES-R1 (C5) \*\*:
+  data: |
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commanderaccesdonneesmesures/v1.0">
+      <SOAP-ENV:Header>
+        <tec:entete>
+          <version>1.0</version>
+          <infoDemandeur>
+            <loginDemandeur>test@example.com</loginDemandeur>
+          </infoDemandeur>
+        </tec:entete>
+      </SOAP-ENV:Header>
+      <ns0:Body>
+        <ns1:commanderAccesDonneesMesures>
+          <demande>
+            <donneesGenerales>
+              <objetCode>AME</objetCode>
+              <pointId>24380318190106</pointId>
+              <initiateurLogin>test@example.com</initiateurLogin>
+              <contrat>
+                <contratId>1234</contratId>
+              </contrat>
+            </donneesGenerales>
+            <accesDonnees>
+              <dateDebut>2022-02-22</dateDebut>
+              <dateFin>2025-02-21</dateFin>
+              <declarationAccordClient>
+                <accord>true</accord>
+                <personnePhysique>
+                  <nom>DUPONT</nom>
+                </personnePhysique>
+              </declarationAccordClient>
+              <typeDonnees>ENERGIE</typeDonnees>
+              <soutirage>true</soutirage>
+              <injection>false</injection>
+            </accesDonnees>
+          </demande>
+        </ns1:commanderAccesDonneesMesures>
+      </ns0:Body>
+    </SOAP-ENV:Envelope>
+  url: https://sge-homologation-b2b.enedis.fr/CommanderAccesDonneesMesures/v1.0
+ACCES-R2 (C2-C4) \*:
+  data: |
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commanderaccesdonneesmesures/v1.0">
+      <SOAP-ENV:Header>
+        <tec:entete>
+          <version>1.0</version>
+          <infoDemandeur>
+            <loginDemandeur>test@example.com</loginDemandeur>
+          </infoDemandeur>
+        </tec:entete>
+      </SOAP-ENV:Header>
+      <ns0:Body>
+        <ns1:commanderAccesDonneesMesures>
+          <demande>
+            <donneesGenerales>
+              <objetCode>AME</objetCode>
+              <pointId>98800002267746</pointId>
+              <initiateurLogin>test@example.com</initiateurLogin>
+              <contrat>
+                <contratId>1234</contratId>
+              </contrat>
+            </donneesGenerales>
+            <accesDonnees>
+              <dateDebut>2022-02-22</dateDebut>
+              <dateFin>2025-02-21</dateFin>
+              <declarationAccordClient>
+                <accord>true</accord>
+                <personnePhysique>
+                  <nom>DUPONT</nom>
+                </personnePhysique>
+              </declarationAccordClient>
+              <typeDonnees>CDC</typeDonnees>
+              <soutirage>true</soutirage>
+              <injection>false</injection>
+            </accesDonnees>
+          </demande>
+        </ns1:commanderAccesDonneesMesures>
+      </ns0:Body>
+    </SOAP-ENV:Envelope>
+  url: https://sge-homologation-b2b.enedis.fr/CommanderAccesDonneesMesures/v1.0
+ACCES-R2 (C5) \*\*:
+  data: |
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commanderaccesdonneesmesures/v1.0">
+      <SOAP-ENV:Header>
+        <tec:entete>
+          <version>1.0</version>
+          <infoDemandeur>
+            <loginDemandeur>test@example.com</loginDemandeur>
+          </infoDemandeur>
+        </tec:entete>
+      </SOAP-ENV:Header>
+      <ns0:Body>
+        <ns1:commanderAccesDonneesMesures>
+          <demande>
+            <donneesGenerales>
+              <objetCode>AME</objetCode>
+              <pointId>24380318190106</pointId>
+              <initiateurLogin>test@example.com</initiateurLogin>
+              <contrat>
+                <contratId>1234</contratId>
+              </contrat>
+            </donneesGenerales>
+            <accesDonnees>
+              <dateDebut>2022-02-22</dateDebut>
+              <dateFin>2025-02-21</dateFin>
+              <declarationAccordClient>
+                <accord>true</accord>
+                <personnePhysique>
+                  <nom>DUPONT</nom>
+                </personnePhysique>
+              </declarationAccordClient>
+              <typeDonnees>CDC</typeDonnees>
+              <soutirage>true</soutirage>
+              <injection>false</injection>
+            </accesDonnees>
+          </demande>
+        </ns1:commanderAccesDonneesMesures>
+      </ns0:Body>
+    </SOAP-ENV:Envelope>
+  url: https://sge-homologation-b2b.enedis.fr/CommanderAccesDonneesMesures/v1.0
+ACCES-R3 \*\*:
+  data: |
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commanderaccesdonneesmesures/v1.0">
+      <SOAP-ENV:Header>
+        <tec:entete>
+          <version>1.0</version>
+          <infoDemandeur>
+            <loginDemandeur>test@example.com</loginDemandeur>
+          </infoDemandeur>
+        </tec:entete>
+      </SOAP-ENV:Header>
+      <ns0:Body>
+        <ns1:commanderAccesDonneesMesures>
+          <demande>
+            <donneesGenerales>
+              <objetCode>AME</objetCode>
+              <pointId>24380318190106</pointId>
+              <initiateurLogin>test@example.com</initiateurLogin>
+              <contrat>
+                <contratId>1234</contratId>
+              </contrat>
+            </donneesGenerales>
+            <accesDonnees>
+              <dateDebut>2022-02-22</dateDebut>
+              <dateFin>2025-02-21</dateFin>
+              <declarationAccordClient>
+                <accord>true</accord>
+                <personnePhysique>
+                  <nom>DUPONT</nom>
+                </personnePhysique>
+              </declarationAccordClient>
+              <typeDonnees>PMAX</typeDonnees>
+              <soutirage>true</soutirage>
+              <injection>false</injection>
+            </accesDonnees>
+          </demande>
+        </ns1:commanderAccesDonneesMesures>
+      </ns0:Body>
+    </SOAP-ENV:Envelope>
+  url: https://sge-homologation-b2b.enedis.fr/CommanderAccesDonneesMesures/v1.0
+ACCES-R4 (C2-C4) \*:
+  data: |
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commanderaccesdonneesmesures/v1.0">
+      <SOAP-ENV:Header>
+        <tec:entete>
+          <version>1.0</version>
+          <infoDemandeur>
+            <loginDemandeur>test@example.com</loginDemandeur>
+          </infoDemandeur>
+        </tec:entete>
+      </SOAP-ENV:Header>
+      <ns0:Body>
+        <ns1:commanderAccesDonneesMesures>
+          <demande>
+            <donneesGenerales>
+              <objetCode>AME</objetCode>
+              <pointId>98800002267746</pointId>
+              <initiateurLogin>test@example.com</initiateurLogin>
+              <contrat>
+                <contratId>1234</contratId>
+              </contrat>
+            </donneesGenerales>
+            <accesDonnees>
+              <dateDebut>2022-02-22</dateDebut>
+              <dateFin>2025-02-21</dateFin>
+              <declarationAccordClient>
+                <accord>true</accord>
+                <personnePhysique>
+                  <nom>DUPONT</nom>
+                </personnePhysique>
+              </declarationAccordClient>
+              <typeDonnees>IDX</typeDonnees>
+              <soutirage>true</soutirage>
+              <injection>false</injection>
+            </accesDonnees>
+          </demande>
+        </ns1:commanderAccesDonneesMesures>
+      </ns0:Body>
+    </SOAP-ENV:Envelope>
+  url: https://sge-homologation-b2b.enedis.fr/CommanderAccesDonneesMesures/v1.0
+ACCES-R4 (C5) \*\*:
+  data: |
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commanderaccesdonneesmesures/v1.0">
+      <SOAP-ENV:Header>
+        <tec:entete>
+          <version>1.0</version>
+          <infoDemandeur>
+            <loginDemandeur>test@example.com</loginDemandeur>
+          </infoDemandeur>
+        </tec:entete>
+      </SOAP-ENV:Header>
+      <ns0:Body>
+        <ns1:commanderAccesDonneesMesures>
+          <demande>
+            <donneesGenerales>
+              <objetCode>AME</objetCode>
+              <pointId>24380318190106</pointId>
+              <initiateurLogin>test@example.com</initiateurLogin>
+              <contrat>
+                <contratId>1234</contratId>
+              </contrat>
+            </donneesGenerales>
+            <accesDonnees>
+              <dateDebut>2022-02-22</dateDebut>
+              <dateFin>2025-02-21</dateFin>
+              <declarationAccordClient>
+                <accord>true</accord>
+                <personnePhysique>
+                  <nom>DUPONT</nom>
+                </personnePhysique>
+              </declarationAccordClient>
+              <typeDonnees>IDX</typeDonnees>
+              <soutirage>true</soutirage>
+              <injection>false</injection>
+            </accesDonnees>
+          </demande>
+        </ns1:commanderAccesDonneesMesures>
+      </ns0:Body>
+    </SOAP-ENV:Envelope>
+  url: https://sge-homologation-b2b.enedis.fr/CommanderAccesDonneesMesures/v1.0
 ADP-NR1:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consulterdonneestechniquescontractuelles/v1.0">
       <SOAP-ENV:Header>
         <tec:entete>
           <version>1.0</version>
           <infoDemandeur>
@@ -115,15 +555,15 @@
           <loginDemandeur>test@example.com</loginDemandeur>
           <contratId>1234</contratId>
           <autorisationClient>false</autorisationClient>
         </ns1:consulterMesures>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesures/v1.1
-AHC-R1 (C1-C4):
+AHC-R1 (C1-C4) \*:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultermesures/v1.1">
       <SOAP-ENV:Header>
         <tec:entete>
           <version>1.1</version>
           <infoDemandeur>
             <loginDemandeur>test@example.com</loginDemandeur>
@@ -157,15 +597,15 @@
           <loginDemandeur>test@example.com</loginDemandeur>
           <contratId>1234</contratId>
           <autorisationClient>true</autorisationClient>
         </ns1:consulterMesures>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesures/v1.1
-ASS-R1 \*:
+ASS-R1 (C5) \*\*:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://www.enedis.fr/sge/b2b/commanderarretservicesouscritmesures/v1.0" xmlns:ns1="http://schemas.xmlsoap.org/soap/envelope/">
       <SOAP-ENV:Header>
         <tec:entete>
           <version>1.0</version>
           <infoDemandeur>
             <loginDemandeur>test@example.com</loginDemandeur>
@@ -185,206 +625,234 @@
               <serviceSouscritId>47761068</serviceSouscritId>
             </arretServiceSouscrit>
           </demande>
         </ns0:commanderArretServiceSouscritMesures>
       </ns1:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/CommandeArretServiceSouscritMesures/v1.0
+Ass-R1 (C2-C4) \* \*\*:
+  data: |
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://www.enedis.fr/sge/b2b/commanderarretservicesouscritmesures/v1.0" xmlns:ns1="http://schemas.xmlsoap.org/soap/envelope/">
+      <SOAP-ENV:Header>
+        <tec:entete>
+          <version>1.0</version>
+          <infoDemandeur>
+            <loginDemandeur>test@example.com</loginDemandeur>
+          </infoDemandeur>
+        </tec:entete>
+      </SOAP-ENV:Header>
+      <ns1:Body>
+        <ns0:commanderArretServiceSouscritMesures>
+          <demande>
+            <donneesGenerales>
+              <objetCode>ASS</objetCode>
+              <pointId>98800000000246</pointId>
+              <initiateurLogin>test@example.com</initiateurLogin>
+              <contratId>1234</contratId>
+            </donneesGenerales>
+            <arretServiceSouscrit>
+              <serviceSouscritId>47761068</serviceSouscritId>
+            </arretServiceSouscrit>
+          </demande>
+        </ns0:commanderArretServiceSouscritMesures>
+      </ns1:Body>
+    </SOAP-ENV:Envelope>
+  url: https://sge-homologation-b2b.enedis.fr/CommandeArretServiceSouscritMesures/v1.0
 CMD2-NR1:
   data: |
-    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0" xmlns:ns1="http://schemas.xmlsoap.org/soap/envelope/">
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0">
       <SOAP-ENV:Header/>
-      <ns1:Body>
-        <ns0:consulterMesuresDetaillees>
+      <ns0:Body>
+        <ns1:consulterMesuresDetaillees>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
             <pointId>25478147557460</pointId>
             <mesuresTypeCode>COURBE</mesuresTypeCode>
             <grandeurPhysique>PA</grandeurPhysique>
             <soutirage>true</soutirage>
             <injection>false</injection>
             <dateDebut>2022-04-01</dateDebut>
-            <dateFin>2022-04-07</dateFin>
+            <dateFin>2022-04-17</dateFin>
             <mesuresCorrigees>false</mesuresCorrigees>
             <accordClient>true</accordClient>
           </demande>
-        </ns0:consulterMesuresDetaillees>
-      </ns1:Body>
+        </ns1:consulterMesuresDetaillees>
+      </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v2.0
 CMD2-NR2:
   data: |
-    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0" xmlns:ns1="http://schemas.xmlsoap.org/soap/envelope/">
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0">
       <SOAP-ENV:Header/>
-      <ns1:Body>
-        <ns0:consulterMesuresDetaillees>
+      <ns0:Body>
+        <ns1:consulterMesuresDetaillees>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
             <pointId>25478147557460</pointId>
             <mesuresTypeCode>ENERGIE</mesuresTypeCode>
             <grandeurPhysique>EA</grandeurPhysique>
             <soutirage>true</soutirage>
             <injection>false</injection>
             <dateDebut>2022-04-01</dateDebut>
             <dateFin>2022-04-07</dateFin>
             <mesuresCorrigees>false</mesuresCorrigees>
             <accordClient>false</accordClient>
           </demande>
-        </ns0:consulterMesuresDetaillees>
-      </ns1:Body>
+        </ns1:consulterMesuresDetaillees>
+      </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v2.0
 CMD2-R1 (C1-C4):
   data: |
-    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0" xmlns:ns1="http://schemas.xmlsoap.org/soap/envelope/">
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0">
       <SOAP-ENV:Header/>
-      <ns1:Body>
-        <ns0:consulterMesuresDetaillees>
+      <ns0:Body>
+        <ns1:consulterMesuresDetaillees>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
             <pointId>30001610071843</pointId>
             <mesuresTypeCode>COURBE</mesuresTypeCode>
             <grandeurPhysique>PA</grandeurPhysique>
             <soutirage>true</soutirage>
             <injection>false</injection>
             <dateDebut>2022-04-01</dateDebut>
             <dateFin>2022-04-07</dateFin>
             <mesuresCorrigees>false</mesuresCorrigees>
             <accordClient>true</accordClient>
           </demande>
-        </ns0:consulterMesuresDetaillees>
-      </ns1:Body>
+        </ns1:consulterMesuresDetaillees>
+      </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v2.0
 CMD2-R1 (C5):
   data: |
-    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0" xmlns:ns1="http://schemas.xmlsoap.org/soap/envelope/">
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0">
       <SOAP-ENV:Header/>
-      <ns1:Body>
-        <ns0:consulterMesuresDetaillees>
+      <ns0:Body>
+        <ns1:consulterMesuresDetaillees>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
             <pointId>25478147557460</pointId>
             <mesuresTypeCode>COURBE</mesuresTypeCode>
             <grandeurPhysique>PA</grandeurPhysique>
             <soutirage>true</soutirage>
             <injection>false</injection>
             <dateDebut>2022-04-01</dateDebut>
             <dateFin>2022-04-07</dateFin>
             <mesuresCorrigees>false</mesuresCorrigees>
             <accordClient>true</accordClient>
           </demande>
-        </ns0:consulterMesuresDetaillees>
-      </ns1:Body>
+        </ns1:consulterMesuresDetaillees>
+      </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v2.0
 CMD2-R2:
   data: |
-    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0" xmlns:ns1="http://schemas.xmlsoap.org/soap/envelope/">
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0">
       <SOAP-ENV:Header/>
-      <ns1:Body>
-        <ns0:consulterMesuresDetaillees>
+      <ns0:Body>
+        <ns1:consulterMesuresDetaillees>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
             <pointId>30001610071843</pointId>
             <mesuresTypeCode>COURBE</mesuresTypeCode>
             <grandeurPhysique>PRI</grandeurPhysique>
             <soutirage>true</soutirage>
             <injection>false</injection>
             <dateDebut>2022-04-01</dateDebut>
             <dateFin>2022-04-07</dateFin>
             <mesuresCorrigees>false</mesuresCorrigees>
             <accordClient>true</accordClient>
           </demande>
-        </ns0:consulterMesuresDetaillees>
-      </ns1:Body>
+        </ns1:consulterMesuresDetaillees>
+      </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v2.0
 CMD2-R3:
   data: |
-    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0" xmlns:ns1="http://schemas.xmlsoap.org/soap/envelope/">
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0">
       <SOAP-ENV:Header/>
-      <ns1:Body>
-        <ns0:consulterMesuresDetaillees>
+      <ns0:Body>
+        <ns1:consulterMesuresDetaillees>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
             <pointId>25478147557460</pointId>
             <mesuresTypeCode>ENERGIE</mesuresTypeCode>
             <grandeurPhysique>EA</grandeurPhysique>
             <soutirage>true</soutirage>
             <injection>false</injection>
             <dateDebut>2022-04-01</dateDebut>
             <dateFin>2022-04-07</dateFin>
             <mesuresCorrigees>false</mesuresCorrigees>
             <accordClient>true</accordClient>
           </demande>
-        </ns0:consulterMesuresDetaillees>
-      </ns1:Body>
+        </ns1:consulterMesuresDetaillees>
+      </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v2.0
 CMD2-R4:
   data: |
-    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0" xmlns:ns1="http://schemas.xmlsoap.org/soap/envelope/">
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/v2.0">
       <SOAP-ENV:Header/>
-      <ns1:Body>
-        <ns0:consulterMesuresDetaillees>
+      <ns0:Body>
+        <ns1:consulterMesuresDetaillees>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
             <pointId>25478147557460</pointId>
             <mesuresTypeCode>PMAX</mesuresTypeCode>
             <grandeurPhysique>PMA</grandeurPhysique>
             <soutirage>true</soutirage>
             <injection>false</injection>
             <dateDebut>2022-04-01</dateDebut>
             <dateFin>2022-04-07</dateFin>
             <mesuresPas>P1D</mesuresPas>
             <mesuresCorrigees>false</mesuresCorrigees>
             <accordClient>true</accordClient>
           </demande>
-        </ns0:consulterMesuresDetaillees>
-      </ns1:Body>
+        </ns1:consulterMesuresDetaillees>
+      </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v2.0
 CMD3-NR1:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/common">
       <SOAP-ENV:Header/>
       <ns0:Body>
         <ns1:consulterMesuresDetailleesV3>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
             <pointId>25478147557460</pointId>
             <mesuresTypeCode>COURBE</mesuresTypeCode>
             <grandeurPhysique>PA</grandeurPhysique>
             <dateDebut>2022-04-01</dateDebut>
-            <dateFin>2022-04-08</dateFin>
+            <dateFin>2022-04-17</dateFin>
             <mesuresCorrigees>false</mesuresCorrigees>
             <sens>SOUTIRAGE</sens>
             <cadreAcces>ACCORD_CLIENT</cadreAcces>
           </demande>
         </ns1:consulterMesuresDetailleesV3>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v3.0
-CMD3-NR2:
+CMD3-NR2 \*:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/common">
       <SOAP-ENV:Header/>
       <ns0:Body>
         <ns1:consulterMesuresDetailleesV3>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
             <pointId>25478147557460</pointId>
             <mesuresTypeCode>INDEX</mesuresTypeCode>
             <grandeurPhysique>EA</grandeurPhysique>
             <dateDebut>2022-04-01</dateDebut>
-            <dateFin>2022-04-08</dateFin>
+            <dateFin>2022-04-17</dateFin>
             <mesuresCorrigees>false</mesuresCorrigees>
             <sens>SOUTIRAGE</sens>
-            <cadreAcces>ACCORD_CLIENT</cadreAcces>
+            <cadreAcces>SERVICE_ACCES</cadreAcces>
           </demande>
         </ns1:consulterMesuresDetailleesV3>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v3.0
 CMD3-R1 (C1-C4):
   data: |
@@ -445,15 +913,15 @@
             <sens>SOUTIRAGE</sens>
             <cadreAcces>ACCORD_CLIENT</cadreAcces>
           </demande>
         </ns1:consulterMesuresDetailleesV3>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v3.0
-CMD3-R3 (C1-C4):
+CMD3-R3 (C1-C4) \*:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/common">
       <SOAP-ENV:Header/>
       <ns0:Body>
         <ns1:consulterMesuresDetailleesV3>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
@@ -509,15 +977,15 @@
             <sens>SOUTIRAGE</sens>
             <cadreAcces>ACCORD_CLIENT</cadreAcces>
           </demande>
         </ns1:consulterMesuresDetailleesV3>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v3.0
-CMD3-R5 (C1-C4):
+CMD3-R5 (C1-C4) \*:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/common">
       <SOAP-ENV:Header/>
       <ns0:Body>
         <ns1:consulterMesuresDetailleesV3>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
@@ -530,15 +998,15 @@
             <sens>SOUTIRAGE</sens>
             <cadreAcces>ACCORD_CLIENT</cadreAcces>
           </demande>
         </ns1:consulterMesuresDetailleesV3>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v3.0
-CMD3-R5 (C5):
+CMD3-R5 (C5) \*:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/common">
       <SOAP-ENV:Header/>
       <ns0:Body>
         <ns1:consulterMesuresDetailleesV3>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
@@ -551,15 +1019,15 @@
             <sens>SOUTIRAGE</sens>
             <cadreAcces>ACCORD_CLIENT</cadreAcces>
           </demande>
         </ns1:consulterMesuresDetailleesV3>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v3.0
-CMD3-R6 (C1-C4):
+CMD3-R6 (C1-C4) \*:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/common">
       <SOAP-ENV:Header/>
       <ns0:Body>
         <ns1:consulterMesuresDetailleesV3>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
@@ -572,15 +1040,15 @@
             <sens>SOUTIRAGE</sens>
             <cadreAcces>SERVICE_ACCES</cadreAcces>
           </demande>
         </ns1:consulterMesuresDetailleesV3>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/ConsultationMesuresDetaillees/v3.0
-CMD3-R6 (C5):
+CMD3-R6 (C5) \*:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/consultationmesuresdetaillees/common">
       <SOAP-ENV:Header/>
       <ns0:Body>
         <ns1:consulterMesuresDetailleesV3>
           <demande>
             <initiateurLogin>test@example.com</initiateurLogin>
@@ -1097,15 +1565,15 @@
               <periodiciteTransmission>P1D</periodiciteTransmission>
             </accesMesures>
           </demande>
         </ns1:commanderCollectePublicationMesures>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/CommandeCollectePublicationMesures/v3.0
-F375A-NR1:
+F375A-NR1 \*:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commandertransmissiondonneesinfraj/v1.0">
       <SOAP-ENV:Header>
         <tec:entete>
           <version>1.0</version>
           <infoDemandeur>
             <loginDemandeur>test@example.com</loginDemandeur>
@@ -1137,15 +1605,15 @@
               <ptd>false</ptd>
             </accesDonnees>
           </demande>
         </ns1:commanderTransmissionDonneesInfraJ>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/CommandeTransmissionDonneesInfraJ/v1.0
-F375A-R1:
+F375A-R1 \*:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commandertransmissiondonneesinfraj/v1.0">
       <SOAP-ENV:Header>
         <tec:entete>
           <version>1.0</version>
           <infoDemandeur>
             <loginDemandeur>test@example.com</loginDemandeur>
@@ -1270,28 +1738,28 @@
 F380-R1 (C5):
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:dc="http://www.erdf.fr/sge/b2b/dictionnaire/v4.0/dc" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/commandertransmissionhistoriquemesures/v1.0">
       <SOAP-ENV:Header>
         <dc:enteteP>
           <version>1.0</version>
           <infoFonctionnelles>
-            <pointId>25957452924301</pointId>
+            <pointId>24551519514005</pointId>
           </infoFonctionnelles>
           <infoDemandeur>
             <loginDemandeur>test@example.com</loginDemandeur>
           </infoDemandeur>
         </dc:enteteP>
       </SOAP-ENV:Header>
       <ns0:Body>
         <ns1:commanderTransmissionHistoriqueMesures>
           <demande>
             <donneesGenerales>
               <objetCode>HDM</objetCode>
               <contratId>1234</contratId>
-              <pointId>25957452924301</pointId>
+              <pointId>24551519514005</pointId>
               <initiateurLogin>test@example.com</initiateurLogin>
             </donneesGenerales>
             <historiqueMesures>
               <dateDebut>2020-02-23</dateDebut>
               <dateFin>2022-02-22</dateFin>
               <declarationAccordClient>
                 <accordClient>true</accordClient>
@@ -1468,15 +1936,15 @@
             <rechercheHorsPerimetre>false</rechercheHorsPerimetre>
           </criteres>
           <loginUtilisateur>test@example.com</loginUtilisateur>
         </ns1:rechercherPoint>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/RecherchePoint/v2.0
-RP-R2:
+RP-R2 \*:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/rechercherpoint/v2.0">
       <SOAP-ENV:Header>
         <tec:entete>
           <version>2.0</version>
           <infoDemandeur>
             <loginDemandeur>test@example.com</loginDemandeur>
@@ -1495,15 +1963,15 @@
             <rechercheHorsPerimetre>true</rechercheHorsPerimetre>
           </criteres>
           <loginUtilisateur>test@example.com</loginUtilisateur>
         </ns1:rechercherPoint>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/RecherchePoint/v2.0
-RP-R3:
+RP-R3 \*:
   data: |
     <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/services/rechercherpoint/v2.0">
       <SOAP-ENV:Header>
         <tec:entete>
           <version>2.0</version>
           <infoDemandeur>
             <loginDemandeur>test@example.com</loginDemandeur>
@@ -1522,73 +1990,51 @@
             <rechercheHorsPerimetre>true</rechercheHorsPerimetre>
           </criteres>
           <loginUtilisateur>test@example.com</loginUtilisateur>
         </ns1:rechercherPoint>
       </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/RecherchePoint/v2.0
-RS-R1 (C1-C4):
+RS-R1 (C2-C4) \*:
   data: |
-    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://www.enedis.fr/sge/b2b/rechercherservicessouscritsmesures/v1.0" xmlns:ns1="http://schemas.xmlsoap.org/soap/envelope/">
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/rechercherservicessouscritsmesures/v1.0">
       <SOAP-ENV:Header>
         <tec:entete>
           <version>1.0</version>
           <infoDemandeur>
             <loginDemandeur>test@example.com</loginDemandeur>
           </infoDemandeur>
         </tec:entete>
       </SOAP-ENV:Header>
-      <ns1:Body>
-        <ns0:rechercherServicesSouscritsMesures>
-          <criteres>
-            <pointId>98800000000246</pointId>
-            <contratId>1234</contratId>
-          </criteres>
-          <loginUtilisateur>test@example.com</loginUtilisateur>
-        </ns0:rechercherServicesSouscritsMesures>
-      </ns1:Body>
-    </SOAP-ENV:Envelope>
-  url: https://sge-homologation-b2b.enedis.fr/RechercheServicesSouscritsMesures/v1.0
-RS-R1 (C2-C4):
-  data: |
-    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://www.enedis.fr/sge/b2b/rechercherservicessouscritsmesures/v1.0" xmlns:ns1="http://schemas.xmlsoap.org/soap/envelope/">
-      <SOAP-ENV:Header>
-        <tec:entete>
-          <version>1.0</version>
-          <infoDemandeur>
-            <loginDemandeur>test@example.com</loginDemandeur>
-          </infoDemandeur>
-        </tec:entete>
-      </SOAP-ENV:Header>
-      <ns1:Body>
-        <ns0:rechercherServicesSouscritsMesures>
+      <ns0:Body>
+        <ns1:rechercherServicesSouscritsMesures>
           <criteres>
             <pointId>98800000000246</pointId>
             <contratId>1234</contratId>
           </criteres>
           <loginUtilisateur>test@example.com</loginUtilisateur>
-        </ns0:rechercherServicesSouscritsMesures>
-      </ns1:Body>
+        </ns1:rechercherServicesSouscritsMesures>
+      </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/RechercheServicesSouscritsMesures/v1.0
 RS-R1 (C5):
   data: |
-    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://www.enedis.fr/sge/b2b/rechercherservicessouscritsmesures/v1.0" xmlns:ns1="http://schemas.xmlsoap.org/soap/envelope/">
+    <SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:tec="http://www.enedis.fr/sge/b2b/technique/v1.0" xmlns:ns0="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ns1="http://www.enedis.fr/sge/b2b/rechercherservicessouscritsmesures/v1.0">
       <SOAP-ENV:Header>
         <tec:entete>
           <version>1.0</version>
           <infoDemandeur>
             <loginDemandeur>test@example.com</loginDemandeur>
           </infoDemandeur>
         </tec:entete>
       </SOAP-ENV:Header>
-      <ns1:Body>
-        <ns0:rechercherServicesSouscritsMesures>
+      <ns0:Body>
+        <ns1:rechercherServicesSouscritsMesures>
           <criteres>
             <pointId>25884515170669</pointId>
             <contratId>1234</contratId>
           </criteres>
           <loginUtilisateur>test@example.com</loginUtilisateur>
-        </ns0:rechercherServicesSouscritsMesures>
-      </ns1:Body>
+        </ns1:rechercherServicesSouscritsMesures>
+      </ns0:Body>
     </SOAP-ENV:Envelope>
   url: https://sge-homologation-b2b.enedis.fr/RechercheServicesSouscritsMesures/v1.0
```

### Comparing `lowatt-enedis-2.1.0/test/test_lowatt_enedis.py` & `lowatt-enedis-2.2.0/test/test_lowatt_enedis.py`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.1.0/test/test_requests.py` & `lowatt-enedis-2.2.0/test/test_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         for line in f:
             match = re.search(r"\|(.*)\|.*`(lowatt-enedis .*)`.*$", line)
             if match:
                 case, command = match.groups()
                 case = case.strip()
                 assert case not in cases
                 cases[case] = command
-    assert len(cases) == 54
+    assert len(cases) == 66
     _cache[None] = cases
     return cases
 
 
 class ExpectedDict(TypedDict):
     url: str
     data: str
```

### Comparing `lowatt-enedis-2.1.0/tox.ini` & `lowatt-enedis-2.2.0/tox.ini`

 * *Files identical despite different names*

