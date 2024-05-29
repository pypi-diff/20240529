# Comparing `tmp/koap-0.2.0.tar.gz` & `tmp/koap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koap-0.2.0.tar", max compression
+gzip compressed data, was "koap-0.3.0.tar", max compression
```

## Comparing `koap-0.2.0.tar` & `koap-0.3.0.tar`

### file list

```diff
@@ -1,246 +1,248 @@
--rw-r--r--   0        0        0     2125 2023-06-07 09:01:38.591048 koap-0.2.0/README.md
--rw-r--r--   0        0        0       22 2023-06-07 09:01:38.591313 koap-0.2.0/koap/__init__.py
--rw-r--r--   0        0        0       46 2023-05-30 05:50:35.004498 koap-0.2.0/koap/api-telematik/.git
--rw-r--r--   0        0        0        0 2023-05-30 05:50:35.019841 koap-0.2.0/koap/api-telematik/.gitignore
--rw-r--r--   0        0        0     3277 2023-05-30 05:50:35.019991 koap-0.2.0/koap/api-telematik/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2948 2023-05-30 05:50:35.020109 koap-0.2.0/koap/api-telematik/CONTRIBUTING.md
--rw-r--r--   0        0        0      555 2023-05-30 05:50:35.020188 koap-0.2.0/koap/api-telematik/LICENSE
--rw-r--r--   0        0        0     1857 2023-05-30 05:50:35.020283 koap-0.2.0/koap/api-telematik/Readme.md
--rw-r--r--   0        0        0     1682 2023-05-30 05:50:35.020378 koap-0.2.0/koap/api-telematik/ReleaseNotes.md
--rw-r--r--   0        0        0     4675 2023-05-30 05:50:35.020650 koap-0.2.0/koap/api-telematik/cm/cc/CCS.wsdl
--rw-r--r--   0        0        0     2513 2023-05-30 05:50:35.020746 koap-0.2.0/koap/api-telematik/cm/cc/CmCcCommon.xsd
--rw-r--r--   0        0        0     1887 2023-05-30 05:50:35.020894 koap-0.2.0/koap/api-telematik/cm/cc/CmCcServiceRequest.xsd
--rw-r--r--   0        0        0     1754 2023-05-30 05:50:35.020973 koap-0.2.0/koap/api-telematik/cm/cc/CmCcServiceResponse.xsd
--rw-r--r--   0        0        0     2962 2023-05-30 05:50:35.021127 koap-0.2.0/koap/api-telematik/cm/common/CmCommon.xsd
--rw-r--r--   0        0        0     1519 2023-05-30 05:50:35.021258 koap-0.2.0/koap/api-telematik/cm/uf/CmUfServiceRequest.xsd
--rw-r--r--   0        0        0     1397 2023-05-30 05:50:35.021355 koap-0.2.0/koap/api-telematik/cm/uf/CmUfServiceResponse.xsd
--rw-r--r--   0        0        0     3106 2023-05-30 05:50:35.021427 koap-0.2.0/koap/api-telematik/cm/uf/UFS.wsdl
--rw-r--r--   0        0        0     3474 2023-05-30 05:50:35.021611 koap-0.2.0/koap/api-telematik/conn/AuthSignatureService.wsdl
--rw-r--r--   0        0        0     3165 2023-05-30 05:50:35.021721 koap-0.2.0/koap/api-telematik/conn/AuthSignatureService_v7_4_1.wsdl
--rw-r--r--   0        0        0     4025 2023-05-30 05:50:35.021844 koap-0.2.0/koap/api-telematik/conn/CardEvents.xsd
--rw-r--r--   0        0        0     6062 2023-05-30 05:50:35.021922 koap-0.2.0/koap/api-telematik/conn/CardService.wsdl
--rw-r--r--   0        0        0     7314 2023-05-30 05:50:35.022065 koap-0.2.0/koap/api-telematik/conn/CardService.xsd
--rw-r--r--   0        0        0     2992 2023-05-30 05:50:35.022188 koap-0.2.0/koap/api-telematik/conn/CardServiceCommon.xsd
--rw-r--r--   0        0        0     5558 2023-05-30 05:50:35.022280 koap-0.2.0/koap/api-telematik/conn/CardService_v8_1_1.wsdl
--rw-r--r--   0        0        0     7252 2023-05-30 05:50:35.022392 koap-0.2.0/koap/api-telematik/conn/CardService_v8_1_1.xsd
--rw-r--r--   0        0        0     7181 2023-05-30 05:50:35.022484 koap-0.2.0/koap/api-telematik/conn/CardService_v8_1_2.wsdl
--rw-r--r--   0        0        0     9266 2023-05-30 05:50:35.022644 koap-0.2.0/koap/api-telematik/conn/CardService_v8_1_3.xsd
--rw-r--r--   0        0        0     4556 2023-05-30 05:50:35.022773 koap-0.2.0/koap/api-telematik/conn/CardTerminalInfo.xsd
--rw-r--r--   0        0        0     3772 2023-05-30 05:50:35.022869 koap-0.2.0/koap/api-telematik/conn/CardTerminalService.wsdl
--rw-r--r--   0        0        0     3478 2023-05-30 05:50:35.023001 koap-0.2.0/koap/api-telematik/conn/CardTerminalService.xsd
--rw-r--r--   0        0        0     4421 2023-05-30 05:50:35.023095 koap-0.2.0/koap/api-telematik/conn/CertificateService.wsdl
--rw-r--r--   0        0        0     5694 2023-05-30 05:50:35.023173 koap-0.2.0/koap/api-telematik/conn/CertificateService.xsd
--rw-r--r--   0        0        0     3959 2023-05-30 05:50:35.023269 koap-0.2.0/koap/api-telematik/conn/CertificateServiceCommon.xsd
--rw-r--r--   0        0        0     4428 2023-05-30 05:50:35.023341 koap-0.2.0/koap/api-telematik/conn/CertificateService_v6_0_1.wsdl
--rw-r--r--   0        0        0     6145 2023-05-30 05:50:35.023411 koap-0.2.0/koap/api-telematik/conn/CertificateService_v6_0_2.xsd
--rw-r--r--   0        0        0     6672 2023-05-30 05:50:35.023484 koap-0.2.0/koap/api-telematik/conn/ConnectorCommon.xsd
--rw-r--r--   0        0        0     2325 2023-05-30 05:50:35.023566 koap-0.2.0/koap/api-telematik/conn/ConnectorContext.xsd
--rw-r--r--   0        0        0     3530 2023-05-30 05:50:35.023635 koap-0.2.0/koap/api-telematik/conn/EncryptionService.wsdl
--rw-r--r--   0        0        0     4567 2023-05-30 05:50:35.023735 koap-0.2.0/koap/api-telematik/conn/EncryptionService.xsd
--rw-r--r--   0        0        0     4045 2023-05-30 05:50:35.023865 koap-0.2.0/koap/api-telematik/conn/EncryptionService_v6_1_1.wsdl
--rw-r--r--   0        0        0     6226 2023-05-30 05:50:35.024105 koap-0.2.0/koap/api-telematik/conn/EncryptionService_v6_1_2.xsd
--rw-r--r--   0        0        0     7882 2023-05-30 05:50:35.024186 koap-0.2.0/koap/api-telematik/conn/EventService.wsdl
--rw-r--r--   0        0        0    11246 2023-05-30 05:50:35.024260 koap-0.2.0/koap/api-telematik/conn/EventService.xsd
--rw-r--r--   0        0        0    18683 2023-05-30 05:50:35.024391 koap-0.2.0/koap/api-telematik/conn/OperatingData.xsd
--rw-r--r--   0        0        0      331 2023-05-30 05:50:35.024484 koap-0.2.0/koap/api-telematik/conn/README.CardService.txt
--rw-r--r--   0        0        0     1714 2023-05-30 05:50:35.024555 koap-0.2.0/koap/api-telematik/conn/ServiceDirectory.xsd
--rw-r--r--   0        0        0     3056 2023-05-30 05:50:35.024631 koap-0.2.0/koap/api-telematik/conn/ServiceInformation.xsd
--rw-r--r--   0        0        0     5771 2023-05-30 05:50:35.024706 koap-0.2.0/koap/api-telematik/conn/SignatureService.wsdl
--rw-r--r--   0        0        0    16413 2023-05-30 05:50:35.024778 koap-0.2.0/koap/api-telematik/conn/SignatureService.xsd
--rw-r--r--   0        0        0     6634 2023-05-30 05:50:35.024863 koap-0.2.0/koap/api-telematik/conn/SignatureService_V7_4_2.wsdl
--rw-r--r--   0        0        0    16939 2023-05-30 05:50:35.024937 koap-0.2.0/koap/api-telematik/conn/SignatureService_V7_4_4.xsd
--rw-r--r--   0        0        0    10283 2023-05-30 05:50:35.025016 koap-0.2.0/koap/api-telematik/conn/SignatureService_V7_5_5.wsdl
--rw-r--r--   0        0        0    20062 2023-05-30 05:50:35.025098 koap-0.2.0/koap/api-telematik/conn/SignatureService_V7_5_5.xsd
--rw-r--r--   0        0        0    10593 2023-05-30 05:50:35.025213 koap-0.2.0/koap/api-telematik/conn/SignatureService_V7_5_6.wsdl
--rw-r--r--   0        0        0    20375 2023-05-30 05:50:35.025349 koap-0.2.0/koap/api-telematik/conn/SignatureService_V7_5_6.xsd
--rw-r--r--   0        0        0     6144 2023-05-30 05:50:35.025488 koap-0.2.0/koap/api-telematik/conn/amtss/AMTSService.wsdl
--rw-r--r--   0        0        0     4231 2023-05-30 05:50:35.025570 koap-0.2.0/koap/api-telematik/conn/amtss/AMTSService.xsd
--rw-r--r--   0        0        0     3703 2023-05-30 05:50:35.025684 koap-0.2.0/koap/api-telematik/conn/nfds/DPEService.wsdl
--rw-r--r--   0        0        0     6011 2023-05-30 05:50:35.025774 koap-0.2.0/koap/api-telematik/conn/nfds/DPEService.xsd
--rw-r--r--   0        0        0     3800 2023-05-30 05:50:35.025854 koap-0.2.0/koap/api-telematik/conn/nfds/NFDService.wsdl
--rw-r--r--   0        0        0     6739 2023-05-30 05:50:35.025949 koap-0.2.0/koap/api-telematik/conn/nfds/NFDService.xsd
--rw-r--r--   0        0        0     8566 2023-05-30 05:50:35.026058 koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService.wsdl
--rw-r--r--   0        0        0     8948 2023-05-30 05:50:35.026195 koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService.xsd
--rw-r--r--   0        0        0    10213 2023-05-30 05:50:35.026281 koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_1.wsdl
--rw-r--r--   0        0        0    12910 2023-05-30 05:50:35.026388 koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_1.xsd
--rw-r--r--   0        0        0    10528 2023-05-30 05:50:35.026509 koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_2.wsdl
--rw-r--r--   0        0        0    13225 2023-05-30 05:50:35.026670 koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_2.xsd
--rw-r--r--   0        0        0    10460 2023-05-30 05:50:35.026742 koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_2.wsdl
--rw-r--r--   0        0        0    13276 2023-05-30 05:50:35.026816 koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_2.xsd
--rw-r--r--   0        0        0    10775 2023-05-30 05:50:35.026888 koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_3.wsdl
--rw-r--r--   0        0        0    13591 2023-05-30 05:50:35.026955 koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_3.xsd
--rw-r--r--   0        0        0    10310 2023-05-30 05:50:35.027076 koap-0.2.0/koap/api-telematik/conn/phrs/PHRService.wsdl
--rw-r--r--   0        0        0     2045 2023-05-30 05:50:35.027174 koap-0.2.0/koap/api-telematik/conn/phrs/PHRService.xsd
--rw-r--r--   0        0        0     9350 2023-05-30 05:50:35.027276 koap-0.2.0/koap/api-telematik/conn/phrs/PHRService_V2_0_1.wsdl
--rw-r--r--   0        0        0     2499 2023-05-30 05:50:35.027359 koap-0.2.0/koap/api-telematik/conn/phrs/PHRService_V2_0_1.xsd
--rw-r--r--   0        0        0     9586 2023-05-30 05:50:35.027456 koap-0.2.0/koap/api-telematik/conn/phrs/PHRService_V2_0_2.wsdl
--rw-r--r--   0        0        0     2734 2023-05-30 05:50:35.027561 koap-0.2.0/koap/api-telematik/conn/phrs/PHRService_V2_0_2.xsd
--rw-r--r--   0        0        0     5868 2023-05-30 05:50:35.027692 koap-0.2.0/koap/api-telematik/conn/tbauth/IdpServiceActiveRequestor.wsdl
--rw-r--r--   0        0        0     4948 2023-05-30 05:50:35.027788 koap-0.2.0/koap/api-telematik/conn/tbauth/LocalIdpService.wsdl
--rw-r--r--   0        0        0     2330 2023-05-30 05:50:35.027908 koap-0.2.0/koap/api-telematik/conn/vsds/KvkService.wsdl
--rw-r--r--   0        0        0     1691 2023-05-30 05:50:35.027991 koap-0.2.0/koap/api-telematik/conn/vsds/KvkService.xsd
--rw-r--r--   0        0        0     2242 2023-05-30 05:50:35.028071 koap-0.2.0/koap/api-telematik/conn/vsds/VSDService.wsdl
--rw-r--r--   0        0        0     2528 2023-05-30 05:50:35.028205 koap-0.2.0/koap/api-telematik/conn/vsds/VSDService.xsd
--rw-r--r--   0        0        0     2554 2023-05-30 05:50:35.028327 koap-0.2.0/koap/api-telematik/consumer/CertificateService.wsdl
--rw-r--r--   0        0        0     3026 2023-05-30 05:50:35.028438 koap-0.2.0/koap/api-telematik/consumer/CertificateService.xsd
--rw-r--r--   0        0        0     1903 2023-05-30 05:50:35.028535 koap-0.2.0/koap/api-telematik/consumer/CertificateServiceCommon.xsd
--rw-r--r--   0        0        0     4521 2023-05-30 05:50:35.028613 koap-0.2.0/koap/api-telematik/consumer/ConsumerCommon.xsd
--rw-r--r--   0        0        0     3112 2023-05-30 05:50:35.028687 koap-0.2.0/koap/api-telematik/consumer/EPAService.wsdl
--rw-r--r--   0        0        0     3583 2023-05-30 05:50:35.028825 koap-0.2.0/koap/api-telematik/consumer/EPAService.xsd
--rw-r--r--   0        0        0     3428 2023-05-30 05:50:35.028940 koap-0.2.0/koap/api-telematik/consumer/EncryptionService.wsdl
--rw-r--r--   0        0        0     3447 2023-05-30 05:50:35.029057 koap-0.2.0/koap/api-telematik/consumer/EncryptionService.xsd
--rw-r--r--   0        0        0     4493 2023-05-30 05:50:35.029156 koap-0.2.0/koap/api-telematik/consumer/SignatureService.wsdl
--rw-r--r--   0        0        0     9529 2023-05-30 05:50:35.029252 koap-0.2.0/koap/api-telematik/consumer/SignatureService.xsd
--rw-r--r--   0        0        0    18833 2023-05-30 05:50:35.029422 koap-0.2.0/koap/api-telematik/ext/DSMLv2.xsd
--rw-r--r--   0        0        0    24995 2023-05-30 05:50:35.029728 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/NarrativeBlock.xsd
--rw-r--r--   0        0        0    79308 2023-05-30 05:50:35.030072 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/datatypes-base.xsd
--rw-r--r--   0        0        0    62014 2023-05-30 05:50:35.030409 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/datatypes.xsd
--rw-r--r--   0        0        0     1633 2023-05-30 05:50:35.030504 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/infrastructureRoot.xsd
--rw-r--r--   0        0        0   837069 2023-05-30 05:50:35.032395 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/voc.xsd
--rw-r--r--   0        0        0    20318 2023-05-30 05:50:35.032847 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030000UV04.xsd
--rw-r--r--   0        0        0    19744 2023-05-30 05:50:35.033006 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030007UV.xsd
--rw-r--r--   0        0        0     5143 2023-05-30 05:50:35.033201 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030202UV01.xsd
--rw-r--r--   0        0        0     4436 2023-05-30 05:50:35.033272 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030203UV02.xsd
--rw-r--r--   0        0        0     4594 2023-05-30 05:50:35.033391 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030207UV.xsd
--rw-r--r--   0        0        0     4484 2023-05-30 05:50:35.033768 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT040008UV.xsd
--rw-r--r--   0        0        0     3999 2023-05-30 05:50:35.034028 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT040203UV01.xsd
--rw-r--r--   0        0        0     4506 2023-05-30 05:50:35.034199 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT050000UV01.xsd
--rw-r--r--   0        0        0     8115 2023-05-30 05:50:35.034307 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT060000UV01.xsd
--rw-r--r--   0        0        0     3751 2023-05-30 05:50:35.034403 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT070000UV01.xsd
--rw-r--r--   0        0        0    37643 2023-05-30 05:50:35.034662 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT080000UV.xsd
--rw-r--r--   0        0        0    13047 2023-05-30 05:50:35.034806 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090000UV01.xsd
--rw-r--r--   0        0        0     6111 2023-05-30 05:50:35.034886 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090002UV01.xsd
--rw-r--r--   0        0        0     6196 2023-05-30 05:50:35.034972 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090003UV01.xsd
--rw-r--r--   0        0        0     9598 2023-05-30 05:50:35.035076 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090100UV01.xsd
--rw-r--r--   0        0        0     4424 2023-05-30 05:50:35.035162 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090102UV02.xsd
--rw-r--r--   0        0        0     4536 2023-05-30 05:50:35.035245 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090108UV.xsd
--rw-r--r--   0        0        0     9682 2023-05-30 05:50:35.035336 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090300UV01.xsd
--rw-r--r--   0        0        0     4672 2023-05-30 05:50:35.035426 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090303UV01.xsd
--rw-r--r--   0        0        0     3557 2023-05-30 05:50:35.035515 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT140007UV.xsd
--rw-r--r--   0        0        0     7942 2023-05-30 05:50:35.035628 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150000UV02.xsd
--rw-r--r--   0        0        0     3564 2023-05-30 05:50:35.035723 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150002UV01.xsd
--rw-r--r--   0        0        0     5094 2023-05-30 05:50:35.035858 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150003UV03.xsd
--rw-r--r--   0        0        0     5082 2023-05-30 05:50:35.035940 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150007UV.xsd
--rw-r--r--   0        0        0    31953 2023-05-30 05:50:35.036044 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT230100UV.xsd
--rw-r--r--   0        0        0     4103 2023-05-30 05:50:35.036186 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT240000UV01.xsd
--rw-r--r--   0        0        0     3938 2023-05-30 05:50:35.036252 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT240003UV02.xsd
--rw-r--r--   0        0        0    13645 2023-05-30 05:50:35.036357 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT260003UV.xsd
--rw-r--r--   0        0        0     3636 2023-05-30 05:50:35.036587 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT280000UV04.xsd
--rw-r--r--   0        0        0    40301 2023-05-30 05:50:35.036753 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT290000UV06.xsd
--rw-r--r--   0        0        0    19515 2023-05-30 05:50:35.036848 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT300000UV04.xsd
--rw-r--r--   0        0        0    11445 2023-05-30 05:50:35.037102 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT310000UV04.xsd
--rw-r--r--   0        0        0     3711 2023-05-30 05:50:35.037242 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT440001UV.xsd
--rw-r--r--   0        0        0    15571 2023-05-30 05:50:35.037363 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT490000UV04.xsd
--rw-r--r--   0        0        0    12585 2023-05-30 05:50:35.037455 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT500000UV04.xsd
--rw-r--r--   0        0        0    51960 2023-05-30 05:50:35.037621 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT510000UV06.xsd
--rw-r--r--   0        0        0    75794 2023-05-30 05:50:35.038007 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT530000UV.xsd
--rw-r--r--   0        0        0    17638 2023-05-30 05:50:35.038164 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT600000UV06.xsd
--rw-r--r--   0        0        0     8190 2023-05-30 05:50:35.038283 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT670000UV04.xsd
--rw-r--r--   0        0        0     5463 2023-05-30 05:50:35.038369 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT710000UV01.xsd
--rw-r--r--   0        0        0     4334 2023-05-30 05:50:35.038620 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT710007UV.xsd
--rw-r--r--   0        0        0    12515 2023-05-30 05:50:35.038781 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT740000UV04.xsd
--rw-r--r--   0        0        0     8037 2023-05-30 05:50:35.038850 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT810000UV.xsd
--rw-r--r--   0        0        0     8104 2023-05-30 05:50:35.038938 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT820000UV.xsd
--rw-r--r--   0        0        0     9586 2023-05-30 05:50:35.039110 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT960000UV05.xsd
--rw-r--r--   0        0        0     9288 2023-05-30 05:50:35.039436 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCAI_MT900001UV01.xsd
--rw-r--r--   0        0        0     1878 2023-05-30 05:50:35.040075 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_IN000002UV01.xsd
--rw-r--r--   0        0        0    13447 2023-05-30 05:50:35.040142 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_MT000100UV01.xsd
--rw-r--r--   0        0        0    15472 2023-05-30 05:50:35.040204 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_MT000200UV01.xsd
--rw-r--r--   0        0        0    15517 2023-05-30 05:50:35.040271 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_MT000300UV01.xsd
--rw-r--r--   0        0        0    23361 2023-05-30 05:50:35.040333 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MFMI_MT700701UV01.xsd
--rw-r--r--   0        0        0    24434 2023-05-30 05:50:35.040412 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MFMI_MT700711UV01.xsd
--rw-r--r--   0        0        0     9172 2023-05-30 05:50:35.040482 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201301UV02.xsd
--rw-r--r--   0        0        0     9172 2023-05-30 05:50:35.040549 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201302UV02.xsd
--rw-r--r--   0        0        0     9172 2023-05-30 05:50:35.040614 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201303UV02.xsd
--rw-r--r--   0        0        0     9172 2023-05-30 05:50:35.040666 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201304UV02.xsd
--rw-r--r--   0        0        0     6149 2023-05-30 05:50:35.040745 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201305UV02.xsd
--rw-r--r--   0        0        0     9622 2023-05-30 05:50:35.040811 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201306UV02.xsd
--rw-r--r--   0        0        0     6149 2023-05-30 05:50:35.040870 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201309UV02.xsd
--rw-r--r--   0        0        0     9622 2023-05-30 05:50:35.040925 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201310UV02.xsd
--rw-r--r--   0        0        0    29790 2023-05-30 05:50:35.040992 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201301UV02.xsd
--rw-r--r--   0        0        0    32540 2023-05-30 05:50:35.041108 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201302UV02.xsd
--rw-r--r--   0        0        0    29790 2023-05-30 05:50:35.041186 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201303UV02.xsd
--rw-r--r--   0        0        0    14556 2023-05-30 05:50:35.041275 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201304UV02.xsd
--rw-r--r--   0        0        0     7460 2023-05-30 05:50:35.041342 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201305UV02.xsd
--rw-r--r--   0        0        0    17454 2023-05-30 05:50:35.041424 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201306UV02.xsd
--rw-r--r--   0        0        0     5386 2023-05-30 05:50:35.041490 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201307UV02.xsd
--rw-r--r--   0        0        0    31181 2023-05-30 05:50:35.041555 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201310UV02.xsd
--rw-r--r--   0        0        0     4107 2023-05-30 05:50:35.041625 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/QUQI_IN000003UV01.xsd
--rw-r--r--   0        0        0    11800 2023-05-30 05:50:35.041683 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/QUQI_MT000001UV01.xsd
--rw-r--r--   0        0        0    11145 2023-05-30 05:50:35.041743 koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/QUQI_MT021001UV01.xsd
--rw-r--r--   0        0        0     1237 2023-05-30 05:50:35.041868 koap-0.2.0/koap/api-telematik/ext/IHE/RMD.xsd
--rw-r--r--   0        0        0     5163 2023-05-30 05:50:35.041947 koap-0.2.0/koap/api-telematik/ext/IHE/XDS.b_DocumentRepository.xsd
--rw-r--r--   0        0        0    13287 2023-05-30 05:50:35.042178 koap-0.2.0/koap/api-telematik/ext/IHE/healthcare-security-audit.xsd
--rw-r--r--   0        0        0      443 2023-05-30 05:50:35.042248 koap-0.2.0/koap/api-telematik/ext/IHE/ihe-appc-xacml-combined-schema-1.0.xsd
--rw-r--r--   0        0        0     2925 2023-05-30 05:50:35.042319 koap-0.2.0/koap/api-telematik/ext/IHE/ihe-appc-xacml-hl7-datatypes-base-1.0.xsd
--rw-r--r--   0        0        0    21304 2023-05-30 05:50:35.042412 koap-0.2.0/koap/api-telematik/ext/XAdES.xsd
--rw-r--r--   0        0        0    23190 2023-05-30 05:50:35.042524 koap-0.2.0/koap/api-telematik/ext/XAdES_NFDM_hardened.xsd
--rw-r--r--   0        0        0    16075 2023-05-30 05:50:35.042639 koap-0.2.0/koap/api-telematik/ext/XMLSchema.dtd
--rw-r--r--   0        0        0    14895 2023-05-30 05:50:35.042729 koap-0.2.0/koap/api-telematik/ext/access_control-xacml-2.0-policy-schema-os.xsd
--rw-r--r--   0        0        0    10081 2023-05-30 05:50:35.042813 koap-0.2.0/koap/api-telematik/ext/charset.xsd
--rw-r--r--   0        0        0     6357 2023-05-30 05:50:35.042895 koap-0.2.0/koap/api-telematik/ext/datatypes.dtd
--rw-r--r--   0        0        0     3474 2023-05-30 05:50:35.043035 koap-0.2.0/koap/api-telematik/ext/ebRS/cms.xsd
--rw-r--r--   0        0        0     6664 2023-05-30 05:50:35.043118 koap-0.2.0/koap/api-telematik/ext/ebRS/lcm.xsd
--rw-r--r--   0        0        0    18228 2023-05-30 05:50:35.043177 koap-0.2.0/koap/api-telematik/ext/ebRS/query.xsd
--rw-r--r--   0        0        0    30819 2023-06-08 19:38:03.733364 koap-0.2.0/koap/api-telematik/ext/ebRS/rim.xsd
--rw-r--r--   0        0        0     3158 2023-05-30 05:50:35.043382 koap-0.2.0/koap/api-telematik/ext/ebRS/rs.xsd
--rw-r--r--   0        0        0     1750 2023-05-30 05:50:35.043457 koap-0.2.0/koap/api-telematik/ext/latinchars.xsd
--rw-r--r--   0        0        0    12396 2023-05-30 05:50:35.043596 koap-0.2.0/koap/api-telematik/ext/oasis-200401-wss-wssecurity-secext-1.0.xsd
--rw-r--r--   0        0        0     6292 2023-05-30 05:50:35.043677 koap-0.2.0/koap/api-telematik/ext/oasis-200401-wss-wssecurity-utility-1.0.xsd
--rw-r--r--   0        0        0    16400 2023-05-30 05:50:35.043774 koap-0.2.0/koap/api-telematik/ext/oasis-dss-core-schema-v1.0-os.xsd
--rw-r--r--   0        0        0    16515 2023-05-30 05:50:35.043880 koap-0.2.0/koap/api-telematik/ext/oasis-dss-core-schema-v1.0-os_hardened.xsd
--rw-r--r--   0        0        0     3209 2023-05-30 05:50:35.043961 koap-0.2.0/koap/api-telematik/ext/oasis-dssx-1.0-profiles-sigpolicy-schema-cd01.xsd
--rw-r--r--   0        0        0    25425 2023-05-30 05:50:35.044075 koap-0.2.0/koap/api-telematik/ext/oasis-dssx-1.0-profiles-vr-cd1.xsd
--rw-r--r--   0        0        0     8342 2023-05-30 05:50:35.044165 koap-0.2.0/koap/api-telematik/ext/oasis-sstc-saml-schema-assertion-1.1.xsd
--rw-r--r--   0        0        0    12821 2023-05-30 05:50:35.044251 koap-0.2.0/koap/api-telematik/ext/saml-schema-assertion-2.0.xsd
--rw-r--r--   0        0        0    14700 2023-05-30 05:50:35.044340 koap-0.2.0/koap/api-telematik/ext/tsl.xsd
--rw-r--r--   0        0        0     2654 2023-05-30 05:50:35.044417 koap-0.2.0/koap/api-telematik/ext/ws-addr-wsdl.xsd
--rw-r--r--   0        0        0     5894 2023-05-30 05:50:35.044489 koap-0.2.0/koap/api-telematik/ext/ws-addr.xsd
--rw-r--r--   0        0        0     5664 2023-05-30 05:50:35.044568 koap-0.2.0/koap/api-telematik/ext/ws-policy.xsd
--rw-r--r--   0        0        0    23045 2023-05-30 05:50:35.044639 koap-0.2.0/koap/api-telematik/ext/ws-trust-1.3.xsd
--rw-r--r--   0        0        0     8762 2023-05-30 05:50:35.044735 koap-0.2.0/koap/api-telematik/ext/ws-trust-1.4.xsd
--rw-r--r--   0        0        0     4760 2023-05-30 05:50:35.044849 koap-0.2.0/koap/api-telematik/ext/xenc-schema-11.xsd
--rw-r--r--   0        0        0     6206 2023-05-30 05:50:35.044981 koap-0.2.0/koap/api-telematik/ext/xenc-schema.xsd
--rw-r--r--   0        0        0     4710 2023-05-30 05:50:35.045057 koap-0.2.0/koap/api-telematik/ext/xml.xsd
--rw-r--r--   0        0        0    11506 2023-06-08 11:44:08.679045 koap-0.2.0/koap/api-telematik/ext/xmldsig-core-schema.xsd
--rw-r--r--   0        0        0    12990 2023-05-30 05:50:35.045250 koap-0.2.0/koap/api-telematik/ext/xmldsig_NFDM_hardened.xsd
--rw-r--r--   0        0        0    10461 2023-05-30 05:50:35.045314 koap-0.2.0/koap/api-telematik/ext/xmldsig_hardened.xsd
--rw-r--r--   0        0        0    56491 2023-05-30 05:50:35.045591 koap-0.2.0/koap/api-telematik/fa/amtss/AMTS_Document_v1_6.xsd
--rw-r--r--   0        0        0     6486 2023-05-30 05:50:35.045686 koap-0.2.0/koap/api-telematik/fa/amtss/AMTS_Einwilligung_Document_v1_0.xsd
--rw-r--r--   0        0        0     7161 2023-05-30 05:50:35.045796 koap-0.2.0/koap/api-telematik/fa/nfds/DPE_Document.xsd
--rw-r--r--   0        0        0    32596 2023-05-30 05:50:35.046029 koap-0.2.0/koap/api-telematik/fa/nfds/NFD_Document_v1_4.xsd
--rw-r--r--   0        0        0     5801 2023-05-30 05:50:35.046207 koap-0.2.0/koap/api-telematik/fa/nfds/common/NFDM_Common_v1_1.xsd
--rw-r--r--   0        0        0     3511 2023-05-30 05:50:35.046302 koap-0.2.0/koap/api-telematik/fa/vsds/Pruefungsnachweis.xsd
--rw-r--r--   0        0        0     4196 2023-05-30 05:50:35.046378 koap-0.2.0/koap/api-telematik/fa/vsds/Pruefungsnachweis_PKV.xsd
--rw-r--r--   0        0        0    27331 2023-05-30 05:50:35.046602 koap-0.2.0/koap/api-telematik/fa/vsds/Schema_VSD.xsd
--rw-r--r--   0        0        0    23214 2023-05-30 05:50:35.046697 koap-0.2.0/koap/api-telematik/fa/vsds/Schema_VSD_PKV.xsd
--rw-r--r--   0        0        0     5657 2023-05-30 05:50:35.046874 koap-0.2.0/koap/api-telematik/fd/phr/PHR_Common.xsd
--rw-r--r--   0        0        0    36991 2023-05-30 05:50:35.047215 koap-0.2.0/koap/api-telematik/images/Gematik_Logo_Flag.png
--rw-r--r--   0        0        0     3834 2023-05-30 05:50:35.047370 koap-0.2.0/koap/api-telematik/ksr/InfrastrukturKonfig.xsd
--rw-r--r--   0        0        0     2479 2023-05-30 05:50:35.047454 koap-0.2.0/koap/api-telematik/ksr/Konfigurationsdienst.wsdl
--rw-r--r--   0        0        0     5682 2023-05-30 05:50:35.047513 koap-0.2.0/koap/api-telematik/ksr/Konfigurationsdienst.xsd
--rw-r--r--   0        0        0     3769 2023-05-30 05:50:35.047644 koap-0.2.0/koap/api-telematik/stoerungsampel/I_Monitoring_Update10.wsdl
--rw-r--r--   0        0        0     7645 2023-05-30 05:50:35.047748 koap-0.2.0/koap/api-telematik/stoerungsampel/I_Monitoring_Update10.xsd
--rw-r--r--   0        0        0     1868 2023-05-30 05:50:35.047896 koap-0.2.0/koap/api-telematik/tel/error/TelematikError.xsd
--rw-r--r--   0        0        0     4811 2023-05-30 05:50:35.048005 koap-0.2.0/koap/api-telematik/tel/version/ProductInformation.xsd
--rw-r--r--   0        0        0    16068 2023-05-30 05:50:35.048122 koap-0.2.0/koap/api-telematik/vpnzugd/OperatingData_vpnzugd_hardened.xsd
--rw-r--r--   0        0        0     5999 2023-05-30 05:50:35.048213 koap-0.2.0/koap/api-telematik/vpnzugd/ProvisioningService.wsdl
--rw-r--r--   0        0        0     6336 2023-05-30 05:50:35.048288 koap-0.2.0/koap/api-telematik/vpnzugd/ProvisioningService.xsd
--rw-r--r--   0        0        0     4268 2023-05-30 05:50:35.048383 koap-0.2.0/koap/api-telematik/vzd/DirectoryApplicationMaintenance.wsdl
--rw-r--r--   0        0        0     2745 2023-05-30 05:50:35.048491 koap-0.2.0/koap/api-telematik/vzd/DirectoryApplicationMaintenance.xsd
--rw-r--r--   0        0        0     4888 2023-05-30 05:50:35.048555 koap-0.2.0/koap/api-telematik/vzd/DirectoryMaintenance.wsdl
--rw-r--r--   0        0        0     4256 2023-05-30 05:50:35.048616 koap-0.2.0/koap/api-telematik/vzd/DirectoryMaintenance.xsd
--rw-r--r--   0        0        0     1819 2023-07-02 15:00:26.232495 koap-0.2.0/koap/cetp.py
--rw-r--r--   0        0        0     4387 2023-07-02 14:31:08.877113 koap-0.2.0/koap/client.py
--rw-r--r--   0        0        0      828 2023-07-02 14:09:29.402045 koap-0.2.0/koap/config.py
--rw-r--r--   0        0        0     1592 2023-06-18 07:57:59.040720 koap-0.2.0/koap/debug.py
--rw-r--r--   0        0        0     9400 2023-06-16 07:04:58.713580 koap-0.2.0/koap/facade/epa/epa_facade.py
--rw-r--r--   0        0        0     2293 2023-06-07 09:01:38.592976 koap-0.2.0/koap/facade/external_authenticate.py
--rw-r--r--   0        0        0      954 2023-06-07 09:01:38.593222 koap-0.2.0/koap/facade/model.py
--rw-r--r--   0        0        0     2812 2023-06-08 09:32:16.710982 koap-0.2.0/koap/facade/vsdm/vsdm_facade.py
--rw-r--r--   0        0        0     2594 2023-06-08 07:44:29.154107 koap-0.2.0/koap/service_directory.py
--rw-r--r--   0        0        0     1673 2023-06-07 09:01:38.593769 koap-0.2.0/koap/tsl_util.py
--rw-r--r--   0        0        0      895 2023-06-07 09:02:24.370626 koap-0.2.0/koap/util.py
--rw-r--r--   0        0        0      494 2023-07-02 14:42:08.940046 koap-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 koap-0.2.0/setup.py
--rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 koap-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3077 2023-10-08 08:36:22.054301 koap-0.3.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-29 14:00:21.309721 koap-0.3.0/koap/__init__.py
+-rw-r--r--   0        0        0       46 2023-10-08 08:36:22.054908 koap-0.3.0/koap/api-telematik/.git
+-rw-r--r--   0        0        0        0 2023-10-08 08:36:22.069086 koap-0.3.0/koap/api-telematik/.gitignore
+-rw-r--r--   0        0        0     3277 2023-10-08 08:36:22.069221 koap-0.3.0/koap/api-telematik/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2948 2023-10-08 08:36:22.069315 koap-0.3.0/koap/api-telematik/CONTRIBUTING.md
+-rw-r--r--   0        0        0      555 2023-10-08 08:36:22.069390 koap-0.3.0/koap/api-telematik/LICENSE
+-rw-r--r--   0        0        0     1857 2023-10-08 08:36:22.069471 koap-0.3.0/koap/api-telematik/Readme.md
+-rw-r--r--   0        0        0     1682 2023-10-08 08:36:22.069560 koap-0.3.0/koap/api-telematik/ReleaseNotes.md
+-rw-r--r--   0        0        0     4675 2023-10-08 08:36:22.069874 koap-0.3.0/koap/api-telematik/cm/cc/CCS.wsdl
+-rw-r--r--   0        0        0     2513 2023-10-08 08:36:22.069978 koap-0.3.0/koap/api-telematik/cm/cc/CmCcCommon.xsd
+-rw-r--r--   0        0        0     1887 2023-10-08 08:36:22.070118 koap-0.3.0/koap/api-telematik/cm/cc/CmCcServiceRequest.xsd
+-rw-r--r--   0        0        0     1754 2023-10-08 08:36:22.070191 koap-0.3.0/koap/api-telematik/cm/cc/CmCcServiceResponse.xsd
+-rw-r--r--   0        0        0     2962 2023-10-08 08:36:22.070317 koap-0.3.0/koap/api-telematik/cm/common/CmCommon.xsd
+-rw-r--r--   0        0        0     1519 2023-10-08 08:36:22.070436 koap-0.3.0/koap/api-telematik/cm/uf/CmUfServiceRequest.xsd
+-rw-r--r--   0        0        0     1397 2023-10-08 08:36:22.070546 koap-0.3.0/koap/api-telematik/cm/uf/CmUfServiceResponse.xsd
+-rw-r--r--   0        0        0     3106 2023-10-08 08:36:22.070617 koap-0.3.0/koap/api-telematik/cm/uf/UFS.wsdl
+-rw-r--r--   0        0        0     3474 2023-10-08 08:36:22.070776 koap-0.3.0/koap/api-telematik/conn/AuthSignatureService.wsdl
+-rw-r--r--   0        0        0     3165 2023-10-08 08:36:22.070885 koap-0.3.0/koap/api-telematik/conn/AuthSignatureService_v7_4_1.wsdl
+-rw-r--r--   0        0        0     4025 2023-10-08 08:36:22.071004 koap-0.3.0/koap/api-telematik/conn/CardEvents.xsd
+-rw-r--r--   0        0        0     6062 2023-10-08 08:36:22.071101 koap-0.3.0/koap/api-telematik/conn/CardService.wsdl
+-rw-r--r--   0        0        0     7314 2023-10-08 08:36:22.071235 koap-0.3.0/koap/api-telematik/conn/CardService.xsd
+-rw-r--r--   0        0        0     2992 2023-10-08 08:36:22.071348 koap-0.3.0/koap/api-telematik/conn/CardServiceCommon.xsd
+-rw-r--r--   0        0        0     5558 2023-10-08 08:36:22.071445 koap-0.3.0/koap/api-telematik/conn/CardService_v8_1_1.wsdl
+-rw-r--r--   0        0        0     7252 2023-10-08 08:36:22.071551 koap-0.3.0/koap/api-telematik/conn/CardService_v8_1_1.xsd
+-rw-r--r--   0        0        0     7181 2023-10-08 08:36:22.071649 koap-0.3.0/koap/api-telematik/conn/CardService_v8_1_2.wsdl
+-rw-r--r--   0        0        0     9266 2023-10-08 08:36:22.071817 koap-0.3.0/koap/api-telematik/conn/CardService_v8_1_3.xsd
+-rw-r--r--   0        0        0     4556 2023-10-08 08:36:22.071963 koap-0.3.0/koap/api-telematik/conn/CardTerminalInfo.xsd
+-rw-r--r--   0        0        0     3772 2023-10-08 08:36:22.072075 koap-0.3.0/koap/api-telematik/conn/CardTerminalService.wsdl
+-rw-r--r--   0        0        0     3478 2023-10-08 08:36:22.072187 koap-0.3.0/koap/api-telematik/conn/CardTerminalService.xsd
+-rw-r--r--   0        0        0     4421 2023-10-08 08:36:22.072296 koap-0.3.0/koap/api-telematik/conn/CertificateService.wsdl
+-rw-r--r--   0        0        0     5694 2023-10-08 08:36:22.072394 koap-0.3.0/koap/api-telematik/conn/CertificateService.xsd
+-rw-r--r--   0        0        0     3959 2023-10-08 08:36:22.072512 koap-0.3.0/koap/api-telematik/conn/CertificateServiceCommon.xsd
+-rw-r--r--   0        0        0     4428 2023-10-08 08:36:22.072609 koap-0.3.0/koap/api-telematik/conn/CertificateService_v6_0_1.wsdl
+-rw-r--r--   0        0        0     6145 2023-10-08 08:36:22.072705 koap-0.3.0/koap/api-telematik/conn/CertificateService_v6_0_2.xsd
+-rw-r--r--   0        0        0     6672 2023-10-08 08:36:22.072796 koap-0.3.0/koap/api-telematik/conn/ConnectorCommon.xsd
+-rw-r--r--   0        0        0     2325 2023-10-08 08:36:22.072873 koap-0.3.0/koap/api-telematik/conn/ConnectorContext.xsd
+-rw-r--r--   0        0        0     3530 2023-10-08 08:36:22.072955 koap-0.3.0/koap/api-telematik/conn/EncryptionService.wsdl
+-rw-r--r--   0        0        0     4567 2023-10-08 08:36:22.073060 koap-0.3.0/koap/api-telematik/conn/EncryptionService.xsd
+-rw-r--r--   0        0        0     4045 2023-10-08 08:36:22.073184 koap-0.3.0/koap/api-telematik/conn/EncryptionService_v6_1_1.wsdl
+-rw-r--r--   0        0        0     6226 2023-10-08 08:36:22.073479 koap-0.3.0/koap/api-telematik/conn/EncryptionService_v6_1_2.xsd
+-rw-r--r--   0        0        0     7882 2023-10-08 08:36:22.073623 koap-0.3.0/koap/api-telematik/conn/EventService.wsdl
+-rw-r--r--   0        0        0    11246 2023-10-08 08:36:22.073775 koap-0.3.0/koap/api-telematik/conn/EventService.xsd
+-rw-r--r--   0        0        0    18683 2023-10-08 08:36:22.073901 koap-0.3.0/koap/api-telematik/conn/OperatingData.xsd
+-rw-r--r--   0        0        0      331 2023-10-08 08:36:22.074047 koap-0.3.0/koap/api-telematik/conn/README.CardService.txt
+-rw-r--r--   0        0        0     1714 2023-10-08 08:36:22.074135 koap-0.3.0/koap/api-telematik/conn/ServiceDirectory.xsd
+-rw-r--r--   0        0        0     3056 2023-10-08 08:36:22.074216 koap-0.3.0/koap/api-telematik/conn/ServiceInformation.xsd
+-rw-r--r--   0        0        0     5771 2023-10-08 08:36:22.074313 koap-0.3.0/koap/api-telematik/conn/SignatureService.wsdl
+-rw-r--r--   0        0        0    16413 2023-10-08 08:36:22.074390 koap-0.3.0/koap/api-telematik/conn/SignatureService.xsd
+-rw-r--r--   0        0        0     6634 2023-10-08 08:36:22.074543 koap-0.3.0/koap/api-telematik/conn/SignatureService_V7_4_2.wsdl
+-rw-r--r--   0        0        0    16939 2023-10-08 08:36:22.074622 koap-0.3.0/koap/api-telematik/conn/SignatureService_V7_4_4.xsd
+-rw-r--r--   0        0        0    10283 2023-10-08 08:36:22.074792 koap-0.3.0/koap/api-telematik/conn/SignatureService_V7_5_5.wsdl
+-rw-r--r--   0        0        0    20062 2023-10-08 08:36:22.074873 koap-0.3.0/koap/api-telematik/conn/SignatureService_V7_5_5.xsd
+-rw-r--r--   0        0        0    10593 2023-10-08 08:36:22.074982 koap-0.3.0/koap/api-telematik/conn/SignatureService_V7_5_6.wsdl
+-rw-r--r--   0        0        0    20375 2023-10-08 08:36:22.075103 koap-0.3.0/koap/api-telematik/conn/SignatureService_V7_5_6.xsd
+-rw-r--r--   0        0        0     6144 2023-10-08 08:36:22.075290 koap-0.3.0/koap/api-telematik/conn/amtss/AMTSService.wsdl
+-rw-r--r--   0        0        0     4231 2023-10-08 08:36:22.075389 koap-0.3.0/koap/api-telematik/conn/amtss/AMTSService.xsd
+-rw-r--r--   0        0        0     3703 2023-10-08 08:36:22.075512 koap-0.3.0/koap/api-telematik/conn/nfds/DPEService.wsdl
+-rw-r--r--   0        0        0     6011 2023-10-08 08:36:22.075616 koap-0.3.0/koap/api-telematik/conn/nfds/DPEService.xsd
+-rw-r--r--   0        0        0     3800 2023-10-08 08:36:22.075702 koap-0.3.0/koap/api-telematik/conn/nfds/NFDService.wsdl
+-rw-r--r--   0        0        0     6739 2023-10-08 08:36:22.075813 koap-0.3.0/koap/api-telematik/conn/nfds/NFDService.xsd
+-rw-r--r--   0        0        0     8566 2023-10-08 08:36:22.075931 koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService.wsdl
+-rw-r--r--   0        0        0     8948 2023-10-08 08:36:22.076081 koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService.xsd
+-rw-r--r--   0        0        0    10213 2023-10-08 08:36:22.076180 koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_1.wsdl
+-rw-r--r--   0        0        0    12910 2023-10-08 08:36:22.076406 koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_1.xsd
+-rw-r--r--   0        0        0    10528 2023-10-08 08:36:22.076513 koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_2.wsdl
+-rw-r--r--   0        0        0    13225 2023-10-08 08:36:22.076776 koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_2.xsd
+-rw-r--r--   0        0        0    10460 2023-10-08 08:36:22.076868 koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_2.wsdl
+-rw-r--r--   0        0        0    13276 2023-10-08 08:36:22.077018 koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_2.xsd
+-rw-r--r--   0        0        0    10775 2023-10-08 08:36:22.077092 koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_3.wsdl
+-rw-r--r--   0        0        0    13591 2023-10-08 08:36:22.077242 koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_3.xsd
+-rw-r--r--   0        0        0    10310 2023-10-08 08:36:22.077357 koap-0.3.0/koap/api-telematik/conn/phrs/PHRService.wsdl
+-rw-r--r--   0        0        0     2045 2023-10-08 08:36:22.077459 koap-0.3.0/koap/api-telematik/conn/phrs/PHRService.xsd
+-rw-r--r--   0        0        0     9350 2023-10-08 08:36:22.077553 koap-0.3.0/koap/api-telematik/conn/phrs/PHRService_V2_0_1.wsdl
+-rw-r--r--   0        0        0     2499 2023-10-08 08:36:22.077643 koap-0.3.0/koap/api-telematik/conn/phrs/PHRService_V2_0_1.xsd
+-rw-r--r--   0        0        0     9586 2023-10-08 08:36:22.077725 koap-0.3.0/koap/api-telematik/conn/phrs/PHRService_V2_0_2.wsdl
+-rw-r--r--   0        0        0     2734 2023-10-08 08:36:22.077821 koap-0.3.0/koap/api-telematik/conn/phrs/PHRService_V2_0_2.xsd
+-rw-r--r--   0        0        0     5868 2023-10-08 08:36:22.077965 koap-0.3.0/koap/api-telematik/conn/tbauth/IdpServiceActiveRequestor.wsdl
+-rw-r--r--   0        0        0     4948 2023-10-08 08:36:22.078076 koap-0.3.0/koap/api-telematik/conn/tbauth/LocalIdpService.wsdl
+-rw-r--r--   0        0        0     2330 2023-10-08 08:36:22.078208 koap-0.3.0/koap/api-telematik/conn/vsds/KvkService.wsdl
+-rw-r--r--   0        0        0     1691 2023-10-08 08:36:22.078293 koap-0.3.0/koap/api-telematik/conn/vsds/KvkService.xsd
+-rw-r--r--   0        0        0     2242 2023-10-08 08:36:22.078380 koap-0.3.0/koap/api-telematik/conn/vsds/VSDService.wsdl
+-rw-r--r--   0        0        0     2528 2023-10-08 08:36:22.078493 koap-0.3.0/koap/api-telematik/conn/vsds/VSDService.xsd
+-rw-r--r--   0        0        0     2554 2023-10-08 08:36:22.078620 koap-0.3.0/koap/api-telematik/consumer/CertificateService.wsdl
+-rw-r--r--   0        0        0     3026 2023-10-08 08:36:22.078722 koap-0.3.0/koap/api-telematik/consumer/CertificateService.xsd
+-rw-r--r--   0        0        0     1903 2023-10-08 08:36:22.078815 koap-0.3.0/koap/api-telematik/consumer/CertificateServiceCommon.xsd
+-rw-r--r--   0        0        0     4521 2023-10-08 08:36:22.078909 koap-0.3.0/koap/api-telematik/consumer/ConsumerCommon.xsd
+-rw-r--r--   0        0        0     3112 2023-10-08 08:36:22.078974 koap-0.3.0/koap/api-telematik/consumer/EPAService.wsdl
+-rw-r--r--   0        0        0     3583 2023-10-08 08:36:22.079040 koap-0.3.0/koap/api-telematik/consumer/EPAService.xsd
+-rw-r--r--   0        0        0     3428 2023-10-08 08:36:22.079094 koap-0.3.0/koap/api-telematik/consumer/EncryptionService.wsdl
+-rw-r--r--   0        0        0     3447 2023-10-08 08:36:22.079172 koap-0.3.0/koap/api-telematik/consumer/EncryptionService.xsd
+-rw-r--r--   0        0        0     4493 2023-10-08 08:36:22.079258 koap-0.3.0/koap/api-telematik/consumer/SignatureService.wsdl
+-rw-r--r--   0        0        0     9529 2023-10-08 08:36:22.079335 koap-0.3.0/koap/api-telematik/consumer/SignatureService.xsd
+-rw-r--r--   0        0        0    18833 2023-10-08 08:36:22.079471 koap-0.3.0/koap/api-telematik/ext/DSMLv2.xsd
+-rw-r--r--   0        0        0    24995 2023-10-08 08:36:22.079760 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/NarrativeBlock.xsd
+-rw-r--r--   0        0        0    79308 2023-10-08 08:36:22.080149 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/datatypes-base.xsd
+-rw-r--r--   0        0        0    62014 2023-10-08 08:36:22.080340 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/datatypes.xsd
+-rw-r--r--   0        0        0     1633 2023-10-08 08:36:22.080428 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/infrastructureRoot.xsd
+-rw-r--r--   0        0        0   837069 2023-10-08 08:36:22.081460 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/voc.xsd
+-rw-r--r--   0        0        0    20318 2023-10-08 08:36:22.081741 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030000UV04.xsd
+-rw-r--r--   0        0        0    19744 2023-10-08 08:36:22.081920 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030007UV.xsd
+-rw-r--r--   0        0        0     5143 2023-10-08 08:36:22.082088 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030202UV01.xsd
+-rw-r--r--   0        0        0     4436 2023-10-08 08:36:22.082176 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030203UV02.xsd
+-rw-r--r--   0        0        0     4594 2023-10-08 08:36:22.082280 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030207UV.xsd
+-rw-r--r--   0        0        0     4484 2023-10-08 08:36:22.082394 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT040008UV.xsd
+-rw-r--r--   0        0        0     3999 2023-10-08 08:36:22.082469 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT040203UV01.xsd
+-rw-r--r--   0        0        0     4506 2023-10-08 08:36:22.082568 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT050000UV01.xsd
+-rw-r--r--   0        0        0     8115 2023-10-08 08:36:22.082650 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT060000UV01.xsd
+-rw-r--r--   0        0        0     3751 2023-10-08 08:36:22.082731 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT070000UV01.xsd
+-rw-r--r--   0        0        0    37643 2023-10-08 08:36:22.082898 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT080000UV.xsd
+-rw-r--r--   0        0        0    13047 2023-10-08 08:36:22.083090 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090000UV01.xsd
+-rw-r--r--   0        0        0     6111 2023-10-08 08:36:22.083182 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090002UV01.xsd
+-rw-r--r--   0        0        0     6196 2023-10-08 08:36:22.083268 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090003UV01.xsd
+-rw-r--r--   0        0        0     9598 2023-10-08 08:36:22.083339 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090100UV01.xsd
+-rw-r--r--   0        0        0     4424 2023-10-08 08:36:22.083425 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090102UV02.xsd
+-rw-r--r--   0        0        0     4536 2023-10-08 08:36:22.083503 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090108UV.xsd
+-rw-r--r--   0        0        0     9682 2023-10-08 08:36:22.083570 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090300UV01.xsd
+-rw-r--r--   0        0        0     4672 2023-10-08 08:36:22.083656 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090303UV01.xsd
+-rw-r--r--   0        0        0     3557 2023-10-08 08:36:22.083756 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT140007UV.xsd
+-rw-r--r--   0        0        0     7942 2023-10-08 08:36:22.083847 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150000UV02.xsd
+-rw-r--r--   0        0        0     3564 2023-10-08 08:36:22.083919 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150002UV01.xsd
+-rw-r--r--   0        0        0     5094 2023-10-08 08:36:22.083997 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150003UV03.xsd
+-rw-r--r--   0        0        0     5082 2023-10-08 08:36:22.084075 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150007UV.xsd
+-rw-r--r--   0        0        0    31953 2023-10-08 08:36:22.084150 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT230100UV.xsd
+-rw-r--r--   0        0        0     4103 2023-10-08 08:36:22.084242 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT240000UV01.xsd
+-rw-r--r--   0        0        0     3938 2023-10-08 08:36:22.084305 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT240003UV02.xsd
+-rw-r--r--   0        0        0    13645 2023-10-08 08:36:22.084454 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT260003UV.xsd
+-rw-r--r--   0        0        0     3636 2023-10-08 08:36:22.084564 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT280000UV04.xsd
+-rw-r--r--   0        0        0    40301 2023-10-08 08:36:22.084702 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT290000UV06.xsd
+-rw-r--r--   0        0        0    19515 2023-10-08 08:36:22.084793 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT300000UV04.xsd
+-rw-r--r--   0        0        0    11445 2023-10-08 08:36:22.084934 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT310000UV04.xsd
+-rw-r--r--   0        0        0     3711 2023-10-08 08:36:22.085016 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT440001UV.xsd
+-rw-r--r--   0        0        0    15571 2023-10-08 08:36:22.085152 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT490000UV04.xsd
+-rw-r--r--   0        0        0    12585 2023-10-08 08:36:22.085304 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT500000UV04.xsd
+-rw-r--r--   0        0        0    51960 2023-10-08 08:36:22.085415 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT510000UV06.xsd
+-rw-r--r--   0        0        0    75794 2023-10-08 08:36:22.085535 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT530000UV.xsd
+-rw-r--r--   0        0        0    17638 2023-10-08 08:36:22.085639 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT600000UV06.xsd
+-rw-r--r--   0        0        0     8190 2023-10-08 08:36:22.085744 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT670000UV04.xsd
+-rw-r--r--   0        0        0     5463 2023-10-08 08:36:22.085846 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT710000UV01.xsd
+-rw-r--r--   0        0        0     4334 2023-10-08 08:36:22.085927 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT710007UV.xsd
+-rw-r--r--   0        0        0    12515 2023-10-08 08:36:22.086070 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT740000UV04.xsd
+-rw-r--r--   0        0        0     8037 2023-10-08 08:36:22.086156 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT810000UV.xsd
+-rw-r--r--   0        0        0     8104 2023-10-08 08:36:22.086239 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT820000UV.xsd
+-rw-r--r--   0        0        0     9586 2023-10-08 08:36:22.086309 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT960000UV05.xsd
+-rw-r--r--   0        0        0     9288 2023-10-08 08:36:22.086411 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCAI_MT900001UV01.xsd
+-rw-r--r--   0        0        0     1878 2023-10-08 08:36:22.086505 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_IN000002UV01.xsd
+-rw-r--r--   0        0        0    13447 2023-10-08 08:36:22.086646 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_MT000100UV01.xsd
+-rw-r--r--   0        0        0    15472 2023-10-08 08:36:22.086783 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_MT000200UV01.xsd
+-rw-r--r--   0        0        0    15517 2023-10-08 08:36:22.086914 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_MT000300UV01.xsd
+-rw-r--r--   0        0        0    23361 2023-10-08 08:36:22.086989 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MFMI_MT700701UV01.xsd
+-rw-r--r--   0        0        0    24434 2023-10-08 08:36:22.087075 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MFMI_MT700711UV01.xsd
+-rw-r--r--   0        0        0     9172 2023-10-08 08:36:22.087152 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201301UV02.xsd
+-rw-r--r--   0        0        0     9172 2023-10-08 08:36:22.087218 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201302UV02.xsd
+-rw-r--r--   0        0        0     9172 2023-10-08 08:36:22.087285 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201303UV02.xsd
+-rw-r--r--   0        0        0     9172 2023-10-08 08:36:22.087351 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201304UV02.xsd
+-rw-r--r--   0        0        0     6149 2023-10-08 08:36:22.087437 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201305UV02.xsd
+-rw-r--r--   0        0        0     9622 2023-10-08 08:36:22.087502 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201306UV02.xsd
+-rw-r--r--   0        0        0     6149 2023-10-08 08:36:22.087582 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201309UV02.xsd
+-rw-r--r--   0        0        0     9622 2023-10-08 08:36:22.087649 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201310UV02.xsd
+-rw-r--r--   0        0        0    29790 2023-10-08 08:36:22.087721 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201301UV02.xsd
+-rw-r--r--   0        0        0    32540 2023-10-08 08:36:22.087834 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201302UV02.xsd
+-rw-r--r--   0        0        0    29790 2023-10-08 08:36:22.087910 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201303UV02.xsd
+-rw-r--r--   0        0        0    14556 2023-10-08 08:36:22.088055 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201304UV02.xsd
+-rw-r--r--   0        0        0     7460 2023-10-08 08:36:22.088168 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201305UV02.xsd
+-rw-r--r--   0        0        0    17454 2023-10-08 08:36:22.088256 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201306UV02.xsd
+-rw-r--r--   0        0        0     5386 2023-10-08 08:36:22.088342 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201307UV02.xsd
+-rw-r--r--   0        0        0    31181 2023-10-08 08:36:22.088412 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201310UV02.xsd
+-rw-r--r--   0        0        0     4107 2023-10-08 08:36:22.088536 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/QUQI_IN000003UV01.xsd
+-rw-r--r--   0        0        0    11800 2023-10-08 08:36:22.088659 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/QUQI_MT000001UV01.xsd
+-rw-r--r--   0        0        0    11145 2023-10-08 08:36:22.088771 koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/QUQI_MT021001UV01.xsd
+-rw-r--r--   0        0        0     1237 2023-10-08 08:36:22.088908 koap-0.3.0/koap/api-telematik/ext/IHE/RMD.xsd
+-rw-r--r--   0        0        0     5163 2023-10-08 08:36:22.088993 koap-0.3.0/koap/api-telematik/ext/IHE/XDS.b_DocumentRepository.xsd
+-rw-r--r--   0        0        0    13287 2023-10-08 08:36:22.089174 koap-0.3.0/koap/api-telematik/ext/IHE/healthcare-security-audit.xsd
+-rw-r--r--   0        0        0      443 2023-10-08 08:36:22.089238 koap-0.3.0/koap/api-telematik/ext/IHE/ihe-appc-xacml-combined-schema-1.0.xsd
+-rw-r--r--   0        0        0     2925 2023-10-08 08:36:22.089301 koap-0.3.0/koap/api-telematik/ext/IHE/ihe-appc-xacml-hl7-datatypes-base-1.0.xsd
+-rw-r--r--   0        0        0    21304 2023-10-08 08:36:22.089372 koap-0.3.0/koap/api-telematik/ext/XAdES.xsd
+-rw-r--r--   0        0        0    23190 2023-10-08 08:36:22.089468 koap-0.3.0/koap/api-telematik/ext/XAdES_NFDM_hardened.xsd
+-rw-r--r--   0        0        0    16075 2023-10-08 08:36:22.089622 koap-0.3.0/koap/api-telematik/ext/XMLSchema.dtd
+-rw-r--r--   0        0        0    14895 2023-10-08 08:36:22.089760 koap-0.3.0/koap/api-telematik/ext/access_control-xacml-2.0-policy-schema-os.xsd
+-rw-r--r--   0        0        0    10081 2023-10-08 08:36:22.089839 koap-0.3.0/koap/api-telematik/ext/charset.xsd
+-rw-r--r--   0        0        0     6357 2023-10-08 08:36:22.089925 koap-0.3.0/koap/api-telematik/ext/datatypes.dtd
+-rw-r--r--   0        0        0     3474 2023-10-08 08:36:22.090037 koap-0.3.0/koap/api-telematik/ext/ebRS/cms.xsd
+-rw-r--r--   0        0        0     6664 2023-10-08 08:36:22.090134 koap-0.3.0/koap/api-telematik/ext/ebRS/lcm.xsd
+-rw-r--r--   0        0        0    18228 2023-10-08 08:36:22.090195 koap-0.3.0/koap/api-telematik/ext/ebRS/query.xsd
+-rw-r--r--   0        0        0    27887 2023-10-08 08:36:22.090295 koap-0.3.0/koap/api-telematik/ext/ebRS/rim.xsd
+-rw-r--r--   0        0        0     3158 2023-10-08 08:36:22.090381 koap-0.3.0/koap/api-telematik/ext/ebRS/rs.xsd
+-rw-r--r--   0        0        0     1750 2023-10-08 08:36:22.090445 koap-0.3.0/koap/api-telematik/ext/latinchars.xsd
+-rw-r--r--   0        0        0    12396 2023-10-08 08:36:22.090607 koap-0.3.0/koap/api-telematik/ext/oasis-200401-wss-wssecurity-secext-1.0.xsd
+-rw-r--r--   0        0        0     6292 2023-10-08 08:36:22.090696 koap-0.3.0/koap/api-telematik/ext/oasis-200401-wss-wssecurity-utility-1.0.xsd
+-rw-r--r--   0        0        0    16400 2023-10-08 08:36:22.090770 koap-0.3.0/koap/api-telematik/ext/oasis-dss-core-schema-v1.0-os.xsd
+-rw-r--r--   0        0        0    16515 2023-10-08 08:36:22.090857 koap-0.3.0/koap/api-telematik/ext/oasis-dss-core-schema-v1.0-os_hardened.xsd
+-rw-r--r--   0        0        0     3209 2023-10-08 08:36:22.090936 koap-0.3.0/koap/api-telematik/ext/oasis-dssx-1.0-profiles-sigpolicy-schema-cd01.xsd
+-rw-r--r--   0        0        0    25425 2023-10-08 08:36:22.091022 koap-0.3.0/koap/api-telematik/ext/oasis-dssx-1.0-profiles-vr-cd1.xsd
+-rw-r--r--   0        0        0     8342 2023-10-08 08:36:22.091099 koap-0.3.0/koap/api-telematik/ext/oasis-sstc-saml-schema-assertion-1.1.xsd
+-rw-r--r--   0        0        0    12821 2023-10-08 08:36:22.091225 koap-0.3.0/koap/api-telematik/ext/saml-schema-assertion-2.0.xsd
+-rw-r--r--   0        0        0    14700 2023-10-08 08:36:22.091359 koap-0.3.0/koap/api-telematik/ext/tsl.xsd
+-rw-r--r--   0        0        0     2654 2023-10-08 08:36:22.091428 koap-0.3.0/koap/api-telematik/ext/ws-addr-wsdl.xsd
+-rw-r--r--   0        0        0     5894 2023-10-08 08:36:22.091524 koap-0.3.0/koap/api-telematik/ext/ws-addr.xsd
+-rw-r--r--   0        0        0     5664 2023-10-08 08:36:22.091613 koap-0.3.0/koap/api-telematik/ext/ws-policy.xsd
+-rw-r--r--   0        0        0    23045 2023-10-08 08:36:22.091690 koap-0.3.0/koap/api-telematik/ext/ws-trust-1.3.xsd
+-rw-r--r--   0        0        0     8762 2023-10-08 08:36:22.091783 koap-0.3.0/koap/api-telematik/ext/ws-trust-1.4.xsd
+-rw-r--r--   0        0        0     4760 2023-10-08 08:36:22.091892 koap-0.3.0/koap/api-telematik/ext/xenc-schema-11.xsd
+-rw-r--r--   0        0        0     6206 2023-10-08 08:36:22.092018 koap-0.3.0/koap/api-telematik/ext/xenc-schema.xsd
+-rw-r--r--   0        0        0     4710 2023-10-08 08:36:22.092095 koap-0.3.0/koap/api-telematik/ext/xml.xsd
+-rw-r--r--   0        0        0    11506 2023-10-08 08:36:22.092158 koap-0.3.0/koap/api-telematik/ext/xmldsig-core-schema.xsd
+-rw-r--r--   0        0        0    12990 2023-10-08 08:36:22.092309 koap-0.3.0/koap/api-telematik/ext/xmldsig_NFDM_hardened.xsd
+-rw-r--r--   0        0        0    10461 2023-10-08 08:36:22.092375 koap-0.3.0/koap/api-telematik/ext/xmldsig_hardened.xsd
+-rw-r--r--   0        0        0    56491 2023-10-08 08:36:22.092660 koap-0.3.0/koap/api-telematik/fa/amtss/AMTS_Document_v1_6.xsd
+-rw-r--r--   0        0        0     6486 2023-10-08 08:36:22.092771 koap-0.3.0/koap/api-telematik/fa/amtss/AMTS_Einwilligung_Document_v1_0.xsd
+-rw-r--r--   0        0        0     7161 2023-10-08 08:36:22.092897 koap-0.3.0/koap/api-telematik/fa/nfds/DPE_Document.xsd
+-rw-r--r--   0        0        0    32596 2023-10-08 08:36:22.093066 koap-0.3.0/koap/api-telematik/fa/nfds/NFD_Document_v1_4.xsd
+-rw-r--r--   0        0        0     5801 2023-10-08 08:36:22.093260 koap-0.3.0/koap/api-telematik/fa/nfds/common/NFDM_Common_v1_1.xsd
+-rw-r--r--   0        0        0     3511 2023-10-08 08:36:22.093355 koap-0.3.0/koap/api-telematik/fa/vsds/Pruefungsnachweis.xsd
+-rw-r--r--   0        0        0     4196 2023-10-08 08:36:22.093438 koap-0.3.0/koap/api-telematik/fa/vsds/Pruefungsnachweis_PKV.xsd
+-rw-r--r--   0        0        0    27331 2023-10-08 08:36:22.093586 koap-0.3.0/koap/api-telematik/fa/vsds/Schema_VSD.xsd
+-rw-r--r--   0        0        0    23214 2023-10-08 08:36:22.093667 koap-0.3.0/koap/api-telematik/fa/vsds/Schema_VSD_PKV.xsd
+-rw-r--r--   0        0        0     5657 2023-10-08 08:36:22.093845 koap-0.3.0/koap/api-telematik/fd/phr/PHR_Common.xsd
+-rw-r--r--   0        0        0    36991 2023-10-08 08:36:22.094054 koap-0.3.0/koap/api-telematik/images/Gematik_Logo_Flag.png
+-rw-r--r--   0        0        0     3834 2023-10-08 08:36:22.094157 koap-0.3.0/koap/api-telematik/ksr/InfrastrukturKonfig.xsd
+-rw-r--r--   0        0        0     2479 2023-10-08 08:36:22.094225 koap-0.3.0/koap/api-telematik/ksr/Konfigurationsdienst.wsdl
+-rw-r--r--   0        0        0     5682 2023-10-08 08:36:22.094296 koap-0.3.0/koap/api-telematik/ksr/Konfigurationsdienst.xsd
+-rw-r--r--   0        0        0     3769 2023-10-08 08:36:22.094400 koap-0.3.0/koap/api-telematik/stoerungsampel/I_Monitoring_Update10.wsdl
+-rw-r--r--   0        0        0     7645 2023-10-08 08:36:22.094486 koap-0.3.0/koap/api-telematik/stoerungsampel/I_Monitoring_Update10.xsd
+-rw-r--r--   0        0        0     1868 2023-10-08 08:36:22.094690 koap-0.3.0/koap/api-telematik/tel/error/TelematikError.xsd
+-rw-r--r--   0        0        0     4811 2023-10-08 08:36:22.094799 koap-0.3.0/koap/api-telematik/tel/version/ProductInformation.xsd
+-rw-r--r--   0        0        0    16068 2023-10-08 08:36:22.094954 koap-0.3.0/koap/api-telematik/vpnzugd/OperatingData_vpnzugd_hardened.xsd
+-rw-r--r--   0        0        0     5999 2023-10-08 08:36:22.095053 koap-0.3.0/koap/api-telematik/vpnzugd/ProvisioningService.wsdl
+-rw-r--r--   0        0        0     6336 2023-10-08 08:36:22.095137 koap-0.3.0/koap/api-telematik/vpnzugd/ProvisioningService.xsd
+-rw-r--r--   0        0        0     4268 2023-10-08 08:36:22.095251 koap-0.3.0/koap/api-telematik/vzd/DirectoryApplicationMaintenance.wsdl
+-rw-r--r--   0        0        0     2745 2023-10-08 08:36:22.095345 koap-0.3.0/koap/api-telematik/vzd/DirectoryApplicationMaintenance.xsd
+-rw-r--r--   0        0        0     4888 2023-10-08 08:36:22.095423 koap-0.3.0/koap/api-telematik/vzd/DirectoryMaintenance.wsdl
+-rw-r--r--   0        0        0     4256 2023-10-08 08:36:22.095498 koap-0.3.0/koap/api-telematik/vzd/DirectoryMaintenance.xsd
+-rw-r--r--   0        0        0     1819 2023-10-08 08:36:22.100579 koap-0.3.0/koap/cetp.py
+-rw-r--r--   0        0        0     4387 2023-10-08 08:36:22.100974 koap-0.3.0/koap/client.py
+-rw-r--r--   0        0        0      828 2023-10-08 08:36:22.101207 koap-0.3.0/koap/config.py
+-rw-r--r--   0        0        0     1604 2023-10-17 15:08:54.441162 koap-0.3.0/koap/debug.py
+-rw-r--r--   0        0        0     7905 2023-10-08 08:36:22.101858 koap-0.3.0/koap/facade/epa/builder.py
+-rw-r--r--   0        0        0     3264 2023-10-08 08:36:22.102147 koap-0.3.0/koap/facade/epa/epa_facade.py
+-rw-r--r--   0        0        0     8681 2023-10-08 08:36:22.102282 koap-0.3.0/koap/facade/epa/epa_record_facade.py
+-rw-r--r--   0        0        0     2709 2023-10-17 14:46:43.475731 koap-0.3.0/koap/facade/external_authenticate.py
+-rw-r--r--   0        0        0      978 2023-10-08 08:36:22.102691 koap-0.3.0/koap/facade/model.py
+-rw-r--r--   0        0        0     2902 2023-10-08 08:36:22.102939 koap-0.3.0/koap/facade/vsdm/vsdm_facade.py
+-rw-r--r--   0        0        0    13984 2024-05-29 13:57:13.645762 koap-0.3.0/koap/gogenerator/generator.py
+-rw-r--r--   0        0        0     2594 2023-10-08 08:36:22.103155 koap-0.3.0/koap/service_directory.py
+-rw-r--r--   0        0        0     1673 2023-10-08 08:36:22.103315 koap-0.3.0/koap/tsl_util.py
+-rw-r--r--   0        0        0      895 2023-10-08 08:36:22.103496 koap-0.3.0/koap/util.py
+-rw-r--r--   0        0        0      559 2024-05-29 14:01:14.439614 koap-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3893 1970-01-01 00:00:00.000000 koap-0.3.0/PKG-INFO
```

### Comparing `koap-0.2.0/README.md` & `koap-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-# KOAP: Modern Konnektor SOAP Library
+# KOAP: Lightweight Konnektor Client Library
+
+## Messages Logs
+Sample Message Logs can be found here: [https://spilikin.dev/koap-python/](https://spilikin.dev/koap-python/)
 
 ## Configuration using environment variables
 
 | Environment variable | Comment |
 | --- | --- |
 | `KONNEKTOR_BASE_URL` | Base URL for Konnektor. The `connector.sds` must be available at `{KONNEKTOR_BASE_URL}/connector.sds`|
 | `KONNEKTOR_MANDANT_ID` | Context Mandant ID (Tenant)|
 | `KONNEKTOR_CLIENT_SYSTEM_ID` | Context Client System ID|
 | `KONNEKTOR_WORKPLACE_ID` | Context Workplace ID|
 | `KONNEKTOR_USER_ID` | Context UserID (optional)|
 | *Basic Auth* |
+| `KONNEKTOR_AUTH_METHOD` | `basic`|
 | `KONNEKTOR_AUTH_BASIC_USERNAME` | Username for Basic authentication| 
 | `KONNEKTOR_AUTH_BASIC_PASSWORD`| Password for Basic authentication| 
 | *Mutual TLS Auth* |
-| Not implemented yet | 
+| `KONNEKTOR_AUTH_METHOD` | `cert`|
+| `KONNEKTOR_AUTH_CERT_P12_FILENAME` | Path to the PKCS#12 file with client credentials| 
+| `KONNEKTOR_AUTH_CERT_P12_PASSWORD`| Password for PKCS#12 file | 
 
 ```bash
 export KONNEKTOR_BASE_URL=https://.../
 export KONNEKTOR_MANDANT_ID=m1
 export KONNEKTOR_CLIENT_SYSTEM_ID=c1
 export KONNEKTOR_WORKPLACE_ID=w1
 export KONNEKTOR_USER_ID=user1
@@ -52,27 +58,62 @@
 config = ConnectorConfig(
     base_url='https://.../',
     mandant_id='m1',
     client_system_id='c1',
     workplace_id='w1',
     user_id='user1',
     # Basic Auth
+    auth_method='basic',
     auth_basic_username='user1',
     auth_basic_password='use secure passwords in production',
 )
 
 client = ConnectorClient(config)
 
 event_service = client.create_service_client('EventService', '7.2.0')
 
 cards = event_service.GetCards(client.context())
 
 print(cards)
 ```
 
+## VSDM Facade
+
+
+```python
+from koap.facade.vsdm.vsdm_facade import VSDMFacade
+from koap.facade.model import CardTypeEnum
+from koap.client import ConnectorClient, ConnectorConfig
+
+config = ConnectorConfig()
+client = ConnectorClient(config)
+
+vsdm = VSDMFacade(client)
+
+egks = vsdm.get_cards([CardTypeEnum.EGK])
+egk_1 = egks[0]
+
+print(egk_1)
+
+smcbs = vsdm.get_cards([CardTypeEnum.SMC_B])
+smcb_1 = smcbs[0]
+
+print(smcb_1)
+
+vsd = vsdm.read_vsd(
+    EhcHandle=egk_1.CardHandle,
+    HpcHandle=smcb_1.CardHandle,
+    PerformOnlineCheck=False,
+    ReadOnlineReceipt=False,
+)
+
+print(vsd)
+
+```
+
 ## Development
 
 ```bash
 git submodule init
 git submodule update
 poetry install
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `koap-0.2.0/koap/api-telematik/CODE_OF_CONDUCT.md` & `koap-0.3.0/koap/api-telematik/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/CONTRIBUTING.md` & `koap-0.3.0/koap/api-telematik/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/LICENSE` & `koap-0.3.0/koap/api-telematik/LICENSE`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/Readme.md` & `koap-0.3.0/koap/api-telematik/Readme.md`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ReleaseNotes.md` & `koap-0.3.0/koap/api-telematik/ReleaseNotes.md`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/cm/cc/CCS.wsdl` & `koap-0.3.0/koap/api-telematik/cm/cc/CCS.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/cm/cc/CmCcCommon.xsd` & `koap-0.3.0/koap/api-telematik/cm/cc/CmCcCommon.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/cm/cc/CmCcServiceRequest.xsd` & `koap-0.3.0/koap/api-telematik/cm/cc/CmCcServiceRequest.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/cm/cc/CmCcServiceResponse.xsd` & `koap-0.3.0/koap/api-telematik/cm/cc/CmCcServiceResponse.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/cm/common/CmCommon.xsd` & `koap-0.3.0/koap/api-telematik/cm/common/CmCommon.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/cm/uf/CmUfServiceRequest.xsd` & `koap-0.3.0/koap/api-telematik/cm/uf/CmUfServiceRequest.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/cm/uf/CmUfServiceResponse.xsd` & `koap-0.3.0/koap/api-telematik/cm/uf/CmUfServiceResponse.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/cm/uf/UFS.wsdl` & `koap-0.3.0/koap/api-telematik/cm/uf/UFS.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/AuthSignatureService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/AuthSignatureService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/AuthSignatureService_v7_4_1.wsdl` & `koap-0.3.0/koap/api-telematik/conn/AuthSignatureService_v7_4_1.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CardEvents.xsd` & `koap-0.3.0/koap/api-telematik/conn/CardEvents.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CardService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/CardService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CardService.xsd` & `koap-0.3.0/koap/api-telematik/conn/CardService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CardServiceCommon.xsd` & `koap-0.3.0/koap/api-telematik/conn/CardServiceCommon.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CardService_v8_1_1.wsdl` & `koap-0.3.0/koap/api-telematik/conn/CardService_v8_1_1.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CardService_v8_1_1.xsd` & `koap-0.3.0/koap/api-telematik/conn/CardService_v8_1_1.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CardService_v8_1_2.wsdl` & `koap-0.3.0/koap/api-telematik/conn/CardService_v8_1_2.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CardService_v8_1_3.xsd` & `koap-0.3.0/koap/api-telematik/conn/CardService_v8_1_3.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CardTerminalInfo.xsd` & `koap-0.3.0/koap/api-telematik/conn/CardTerminalInfo.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CardTerminalService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/CardTerminalService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CardTerminalService.xsd` & `koap-0.3.0/koap/api-telematik/conn/CardTerminalService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CertificateService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/CertificateService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CertificateService.xsd` & `koap-0.3.0/koap/api-telematik/conn/CertificateService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CertificateServiceCommon.xsd` & `koap-0.3.0/koap/api-telematik/conn/CertificateServiceCommon.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CertificateService_v6_0_1.wsdl` & `koap-0.3.0/koap/api-telematik/conn/CertificateService_v6_0_1.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/CertificateService_v6_0_2.xsd` & `koap-0.3.0/koap/api-telematik/conn/CertificateService_v6_0_2.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/ConnectorCommon.xsd` & `koap-0.3.0/koap/api-telematik/conn/ConnectorCommon.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/ConnectorContext.xsd` & `koap-0.3.0/koap/api-telematik/conn/ConnectorContext.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/EncryptionService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/EncryptionService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/EncryptionService.xsd` & `koap-0.3.0/koap/api-telematik/conn/EncryptionService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/EncryptionService_v6_1_1.wsdl` & `koap-0.3.0/koap/api-telematik/conn/EncryptionService_v6_1_1.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/EncryptionService_v6_1_2.xsd` & `koap-0.3.0/koap/api-telematik/conn/EncryptionService_v6_1_2.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/EventService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/EventService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/EventService.xsd` & `koap-0.3.0/koap/api-telematik/conn/EventService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/OperatingData.xsd` & `koap-0.3.0/koap/api-telematik/conn/OperatingData.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/ServiceDirectory.xsd` & `koap-0.3.0/koap/api-telematik/conn/ServiceDirectory.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/ServiceInformation.xsd` & `koap-0.3.0/koap/api-telematik/conn/ServiceInformation.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/SignatureService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/SignatureService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/SignatureService.xsd` & `koap-0.3.0/koap/api-telematik/conn/SignatureService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/SignatureService_V7_4_2.wsdl` & `koap-0.3.0/koap/api-telematik/conn/SignatureService_V7_4_2.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/SignatureService_V7_4_4.xsd` & `koap-0.3.0/koap/api-telematik/conn/SignatureService_V7_4_4.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/SignatureService_V7_5_5.wsdl` & `koap-0.3.0/koap/api-telematik/conn/SignatureService_V7_5_5.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/SignatureService_V7_5_5.xsd` & `koap-0.3.0/koap/api-telematik/conn/SignatureService_V7_5_5.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/SignatureService_V7_5_6.wsdl` & `koap-0.3.0/koap/api-telematik/conn/SignatureService_V7_5_6.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/SignatureService_V7_5_6.xsd` & `koap-0.3.0/koap/api-telematik/conn/SignatureService_V7_5_6.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/amtss/AMTSService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/amtss/AMTSService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/amtss/AMTSService.xsd` & `koap-0.3.0/koap/api-telematik/conn/amtss/AMTSService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/nfds/DPEService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/nfds/DPEService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/nfds/DPEService.xsd` & `koap-0.3.0/koap/api-telematik/conn/nfds/DPEService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/nfds/NFDService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/nfds/NFDService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/nfds/NFDService.xsd` & `koap-0.3.0/koap/api-telematik/conn/nfds/NFDService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService.xsd` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_1.wsdl` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_1.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_1.xsd` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_1.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_2.wsdl` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_2.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_2.xsd` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_0_2.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_2.wsdl` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_2.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_2.xsd` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_2.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_3.wsdl` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_3.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_3.xsd` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRManagementService_V2_5_3.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRService.xsd` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRService_V2_0_1.wsdl` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRService_V2_0_1.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRService_V2_0_1.xsd` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRService_V2_0_1.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRService_V2_0_2.wsdl` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRService_V2_0_2.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/phrs/PHRService_V2_0_2.xsd` & `koap-0.3.0/koap/api-telematik/conn/phrs/PHRService_V2_0_2.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/tbauth/IdpServiceActiveRequestor.wsdl` & `koap-0.3.0/koap/api-telematik/conn/tbauth/IdpServiceActiveRequestor.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/tbauth/LocalIdpService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/tbauth/LocalIdpService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/vsds/KvkService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/vsds/KvkService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/vsds/KvkService.xsd` & `koap-0.3.0/koap/api-telematik/conn/vsds/KvkService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/vsds/VSDService.wsdl` & `koap-0.3.0/koap/api-telematik/conn/vsds/VSDService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/conn/vsds/VSDService.xsd` & `koap-0.3.0/koap/api-telematik/conn/vsds/VSDService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/consumer/CertificateService.wsdl` & `koap-0.3.0/koap/api-telematik/consumer/CertificateService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/consumer/CertificateService.xsd` & `koap-0.3.0/koap/api-telematik/consumer/CertificateService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/consumer/CertificateServiceCommon.xsd` & `koap-0.3.0/koap/api-telematik/consumer/CertificateServiceCommon.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/consumer/ConsumerCommon.xsd` & `koap-0.3.0/koap/api-telematik/consumer/ConsumerCommon.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/consumer/EPAService.wsdl` & `koap-0.3.0/koap/api-telematik/consumer/EPAService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/consumer/EPAService.xsd` & `koap-0.3.0/koap/api-telematik/consumer/EPAService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/consumer/EncryptionService.wsdl` & `koap-0.3.0/koap/api-telematik/consumer/EncryptionService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/consumer/EncryptionService.xsd` & `koap-0.3.0/koap/api-telematik/consumer/EncryptionService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/consumer/SignatureService.wsdl` & `koap-0.3.0/koap/api-telematik/consumer/SignatureService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/consumer/SignatureService.xsd` & `koap-0.3.0/koap/api-telematik/consumer/SignatureService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/DSMLv2.xsd` & `koap-0.3.0/koap/api-telematik/ext/DSMLv2.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/NarrativeBlock.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/NarrativeBlock.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/datatypes-base.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/datatypes-base.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/datatypes.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/infrastructureRoot.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/infrastructureRoot.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/voc.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/coreschemas/voc.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030000UV04.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030000UV04.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030007UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030007UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030202UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030202UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030203UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030203UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030207UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT030207UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT040008UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT040008UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT040203UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT040203UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT050000UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT050000UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT060000UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT060000UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT070000UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT070000UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT080000UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT080000UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090000UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090000UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090002UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090002UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090003UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090003UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090100UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090100UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090102UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090102UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090108UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090108UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090300UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090300UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090303UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT090303UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT140007UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT140007UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150000UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150000UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150002UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150002UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150003UV03.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150003UV03.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150007UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT150007UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT230100UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT230100UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT240000UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT240000UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT240003UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT240003UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT260003UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT260003UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT280000UV04.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT280000UV04.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT290000UV06.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT290000UV06.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT300000UV04.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT300000UV04.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT310000UV04.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT310000UV04.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT440001UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT440001UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT490000UV04.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT490000UV04.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT500000UV04.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT500000UV04.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT510000UV06.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT510000UV06.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT530000UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT530000UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT600000UV06.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT600000UV06.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT670000UV04.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT670000UV04.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT710000UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT710000UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT710007UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT710007UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT740000UV04.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT740000UV04.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT810000UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT810000UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT820000UV.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT820000UV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT960000UV05.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/COCT_MT960000UV05.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCAI_MT900001UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCAI_MT900001UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_IN000002UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_IN000002UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_MT000100UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_MT000100UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_MT000200UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_MT000200UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_MT000300UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MCCI_MT000300UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MFMI_MT700701UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MFMI_MT700701UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MFMI_MT700711UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/MFMI_MT700711UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201301UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201301UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201302UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201302UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201303UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201303UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201304UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201304UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201305UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201305UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201306UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201306UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201309UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201309UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201310UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_IN201310UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201301UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201301UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201302UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201302UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201303UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201303UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201304UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201304UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201305UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201305UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201306UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201306UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201307UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201307UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201310UV02.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/PRPA_MT201310UV02.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/QUQI_IN000003UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/QUQI_IN000003UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/QUQI_MT000001UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/QUQI_MT000001UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/QUQI_MT021001UV01.xsd` & `koap-0.3.0/koap/api-telematik/ext/HL7V3/NE2008/multicacheschemas/QUQI_MT021001UV01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/IHE/RMD.xsd` & `koap-0.3.0/koap/api-telematik/ext/IHE/RMD.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/IHE/XDS.b_DocumentRepository.xsd` & `koap-0.3.0/koap/api-telematik/ext/IHE/XDS.b_DocumentRepository.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/IHE/healthcare-security-audit.xsd` & `koap-0.3.0/koap/api-telematik/ext/IHE/healthcare-security-audit.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/IHE/ihe-appc-xacml-hl7-datatypes-base-1.0.xsd` & `koap-0.3.0/koap/api-telematik/ext/IHE/ihe-appc-xacml-hl7-datatypes-base-1.0.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/XAdES.xsd` & `koap-0.3.0/koap/api-telematik/ext/XAdES.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/XAdES_NFDM_hardened.xsd` & `koap-0.3.0/koap/api-telematik/ext/XAdES_NFDM_hardened.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/XMLSchema.dtd` & `koap-0.3.0/koap/api-telematik/ext/XMLSchema.dtd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/access_control-xacml-2.0-policy-schema-os.xsd` & `koap-0.3.0/koap/api-telematik/ext/access_control-xacml-2.0-policy-schema-os.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/charset.xsd` & `koap-0.3.0/koap/api-telematik/ext/charset.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/datatypes.dtd` & `koap-0.3.0/koap/api-telematik/ext/datatypes.dtd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/ebRS/cms.xsd` & `koap-0.3.0/koap/api-telematik/ext/ebRS/cms.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/ebRS/lcm.xsd` & `koap-0.3.0/koap/api-telematik/ext/ebRS/lcm.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/ebRS/query.xsd` & `koap-0.3.0/koap/api-telematik/ext/ebRS/query.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/ebRS/rim.xsd` & `koap-0.3.0/koap/api-telematik/ext/ebRS/rim.xsd`

 * *Files 12% similar despite different names*

#### Comparing `koap-0.2.0/koap/api-telematik/ext/ebRS/rim.xsd` & `koap-0.3.0/koap/api-telematik/ext/ebRS/rim.xsd`

```diff
@@ -139,46 +139,34 @@
         <attribute name="status" type="tns:referenceURI" use="optional"/>
       </extension>
     </complexContent>
   </complexType>
   <element name="RegistryObject" type="tns:RegistryObjectType" substitutionGroup="tns:Identifiable"/>
   <complexType name="RegistryObjectListType">
     <sequence>
-      <element ref="tns:RegistryPackage" minOccurs="0" maxOccurs="unbounded"/>
-      <element ref="tns:Classification" minOccurs="0" maxOccurs="unbounded"/>
-      <element ref="tns:Association" minOccurs="0" maxOccurs="unbounded"/>
-      <element ref="tns:ExtrinsicObject" minOccurs="0" maxOccurs="unbounded"/>
+      <element ref="tns:Identifiable" minOccurs="0" maxOccurs="unbounded"/>
     </sequence>
   </complexType>
   <element name="RegistryObjectList" type="tns:RegistryObjectListType"/>
   <complexType name="AssociationType1">
     <annotation>
       <documentation xml:lang="en">Association is the mapping of the same named interface in ebRIM.
         It extends RegistryObject.
         An Association specifies references to two previously submitted
         registry entrys.
         The sourceObject is id of the sourceObject in association
         The targetObject is id of the targetObject in association</documentation>
     </annotation>
-    <sequence>
-      <element ref="tns:Slot" minOccurs="0" maxOccurs="unbounded"/>
-      <element ref="tns:Name" minOccurs="0" maxOccurs="1"/>
-      <element ref="tns:Description" minOccurs="0" maxOccurs="1"/>
-      <element name="VersionInfo" type="tns:VersionInfoType" minOccurs="0" maxOccurs="1"/>
-      <element ref="tns:Classification" minOccurs="0" maxOccurs="unbounded"/>
-      <element ref="tns:ExternalIdentifier" minOccurs="0" maxOccurs="unbounded"/>
-    </sequence>
-    <attribute name="id" type="anyURI" use="required"/>
-    <attribute name="home" type="anyURI" use="optional"/>
-    <attribute name="lid" type="anyURI" use="optional"/>
-    <attribute name="objectType" type="tns:referenceURI" use="optional"/>
-    <attribute name="status" type="tns:referenceURI" use="optional"/>
-    <attribute name="associationType" type="tns:referenceURI" use="required"/>
-    <attribute name="sourceObject" type="tns:referenceURI" use="required"/>
-    <attribute name="targetObject" type="tns:referenceURI" use="required"/>
+    <complexContent>
+      <extension base="tns:RegistryObjectType">
+        <attribute name="associationType" type="tns:referenceURI" use="required"/>
+        <attribute name="sourceObject" type="tns:referenceURI" use="required"/>
+        <attribute name="targetObject" type="tns:referenceURI" use="required"/>
+      </extension>
+    </complexContent>
   </complexType>
   <element name="Association" type="tns:AssociationType1" substitutionGroup="tns:Identifiable"/>
   <complexType name="AuditableEventType">
     <annotation>
       <documentation xml:lang="en">An Event that forms an audit trail in ebXML Registry.</documentation>
     </annotation>
     <complexContent>
@@ -199,31 +187,22 @@
     <annotation>
       <documentation xml:lang="en">Classification is the mapping of the same named interface in ebRIM.
         It extends RegistryObject.
         A Classification specifies references to two registry entrys.
         The classifiedObject is id of the Object being classified.
         The classificationNode is id of the ClassificationNode classying the object</documentation>
     </annotation>
-    <sequence>
-      <element ref="tns:Slot" minOccurs="0" maxOccurs="unbounded"/>
-      <element ref="tns:Name" minOccurs="0" maxOccurs="1"/>
-      <element ref="tns:Description" minOccurs="0" maxOccurs="1"/>
-      <element name="VersionInfo" type="tns:VersionInfoType" minOccurs="0" maxOccurs="1"/>
-      <element ref="tns:Classification" minOccurs="0" maxOccurs="unbounded"/>
-      <element ref="tns:ExternalIdentifier" minOccurs="0" maxOccurs="unbounded"/>
-    </sequence>
-    <attribute name="id" type="anyURI" use="required"/>
-    <attribute name="home" type="anyURI" use="optional"/>
-    <attribute name="lid" type="anyURI" use="optional"/>
-    <attribute name="objectType" type="tns:referenceURI" use="optional"/>
-    <attribute name="status" type="tns:referenceURI" use="optional"/>
-    <attribute name="classificationScheme" type="tns:referenceURI" use="optional"/>
-    <attribute name="classifiedObject" type="tns:referenceURI" use="required"/>
-    <attribute name="classificationNode" type="tns:referenceURI" use="optional"/>
-    <attribute name="nodeRepresentation" type="tns:LongName" use="optional"/>
+    <complexContent>
+      <extension base="tns:RegistryObjectType">
+        <attribute name="classificationScheme" type="tns:referenceURI" use="optional"/>
+        <attribute name="classifiedObject" type="tns:referenceURI" use="required"/>
+        <attribute name="classificationNode" type="tns:referenceURI" use="optional"/>
+        <attribute name="nodeRepresentation" type="tns:LongName" use="optional"/>
+      </extension>
+    </complexContent>
   </complexType>
   <element name="Classification" type="tns:ClassificationType" substitutionGroup="tns:Identifiable"/>
   <complexType name="ClassificationNodeType">
     <annotation>
       <documentation xml:lang="en">ClassificationNode is the mapping of the same named interface in ebRIM.
         It extends RegistryObject.
         ClassificationNode is used to submit a Classification tree to the Registry.
@@ -285,30 +264,23 @@
   </complexType>
   <element name="ExternalLink" type="tns:ExternalLinkType" substitutionGroup="tns:Identifiable"/>
   <complexType name="ExtrinsicObjectType">
     <annotation>
       <documentation xml:lang="en">ExtrinsicObject is the mapping of the same named interface in ebRIM.
         It extends RegistryObject.</documentation>
     </annotation>
-    <sequence>
-      <element ref="tns:Slot" minOccurs="0" maxOccurs="unbounded"/>
-      <element ref="tns:Name" minOccurs="0" maxOccurs="1"/>
-      <element ref="tns:Description" minOccurs="0" maxOccurs="1"/>
-      <element name="VersionInfo" type="tns:VersionInfoType" minOccurs="0" maxOccurs="1"/>
-      <element ref="tns:Classification" minOccurs="0" maxOccurs="unbounded"/>
-      <element ref="tns:ExternalIdentifier" minOccurs="0" maxOccurs="unbounded"/>
-      <element name="ContentVersionInfo" type="tns:VersionInfoType" minOccurs="0" maxOccurs="1"/>
-    </sequence>
-    <attribute name="id" type="anyURI" use="required"/>
-    <attribute name="home" type="anyURI" use="optional"/>
-    <attribute name="lid" type="anyURI" use="optional"/>
-    <attribute name="objectType" type="tns:referenceURI" use="optional"/>
-    <attribute name="status" type="tns:referenceURI" use="optional"/>
-    <attribute name="mimeType" type="tns:LongName" default="application/octet-stream"/>
-    <attribute name="isOpaque" type="boolean" default="false"/>
+    <complexContent>
+      <extension base="tns:RegistryObjectType">
+        <sequence>
+          <element name="ContentVersionInfo" type="tns:VersionInfoType" minOccurs="0" maxOccurs="1"/>
+        </sequence>
+        <attribute name="mimeType" type="tns:LongName" default="application/octet-stream"/>
+        <attribute name="isOpaque" type="boolean" default="false"/>
+      </extension>
+    </complexContent>
   </complexType>
   <!-- Following element decl nneds to be lower case but using upper camel case for backward compatibility -->
   <element name="ExtrinsicObject" type="tns:ExtrinsicObjectType" substitutionGroup="tns:Identifiable"/>
   <element name="Address" type="tns:PostalAddressType"/>
   <complexType name="OrganizationType">
     <annotation>
       <documentation xml:lang="en">Mapping of the same named interface in ebRIM.</documentation>
@@ -361,27 +333,21 @@
   </complexType>
   <complexType name="RegistryPackageType">
     <annotation>
       <documentation xml:lang="en">RegistryPackage is the mapping of the same named interface in ebRIM.
         It extends RegistryObject.
         A RegistryPackage is a named collection of objects.</documentation>
     </annotation>
-    <sequence>
-      <element ref="tns:Slot" minOccurs="0" maxOccurs="unbounded"/>
-      <element ref="tns:Name" minOccurs="0" maxOccurs="1"/>
-      <element ref="tns:Description" minOccurs="0" maxOccurs="1"/>
-      <element name="VersionInfo" type="tns:VersionInfoType" minOccurs="0" maxOccurs="1"/>
-      <element ref="tns:Classification" minOccurs="0" maxOccurs="unbounded"/>
-      <element ref="tns:ExternalIdentifier" minOccurs="0" maxOccurs="unbounded"/>
-    </sequence>
-    <attribute name="id" type="anyURI" use="required"/>
-    <attribute name="home" type="anyURI" use="optional"/>
-    <attribute name="lid" type="anyURI" use="optional"/>
-    <attribute name="objectType" type="tns:referenceURI" use="optional"/>
-    <attribute name="status" type="tns:referenceURI" use="optional"/>
+    <complexContent>
+      <extension base="tns:RegistryObjectType">
+        <sequence>
+          <element ref="tns:RegistryObjectList" minOccurs="0" maxOccurs="1"/>
+        </sequence>
+      </extension>
+    </complexContent>
   </complexType>
   <element name="RegistryPackage" type="tns:RegistryPackageType" substitutionGroup="tns:Identifiable"/>
   <complexType name="ServiceType">
     <complexContent>
       <extension base="tns:RegistryObjectType">
         <sequence>
           <element ref="tns:ServiceBinding" minOccurs="0" maxOccurs="unbounded"/>
```

### Comparing `koap-0.2.0/koap/api-telematik/ext/ebRS/rs.xsd` & `koap-0.3.0/koap/api-telematik/ext/ebRS/rs.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/latinchars.xsd` & `koap-0.3.0/koap/api-telematik/ext/latinchars.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/oasis-200401-wss-wssecurity-secext-1.0.xsd` & `koap-0.3.0/koap/api-telematik/ext/oasis-200401-wss-wssecurity-secext-1.0.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/oasis-200401-wss-wssecurity-utility-1.0.xsd` & `koap-0.3.0/koap/api-telematik/ext/oasis-200401-wss-wssecurity-utility-1.0.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/oasis-dss-core-schema-v1.0-os.xsd` & `koap-0.3.0/koap/api-telematik/ext/oasis-dss-core-schema-v1.0-os.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/oasis-dss-core-schema-v1.0-os_hardened.xsd` & `koap-0.3.0/koap/api-telematik/ext/oasis-dss-core-schema-v1.0-os_hardened.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/oasis-dssx-1.0-profiles-sigpolicy-schema-cd01.xsd` & `koap-0.3.0/koap/api-telematik/ext/oasis-dssx-1.0-profiles-sigpolicy-schema-cd01.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/oasis-dssx-1.0-profiles-vr-cd1.xsd` & `koap-0.3.0/koap/api-telematik/ext/oasis-dssx-1.0-profiles-vr-cd1.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/oasis-sstc-saml-schema-assertion-1.1.xsd` & `koap-0.3.0/koap/api-telematik/ext/oasis-sstc-saml-schema-assertion-1.1.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/saml-schema-assertion-2.0.xsd` & `koap-0.3.0/koap/api-telematik/ext/saml-schema-assertion-2.0.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/tsl.xsd` & `koap-0.3.0/koap/api-telematik/ext/tsl.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/ws-addr-wsdl.xsd` & `koap-0.3.0/koap/api-telematik/ext/ws-addr-wsdl.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/ws-addr.xsd` & `koap-0.3.0/koap/api-telematik/ext/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/ws-policy.xsd` & `koap-0.3.0/koap/api-telematik/ext/ws-policy.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/ws-trust-1.3.xsd` & `koap-0.3.0/koap/api-telematik/ext/ws-trust-1.3.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/ws-trust-1.4.xsd` & `koap-0.3.0/koap/api-telematik/ext/ws-trust-1.4.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/xenc-schema-11.xsd` & `koap-0.3.0/koap/api-telematik/ext/xenc-schema-11.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/xenc-schema.xsd` & `koap-0.3.0/koap/api-telematik/ext/xenc-schema.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/xml.xsd` & `koap-0.3.0/koap/api-telematik/ext/xml.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/xmldsig-core-schema.xsd` & `koap-0.3.0/koap/api-telematik/ext/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/xmldsig_NFDM_hardened.xsd` & `koap-0.3.0/koap/api-telematik/ext/xmldsig_NFDM_hardened.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ext/xmldsig_hardened.xsd` & `koap-0.3.0/koap/api-telematik/ext/xmldsig_hardened.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/fa/amtss/AMTS_Document_v1_6.xsd` & `koap-0.3.0/koap/api-telematik/fa/amtss/AMTS_Document_v1_6.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/fa/amtss/AMTS_Einwilligung_Document_v1_0.xsd` & `koap-0.3.0/koap/api-telematik/fa/amtss/AMTS_Einwilligung_Document_v1_0.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/fa/nfds/DPE_Document.xsd` & `koap-0.3.0/koap/api-telematik/fa/nfds/DPE_Document.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/fa/nfds/NFD_Document_v1_4.xsd` & `koap-0.3.0/koap/api-telematik/fa/nfds/NFD_Document_v1_4.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/fa/nfds/common/NFDM_Common_v1_1.xsd` & `koap-0.3.0/koap/api-telematik/fa/nfds/common/NFDM_Common_v1_1.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/fa/vsds/Pruefungsnachweis.xsd` & `koap-0.3.0/koap/api-telematik/fa/vsds/Pruefungsnachweis.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/fa/vsds/Pruefungsnachweis_PKV.xsd` & `koap-0.3.0/koap/api-telematik/fa/vsds/Pruefungsnachweis_PKV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/fa/vsds/Schema_VSD.xsd` & `koap-0.3.0/koap/api-telematik/fa/vsds/Schema_VSD.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/fa/vsds/Schema_VSD_PKV.xsd` & `koap-0.3.0/koap/api-telematik/fa/vsds/Schema_VSD_PKV.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/fd/phr/PHR_Common.xsd` & `koap-0.3.0/koap/api-telematik/fd/phr/PHR_Common.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/images/Gematik_Logo_Flag.png` & `koap-0.3.0/koap/api-telematik/images/Gematik_Logo_Flag.png`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ksr/InfrastrukturKonfig.xsd` & `koap-0.3.0/koap/api-telematik/ksr/InfrastrukturKonfig.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ksr/Konfigurationsdienst.wsdl` & `koap-0.3.0/koap/api-telematik/ksr/Konfigurationsdienst.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/ksr/Konfigurationsdienst.xsd` & `koap-0.3.0/koap/api-telematik/ksr/Konfigurationsdienst.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/stoerungsampel/I_Monitoring_Update10.wsdl` & `koap-0.3.0/koap/api-telematik/stoerungsampel/I_Monitoring_Update10.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/stoerungsampel/I_Monitoring_Update10.xsd` & `koap-0.3.0/koap/api-telematik/stoerungsampel/I_Monitoring_Update10.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/tel/error/TelematikError.xsd` & `koap-0.3.0/koap/api-telematik/tel/error/TelematikError.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/tel/version/ProductInformation.xsd` & `koap-0.3.0/koap/api-telematik/tel/version/ProductInformation.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/vpnzugd/OperatingData_vpnzugd_hardened.xsd` & `koap-0.3.0/koap/api-telematik/vpnzugd/OperatingData_vpnzugd_hardened.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/vpnzugd/ProvisioningService.wsdl` & `koap-0.3.0/koap/api-telematik/vpnzugd/ProvisioningService.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/vpnzugd/ProvisioningService.xsd` & `koap-0.3.0/koap/api-telematik/vpnzugd/ProvisioningService.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/vzd/DirectoryApplicationMaintenance.wsdl` & `koap-0.3.0/koap/api-telematik/vzd/DirectoryApplicationMaintenance.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/vzd/DirectoryApplicationMaintenance.xsd` & `koap-0.3.0/koap/api-telematik/vzd/DirectoryApplicationMaintenance.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/vzd/DirectoryMaintenance.wsdl` & `koap-0.3.0/koap/api-telematik/vzd/DirectoryMaintenance.wsdl`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/api-telematik/vzd/DirectoryMaintenance.xsd` & `koap-0.3.0/koap/api-telematik/vzd/DirectoryMaintenance.xsd`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/cetp.py` & `koap-0.3.0/koap/cetp.py`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/client.py` & `koap-0.3.0/koap/client.py`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/config.py` & `koap-0.3.0/koap/config.py`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/debug.py` & `koap-0.3.0/koap/debug.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.debug_console.print("Body:")
         self.debug_console.print(etree.tostring(envelope, pretty_print=True).decode())
 
         return envelope, http_headers
 
     def egress(self, envelope, http_headers, operation, binding_options):
         self.last_request_timestamp = datetime.datetime.now()
-        self.debug_console.print(f"Request {operation}")
+        self.debug_console.print(f"SOAP Operation {operation.name}")
         self.debug_console.print("Headers:")
         for key, value in http_headers.items():
             self.debug_console.print(f"{key}: {value}")
         self.debug_console.print("Body:")
         self.debug_console.print(etree.tostring(envelope, pretty_print=True).decode())
 
         return envelope, http_headers
```

### Comparing `koap-0.2.0/koap/facade/external_authenticate.py` & `koap-0.3.0/koap/facade/external_authenticate.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 AUTH_CARDS = [CardTypeEnum.HBA, CardTypeEnum.SMC_B, CardTypeEnum.HSM_B, CardTypeEnum.SM_B]
 
 
 class ExternalAuthenticateFacade:
     def __init__(self, client: ConnectorClient):
         self.client = client
         self.event_service = client.create_service_client('EventService', '7.2.0')
+        self.card_service = client.create_service_client('CardService', '8.1.2')
         self.certificate_service = client.create_service_client('CertificateService', '6.0.1')
         self.auth_signature_service = client.create_service_client('AuthSignatureService', '7.4.1')
 
     def get_auth_cards(self) -> List[Card]:
         get_cards_response = self.event_service.GetCards(
             Context=self.client.context()
         )
@@ -32,14 +33,25 @@
             Context=self.client.context(),
             CertRefList=list(map(lambda cert_type: cert_type.value, cert_types)),
             Crypt=crypt.value,
         )
 
         return response.X509DataInfoList.X509DataInfo
 
+    def verify_pin(self, card_type: CardTypeEnum, card_handle: str) -> any:
+        if card_type == CardTypeEnum.SMC_B:
+            pin_type = "PIN.SMC"
+        else:
+            pin_type = "PIN.CH"
+        return self.card_service.VerifyPin(
+            self.client.context(),
+            card_handle,
+            pin_type
+        )
+
     def external_authenticate(self, card_handle: str, hash: bytes, crypt: CertRefEnum) -> bytes:
         if crypt == "RSA":
             optional_outputs = {
                 'SignatureType': 'urn:ietf:rfc:3447',
                 'SignatureSchemes': 'RSASSA-PSS'
             }
         else:
```

### Comparing `koap-0.2.0/koap/facade/model.py` & `koap-0.3.0/koap/facade/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 ]
 
 
 class Card(BaseModel):
     CardType: CardTypeEnum | str
     CardHandle: str
     CardHolderName: str
+    Kvnr: Optional[str]
     raw: Optional[Mapping[str, Any]]
 
 
 def obj_to_card(zeep_obj) -> Card:
     card_dict = serialize_object(zeep_obj)
     card = Card.parse_obj(card_dict)
     card.raw = card_dict
```

### Comparing `koap-0.2.0/koap/facade/vsdm/vsdm_facade.py` & `koap-0.3.0/koap/facade/vsdm/vsdm_facade.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from koap.facade.model import (
     CardTypeEnum,
     Card,
     obj_to_card,
     CryptEnum,
     CertRefEnum,
 )
-from typing import List
+from typing import List, Optional
 from pydantic import BaseModel
 import gzip
 import xmltodict
 from zeep.helpers import serialize_object
 
 
 class VSD(BaseModel):
     PersoenlicheVersichertendaten: dict
     AllgemeineVersicherungsdaten: dict
     GeschuetzteVersichertendaten: dict
-    Pruefungsnachweis: dict
-    VSD_Status: dict
+    Pruefungsnachweis: Optional[dict]
+    VSD_Status: Optional[dict]
 
 
 class VSDMFacade:
     def __init__(self, client: ConnectorClient):
         self.client = client
         self.event_service = client.create_service_client('EventService', '7.2.0')
         self.vsd_service = client.create_service_client('VSDService', '5.2.0', module="vsds")        
@@ -61,13 +61,15 @@
             GeschuetzteVersichertendaten=self.vsd_data_to_dict(response, 'GeschuetzteVersichertendaten'),
             Pruefungsnachweis=self.vsd_data_to_dict(response, 'Pruefungsnachweis'),
             VSD_Status=serialize_object(response['VSD_Status']),
         )
 
     def vsd_data_to_dict(self, response: dict, field_name: str) -> dict:
         compressed_data = response[field_name]
+        if compressed_data is None:
+            return None
         # gunzip comnpresed data
         data = gzip.decompress(compressed_data)
         xml_as_dict = xmltodict.parse(data)
         # first value in the dict
         xml_as_dict = xml_as_dict[list(xml_as_dict.keys())[0]]
         return xml_as_dict
```

### Comparing `koap-0.2.0/koap/service_directory.py` & `koap-0.3.0/koap/service_directory.py`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/tsl_util.py` & `koap-0.3.0/koap/tsl_util.py`

 * *Files identical despite different names*

### Comparing `koap-0.2.0/koap/util.py` & `koap-0.3.0/koap/util.py`

 * *Files identical despite different names*

