# Comparing `tmp/pyocient-1.0.7.tar.gz` & `tmp/pyocient-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyocient-1.0.7.tar", last modified: Sun Mar  6 19:52:14 2022, max compression
+gzip compressed data, was "pyocient-1.0.9.tar", last modified: Fri May 20 16:21:03 2022, max compression
```

## Comparing `pyocient-1.0.7.tar` & `pyocient-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-06 19:52:14.963625 pyocient-1.0.7/
--r-xr-xr-x   0 root         (0) root         (0)   297517 2022-02-07 14:19:53.000000 pyocient-1.0.7/ClientWireProtocol_pb2.py
--r-xr-xr-x   0 root         (0) root         (0)      581 2021-09-27 15:39:07.000000 pyocient-1.0.7/LICENSE.txt
--r-xr-xr-x   0 root         (0) root         (0)       93 2022-02-11 15:53:45.000000 pyocient-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2054 2022-03-06 19:52:14.963625 pyocient-1.0.7/PKG-INFO
--r-xr-xr-x   0 root         (0) root         (0)     1175 2022-02-11 15:53:45.000000 pyocient-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-06 19:52:14.963625 pyocient-1.0.7/pyocient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2054 2022-03-06 19:52:14.000000 pyocient-1.0.7/pyocient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      295 2022-03-06 19:52:14.000000 pyocient-1.0.7/pyocient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-06 19:52:14.000000 pyocient-1.0.7/pyocient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-03-06 19:52:14.000000 pyocient-1.0.7/pyocient.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      116 2022-03-06 19:52:14.000000 pyocient-1.0.7/pyocient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       40 2022-03-06 19:52:14.000000 pyocient-1.0.7/pyocient.egg-info/top_level.txt
--r-xr-xr-x   0 root         (0) root         (0)   104004 2022-03-06 19:52:14.000000 pyocient-1.0.7/pyocient.py
--r-xr-xr-x   0 root         (0) root         (0)      107 2022-03-06 19:52:14.963625 pyocient-1.0.7/setup.cfg
--r-xr-xr-x   0 root         (0) root         (0)     2004 2022-02-11 15:53:45.000000 pyocient-1.0.7/setup.py
--r-xr-xr-x   0 root         (0) root         (0)       20 2022-03-06 19:52:14.000000 pyocient-1.0.7/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 16:21:03.742177 pyocient-1.0.9/
+-r-xr-xr-x   0 root         (0) root         (0)   312011 2022-05-10 16:56:57.000000 pyocient-1.0.9/ClientWireProtocol_pb2.py
+-r-xr-xr-x   0 root         (0) root         (0)      581 2022-05-20 16:21:03.000000 pyocient-1.0.9/LICENSE.txt
+-r-xr-xr-x   0 root         (0) root         (0)       93 2022-05-20 16:21:03.000000 pyocient-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2054 2022-05-20 16:21:03.742177 pyocient-1.0.9/PKG-INFO
+-r-xr-xr-x   0 root         (0) root         (0)     1175 2022-05-20 16:21:03.000000 pyocient-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 16:21:03.742177 pyocient-1.0.9/pyocient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2054 2022-05-20 16:21:03.000000 pyocient-1.0.9/pyocient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      295 2022-05-20 16:21:03.000000 pyocient-1.0.9/pyocient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 16:21:03.000000 pyocient-1.0.9/pyocient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2022-05-20 16:21:03.000000 pyocient-1.0.9/pyocient.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2022-05-20 16:21:03.000000 pyocient-1.0.9/pyocient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2022-05-20 16:21:03.000000 pyocient-1.0.9/pyocient.egg-info/top_level.txt
+-r-xr-xr-x   0 root         (0) root         (0)   107463 2022-05-17 17:43:55.000000 pyocient-1.0.9/pyocient.py
+-r-xr-xr-x   0 root         (0) root         (0)      107 2022-05-20 16:21:03.743177 pyocient-1.0.9/setup.cfg
+-r-xr-xr-x   0 root         (0) root         (0)     2098 2022-05-20 16:21:03.000000 pyocient-1.0.9/setup.py
+-r-xr-xr-x   0 root         (0) root         (0)       20 2022-05-20 16:21:03.000000 pyocient-1.0.9/version.py
```

### Comparing `pyocient-1.0.7/ClientWireProtocol_pb2.py` & `pyocient-1.0.9/ClientWireProtocol_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='sharedMessages/clientWireProtocol.proto',
   package='xg.cmdcomp',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\'sharedMessages/clientWireProtocol.proto\x12\nxg.cmdcomp\x1a\x1egoogle/protobuf/wrappers.proto\"\xa2\x01\n\x10\x43lientConnection\x12\x0e\n\x06userid\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x10\n\x08\x63lientid\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x05 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x06 \x01(\x05\x12\x11\n\tsessionID\x18\x07 \x01(\t\"\xba\x01\n\x13\x43lientConnectionGCM\x12\x0e\n\x06userid\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x10\n\x08\x63lientid\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x05 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x06 \x01(\x05\x12\x11\n\tsessionID\x18\x07 \x01(\t\x12\x13\n\x0b\x65xplicitSSO\x18\x08 \x01(\x08\"\x95\x01\n\x13\x43lientConnectionSSO\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x10\n\x08\x63lientid\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x04 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x05 \x01(\x05\x12\x11\n\tsessionID\x18\x06 \x01(\t\"\xf8\x01\n\x1d\x43lientConnectionSecurityToken\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x10\n\x08\x63lientid\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x04 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x05 \x01(\x05\x12\x11\n\tsessionID\x18\x06 \x01(\t\x12\x15\n\rsecurityToken\x18\x07 \x01(\t\x12\x16\n\x0etokenSignature\x18\x08 \x01(\t\x12\x19\n\x11issuerFingerprint\x18\t \x01(\t\x12\r\n\x05\x66orce\x18\n \x01(\x08\"j\n\x18\x43lientConnectionResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\n\n\x02iv\x18\x02 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x03 \x01(\t\"m\n\x1b\x43lientConnectionGCMResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\n\n\x02iv\x18\x02 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x03 \x01(\t\"u\n\x1b\x43lientConnectionSSOResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x11\n\trequestId\x18\x02 \x01(\t\x12\x0f\n\x07\x61uthUrl\x18\x03 \x01(\t\"\xfb\x01\n%ClientConnectionSecurityTokenResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x05 \x03(\t\x12\x35\n\tsecondary\x18\x06 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceList\x12\x17\n\x0fserverSessionId\x18\x07 \x01(\t\"P\n\x11\x43lientConnection2\x12\x0e\n\x06\x63ipher\x18\x01 \x01(\x0c\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x0c\n\x04hmac\x18\x03 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x04 \x01(\t\"h\n\x14\x43lientConnectionGCM2\x12\x0e\n\x06\x63ipher\x18\x01 \x01(\x0c\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x0c\n\x04hmac\x18\x03 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x04 \x01(\t\x12\x13\n\x0b\x65xplicitSSO\x18\x05 \x01(\x08\"8\n\x14\x43lientConnectionSSO2\x12\x11\n\trequestId\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"K\n\rSecurityToken\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\x12\x11\n\tsignature\x18\x02 \x01(\t\x12\x19\n\x11issuerFingerprint\x18\x03 \x01(\t\"X\n\x0bSessionInfo\x12\x17\n\x0fserverSessionId\x18\x01 \x01(\t\x12\x30\n\rsecurityToken\x18\x02 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\" \n\x1e\x43lientConnectionRefreshSession\"\x8a\x01\n&ClientConnectionRefreshSessionResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12,\n\x0bsessionInfo\x18\x02 \x01(\x0b\x32\x17.xg.cmdcomp.SessionInfo\"S\n\x1c\x43lientConnectionRefreshToken\x12\x33\n\x10oldSecurityToken\x18\x01 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\"\x8f\x01\n$ClientConnectionRefreshTokenResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x33\n\x10newSecurityToken\x18\x02 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\")\n\x16SecondaryInterfaceList\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x03(\t\"\xef\x01\n\x19\x43lientConnection2Response\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x05 \x03(\t\x12\x35\n\tsecondary\x18\x06 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceList\x12\x17\n\x0fserverSessionId\x18\x07 \x01(\t\"\xf2\x01\n\x1c\x43lientConnectionGCM2Response\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x05 \x03(\t\x12\x35\n\tsecondary\x18\x06 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceList\x12\x17\n\x0fserverSessionId\x18\x07 \x01(\t\"\xbd\x02\n\x1c\x43lientConnectionSSO2Response\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12 \n\x16pollingIntervalSeconds\x18\x02 \x01(\x05H\x00\x12.\n\x0bsessionInfo\x18\x03 \x01(\x0b\x32\x17.xg.cmdcomp.SessionInfoH\x00\x12\x10\n\x08redirect\x18\x04 \x01(\x08\x12\x14\n\x0credirectHost\x18\x05 \x01(\t\x12\x14\n\x0credirectPort\x18\x06 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x07 \x03(\t\x12\x35\n\tsecondary\x18\x08 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceListB\x10\n\x0eresponse_oneof\"\x0b\n\tGetSchema\"W\n\x11GetSchemaResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x0e\n\x06schema\x18\x02 \x01(\t\"\x1b\n\tSetSchema\x12\x0e\n\x06schema\x18\x01 \x01(\t\"%\n\x0f\x43loseConnection\x12\x12\n\nendSession\x18\x01 \x01(\x08\"\x10\n\x0eTestConnection\" \n\rAttachToQuery\x12\x0f\n\x07queryId\x18\x01 \x01(\t\"\x1f\n\tFetchData\x12\x12\n\nfetch_size\x18\x01 \x01(\x0f\"A\n\tResultSet\x12\x10\n\x08numParts\x18\x01 \x01(\x05\x12\x13\n\x0b\x62lobLengths\x18\x02 \x03(\x05\x12\r\n\x05\x62lobs\x18\x03 \x03(\x0c\"r\n\x11\x46\x65tchDataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12)\n\nresult_set\x18\x02 \x01(\x0b\x32\x15.xg.cmdcomp.ResultSet\"\x0f\n\rFetchMetadata\"\xb9\x02\n\x15\x46\x65tchMetadataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x41\n\x08\x63ols2pos\x18\x02 \x03(\x0b\x32/.xg.cmdcomp.FetchMetadataResponse.Cols2posEntry\x12\x45\n\ncols2Types\x18\x03 \x03(\x0b\x32\x31.xg.cmdcomp.FetchMetadataResponse.Cols2TypesEntry\x1a/\n\rCols2posEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0f:\x02\x38\x01\x1a\x31\n\x0f\x43ols2TypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xde\x04\n\x13\x46\x65tchSystemMetadata\x12@\n\x04\x63\x61ll\x18\x01 \x01(\x0e\x32\x32.xg.cmdcomp.FetchSystemMetadata.SystemMetadataCall\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\r\n\x05table\x18\x03 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x04 \x01(\t\x12\x0c\n\x04view\x18\x05 \x01(\t\x12\x0c\n\x04test\x18\x06 \x01(\x08\"\xb9\x03\n\x12SystemMetadataCall\x12\x0b\n\x07INVALID\x10\x00\x12\x0f\n\x0bGET_SCHEMAS\x10\x01\x12\x0e\n\nGET_TABLES\x10\x02\x12\x15\n\x11GET_SYSTEM_TABLES\x10\x0e\x12\x18\n\x14GET_TABLE_PRIVILEGES\x10\x0f\x12\x19\n\x15GET_COLUMN_PRIVILEGES\x10\x10\x12\r\n\tGET_VIEWS\x10\x19\x12\x0f\n\x0bGET_COLUMNS\x10\x03\x12\x12\n\x0eGET_INDEX_INFO\x10\x04\x12\x11\n\rGET_TYPE_INFO\x10\x05\x12\x14\n\x10GET_SQL_KEYWORDS\x10\x06\x12\x19\n\x15GET_NUMERIC_FUNCTIONS\x10\x07\x12\x18\n\x14GET_STRING_FUNCTIONS\x10\x08\x12\x1b\n\x17GET_TIME_DATE_FUNCTIONS\x10\t\x12\x18\n\x14GET_SYSTEM_FUNCTIONS\x10\n\x12 \n\x1cGET_DATABASE_PRODUCT_VERSION\x10\x0b\x12\x1e\n\x1aGET_DATABASE_MAJOR_VERSION\x10\x0c\x12\x1e\n\x1aGET_DATABASE_MINOR_VERSION\x10\r\"\xbb\x01\n\x1b\x46\x65tchSystemMetadataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12/\n\x0eresult_set_val\x18\x02 \x01(\x0b\x32\x15.xg.cmdcomp.ResultSetH\x00\x12\x14\n\nstring_val\x18\x03 \x01(\tH\x00\x12\x11\n\x07int_val\x18\x04 \x01(\x0fH\x00\x42\x0e\n\x0cresult_oneof\"\x10\n\x0e\x43loseResultSet\"A\n\x0c\x45xecuteQuery\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x15\n\rforceRedirect\x18\x03 \x01(\x08\"\xb3\x01\n\x14\x45xecuteQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x0f\n\x07queryId\x18\x05 \x01(\t\x12\x18\n\x10numClientThreads\x18\x06 \x01(\x07\"+\n\rExecuteUpdate\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa1\x01\n\x15\x45xecuteUpdateResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x16\n\x0eupdateRowCount\x18\x02 \x01(\x0f\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"W\n\x0e\x45xecuteExplain\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12)\n\x06\x66ormat\x18\x03 \x01(\x0e\x32\x19.xg.cmdcomp.ExplainFormat\"\xdc\x01\n\x16\x45xecuteExplainForSpark\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x41\n\x04type\x18\x02 \x01(\x0e\x32\x33.xg.cmdcomp.ExecuteExplainForSpark.PartitioningType\x12\x19\n\x11partitioningParam\x18\x03 \x01(\x0f\x12\r\n\x05\x66orce\x18\x04 \x01(\x08\"H\n\x10PartitioningType\x12\x18\n\x14INVALID_PARTITIONING\x10\x00\x12\x0b\n\x07\x42Y_SIZE\x10\x01\x12\r\n\tBY_NUMBER\x10\x02\"\x9b\x01\n\x19\x45xplainResponseStringPlan\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x0c\n\x04plan\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"V\n\x15\x42\x65ginQueryConcurrency\x12\x14\n\x0cnodeEndpoint\x18\x01 \x01(\t\x12\x16\n\x0eserviceClassId\x18\x02 \x01(\t\x12\x0f\n\x07queryId\x18\x03 \x01(\t\"W\n\x16\x46inishQueryConcurrency\x12\x14\n\x0cnodeEndpoint\x18\x01 \x01(\t\x12\x16\n\x0eserviceClassId\x18\x02 \x01(\t\x12\x0f\n\x07queryId\x18\x03 \x01(\t\"\xd3\x01\n\x19\x42roadcastQueryConcurrency\x12\x14\n\x0cnodeEndpoint\x18\x01 \x01(\t\x12\x61\n\x16serviceClassIdToCounts\x18\x02 \x03(\x0b\x32\x41.xg.cmdcomp.BroadcastQueryConcurrency.ServiceClassIdToCountsEntry\x1a=\n\x1bServiceClassIdToCountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"N\n\x18QueryConcurrencyResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\x13\n\x11SystemWideQueries\"x\n\x19SystemWideQueriesResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\'\n\x04rows\x18\x02 \x03(\x0b\x32\x19.xg.cmdcomp.SysQueriesRow\"\x87\x02\n\x0cLocalQueries\x12\x14\n\x08identity\x18\x01 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\ruuid_identity\x18\x02 \x01(\x0c\x42\x02\x18\x01H\x00\x12\x10\n\x08\x64\x61tabase\x18\x03 \x01(\t\x12\r\n\x05token\x18\x04 \x01(\x0c\x12\x15\n\tsignature\x18\x05 \x01(\x0c\x42\x02\x18\x01\x12\x1e\n\x12issuer_certificate\x18\x06 \x01(\x0c\x42\x02\x18\x01\x12\x1a\n\x12issuer_fingerprint\x18\x07 \x01(\x0c\x12\x14\n\x08username\x18\x08 \x01(\x0c\x42\x02\x18\x01\x12\x11\n\tcompleted\x18\t \x01(\x08\x12\x10\n\x04user\x18\n \x01(\x0c\x42\x02\x18\x01\x42\x15\n\x13one_identity_option\"s\n\x14LocalQueriesResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\'\n\x04rows\x18\x02 \x03(\x0b\x32\x19.xg.cmdcomp.SysQueriesRow\"\xd3\x02\n\rSysQueriesRow\x12\x10\n\x08query_id\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x02\x12\x1a\n\x12\x65stimated_time_sec\x18\x03 \x01(\x05\x12\x0e\n\x06userid\x18\x04 \x01(\t\x12\x10\n\x08sql_text\x18\x05 \x01(\t\x12\x18\n\x10\x65lapsed_time_sec\x18\x06 \x01(\x05\x12\x0e\n\x06status\x18\x07 \x01(\t\x12\x14\n\x0cquery_server\x18\x08 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\t \x01(\t\x12\x10\n\x08remoteIP\x18\n \x01(\t\x12\x15\n\rservice_class\x18\x0b \x01(\t\x12\x1d\n\x15\x65stimated_result_rows\x18\x0c \x01(\x03\x12\x1d\n\x15\x65stimated_result_size\x18\r \x01(\x03\x12\x11\n\tsent_rows\x18\x0e \x01(\x03\x12\x12\n\nsent_bytes\x18\x0f \x01(\x03\"\x1c\n\x1aSystemWideCompletedQueries\"}\n\x18\x43ompletedQueriesResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12-\n\x04rows\x18\x02 \x03(\x0b\x32\x1f.xg.cmdcomp.CompletedQueriesRow\"\xb9\x04\n\x13\x43ompletedQueriesRow\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x31\n\x0b\x64\x61tabase_id\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x16\n\x0e\x63lient_version\x18\x03 \x01(\t\x12\x11\n\tclient_ip\x18\x04 \x01(\t\x12\x0b\n\x03sql\x18\x05 \x01(\t\x12\x17\n\x0ftimestamp_start\x18\x06 \x01(\x04\x12\x12\n\ntime_start\x18\x07 \x01(\t\x12\x1a\n\x12timestamp_complete\x18\x08 \x01(\x04\x12\x15\n\rtime_complete\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\x05\x12\r\n\x05state\x18\x0b \x01(\t\x12\x0e\n\x06reason\x18\x0c \x01(\t\x12\x1c\n\x14timestamp_exec_start\x18\r \x01(\x04\x12\x17\n\x0ftime_exec_start\x18\x0e \x01(\t\x12\x0c\n\x04uuid\x18\x0f \x01(\t\x12\x15\n\rplan_priority\x18\x10 \x01(\x01\x12\x15\n\rcost_estimate\x18\x11 \x01(\x01\x12\x18\n\x10plan_parallelism\x18\x12 \x01(\r\x12\x16\n\x0eheuristic_cost\x18\x13 \x01(\x01\x12\x15\n\rpso_threshold\x18\x14 \x01(\x03\x12\x15\n\rrows_returned\x18\x15 \x01(\x04\x12\x16\n\x0e\x62ytes_returned\x18\x16 \x01(\x04\x12\x0f\n\x07runtime\x18\x17 \x01(\x04\x12 \n\x18temp_disk_space_consumed\x18\x18 \x01(\x04\"0\n\rLoadBroadcast\x12\x11\n\tcmdcompId\x18\x01 \x01(\t\x12\x0c\n\x04load\x18\x02 \x01(\x01\"\xd1\x01\n\nCacheEntry\x12\x10\n\x08\x63md_time\x18\x01 \x01(\x04\x12\x12\n\nquery_uuid\x18\x02 \x01(\t\x12\x12\n\nquery_hash\x18\x03 \x01(\x04\x12-\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x1d.xg.cmdcomp.CacheEntry.Action\x12\x15\n\rdatabase_uuid\x18\x05 \x01(\t\x12\x17\n\x0fmax_cached_time\x18\x06 \x01(\x04\"*\n\x06\x41\x63tion\x12\x0b\n\x07INVALID\x10\x00\x12\x07\n\x03\x41\x44\x44\x10\x01\x12\n\n\x06REMOVE\x10\x02\"X\n\x0bUpdateCache\x12\x13\n\x0bserver_uuid\x18\x01 \x01(\t\x12\r\n\x05\x63lear\x18\x02 \x01(\x08\x12%\n\x05\x65ntry\x18\x03 \x03(\x0b\x32\x16.xg.cmdcomp.CacheEntry\"-\n\nClearCache\x12\x11\n\tall_nodes\x18\x01 \x01(\x08\x12\x0c\n\x04user\x18\x04 \x01(\x0c\"\xca\x1d\n\x07Request\x12-\n\x04type\x18\x01 \x01(\x0e\x32\x1f.xg.cmdcomp.Request.RequestType\x12\x39\n\x11\x63lient_connection\x18\x02 \x01(\x0b\x32\x1c.xg.cmdcomp.ClientConnectionH\x00\x12;\n\x12\x63lient_connection2\x18\x03 \x01(\x0b\x32\x1d.xg.cmdcomp.ClientConnection2H\x00\x12+\n\nget_schema\x18\x04 \x01(\x0b\x32\x15.xg.cmdcomp.GetSchemaH\x00\x12\x37\n\x10\x63lose_connection\x18\x05 \x01(\x0b\x32\x1b.xg.cmdcomp.CloseConnectionH\x00\x12+\n\nset_schema\x18\x06 \x01(\x0b\x32\x15.xg.cmdcomp.SetSchemaH\x00\x12\x35\n\x0ftest_connection\x18\x07 \x01(\x0b\x32\x1a.xg.cmdcomp.TestConnectionH\x00\x12+\n\nfetch_data\x18\x08 \x01(\x0b\x32\x15.xg.cmdcomp.FetchDataH\x00\x12\x33\n\x0e\x66\x65tch_metadata\x18\t \x01(\x0b\x32\x19.xg.cmdcomp.FetchMetadataH\x00\x12\x36\n\x10\x63lose_result_set\x18\n \x01(\x0b\x32\x1a.xg.cmdcomp.CloseResultSetH\x00\x12\x31\n\rexecute_query\x18\x0b \x01(\x0b\x32\x18.xg.cmdcomp.ExecuteQueryH\x00\x12\x35\n\x0f\x65xecute_explain\x18\x0c \x01(\x0b\x32\x1a.xg.cmdcomp.ExecuteExplainH\x00\x12G\n\x19\x65xecute_explain_for_spark\x18\r \x01(\x0b\x32\".xg.cmdcomp.ExecuteExplainForSparkH\x00\x12\x33\n\x0e\x65xecute_update\x18\x0e \x01(\x0b\x32\x19.xg.cmdcomp.ExecuteUpdateH\x00\x12\x33\n\x0eload_broadcast\x18\x0f \x01(\x0b\x32\x19.xg.cmdcomp.LoadBroadcastH\x00\x12@\n\x15\x66\x65tch_system_metadata\x18\x10 \x01(\x0b\x32\x1f.xg.cmdcomp.FetchSystemMetadataH\x00\x12/\n\x0c\x63\x61ncel_query\x18\x11 \x01(\x0b\x32\x17.xg.cmdcomp.CancelQueryH\x00\x12:\n\x12local_cancel_query\x18\x1c \x01(\x0b\x32\x1c.xg.cmdcomp.LocalCancelQueryH\x00\x12<\n\x13system_wide_queries\x18\x12 \x01(\x0b\x32\x1d.xg.cmdcomp.SystemWideQueriesH\x00\x12\x31\n\rlocal_queries\x18\x13 \x01(\x0b\x32\x18.xg.cmdcomp.LocalQueriesH\x00\x12O\n\x1dsystem_wide_completed_queries\x18\x1f \x01(\x0b\x32&.xg.cmdcomp.SystemWideCompletedQueriesH\x00\x12/\n\x0c\x65xecute_plan\x18\x14 \x01(\x0b\x32\x17.xg.cmdcomp.ExecutePlanH\x00\x12/\n\x0c\x65xplain_plan\x18\x15 \x01(\x0b\x32\x17.xg.cmdcomp.ExplainPlanH\x00\x12)\n\tlist_plan\x18\x16 \x01(\x0b\x32\x14.xg.cmdcomp.ListPlanH\x00\x12+\n\nkill_query\x18\x17 \x01(\x0b\x32\x15.xg.cmdcomp.KillQueryH\x00\x12\x36\n\x10local_kill_query\x18\x1d \x01(\x0b\x32\x1a.xg.cmdcomp.LocalKillQueryH\x00\x12<\n\x13\x65xecute_inline_plan\x18\x18 \x01(\x0b\x32\x1d.xg.cmdcomp.ExecuteInlinePlanH\x00\x12\x37\n\x0e\x66orce_external\x18\x19 \x01(\x0b\x32\x19.xg.cmdcomp.ForceExternalB\x02\x18\x01H\x00\x12\x33\n\x0e\x65xecute_export\x18\x1a \x01(\x0b\x32\x19.xg.cmdcomp.ExecuteExportH\x00\x12%\n\x07set_pso\x18\x1b \x01(\x0b\x32\x12.xg.cmdcomp.SetPSOH\x00\x12\x34\n\x0f\x61ttach_to_query\x18\x1e \x01(\x0b\x32\x19.xg.cmdcomp.AttachToQueryH\x00\x12\x44\n\x17\x62\x65gin_query_concurrency\x18  \x01(\x0b\x32!.xg.cmdcomp.BeginQueryConcurrencyH\x00\x12\x46\n\x18\x66inish_query_concurrency\x18! \x01(\x0b\x32\".xg.cmdcomp.FinishQueryConcurrencyH\x00\x12L\n\x1b\x62roadcast_query_concurrency\x18\" \x01(\x0b\x32%.xg.cmdcomp.BroadcastQueryConcurrencyH\x00\x12\x31\n\rset_parameter\x18# \x01(\x0b\x32\x18.xg.cmdcomp.SetParameterH\x00\x12>\n\x10\x65xplain_pipeline\x18$ \x01(\x0b\x32\".xg.cmdcomp.ExplainPipelineRequestH\x00\x12@\n\x15\x63lient_connection_gcm\x18% \x01(\x0b\x32\x1f.xg.cmdcomp.ClientConnectionGCMH\x00\x12\x42\n\x16\x63lient_connection_gcm2\x18& \x01(\x0b\x32 .xg.cmdcomp.ClientConnectionGCM2H\x00\x12\x32\n\ncheck_data\x18\' \x01(\x0b\x32\x1c.xg.cmdcomp.CheckDataRequestH\x00\x12/\n\x0cupdate_cache\x18( \x01(\x0b\x32\x17.xg.cmdcomp.UpdateCacheH\x00\x12-\n\x0b\x63lear_cache\x18) \x01(\x0b\x32\x16.xg.cmdcomp.ClearCacheH\x00\x12@\n\x15\x63lient_connection_sso\x18* \x01(\x0b\x32\x1f.xg.cmdcomp.ClientConnectionSSOH\x00\x12\x42\n\x16\x63lient_connection_sso2\x18+ \x01(\x0b\x32 .xg.cmdcomp.ClientConnectionSSO2H\x00\x12U\n client_connection_security_token\x18, \x01(\x0b\x32).xg.cmdcomp.ClientConnectionSecurityTokenH\x00\x12W\n!client_connection_refresh_session\x18- \x01(\x0b\x32*.xg.cmdcomp.ClientConnectionRefreshSessionH\x00\x12S\n\x1f\x63lient_connection_refresh_token\x18. \x01(\x0b\x32(.xg.cmdcomp.ClientConnectionRefreshTokenH\x00\"\xa5\x08\n\x0bRequestType\x12\x0b\n\x07INVALID\x10\x00\x12\x15\n\x11\x43LIENT_CONNECTION\x10\x01\x12\x16\n\x12\x43LIENT_CONNECTION2\x10\x02\x12\x0e\n\nGET_SCHEMA\x10\x03\x12\x14\n\x10\x43LOSE_CONNECTION\x10\x04\x12\x0e\n\nSET_SCHEMA\x10\x05\x12\x13\n\x0fTEST_CONNECTION\x10\x06\x12\x0e\n\nFETCH_DATA\x10\x07\x12\x12\n\x0e\x46\x45TCH_METADATA\x10\x08\x12\x14\n\x10\x43LOSE_RESULT_SET\x10\t\x12\x11\n\rEXECUTE_QUERY\x10\n\x12\x13\n\x0f\x45XECUTE_EXPLAIN\x10\x0b\x12\x1d\n\x19\x45XECUTE_EXPLAIN_FOR_SPARK\x10\x0c\x12\x12\n\x0e\x45XECUTE_UPDATE\x10\r\x12\x12\n\x0eLOAD_BROADCAST\x10\x0e\x12\x19\n\x15\x46\x45TCH_SYSTEM_METADATA\x10\x0f\x12\x10\n\x0c\x43\x41NCEL_QUERY\x10\x10\x12\x16\n\x12LOCAL_CANCEL_QUERY\x10\x1b\x12\x17\n\x13SYSTEM_WIDE_QUERIES\x10\x11\x12\x11\n\rLOCAL_QUERIES\x10\x12\x12!\n\x1dSYSTEM_WIDE_COMPLETED_QUERIES\x10\x1e\x12\x10\n\x0c\x45XECUTE_PLAN\x10\x13\x12\x10\n\x0c\x45XPLAIN_PLAN\x10\x14\x12\r\n\tLIST_PLAN\x10\x15\x12\x0e\n\nKILL_QUERY\x10\x16\x12\x14\n\x10LOCAL_KILL_QUERY\x10\x1c\x12\x17\n\x13\x45XECUTE_INLINE_PLAN\x10\x17\x12\x12\n\x0e\x46ORCE_EXTERNAL\x10\x18\x12\x12\n\x0e\x45XECUTE_EXPORT\x10\x19\x12\x0b\n\x07SET_PSO\x10\x1a\x12\x13\n\x0f\x41TTACH_TO_QUERY\x10\x1d\x12\x1b\n\x17\x42\x45GIN_QUERY_CONCURRENCY\x10\x1f\x12\x1c\n\x18\x46INISH_QUERY_CONCURRENCY\x10 \x12\x1f\n\x1b\x42ROADCAST_QUERY_CONCURRENCY\x10!\x12\x11\n\rSET_PARAMETER\x10\"\x12\x14\n\x10\x45XPLAIN_PIPELINE\x10#\x12\x19\n\x15\x43LIENT_CONNECTION_GCM\x10$\x12\x1a\n\x16\x43LIENT_CONNECTION_GCM2\x10%\x12\x0e\n\nCHECK_DATA\x10&\x12\x10\n\x0cUPDATE_CACHE\x10\'\x12\x0f\n\x0b\x43LEAR_CACHE\x10(\x12\x19\n\x15\x43LIENT_CONNECTION_SSO\x10)\x12\x1a\n\x16\x43LIENT_CONNECTION_SSO2\x10*\x12$\n CLIENT_CONNECTION_SECURITY_TOKEN\x10+\x12%\n!CLIENT_CONNECTION_REFRESH_SESSION\x10,\x12#\n\x1f\x43LIENT_CONNECTION_REFRESH_TOKEN\x10-B\x0f\n\rrequest_oneof\"\xe0\x01\n\x14\x43onfirmationResponse\x12;\n\x04type\x18\x01 \x01(\x0e\x32-.xg.cmdcomp.ConfirmationResponse.ResponseType\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x11\n\tsql_state\x18\x03 \x01(\t\x12\x13\n\x0bvendor_code\x18\x04 \x01(\x0f\"S\n\x0cResponseType\x12\x0b\n\x07INVALID\x10\x00\x12\x0f\n\x0bRESPONSE_OK\x10\x01\x12\x11\n\rRESPONSE_WARN\x10\x02\x12\x12\n\x0eRESPONSE_ERROR\x10\x03\")\n\x0b\x45xecutePlan\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"/\n\x11\x45xecuteInlinePlan\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"T\n\x0b\x45xplainPlan\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12)\n\x06\x66ormat\x18\x03 \x01(\x0e\x32\x19.xg.cmdcomp.ExplainFormat\"\"\n\rForceExternal\x12\r\n\x05\x66orce\x18\x01 \x01(\x08:\x02\x18\x01\"\n\n\x08ListPlan\"\x96\x01\n\x10ListPlanResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08planName\x18\x02 \x03(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"\x1a\n\x0b\x43\x61ncelQuery\x12\x0b\n\x03sql\x18\x01 \x01(\t\"I\n\x13\x43\x61ncelQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\xdd\x01\n\x10LocalCancelQuery\x12\x14\n\x08identity\x18\x01 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\ruuid_identity\x18\x02 \x01(\x0c\x42\x02\x18\x01H\x00\x12\x0b\n\x03sql\x18\x03 \x01(\t\x12\x10\n\x04user\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12\r\n\x05token\x18\x05 \x01(\x0c\x12\x15\n\tsignature\x18\x06 \x01(\x0c\x42\x02\x18\x01\x12\x1e\n\x12issuer_certificate\x18\x07 \x01(\x0c\x42\x02\x18\x01\x12\x1a\n\x12issuer_fingerprint\x18\x08 \x01(\x0c\x42\x15\n\x13one_identity_option\"N\n\x18LocalCancelQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\x18\n\tKillQuery\x12\x0b\n\x03sql\x18\x01 \x01(\t\"G\n\x11KillQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\xdb\x01\n\x0eLocalKillQuery\x12\x14\n\x08identity\x18\x01 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\ruuid_identity\x18\x02 \x01(\x0c\x42\x02\x18\x01H\x00\x12\x0b\n\x03sql\x18\x03 \x01(\t\x12\x10\n\x04user\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12\r\n\x05token\x18\x05 \x01(\x0c\x12\x15\n\tsignature\x18\x06 \x01(\x0c\x42\x02\x18\x01\x12\x1e\n\x12issuer_certificate\x18\x07 \x01(\x0c\x42\x02\x18\x01\x12\x1a\n\x12issuer_fingerprint\x18\x08 \x01(\x0c\x42\x15\n\x13one_identity_option\"L\n\x16LocalKillQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\x1c\n\rExecuteExport\x12\x0b\n\x03sql\x18\x01 \x01(\t\"d\n\x15\x45xecuteExportResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x17\n\x0f\x65xportStatement\x18\x02 \x01(\t\"%\n\x16\x45xplainPipelineRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\"h\n\x17\x45xplainPipelineResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x19\n\x11pipelineStatement\x18\x02 \x01(\t\"\x1f\n\x10\x43heckDataRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\"c\n\x11\x43heckDataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x1a\n\x12\x63heckDataStatement\x18\x02 \x01(\t\"*\n\x06SetPSO\x12\x11\n\tthreshold\x18\x01 \x01(\x03\x12\r\n\x05reset\x18\x02 \x01(\x08\"\x8b\x07\n\x0cSetParameter\x12\r\n\x05reset\x18\x01 \x01(\x08\x12\x35\n\rpso_threshold\x18\x02 \x01(\x0b\x32\x1c.xg.cmdcomp.SetParameter.PSOH\x00\x12\x36\n\trow_limit\x18\x03 \x01(\x0b\x32!.xg.cmdcomp.SetParameter.RowLimitH\x00\x12\x38\n\ntime_limit\x18\x04 \x01(\x0b\x32\".xg.cmdcomp.SetParameter.TimeLimitH\x00\x12\x44\n\x0ftemp_disk_limit\x18\x05 \x01(\x0b\x32).xg.cmdcomp.SetParameter.MaxTempDiskLimitH\x00\x12\x35\n\x08priority\x18\x06 \x01(\x0b\x32!.xg.cmdcomp.SetParameter.PriorityH\x00\x12;\n\x0b\x63oncurrency\x18\x07 \x01(\x0b\x32$.xg.cmdcomp.SetParameter.ConcurrencyH\x00\x12\x34\n\x08pso_seed\x18\x08 \x01(\x0b\x32 .xg.cmdcomp.SetParameter.PSOSeedH\x00\x12P\n\x17result_set_column_limit\x18\t \x01(\x0b\x32-.xg.cmdcomp.SetParameter.ResultSetColumnLimitH\x00\x12@\n\x0e\x66orce_external\x18\n \x01(\x0b\x32&.xg.cmdcomp.SetParameter.ForceExternalH\x00\x1a\x18\n\x03PSO\x12\x11\n\tthreshold\x18\x01 \x01(\x03\x1a\x1c\n\x08RowLimit\x12\x10\n\x08rowLimit\x18\x01 \x01(\x03\x1a\x1e\n\tTimeLimit\x12\x11\n\ttimeLimit\x18\x01 \x01(\x03\x1a)\n\x10MaxTempDiskLimit\x12\x15\n\rtempDiskLimit\x18\x01 \x01(\x03\x1a\x34\n\x14ResultSetColumnLimit\x12\x1c\n\x14resultSetColumnLimit\x18\x01 \x01(\x03\x1a\x1c\n\x08Priority\x12\x10\n\x08priority\x18\x01 \x01(\x01\x1a\"\n\x0b\x43oncurrency\x12\x13\n\x0b\x63oncurrency\x18\x01 \x01(\x03\x1a\x17\n\x07PSOSeed\x12\x0c\n\x04seed\x18\x01 \x01(\x04\x1a\x1e\n\rForceExternal\x12\r\n\x05is_on\x18\x01 \x01(\x08\x42\x0b\n\tParameter*/\n\rExplainFormat\x12\t\n\x05PROTO\x10\x00\x12\x08\n\x04JSON\x10\x01\x12\t\n\x05\x44\x45\x42UG\x10\x02\x62\x06proto3'
+  serialized_pb=b'\n\'sharedMessages/clientWireProtocol.proto\x12\nxg.cmdcomp\x1a\x1egoogle/protobuf/wrappers.proto\"\xa2\x01\n\x10\x43lientConnection\x12\x0e\n\x06userid\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x10\n\x08\x63lientid\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x05 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x06 \x01(\x05\x12\x11\n\tsessionID\x18\x07 \x01(\t\"\xba\x01\n\x13\x43lientConnectionGCM\x12\x0e\n\x06userid\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x10\n\x08\x63lientid\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x05 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x06 \x01(\x05\x12\x11\n\tsessionID\x18\x07 \x01(\t\x12\x13\n\x0b\x65xplicitSSO\x18\x08 \x01(\x08\"\x95\x01\n\x13\x43lientConnectionSSO\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x10\n\x08\x63lientid\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x04 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x05 \x01(\x05\x12\x11\n\tsessionID\x18\x06 \x01(\t\"\xf8\x01\n\x1d\x43lientConnectionSecurityToken\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x10\n\x08\x63lientid\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x04 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x05 \x01(\x05\x12\x11\n\tsessionID\x18\x06 \x01(\t\x12\x15\n\rsecurityToken\x18\x07 \x01(\t\x12\x16\n\x0etokenSignature\x18\x08 \x01(\t\x12\x19\n\x11issuerFingerprint\x18\t \x01(\t\x12\r\n\x05\x66orce\x18\n \x01(\x08\"j\n\x18\x43lientConnectionResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\n\n\x02iv\x18\x02 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x03 \x01(\t\"m\n\x1b\x43lientConnectionGCMResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\n\n\x02iv\x18\x02 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x03 \x01(\t\"u\n\x1b\x43lientConnectionSSOResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x11\n\trequestId\x18\x02 \x01(\t\x12\x0f\n\x07\x61uthUrl\x18\x03 \x01(\t\"\xfb\x01\n%ClientConnectionSecurityTokenResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x05 \x03(\t\x12\x35\n\tsecondary\x18\x06 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceList\x12\x17\n\x0fserverSessionId\x18\x07 \x01(\t\"P\n\x11\x43lientConnection2\x12\x0e\n\x06\x63ipher\x18\x01 \x01(\x0c\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x0c\n\x04hmac\x18\x03 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x04 \x01(\t\"h\n\x14\x43lientConnectionGCM2\x12\x0e\n\x06\x63ipher\x18\x01 \x01(\x0c\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x0c\n\x04hmac\x18\x03 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x04 \x01(\t\x12\x13\n\x0b\x65xplicitSSO\x18\x05 \x01(\x08\"8\n\x14\x43lientConnectionSSO2\x12\x11\n\trequestId\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"K\n\rSecurityToken\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\x12\x11\n\tsignature\x18\x02 \x01(\t\x12\x19\n\x11issuerFingerprint\x18\x03 \x01(\t\"X\n\x0bSessionInfo\x12\x17\n\x0fserverSessionId\x18\x01 \x01(\t\x12\x30\n\rsecurityToken\x18\x02 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\" \n\x1e\x43lientConnectionRefreshSession\"\x8a\x01\n&ClientConnectionRefreshSessionResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12,\n\x0bsessionInfo\x18\x02 \x01(\x0b\x32\x17.xg.cmdcomp.SessionInfo\"S\n\x1c\x43lientConnectionRefreshToken\x12\x33\n\x10oldSecurityToken\x18\x01 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\"\x8f\x01\n$ClientConnectionRefreshTokenResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x33\n\x10newSecurityToken\x18\x02 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\")\n\x16SecondaryInterfaceList\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x03(\t\"\xef\x01\n\x19\x43lientConnection2Response\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x05 \x03(\t\x12\x35\n\tsecondary\x18\x06 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceList\x12\x17\n\x0fserverSessionId\x18\x07 \x01(\t\"\xf2\x01\n\x1c\x43lientConnectionGCM2Response\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x05 \x03(\t\x12\x35\n\tsecondary\x18\x06 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceList\x12\x17\n\x0fserverSessionId\x18\x07 \x01(\t\"\xbd\x02\n\x1c\x43lientConnectionSSO2Response\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12 \n\x16pollingIntervalSeconds\x18\x02 \x01(\x05H\x00\x12.\n\x0bsessionInfo\x18\x03 \x01(\x0b\x32\x17.xg.cmdcomp.SessionInfoH\x00\x12\x10\n\x08redirect\x18\x04 \x01(\x08\x12\x14\n\x0credirectHost\x18\x05 \x01(\t\x12\x14\n\x0credirectPort\x18\x06 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x07 \x03(\t\x12\x35\n\tsecondary\x18\x08 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceListB\x10\n\x0eresponse_oneof\"\x0b\n\tGetSchema\"W\n\x11GetSchemaResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x0e\n\x06schema\x18\x02 \x01(\t\"\x1b\n\tSetSchema\x12\x0e\n\x06schema\x18\x01 \x01(\t\"%\n\x0f\x43loseConnection\x12\x12\n\nendSession\x18\x01 \x01(\x08\"\x10\n\x0eTestConnection\" \n\rAttachToQuery\x12\x0f\n\x07queryId\x18\x01 \x01(\t\"\x1f\n\tFetchData\x12\x12\n\nfetch_size\x18\x01 \x01(\x0f\"A\n\tResultSet\x12\x10\n\x08numParts\x18\x01 \x01(\x05\x12\x13\n\x0b\x62lobLengths\x18\x02 \x03(\x05\x12\r\n\x05\x62lobs\x18\x03 \x03(\x0c\"r\n\x11\x46\x65tchDataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12)\n\nresult_set\x18\x02 \x01(\x0b\x32\x15.xg.cmdcomp.ResultSet\"\x0f\n\rFetchMetadata\"\xb9\x02\n\x15\x46\x65tchMetadataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x41\n\x08\x63ols2pos\x18\x02 \x03(\x0b\x32/.xg.cmdcomp.FetchMetadataResponse.Cols2posEntry\x12\x45\n\ncols2Types\x18\x03 \x03(\x0b\x32\x31.xg.cmdcomp.FetchMetadataResponse.Cols2TypesEntry\x1a/\n\rCols2posEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0f:\x02\x38\x01\x1a\x31\n\x0f\x43ols2TypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xde\x04\n\x13\x46\x65tchSystemMetadata\x12@\n\x04\x63\x61ll\x18\x01 \x01(\x0e\x32\x32.xg.cmdcomp.FetchSystemMetadata.SystemMetadataCall\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\r\n\x05table\x18\x03 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x04 \x01(\t\x12\x0c\n\x04view\x18\x05 \x01(\t\x12\x0c\n\x04test\x18\x06 \x01(\x08\"\xb9\x03\n\x12SystemMetadataCall\x12\x0b\n\x07INVALID\x10\x00\x12\x0f\n\x0bGET_SCHEMAS\x10\x01\x12\x0e\n\nGET_TABLES\x10\x02\x12\x15\n\x11GET_SYSTEM_TABLES\x10\x0e\x12\x18\n\x14GET_TABLE_PRIVILEGES\x10\x0f\x12\x19\n\x15GET_COLUMN_PRIVILEGES\x10\x10\x12\r\n\tGET_VIEWS\x10\x19\x12\x0f\n\x0bGET_COLUMNS\x10\x03\x12\x12\n\x0eGET_INDEX_INFO\x10\x04\x12\x11\n\rGET_TYPE_INFO\x10\x05\x12\x14\n\x10GET_SQL_KEYWORDS\x10\x06\x12\x19\n\x15GET_NUMERIC_FUNCTIONS\x10\x07\x12\x18\n\x14GET_STRING_FUNCTIONS\x10\x08\x12\x1b\n\x17GET_TIME_DATE_FUNCTIONS\x10\t\x12\x18\n\x14GET_SYSTEM_FUNCTIONS\x10\n\x12 \n\x1cGET_DATABASE_PRODUCT_VERSION\x10\x0b\x12\x1e\n\x1aGET_DATABASE_MAJOR_VERSION\x10\x0c\x12\x1e\n\x1aGET_DATABASE_MINOR_VERSION\x10\r\"\xbb\x01\n\x1b\x46\x65tchSystemMetadataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12/\n\x0eresult_set_val\x18\x02 \x01(\x0b\x32\x15.xg.cmdcomp.ResultSetH\x00\x12\x14\n\nstring_val\x18\x03 \x01(\tH\x00\x12\x11\n\x07int_val\x18\x04 \x01(\x0fH\x00\x42\x0e\n\x0cresult_oneof\"\x10\n\x0e\x43loseResultSet\"A\n\x0c\x45xecuteQuery\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x15\n\rforceRedirect\x18\x03 \x01(\x08\"\xb3\x01\n\x14\x45xecuteQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x0f\n\x07queryId\x18\x05 \x01(\t\x12\x18\n\x10numClientThreads\x18\x06 \x01(\x07\"+\n\rExecuteUpdate\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa1\x01\n\x15\x45xecuteUpdateResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x16\n\x0eupdateRowCount\x18\x02 \x01(\x0f\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"W\n\x0e\x45xecuteExplain\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12)\n\x06\x66ormat\x18\x03 \x01(\x0e\x32\x19.xg.cmdcomp.ExplainFormat\"\xdc\x01\n\x16\x45xecuteExplainForSpark\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x41\n\x04type\x18\x02 \x01(\x0e\x32\x33.xg.cmdcomp.ExecuteExplainForSpark.PartitioningType\x12\x19\n\x11partitioningParam\x18\x03 \x01(\x0f\x12\r\n\x05\x66orce\x18\x04 \x01(\x08\"H\n\x10PartitioningType\x12\x18\n\x14INVALID_PARTITIONING\x10\x00\x12\x0b\n\x07\x42Y_SIZE\x10\x01\x12\r\n\tBY_NUMBER\x10\x02\"\x9b\x01\n\x19\x45xplainResponseStringPlan\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x0c\n\x04plan\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"V\n\x15\x42\x65ginQueryConcurrency\x12\x14\n\x0cnodeEndpoint\x18\x01 \x01(\t\x12\x16\n\x0eserviceClassId\x18\x02 \x01(\t\x12\x0f\n\x07queryId\x18\x03 \x01(\t\"W\n\x16\x46inishQueryConcurrency\x12\x14\n\x0cnodeEndpoint\x18\x01 \x01(\t\x12\x16\n\x0eserviceClassId\x18\x02 \x01(\t\x12\x0f\n\x07queryId\x18\x03 \x01(\t\"\xd3\x01\n\x19\x42roadcastQueryConcurrency\x12\x14\n\x0cnodeEndpoint\x18\x01 \x01(\t\x12\x61\n\x16serviceClassIdToCounts\x18\x02 \x03(\x0b\x32\x41.xg.cmdcomp.BroadcastQueryConcurrency.ServiceClassIdToCountsEntry\x1a=\n\x1bServiceClassIdToCountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"N\n\x18QueryConcurrencyResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\x13\n\x11SystemWideQueries\"x\n\x19SystemWideQueriesResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\'\n\x04rows\x18\x02 \x03(\x0b\x32\x19.xg.cmdcomp.SysQueriesRow\"\x87\x02\n\x0cLocalQueries\x12\x14\n\x08identity\x18\x01 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\ruuid_identity\x18\x02 \x01(\x0c\x42\x02\x18\x01H\x00\x12\x10\n\x08\x64\x61tabase\x18\x03 \x01(\t\x12\r\n\x05token\x18\x04 \x01(\x0c\x12\x15\n\tsignature\x18\x05 \x01(\x0c\x42\x02\x18\x01\x12\x1e\n\x12issuer_certificate\x18\x06 \x01(\x0c\x42\x02\x18\x01\x12\x1a\n\x12issuer_fingerprint\x18\x07 \x01(\x0c\x12\x14\n\x08username\x18\x08 \x01(\x0c\x42\x02\x18\x01\x12\x11\n\tcompleted\x18\t \x01(\x08\x12\x10\n\x04user\x18\n \x01(\x0c\x42\x02\x18\x01\x42\x15\n\x13one_identity_option\"s\n\x14LocalQueriesResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\'\n\x04rows\x18\x02 \x03(\x0b\x32\x19.xg.cmdcomp.SysQueriesRow\"\xd7\x03\n\rSysQueriesRow\x12\x10\n\x08query_id\x18\x01 \x01(\t\x12\x1a\n\x12\x65\x66\x66\x65\x63tive_priority\x18\x02 \x01(\x02\x12\x1a\n\x12\x65stimated_time_sec\x18\x03 \x01(\x05\x12\x0e\n\x06userid\x18\x04 \x01(\t\x12\x10\n\x08sql_text\x18\x05 \x01(\t\x12\x18\n\x10\x65lapsed_time_sec\x18\x06 \x01(\x05\x12\x0e\n\x06status\x18\x07 \x01(\t\x12\x14\n\x0cquery_server\x18\x08 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\t \x01(\t\x12\x10\n\x08remoteIP\x18\n \x01(\t\x12\x15\n\rservice_class\x18\x0b \x01(\t\x12\x1d\n\x15\x65stimated_result_rows\x18\x0c \x01(\x03\x12\x1d\n\x15\x65stimated_result_size\x18\r \x01(\x03\x12\x11\n\tsent_rows\x18\x0e \x01(\x03\x12\x12\n\nsent_bytes\x18\x0f \x01(\x03\x12\x18\n\x10initial_priority\x18\x10 \x01(\x02\x12\"\n\x1ainitial_effective_priority\x18\x11 \x01(\x02\x12\x1e\n\x16priority_adjust_factor\x18\x12 \x01(\x02\x12\x1c\n\x14priority_adjust_time\x18\x13 \x01(\r\"\x1c\n\x1aSystemWideCompletedQueries\"}\n\x18\x43ompletedQueriesResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12-\n\x04rows\x18\x02 \x03(\x0b\x32\x1f.xg.cmdcomp.CompletedQueriesRow\"\xc0\x05\n\x13\x43ompletedQueriesRow\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x31\n\x0b\x64\x61tabase_id\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x16\n\x0e\x63lient_version\x18\x03 \x01(\t\x12\x11\n\tclient_ip\x18\x04 \x01(\t\x12\x0b\n\x03sql\x18\x05 \x01(\t\x12\x17\n\x0ftimestamp_start\x18\x06 \x01(\x04\x12\x12\n\ntime_start\x18\x07 \x01(\t\x12\x1a\n\x12timestamp_complete\x18\x08 \x01(\x04\x12\x15\n\rtime_complete\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\x05\x12\r\n\x05state\x18\x0b \x01(\t\x12\x0e\n\x06reason\x18\x0c \x01(\t\x12\x1c\n\x14timestamp_exec_start\x18\r \x01(\x04\x12\x17\n\x0ftime_exec_start\x18\x0e \x01(\t\x12\x0c\n\x04uuid\x18\x0f \x01(\t\x12 \n\x18\x66inal_effective_priority\x18\x10 \x01(\x01\x12\x15\n\rcost_estimate\x18\x11 \x01(\x01\x12\x18\n\x10plan_parallelism\x18\x12 \x01(\r\x12\x16\n\x0eheuristic_cost\x18\x13 \x01(\x01\x12\x15\n\rpso_threshold\x18\x14 \x01(\x03\x12\x15\n\rrows_returned\x18\x15 \x01(\x04\x12\x16\n\x0e\x62ytes_returned\x18\x16 \x01(\x04\x12\x0f\n\x07runtime\x18\x17 \x01(\x04\x12 \n\x18temp_disk_space_consumed\x18\x18 \x01(\x04\x12\x1e\n\x16priority_adjust_factor\x18\x19 \x01(\x02\x12\x1c\n\x14priority_adjust_time\x18\x1a \x01(\r\x12\x18\n\x10initial_priority\x18\x1b \x01(\x02\x12\"\n\x1ainitial_effective_priority\x18\x1c \x01(\x02\"0\n\rLoadBroadcast\x12\x11\n\tcmdcompId\x18\x01 \x01(\t\x12\x0c\n\x04load\x18\x02 \x01(\x01\"\xd1\x01\n\nCacheEntry\x12\x10\n\x08\x63md_time\x18\x01 \x01(\x04\x12\x12\n\nquery_uuid\x18\x02 \x01(\t\x12\x12\n\nquery_hash\x18\x03 \x01(\x04\x12-\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x1d.xg.cmdcomp.CacheEntry.Action\x12\x15\n\rdatabase_uuid\x18\x05 \x01(\t\x12\x17\n\x0fmax_cached_time\x18\x06 \x01(\x04\"*\n\x06\x41\x63tion\x12\x0b\n\x07INVALID\x10\x00\x12\x07\n\x03\x41\x44\x44\x10\x01\x12\n\n\x06REMOVE\x10\x02\"X\n\x0bUpdateCache\x12\x13\n\x0bserver_uuid\x18\x01 \x01(\t\x12\r\n\x05\x63lear\x18\x02 \x01(\x08\x12%\n\x05\x65ntry\x18\x03 \x03(\x0b\x32\x16.xg.cmdcomp.CacheEntry\"-\n\nClearCache\x12\x11\n\tall_nodes\x18\x01 \x01(\x08\x12\x0c\n\x04user\x18\x04 \x01(\x0c\"\xca\x1d\n\x07Request\x12-\n\x04type\x18\x01 \x01(\x0e\x32\x1f.xg.cmdcomp.Request.RequestType\x12\x39\n\x11\x63lient_connection\x18\x02 \x01(\x0b\x32\x1c.xg.cmdcomp.ClientConnectionH\x00\x12;\n\x12\x63lient_connection2\x18\x03 \x01(\x0b\x32\x1d.xg.cmdcomp.ClientConnection2H\x00\x12+\n\nget_schema\x18\x04 \x01(\x0b\x32\x15.xg.cmdcomp.GetSchemaH\x00\x12\x37\n\x10\x63lose_connection\x18\x05 \x01(\x0b\x32\x1b.xg.cmdcomp.CloseConnectionH\x00\x12+\n\nset_schema\x18\x06 \x01(\x0b\x32\x15.xg.cmdcomp.SetSchemaH\x00\x12\x35\n\x0ftest_connection\x18\x07 \x01(\x0b\x32\x1a.xg.cmdcomp.TestConnectionH\x00\x12+\n\nfetch_data\x18\x08 \x01(\x0b\x32\x15.xg.cmdcomp.FetchDataH\x00\x12\x33\n\x0e\x66\x65tch_metadata\x18\t \x01(\x0b\x32\x19.xg.cmdcomp.FetchMetadataH\x00\x12\x36\n\x10\x63lose_result_set\x18\n \x01(\x0b\x32\x1a.xg.cmdcomp.CloseResultSetH\x00\x12\x31\n\rexecute_query\x18\x0b \x01(\x0b\x32\x18.xg.cmdcomp.ExecuteQueryH\x00\x12\x35\n\x0f\x65xecute_explain\x18\x0c \x01(\x0b\x32\x1a.xg.cmdcomp.ExecuteExplainH\x00\x12G\n\x19\x65xecute_explain_for_spark\x18\r \x01(\x0b\x32\".xg.cmdcomp.ExecuteExplainForSparkH\x00\x12\x33\n\x0e\x65xecute_update\x18\x0e \x01(\x0b\x32\x19.xg.cmdcomp.ExecuteUpdateH\x00\x12\x33\n\x0eload_broadcast\x18\x0f \x01(\x0b\x32\x19.xg.cmdcomp.LoadBroadcastH\x00\x12@\n\x15\x66\x65tch_system_metadata\x18\x10 \x01(\x0b\x32\x1f.xg.cmdcomp.FetchSystemMetadataH\x00\x12/\n\x0c\x63\x61ncel_query\x18\x11 \x01(\x0b\x32\x17.xg.cmdcomp.CancelQueryH\x00\x12:\n\x12local_cancel_query\x18\x1c \x01(\x0b\x32\x1c.xg.cmdcomp.LocalCancelQueryH\x00\x12<\n\x13system_wide_queries\x18\x12 \x01(\x0b\x32\x1d.xg.cmdcomp.SystemWideQueriesH\x00\x12\x31\n\rlocal_queries\x18\x13 \x01(\x0b\x32\x18.xg.cmdcomp.LocalQueriesH\x00\x12O\n\x1dsystem_wide_completed_queries\x18\x1f \x01(\x0b\x32&.xg.cmdcomp.SystemWideCompletedQueriesH\x00\x12/\n\x0c\x65xecute_plan\x18\x14 \x01(\x0b\x32\x17.xg.cmdcomp.ExecutePlanH\x00\x12/\n\x0c\x65xplain_plan\x18\x15 \x01(\x0b\x32\x17.xg.cmdcomp.ExplainPlanH\x00\x12)\n\tlist_plan\x18\x16 \x01(\x0b\x32\x14.xg.cmdcomp.ListPlanH\x00\x12+\n\nkill_query\x18\x17 \x01(\x0b\x32\x15.xg.cmdcomp.KillQueryH\x00\x12\x36\n\x10local_kill_query\x18\x1d \x01(\x0b\x32\x1a.xg.cmdcomp.LocalKillQueryH\x00\x12<\n\x13\x65xecute_inline_plan\x18\x18 \x01(\x0b\x32\x1d.xg.cmdcomp.ExecuteInlinePlanH\x00\x12\x37\n\x0e\x66orce_external\x18\x19 \x01(\x0b\x32\x19.xg.cmdcomp.ForceExternalB\x02\x18\x01H\x00\x12\x33\n\x0e\x65xecute_export\x18\x1a \x01(\x0b\x32\x19.xg.cmdcomp.ExecuteExportH\x00\x12%\n\x07set_pso\x18\x1b \x01(\x0b\x32\x12.xg.cmdcomp.SetPSOH\x00\x12\x34\n\x0f\x61ttach_to_query\x18\x1e \x01(\x0b\x32\x19.xg.cmdcomp.AttachToQueryH\x00\x12\x44\n\x17\x62\x65gin_query_concurrency\x18  \x01(\x0b\x32!.xg.cmdcomp.BeginQueryConcurrencyH\x00\x12\x46\n\x18\x66inish_query_concurrency\x18! \x01(\x0b\x32\".xg.cmdcomp.FinishQueryConcurrencyH\x00\x12L\n\x1b\x62roadcast_query_concurrency\x18\" \x01(\x0b\x32%.xg.cmdcomp.BroadcastQueryConcurrencyH\x00\x12\x31\n\rset_parameter\x18# \x01(\x0b\x32\x18.xg.cmdcomp.SetParameterH\x00\x12>\n\x10\x65xplain_pipeline\x18$ \x01(\x0b\x32\".xg.cmdcomp.ExplainPipelineRequestH\x00\x12@\n\x15\x63lient_connection_gcm\x18% \x01(\x0b\x32\x1f.xg.cmdcomp.ClientConnectionGCMH\x00\x12\x42\n\x16\x63lient_connection_gcm2\x18& \x01(\x0b\x32 .xg.cmdcomp.ClientConnectionGCM2H\x00\x12\x32\n\ncheck_data\x18\' \x01(\x0b\x32\x1c.xg.cmdcomp.CheckDataRequestH\x00\x12/\n\x0cupdate_cache\x18( \x01(\x0b\x32\x17.xg.cmdcomp.UpdateCacheH\x00\x12-\n\x0b\x63lear_cache\x18) \x01(\x0b\x32\x16.xg.cmdcomp.ClearCacheH\x00\x12@\n\x15\x63lient_connection_sso\x18* \x01(\x0b\x32\x1f.xg.cmdcomp.ClientConnectionSSOH\x00\x12\x42\n\x16\x63lient_connection_sso2\x18+ \x01(\x0b\x32 .xg.cmdcomp.ClientConnectionSSO2H\x00\x12U\n client_connection_security_token\x18, \x01(\x0b\x32).xg.cmdcomp.ClientConnectionSecurityTokenH\x00\x12W\n!client_connection_refresh_session\x18- \x01(\x0b\x32*.xg.cmdcomp.ClientConnectionRefreshSessionH\x00\x12S\n\x1f\x63lient_connection_refresh_token\x18. \x01(\x0b\x32(.xg.cmdcomp.ClientConnectionRefreshTokenH\x00\"\xa5\x08\n\x0bRequestType\x12\x0b\n\x07INVALID\x10\x00\x12\x15\n\x11\x43LIENT_CONNECTION\x10\x01\x12\x16\n\x12\x43LIENT_CONNECTION2\x10\x02\x12\x0e\n\nGET_SCHEMA\x10\x03\x12\x14\n\x10\x43LOSE_CONNECTION\x10\x04\x12\x0e\n\nSET_SCHEMA\x10\x05\x12\x13\n\x0fTEST_CONNECTION\x10\x06\x12\x0e\n\nFETCH_DATA\x10\x07\x12\x12\n\x0e\x46\x45TCH_METADATA\x10\x08\x12\x14\n\x10\x43LOSE_RESULT_SET\x10\t\x12\x11\n\rEXECUTE_QUERY\x10\n\x12\x13\n\x0f\x45XECUTE_EXPLAIN\x10\x0b\x12\x1d\n\x19\x45XECUTE_EXPLAIN_FOR_SPARK\x10\x0c\x12\x12\n\x0e\x45XECUTE_UPDATE\x10\r\x12\x12\n\x0eLOAD_BROADCAST\x10\x0e\x12\x19\n\x15\x46\x45TCH_SYSTEM_METADATA\x10\x0f\x12\x10\n\x0c\x43\x41NCEL_QUERY\x10\x10\x12\x16\n\x12LOCAL_CANCEL_QUERY\x10\x1b\x12\x17\n\x13SYSTEM_WIDE_QUERIES\x10\x11\x12\x11\n\rLOCAL_QUERIES\x10\x12\x12!\n\x1dSYSTEM_WIDE_COMPLETED_QUERIES\x10\x1e\x12\x10\n\x0c\x45XECUTE_PLAN\x10\x13\x12\x10\n\x0c\x45XPLAIN_PLAN\x10\x14\x12\r\n\tLIST_PLAN\x10\x15\x12\x0e\n\nKILL_QUERY\x10\x16\x12\x14\n\x10LOCAL_KILL_QUERY\x10\x1c\x12\x17\n\x13\x45XECUTE_INLINE_PLAN\x10\x17\x12\x12\n\x0e\x46ORCE_EXTERNAL\x10\x18\x12\x12\n\x0e\x45XECUTE_EXPORT\x10\x19\x12\x0b\n\x07SET_PSO\x10\x1a\x12\x13\n\x0f\x41TTACH_TO_QUERY\x10\x1d\x12\x1b\n\x17\x42\x45GIN_QUERY_CONCURRENCY\x10\x1f\x12\x1c\n\x18\x46INISH_QUERY_CONCURRENCY\x10 \x12\x1f\n\x1b\x42ROADCAST_QUERY_CONCURRENCY\x10!\x12\x11\n\rSET_PARAMETER\x10\"\x12\x14\n\x10\x45XPLAIN_PIPELINE\x10#\x12\x19\n\x15\x43LIENT_CONNECTION_GCM\x10$\x12\x1a\n\x16\x43LIENT_CONNECTION_GCM2\x10%\x12\x0e\n\nCHECK_DATA\x10&\x12\x10\n\x0cUPDATE_CACHE\x10\'\x12\x0f\n\x0b\x43LEAR_CACHE\x10(\x12\x19\n\x15\x43LIENT_CONNECTION_SSO\x10)\x12\x1a\n\x16\x43LIENT_CONNECTION_SSO2\x10*\x12$\n CLIENT_CONNECTION_SECURITY_TOKEN\x10+\x12%\n!CLIENT_CONNECTION_REFRESH_SESSION\x10,\x12#\n\x1f\x43LIENT_CONNECTION_REFRESH_TOKEN\x10-B\x0f\n\rrequest_oneof\"\xe0\x01\n\x14\x43onfirmationResponse\x12;\n\x04type\x18\x01 \x01(\x0e\x32-.xg.cmdcomp.ConfirmationResponse.ResponseType\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x11\n\tsql_state\x18\x03 \x01(\t\x12\x13\n\x0bvendor_code\x18\x04 \x01(\x0f\"S\n\x0cResponseType\x12\x0b\n\x07INVALID\x10\x00\x12\x0f\n\x0bRESPONSE_OK\x10\x01\x12\x11\n\rRESPONSE_WARN\x10\x02\x12\x12\n\x0eRESPONSE_ERROR\x10\x03\")\n\x0b\x45xecutePlan\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"/\n\x11\x45xecuteInlinePlan\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"T\n\x0b\x45xplainPlan\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12)\n\x06\x66ormat\x18\x03 \x01(\x0e\x32\x19.xg.cmdcomp.ExplainFormat\"\"\n\rForceExternal\x12\r\n\x05\x66orce\x18\x01 \x01(\x08:\x02\x18\x01\"\n\n\x08ListPlan\"\x96\x01\n\x10ListPlanResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08planName\x18\x02 \x03(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"\x1a\n\x0b\x43\x61ncelQuery\x12\x0b\n\x03sql\x18\x01 \x01(\t\"I\n\x13\x43\x61ncelQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\xdd\x01\n\x10LocalCancelQuery\x12\x14\n\x08identity\x18\x01 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\ruuid_identity\x18\x02 \x01(\x0c\x42\x02\x18\x01H\x00\x12\x0b\n\x03sql\x18\x03 \x01(\t\x12\x10\n\x04user\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12\r\n\x05token\x18\x05 \x01(\x0c\x12\x15\n\tsignature\x18\x06 \x01(\x0c\x42\x02\x18\x01\x12\x1e\n\x12issuer_certificate\x18\x07 \x01(\x0c\x42\x02\x18\x01\x12\x1a\n\x12issuer_fingerprint\x18\x08 \x01(\x0c\x42\x15\n\x13one_identity_option\"N\n\x18LocalCancelQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\x18\n\tKillQuery\x12\x0b\n\x03sql\x18\x01 \x01(\t\"G\n\x11KillQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\xdb\x01\n\x0eLocalKillQuery\x12\x14\n\x08identity\x18\x01 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\ruuid_identity\x18\x02 \x01(\x0c\x42\x02\x18\x01H\x00\x12\x0b\n\x03sql\x18\x03 \x01(\t\x12\x10\n\x04user\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12\r\n\x05token\x18\x05 \x01(\x0c\x12\x15\n\tsignature\x18\x06 \x01(\x0c\x42\x02\x18\x01\x12\x1e\n\x12issuer_certificate\x18\x07 \x01(\x0c\x42\x02\x18\x01\x12\x1a\n\x12issuer_fingerprint\x18\x08 \x01(\x0c\x42\x15\n\x13one_identity_option\"L\n\x16LocalKillQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"+\n\rExecuteExport\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa2\x01\n\x15\x45xecuteExportResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x17\n\x0f\x65xportStatement\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"4\n\x16\x45xplainPipelineRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa6\x01\n\x17\x45xplainPipelineResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x19\n\x11pipelineStatement\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\".\n\x10\x43heckDataRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa1\x01\n\x11\x43heckDataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x1a\n\x12\x63heckDataStatement\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"*\n\x06SetPSO\x12\x11\n\tthreshold\x18\x01 \x01(\x03\x12\r\n\x05reset\x18\x02 \x01(\x08\"\x95\t\n\x0cSetParameter\x12\r\n\x05reset\x18\x01 \x01(\x08\x12\x35\n\rpso_threshold\x18\x02 \x01(\x0b\x32\x1c.xg.cmdcomp.SetParameter.PSOH\x00\x12\x36\n\trow_limit\x18\x03 \x01(\x0b\x32!.xg.cmdcomp.SetParameter.RowLimitH\x00\x12\x38\n\ntime_limit\x18\x04 \x01(\x0b\x32\".xg.cmdcomp.SetParameter.TimeLimitH\x00\x12\x44\n\x0ftemp_disk_limit\x18\x05 \x01(\x0b\x32).xg.cmdcomp.SetParameter.MaxTempDiskLimitH\x00\x12\x35\n\x08priority\x18\x06 \x01(\x0b\x32!.xg.cmdcomp.SetParameter.PriorityH\x00\x12;\n\x0b\x63oncurrency\x18\x07 \x01(\x0b\x32$.xg.cmdcomp.SetParameter.ConcurrencyH\x00\x12\x34\n\x08pso_seed\x18\x08 \x01(\x0b\x32 .xg.cmdcomp.SetParameter.PSOSeedH\x00\x12P\n\x17result_set_column_limit\x18\t \x01(\x0b\x32-.xg.cmdcomp.SetParameter.ResultSetColumnLimitH\x00\x12@\n\x0e\x66orce_external\x18\n \x01(\x0b\x32&.xg.cmdcomp.SetParameter.ForceExternalH\x00\x12O\n\x16priority_adjust_factor\x18\x0b \x01(\x0b\x32-.xg.cmdcomp.SetParameter.PriorityAdjustFactorH\x00\x12K\n\x14priority_adjust_time\x18\x0c \x01(\x0b\x32+.xg.cmdcomp.SetParameter.PriorityAdjustTimeH\x00\x1a\x18\n\x03PSO\x12\x11\n\tthreshold\x18\x01 \x01(\x03\x1a\x1c\n\x08RowLimit\x12\x10\n\x08rowLimit\x18\x01 \x01(\x03\x1a\x1e\n\tTimeLimit\x12\x11\n\ttimeLimit\x18\x01 \x01(\x03\x1a)\n\x10MaxTempDiskLimit\x12\x15\n\rtempDiskLimit\x18\x01 \x01(\x03\x1a\x34\n\x14ResultSetColumnLimit\x12\x1c\n\x14resultSetColumnLimit\x18\x01 \x01(\x03\x1a\x1c\n\x08Priority\x12\x10\n\x08priority\x18\x01 \x01(\x01\x1a\"\n\x0b\x43oncurrency\x12\x13\n\x0b\x63oncurrency\x18\x01 \x01(\x03\x1a\x17\n\x07PSOSeed\x12\x0c\n\x04seed\x18\x01 \x01(\x04\x1a\x1e\n\rForceExternal\x12\r\n\x05is_on\x18\x01 \x01(\x08\x1a\x36\n\x14PriorityAdjustFactor\x12\x1e\n\x16priority_adjust_factor\x18\x01 \x01(\x01\x1a\x32\n\x12PriorityAdjustTime\x12\x1c\n\x14priority_adjust_time\x18\x01 \x01(\rB\x0b\n\tParameter*/\n\rExplainFormat\x12\t\n\x05PROTO\x10\x00\x12\x08\n\x04JSON\x10\x01\x12\t\n\x05\x44\x45\x42UG\x10\x02\x62\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_wrappers__pb2.DESCRIPTOR,])
 
 _EXPLAINFORMAT = _descriptor.EnumDescriptor(
   name='ExplainFormat',
   full_name='xg.cmdcomp.ExplainFormat',
   filename=None,
@@ -46,16 +46,16 @@
       name='DEBUG', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=14654,
-  serialized_end=14701,
+  serialized_start=15421,
+  serialized_end=15468,
 )
 _sym_db.RegisterEnumDescriptor(_EXPLAINFORMAT)
 
 ExplainFormat = enum_type_wrapper.EnumTypeWrapper(_EXPLAINFORMAT)
 PROTO = 0
 JSON = 1
 DEBUG = 2
@@ -217,16 +217,16 @@
       name='REMOVE', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=7907,
-  serialized_end=7949,
+  serialized_start=8174,
+  serialized_end=8216,
 )
 _sym_db.RegisterEnumDescriptor(_CACHEENTRY_ACTION)
 
 _REQUEST_REQUESTTYPE = _descriptor.EnumDescriptor(
   name='RequestType',
   full_name='xg.cmdcomp.Request.RequestType',
   filename=None,
@@ -462,16 +462,16 @@
       name='CLIENT_CONNECTION_REFRESH_TOKEN', index=45, number=45,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=10797,
-  serialized_end=11858,
+  serialized_start=11064,
+  serialized_end=12125,
 )
 _sym_db.RegisterEnumDescriptor(_REQUEST_REQUESTTYPE)
 
 _CONFIRMATIONRESPONSE_RESPONSETYPE = _descriptor.EnumDescriptor(
   name='ResponseType',
   full_name='xg.cmdcomp.ConfirmationResponse.ResponseType',
   filename=None,
@@ -497,16 +497,16 @@
       name='RESPONSE_ERROR', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=12019,
-  serialized_end=12102,
+  serialized_start=12286,
+  serialized_end=12369,
 )
 _sym_db.RegisterEnumDescriptor(_CONFIRMATIONRESPONSE_RESPONSETYPE)
 
 
 _CLIENTCONNECTION = _descriptor.Descriptor(
   name='ClientConnection',
   full_name='xg.cmdcomp.ClientConnection',
@@ -3062,15 +3062,15 @@
       name='query_id', full_name='xg.cmdcomp.SysQueriesRow.query_id', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='importance', full_name='xg.cmdcomp.SysQueriesRow.importance', index=1,
+      name='effective_priority', full_name='xg.cmdcomp.SysQueriesRow.effective_priority', index=1,
       number=2, type=2, cpp_type=6, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
       name='estimated_time_sec', full_name='xg.cmdcomp.SysQueriesRow.estimated_time_sec', index=2,
@@ -3159,28 +3159,56 @@
     _descriptor.FieldDescriptor(
       name='sent_bytes', full_name='xg.cmdcomp.SysQueriesRow.sent_bytes', index=14,
       number=15, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='initial_priority', full_name='xg.cmdcomp.SysQueriesRow.initial_priority', index=15,
+      number=16, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='initial_effective_priority', full_name='xg.cmdcomp.SysQueriesRow.initial_effective_priority', index=16,
+      number=17, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='priority_adjust_factor', full_name='xg.cmdcomp.SysQueriesRow.priority_adjust_factor', index=17,
+      number=18, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='priority_adjust_time', full_name='xg.cmdcomp.SysQueriesRow.priority_adjust_time', index=18,
+      number=19, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=6619,
-  serialized_end=6958,
+  serialized_end=7090,
 )
 
 
 _SYSTEMWIDECOMPLETEDQUERIES = _descriptor.Descriptor(
   name='SystemWideCompletedQueries',
   full_name='xg.cmdcomp.SystemWideCompletedQueries',
   filename=None,
@@ -3196,16 +3224,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6960,
-  serialized_end=6988,
+  serialized_start=7092,
+  serialized_end=7120,
 )
 
 
 _COMPLETEDQUERIESRESPONSE = _descriptor.Descriptor(
   name='CompletedQueriesResponse',
   full_name='xg.cmdcomp.CompletedQueriesResponse',
   filename=None,
@@ -3235,16 +3263,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6990,
-  serialized_end=7115,
+  serialized_start=7122,
+  serialized_end=7247,
 )
 
 
 _COMPLETEDQUERIESROW = _descriptor.Descriptor(
   name='CompletedQueriesRow',
   full_name='xg.cmdcomp.CompletedQueriesRow',
   filename=None,
@@ -3354,15 +3382,15 @@
       name='uuid', full_name='xg.cmdcomp.CompletedQueriesRow.uuid', index=14,
       number=15, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='plan_priority', full_name='xg.cmdcomp.CompletedQueriesRow.plan_priority', index=15,
+      name='final_effective_priority', full_name='xg.cmdcomp.CompletedQueriesRow.final_effective_priority', index=15,
       number=16, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
       name='cost_estimate', full_name='xg.cmdcomp.CompletedQueriesRow.cost_estimate', index=16,
@@ -3416,28 +3444,56 @@
     _descriptor.FieldDescriptor(
       name='temp_disk_space_consumed', full_name='xg.cmdcomp.CompletedQueriesRow.temp_disk_space_consumed', index=23,
       number=24, type=4, cpp_type=4, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='priority_adjust_factor', full_name='xg.cmdcomp.CompletedQueriesRow.priority_adjust_factor', index=24,
+      number=25, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='priority_adjust_time', full_name='xg.cmdcomp.CompletedQueriesRow.priority_adjust_time', index=25,
+      number=26, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='initial_priority', full_name='xg.cmdcomp.CompletedQueriesRow.initial_priority', index=26,
+      number=27, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='initial_effective_priority', full_name='xg.cmdcomp.CompletedQueriesRow.initial_effective_priority', index=27,
+      number=28, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7118,
-  serialized_end=7687,
+  serialized_start=7250,
+  serialized_end=7954,
 )
 
 
 _LOADBROADCAST = _descriptor.Descriptor(
   name='LoadBroadcast',
   full_name='xg.cmdcomp.LoadBroadcast',
   filename=None,
@@ -3467,16 +3523,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7689,
-  serialized_end=7737,
+  serialized_start=7956,
+  serialized_end=8004,
 )
 
 
 _CACHEENTRY = _descriptor.Descriptor(
   name='CacheEntry',
   full_name='xg.cmdcomp.CacheEntry',
   filename=None,
@@ -3535,16 +3591,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7740,
-  serialized_end=7949,
+  serialized_start=8007,
+  serialized_end=8216,
 )
 
 
 _UPDATECACHE = _descriptor.Descriptor(
   name='UpdateCache',
   full_name='xg.cmdcomp.UpdateCache',
   filename=None,
@@ -3581,16 +3637,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7951,
-  serialized_end=8039,
+  serialized_start=8218,
+  serialized_end=8306,
 )
 
 
 _CLEARCACHE = _descriptor.Descriptor(
   name='ClearCache',
   full_name='xg.cmdcomp.ClearCache',
   filename=None,
@@ -3620,16 +3676,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8041,
-  serialized_end=8086,
+  serialized_start=8308,
+  serialized_end=8353,
 )
 
 
 _REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='xg.cmdcomp.Request',
   filename=None,
@@ -3973,16 +4029,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='request_oneof', full_name='xg.cmdcomp.Request.request_oneof',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=8089,
-  serialized_end=11875,
+  serialized_start=8356,
+  serialized_end=12142,
 )
 
 
 _CONFIRMATIONRESPONSE = _descriptor.Descriptor(
   name='ConfirmationResponse',
   full_name='xg.cmdcomp.ConfirmationResponse',
   filename=None,
@@ -4027,16 +4083,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11878,
-  serialized_end=12102,
+  serialized_start=12145,
+  serialized_end=12369,
 )
 
 
 _EXECUTEPLAN = _descriptor.Descriptor(
   name='ExecutePlan',
   full_name='xg.cmdcomp.ExecutePlan',
   filename=None,
@@ -4066,16 +4122,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12104,
-  serialized_end=12145,
+  serialized_start=12371,
+  serialized_end=12412,
 )
 
 
 _EXECUTEINLINEPLAN = _descriptor.Descriptor(
   name='ExecuteInlinePlan',
   full_name='xg.cmdcomp.ExecuteInlinePlan',
   filename=None,
@@ -4105,16 +4161,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12147,
-  serialized_end=12194,
+  serialized_start=12414,
+  serialized_end=12461,
 )
 
 
 _EXPLAINPLAN = _descriptor.Descriptor(
   name='ExplainPlan',
   full_name='xg.cmdcomp.ExplainPlan',
   filename=None,
@@ -4151,16 +4207,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12196,
-  serialized_end=12280,
+  serialized_start=12463,
+  serialized_end=12547,
 )
 
 
 _FORCEEXTERNAL = _descriptor.Descriptor(
   name='ForceExternal',
   full_name='xg.cmdcomp.ForceExternal',
   filename=None,
@@ -4183,16 +4239,16 @@
   ],
   serialized_options=b'\030\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12282,
-  serialized_end=12316,
+  serialized_start=12549,
+  serialized_end=12583,
 )
 
 
 _LISTPLAN = _descriptor.Descriptor(
   name='ListPlan',
   full_name='xg.cmdcomp.ListPlan',
   filename=None,
@@ -4208,16 +4264,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12318,
-  serialized_end=12328,
+  serialized_start=12585,
+  serialized_end=12595,
 )
 
 
 _LISTPLANRESPONSE = _descriptor.Descriptor(
   name='ListPlanResponse',
   full_name='xg.cmdcomp.ListPlanResponse',
   filename=None,
@@ -4268,16 +4324,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12331,
-  serialized_end=12481,
+  serialized_start=12598,
+  serialized_end=12748,
 )
 
 
 _CANCELQUERY = _descriptor.Descriptor(
   name='CancelQuery',
   full_name='xg.cmdcomp.CancelQuery',
   filename=None,
@@ -4300,16 +4356,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12483,
-  serialized_end=12509,
+  serialized_start=12750,
+  serialized_end=12776,
 )
 
 
 _CANCELQUERYRESPONSE = _descriptor.Descriptor(
   name='CancelQueryResponse',
   full_name='xg.cmdcomp.CancelQueryResponse',
   filename=None,
@@ -4332,16 +4388,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12511,
-  serialized_end=12584,
+  serialized_start=12778,
+  serialized_end=12851,
 )
 
 
 _LOCALCANCELQUERY = _descriptor.Descriptor(
   name='LocalCancelQuery',
   full_name='xg.cmdcomp.LocalCancelQuery',
   filename=None,
@@ -4418,16 +4474,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='one_identity_option', full_name='xg.cmdcomp.LocalCancelQuery.one_identity_option',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=12587,
-  serialized_end=12808,
+  serialized_start=12854,
+  serialized_end=13075,
 )
 
 
 _LOCALCANCELQUERYRESPONSE = _descriptor.Descriptor(
   name='LocalCancelQueryResponse',
   full_name='xg.cmdcomp.LocalCancelQueryResponse',
   filename=None,
@@ -4450,16 +4506,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12810,
-  serialized_end=12888,
+  serialized_start=13077,
+  serialized_end=13155,
 )
 
 
 _KILLQUERY = _descriptor.Descriptor(
   name='KillQuery',
   full_name='xg.cmdcomp.KillQuery',
   filename=None,
@@ -4482,16 +4538,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12890,
-  serialized_end=12914,
+  serialized_start=13157,
+  serialized_end=13181,
 )
 
 
 _KILLQUERYRESPONSE = _descriptor.Descriptor(
   name='KillQueryResponse',
   full_name='xg.cmdcomp.KillQueryResponse',
   filename=None,
@@ -4514,16 +4570,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12916,
-  serialized_end=12987,
+  serialized_start=13183,
+  serialized_end=13254,
 )
 
 
 _LOCALKILLQUERY = _descriptor.Descriptor(
   name='LocalKillQuery',
   full_name='xg.cmdcomp.LocalKillQuery',
   filename=None,
@@ -4600,16 +4656,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='one_identity_option', full_name='xg.cmdcomp.LocalKillQuery.one_identity_option',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=12990,
-  serialized_end=13209,
+  serialized_start=13257,
+  serialized_end=13476,
 )
 
 
 _LOCALKILLQUERYRESPONSE = _descriptor.Descriptor(
   name='LocalKillQueryResponse',
   full_name='xg.cmdcomp.LocalKillQueryResponse',
   filename=None,
@@ -4632,16 +4688,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13211,
-  serialized_end=13287,
+  serialized_start=13478,
+  serialized_end=13554,
 )
 
 
 _EXECUTEEXPORT = _descriptor.Descriptor(
   name='ExecuteExport',
   full_name='xg.cmdcomp.ExecuteExport',
   filename=None,
@@ -4652,28 +4708,35 @@
     _descriptor.FieldDescriptor(
       name='sql', full_name='xg.cmdcomp.ExecuteExport.sql', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='force', full_name='xg.cmdcomp.ExecuteExport.force', index=1,
+      number=2, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13289,
-  serialized_end=13317,
+  serialized_start=13556,
+  serialized_end=13599,
 )
 
 
 _EXECUTEEXPORTRESPONSE = _descriptor.Descriptor(
   name='ExecuteExportResponse',
   full_name='xg.cmdcomp.ExecuteExportResponse',
   filename=None,
@@ -4691,28 +4754,49 @@
     _descriptor.FieldDescriptor(
       name='exportStatement', full_name='xg.cmdcomp.ExecuteExportResponse.exportStatement', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='redirect', full_name='xg.cmdcomp.ExecuteExportResponse.redirect', index=2,
+      number=3, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='redirectHost', full_name='xg.cmdcomp.ExecuteExportResponse.redirectHost', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='redirectPort', full_name='xg.cmdcomp.ExecuteExportResponse.redirectPort', index=4,
+      number=5, type=7, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13319,
-  serialized_end=13419,
+  serialized_start=13602,
+  serialized_end=13764,
 )
 
 
 _EXPLAINPIPELINEREQUEST = _descriptor.Descriptor(
   name='ExplainPipelineRequest',
   full_name='xg.cmdcomp.ExplainPipelineRequest',
   filename=None,
@@ -4723,28 +4807,35 @@
     _descriptor.FieldDescriptor(
       name='sql', full_name='xg.cmdcomp.ExplainPipelineRequest.sql', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='force', full_name='xg.cmdcomp.ExplainPipelineRequest.force', index=1,
+      number=2, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13421,
-  serialized_end=13458,
+  serialized_start=13766,
+  serialized_end=13818,
 )
 
 
 _EXPLAINPIPELINERESPONSE = _descriptor.Descriptor(
   name='ExplainPipelineResponse',
   full_name='xg.cmdcomp.ExplainPipelineResponse',
   filename=None,
@@ -4762,28 +4853,49 @@
     _descriptor.FieldDescriptor(
       name='pipelineStatement', full_name='xg.cmdcomp.ExplainPipelineResponse.pipelineStatement', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='redirect', full_name='xg.cmdcomp.ExplainPipelineResponse.redirect', index=2,
+      number=3, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='redirectHost', full_name='xg.cmdcomp.ExplainPipelineResponse.redirectHost', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='redirectPort', full_name='xg.cmdcomp.ExplainPipelineResponse.redirectPort', index=4,
+      number=5, type=7, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13460,
-  serialized_end=13564,
+  serialized_start=13821,
+  serialized_end=13987,
 )
 
 
 _CHECKDATAREQUEST = _descriptor.Descriptor(
   name='CheckDataRequest',
   full_name='xg.cmdcomp.CheckDataRequest',
   filename=None,
@@ -4794,28 +4906,35 @@
     _descriptor.FieldDescriptor(
       name='sql', full_name='xg.cmdcomp.CheckDataRequest.sql', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='force', full_name='xg.cmdcomp.CheckDataRequest.force', index=1,
+      number=2, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13566,
-  serialized_end=13597,
+  serialized_start=13989,
+  serialized_end=14035,
 )
 
 
 _CHECKDATARESPONSE = _descriptor.Descriptor(
   name='CheckDataResponse',
   full_name='xg.cmdcomp.CheckDataResponse',
   filename=None,
@@ -4833,28 +4952,49 @@
     _descriptor.FieldDescriptor(
       name='checkDataStatement', full_name='xg.cmdcomp.CheckDataResponse.checkDataStatement', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='redirect', full_name='xg.cmdcomp.CheckDataResponse.redirect', index=2,
+      number=3, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='redirectHost', full_name='xg.cmdcomp.CheckDataResponse.redirectHost', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='redirectPort', full_name='xg.cmdcomp.CheckDataResponse.redirectPort', index=4,
+      number=5, type=7, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13599,
-  serialized_end=13698,
+  serialized_start=14038,
+  serialized_end=14199,
 )
 
 
 _SETPSO = _descriptor.Descriptor(
   name='SetPSO',
   full_name='xg.cmdcomp.SetPSO',
   filename=None,
@@ -4884,16 +5024,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13700,
-  serialized_end=13742,
+  serialized_start=14201,
+  serialized_end=14243,
 )
 
 
 _SETPARAMETER_PSO = _descriptor.Descriptor(
   name='PSO',
   full_name='xg.cmdcomp.SetParameter.PSO',
   filename=None,
@@ -4916,16 +5056,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14333,
-  serialized_end=14357,
+  serialized_start=14992,
+  serialized_end=15016,
 )
 
 _SETPARAMETER_ROWLIMIT = _descriptor.Descriptor(
   name='RowLimit',
   full_name='xg.cmdcomp.SetParameter.RowLimit',
   filename=None,
   file=DESCRIPTOR,
@@ -4947,16 +5087,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14359,
-  serialized_end=14387,
+  serialized_start=15018,
+  serialized_end=15046,
 )
 
 _SETPARAMETER_TIMELIMIT = _descriptor.Descriptor(
   name='TimeLimit',
   full_name='xg.cmdcomp.SetParameter.TimeLimit',
   filename=None,
   file=DESCRIPTOR,
@@ -4978,16 +5118,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14389,
-  serialized_end=14419,
+  serialized_start=15048,
+  serialized_end=15078,
 )
 
 _SETPARAMETER_MAXTEMPDISKLIMIT = _descriptor.Descriptor(
   name='MaxTempDiskLimit',
   full_name='xg.cmdcomp.SetParameter.MaxTempDiskLimit',
   filename=None,
   file=DESCRIPTOR,
@@ -5009,16 +5149,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14421,
-  serialized_end=14462,
+  serialized_start=15080,
+  serialized_end=15121,
 )
 
 _SETPARAMETER_RESULTSETCOLUMNLIMIT = _descriptor.Descriptor(
   name='ResultSetColumnLimit',
   full_name='xg.cmdcomp.SetParameter.ResultSetColumnLimit',
   filename=None,
   file=DESCRIPTOR,
@@ -5040,16 +5180,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14464,
-  serialized_end=14516,
+  serialized_start=15123,
+  serialized_end=15175,
 )
 
 _SETPARAMETER_PRIORITY = _descriptor.Descriptor(
   name='Priority',
   full_name='xg.cmdcomp.SetParameter.Priority',
   filename=None,
   file=DESCRIPTOR,
@@ -5071,16 +5211,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14518,
-  serialized_end=14546,
+  serialized_start=15177,
+  serialized_end=15205,
 )
 
 _SETPARAMETER_CONCURRENCY = _descriptor.Descriptor(
   name='Concurrency',
   full_name='xg.cmdcomp.SetParameter.Concurrency',
   filename=None,
   file=DESCRIPTOR,
@@ -5102,16 +5242,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14548,
-  serialized_end=14582,
+  serialized_start=15207,
+  serialized_end=15241,
 )
 
 _SETPARAMETER_PSOSEED = _descriptor.Descriptor(
   name='PSOSeed',
   full_name='xg.cmdcomp.SetParameter.PSOSeed',
   filename=None,
   file=DESCRIPTOR,
@@ -5133,16 +5273,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14584,
-  serialized_end=14607,
+  serialized_start=15243,
+  serialized_end=15266,
 )
 
 _SETPARAMETER_FORCEEXTERNAL = _descriptor.Descriptor(
   name='ForceExternal',
   full_name='xg.cmdcomp.SetParameter.ForceExternal',
   filename=None,
   file=DESCRIPTOR,
@@ -5164,16 +5304,78 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14609,
-  serialized_end=14639,
+  serialized_start=15268,
+  serialized_end=15298,
+)
+
+_SETPARAMETER_PRIORITYADJUSTFACTOR = _descriptor.Descriptor(
+  name='PriorityAdjustFactor',
+  full_name='xg.cmdcomp.SetParameter.PriorityAdjustFactor',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='priority_adjust_factor', full_name='xg.cmdcomp.SetParameter.PriorityAdjustFactor.priority_adjust_factor', index=0,
+      number=1, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=15300,
+  serialized_end=15354,
+)
+
+_SETPARAMETER_PRIORITYADJUSTTIME = _descriptor.Descriptor(
+  name='PriorityAdjustTime',
+  full_name='xg.cmdcomp.SetParameter.PriorityAdjustTime',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='priority_adjust_time', full_name='xg.cmdcomp.SetParameter.PriorityAdjustTime.priority_adjust_time', index=0,
+      number=1, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=15356,
+  serialized_end=15406,
 )
 
 _SETPARAMETER = _descriptor.Descriptor(
   name='SetParameter',
   full_name='xg.cmdcomp.SetParameter',
   filename=None,
   file=DESCRIPTOR,
@@ -5246,33 +5448,47 @@
     _descriptor.FieldDescriptor(
       name='force_external', full_name='xg.cmdcomp.SetParameter.force_external', index=9,
       number=10, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='priority_adjust_factor', full_name='xg.cmdcomp.SetParameter.priority_adjust_factor', index=10,
+      number=11, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='priority_adjust_time', full_name='xg.cmdcomp.SetParameter.priority_adjust_time', index=11,
+      number=12, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_SETPARAMETER_PSO, _SETPARAMETER_ROWLIMIT, _SETPARAMETER_TIMELIMIT, _SETPARAMETER_MAXTEMPDISKLIMIT, _SETPARAMETER_RESULTSETCOLUMNLIMIT, _SETPARAMETER_PRIORITY, _SETPARAMETER_CONCURRENCY, _SETPARAMETER_PSOSEED, _SETPARAMETER_FORCEEXTERNAL, ],
+  nested_types=[_SETPARAMETER_PSO, _SETPARAMETER_ROWLIMIT, _SETPARAMETER_TIMELIMIT, _SETPARAMETER_MAXTEMPDISKLIMIT, _SETPARAMETER_RESULTSETCOLUMNLIMIT, _SETPARAMETER_PRIORITY, _SETPARAMETER_CONCURRENCY, _SETPARAMETER_PSOSEED, _SETPARAMETER_FORCEEXTERNAL, _SETPARAMETER_PRIORITYADJUSTFACTOR, _SETPARAMETER_PRIORITYADJUSTTIME, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='Parameter', full_name='xg.cmdcomp.SetParameter.Parameter',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=13745,
-  serialized_end=14652,
+  serialized_start=14246,
+  serialized_end=15419,
 )
 
 _CLIENTCONNECTIONRESPONSE.fields_by_name['response'].message_type = _CONFIRMATIONRESPONSE
 _CLIENTCONNECTIONGCMRESPONSE.fields_by_name['response'].message_type = _CONFIRMATIONRESPONSE
 _CLIENTCONNECTIONSSORESPONSE.fields_by_name['response'].message_type = _CONFIRMATIONRESPONSE
 _CLIENTCONNECTIONSECURITYTOKENRESPONSE.fields_by_name['response'].message_type = _CONFIRMATIONRESPONSE
 _CLIENTCONNECTIONSECURITYTOKENRESPONSE.fields_by_name['secondary'].message_type = _SECONDARYINTERFACELIST
@@ -5542,23 +5758,27 @@
 _SETPARAMETER_TIMELIMIT.containing_type = _SETPARAMETER
 _SETPARAMETER_MAXTEMPDISKLIMIT.containing_type = _SETPARAMETER
 _SETPARAMETER_RESULTSETCOLUMNLIMIT.containing_type = _SETPARAMETER
 _SETPARAMETER_PRIORITY.containing_type = _SETPARAMETER
 _SETPARAMETER_CONCURRENCY.containing_type = _SETPARAMETER
 _SETPARAMETER_PSOSEED.containing_type = _SETPARAMETER
 _SETPARAMETER_FORCEEXTERNAL.containing_type = _SETPARAMETER
+_SETPARAMETER_PRIORITYADJUSTFACTOR.containing_type = _SETPARAMETER
+_SETPARAMETER_PRIORITYADJUSTTIME.containing_type = _SETPARAMETER
 _SETPARAMETER.fields_by_name['pso_threshold'].message_type = _SETPARAMETER_PSO
 _SETPARAMETER.fields_by_name['row_limit'].message_type = _SETPARAMETER_ROWLIMIT
 _SETPARAMETER.fields_by_name['time_limit'].message_type = _SETPARAMETER_TIMELIMIT
 _SETPARAMETER.fields_by_name['temp_disk_limit'].message_type = _SETPARAMETER_MAXTEMPDISKLIMIT
 _SETPARAMETER.fields_by_name['priority'].message_type = _SETPARAMETER_PRIORITY
 _SETPARAMETER.fields_by_name['concurrency'].message_type = _SETPARAMETER_CONCURRENCY
 _SETPARAMETER.fields_by_name['pso_seed'].message_type = _SETPARAMETER_PSOSEED
 _SETPARAMETER.fields_by_name['result_set_column_limit'].message_type = _SETPARAMETER_RESULTSETCOLUMNLIMIT
 _SETPARAMETER.fields_by_name['force_external'].message_type = _SETPARAMETER_FORCEEXTERNAL
+_SETPARAMETER.fields_by_name['priority_adjust_factor'].message_type = _SETPARAMETER_PRIORITYADJUSTFACTOR
+_SETPARAMETER.fields_by_name['priority_adjust_time'].message_type = _SETPARAMETER_PRIORITYADJUSTTIME
 _SETPARAMETER.oneofs_by_name['Parameter'].fields.append(
   _SETPARAMETER.fields_by_name['pso_threshold'])
 _SETPARAMETER.fields_by_name['pso_threshold'].containing_oneof = _SETPARAMETER.oneofs_by_name['Parameter']
 _SETPARAMETER.oneofs_by_name['Parameter'].fields.append(
   _SETPARAMETER.fields_by_name['row_limit'])
 _SETPARAMETER.fields_by_name['row_limit'].containing_oneof = _SETPARAMETER.oneofs_by_name['Parameter']
 _SETPARAMETER.oneofs_by_name['Parameter'].fields.append(
@@ -5578,14 +5798,20 @@
 _SETPARAMETER.fields_by_name['pso_seed'].containing_oneof = _SETPARAMETER.oneofs_by_name['Parameter']
 _SETPARAMETER.oneofs_by_name['Parameter'].fields.append(
   _SETPARAMETER.fields_by_name['result_set_column_limit'])
 _SETPARAMETER.fields_by_name['result_set_column_limit'].containing_oneof = _SETPARAMETER.oneofs_by_name['Parameter']
 _SETPARAMETER.oneofs_by_name['Parameter'].fields.append(
   _SETPARAMETER.fields_by_name['force_external'])
 _SETPARAMETER.fields_by_name['force_external'].containing_oneof = _SETPARAMETER.oneofs_by_name['Parameter']
+_SETPARAMETER.oneofs_by_name['Parameter'].fields.append(
+  _SETPARAMETER.fields_by_name['priority_adjust_factor'])
+_SETPARAMETER.fields_by_name['priority_adjust_factor'].containing_oneof = _SETPARAMETER.oneofs_by_name['Parameter']
+_SETPARAMETER.oneofs_by_name['Parameter'].fields.append(
+  _SETPARAMETER.fields_by_name['priority_adjust_time'])
+_SETPARAMETER.fields_by_name['priority_adjust_time'].containing_oneof = _SETPARAMETER.oneofs_by_name['Parameter']
 DESCRIPTOR.message_types_by_name['ClientConnection'] = _CLIENTCONNECTION
 DESCRIPTOR.message_types_by_name['ClientConnectionGCM'] = _CLIENTCONNECTIONGCM
 DESCRIPTOR.message_types_by_name['ClientConnectionSSO'] = _CLIENTCONNECTIONSSO
 DESCRIPTOR.message_types_by_name['ClientConnectionSecurityToken'] = _CLIENTCONNECTIONSECURITYTOKEN
 DESCRIPTOR.message_types_by_name['ClientConnectionResponse'] = _CLIENTCONNECTIONRESPONSE
 DESCRIPTOR.message_types_by_name['ClientConnectionGCMResponse'] = _CLIENTCONNECTIONGCMRESPONSE
 DESCRIPTOR.message_types_by_name['ClientConnectionSSOResponse'] = _CLIENTCONNECTIONSSORESPONSE
@@ -6318,28 +6544,44 @@
 
   'ForceExternal' : _reflection.GeneratedProtocolMessageType('ForceExternal', (_message.Message,), {
     'DESCRIPTOR' : _SETPARAMETER_FORCEEXTERNAL,
     '__module__' : 'sharedMessages.clientWireProtocol_pb2'
     # @@protoc_insertion_point(class_scope:xg.cmdcomp.SetParameter.ForceExternal)
     })
   ,
+
+  'PriorityAdjustFactor' : _reflection.GeneratedProtocolMessageType('PriorityAdjustFactor', (_message.Message,), {
+    'DESCRIPTOR' : _SETPARAMETER_PRIORITYADJUSTFACTOR,
+    '__module__' : 'sharedMessages.clientWireProtocol_pb2'
+    # @@protoc_insertion_point(class_scope:xg.cmdcomp.SetParameter.PriorityAdjustFactor)
+    })
+  ,
+
+  'PriorityAdjustTime' : _reflection.GeneratedProtocolMessageType('PriorityAdjustTime', (_message.Message,), {
+    'DESCRIPTOR' : _SETPARAMETER_PRIORITYADJUSTTIME,
+    '__module__' : 'sharedMessages.clientWireProtocol_pb2'
+    # @@protoc_insertion_point(class_scope:xg.cmdcomp.SetParameter.PriorityAdjustTime)
+    })
+  ,
   'DESCRIPTOR' : _SETPARAMETER,
   '__module__' : 'sharedMessages.clientWireProtocol_pb2'
   # @@protoc_insertion_point(class_scope:xg.cmdcomp.SetParameter)
   })
 _sym_db.RegisterMessage(SetParameter)
 _sym_db.RegisterMessage(SetParameter.PSO)
 _sym_db.RegisterMessage(SetParameter.RowLimit)
 _sym_db.RegisterMessage(SetParameter.TimeLimit)
 _sym_db.RegisterMessage(SetParameter.MaxTempDiskLimit)
 _sym_db.RegisterMessage(SetParameter.ResultSetColumnLimit)
 _sym_db.RegisterMessage(SetParameter.Priority)
 _sym_db.RegisterMessage(SetParameter.Concurrency)
 _sym_db.RegisterMessage(SetParameter.PSOSeed)
 _sym_db.RegisterMessage(SetParameter.ForceExternal)
+_sym_db.RegisterMessage(SetParameter.PriorityAdjustFactor)
+_sym_db.RegisterMessage(SetParameter.PriorityAdjustTime)
 
 
 _FETCHMETADATARESPONSE_COLS2POSENTRY._options = None
 _FETCHMETADATARESPONSE_COLS2TYPESENTRY._options = None
 _BROADCASTQUERYCONCURRENCY_SERVICECLASSIDTOCOUNTSENTRY._options = None
 _LOCALQUERIES.fields_by_name['identity']._options = None
 _LOCALQUERIES.fields_by_name['uuid_identity']._options = None
```

### Comparing `pyocient-1.0.7/LICENSE.txt` & `pyocient-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyocient-1.0.7/PKG-INFO` & `pyocient-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyocient
-Version: 1.0.7
+Version: 1.0.9
 Summary: Ocient Database Python API
 Home-page: https://www.ocient.com/
 Author: Ocient Inc
 Author-email: info@ocient.com
 License: UNKNOWN
 Description: # Ocient Database Python API
```

### Comparing `pyocient-1.0.7/README.md` & `pyocient-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyocient-1.0.7/pyocient.egg-info/PKG-INFO` & `pyocient-1.0.9/pyocient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyocient
-Version: 1.0.7
+Version: 1.0.9
 Summary: Ocient Database Python API
 Home-page: https://www.ocient.com/
 Author: Ocient Inc
 Author-email: info@ocient.com
 License: UNKNOWN
 Description: # Ocient Database Python API
```

### Comparing `pyocient-1.0.7/pyocient.py` & `pyocient-1.0.9/pyocient.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,6077 +425,6293 @@
 00001a80: 6c69 6620 7063 6c61 7373 203d 3d20 4f70  lif pclass == Op
 00001a90: 7469 6f6e 616c 5b75 7569 642e 5555 4944  tional[uuid.UUID
 00001aa0: 5d3a 0a20 2020 2020 2020 2020 2020 2072  ]:.            r
 00001ab0: 6574 7572 6e20 636c 732e 5555 4944 0a20  eturn cls.UUID. 
 00001ac0: 2020 2020 2020 2072 6169 7365 2045 7272         raise Err
 00001ad0: 6f72 2866 2255 6e6b 6e6f 776e 2063 6f6c  or(f"Unknown col
 00001ae0: 756d 6e20 636c 6173 7320 7b70 636c 6173  umn class {pclas
-00001af0: 737d 2229 0a0a 0a23 2323 2323 2323 2323  s}")...#########
-00001b00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b40: 0a23 2044 6174 6162 6173 6520 4150 4920  .# Database API 
-00001b50: 322e 3020 7479 7065 732e 2020 5468 6573  2.0 types.  Thes
-00001b60: 6520 6172 6520 7265 7175 6972 6564 2062  e are required b
-00001b70: 7920 5045 4d20 3234 390a 2323 2323 2323  y PEM 249.######
-00001b80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001ba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001bb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001bc0: 2323 230a 4269 6e61 7279 203d 2062 7974  ###.Binary = byt
-00001bd0: 6573 2020 2320 3a20 3a6d 6574 6120 7072  es  # : :meta pr
-00001be0: 6976 6174 653a 0a53 5452 494e 4720 3d20  ivate:.STRING = 
-00001bf0: 5479 7065 436f 6465 732e 5354 5249 4e47  TypeCodes.STRING
-00001c00: 2020 2320 3a20 3a6d 6574 6120 7072 6976    # : :meta priv
-00001c10: 6174 653a 0a42 494e 4152 5920 3d20 5479  ate:.BINARY = Ty
-00001c20: 7065 436f 6465 732e 4249 4e41 5259 2020  peCodes.BINARY  
-00001c30: 2320 3a20 3a6d 6574 6120 7072 6976 6174  # : :meta privat
-00001c40: 653a 0a4e 554d 4245 5220 3d20 5479 7065  e:.NUMBER = Type
-00001c50: 436f 6465 732e 494e 5420 2023 203a 203a  Codes.INT  # : :
-00001c60: 6d65 7461 2070 7269 7661 7465 3a0a 4441  meta private:.DA
-00001c70: 5445 5449 4d45 203d 2054 7970 6543 6f64  TETIME = TypeCod
-00001c80: 6573 2e54 494d 4553 5441 4d50 2020 2320  es.TIMESTAMP  # 
-00001c90: 3a20 3a6d 6574 6120 7072 6976 6174 653a  : :meta private:
-00001ca0: 0a52 4f57 4944 203d 2054 7970 6543 6f64  .ROWID = TypeCod
-00001cb0: 6573 2e49 4e54 2020 2320 3a20 3a6d 6574  es.INT  # : :met
-00001cc0: 6120 7072 6976 6174 653a 0a0a 2323 2323  a private:..####
-00001cd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001ce0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001cf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001d00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001d10: 2323 2323 230a 2320 496d 706f 7274 206f  #####.# Import o
-00001d20: 7572 2067 6f6f 676c 6520 7072 6f74 6f62  ur google protob
-00001d30: 7566 206d 6573 7361 6765 2064 6566 696e  uf message defin
-00001d40: 6974 696f 6e73 0a23 2057 6520 6173 7375  itions.# We assu
-00001d50: 6d65 2074 6861 7420 7468 6520 436c 6965  me that the Clie
-00001d60: 6e74 5769 7265 5072 6f74 6f63 6f6c 5f70  ntWireProtocol_p
-00001d70: 622e 7079 2066 696c 6520 6973 2069 6e20  b.py file is in 
-00001d80: 7468 6520 7361 6d65 2064 6972 6563 746f  the same directo
-00001d90: 7279 0a23 2061 7320 7468 6973 2066 696c  ry.# as this fil
-00001da0: 650a 2323 2323 2323 2323 2323 2323 2323  e.##############
-00001db0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001dc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001dd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001de0: 2323 2323 2323 2323 2323 230a 7379 732e  ###########.sys.
-00001df0: 7061 7468 2e61 7070 656e 6428 6f73 2e70  path.append(os.p
-00001e00: 6174 682e 6162 7370 6174 6828 6f73 2e70  ath.abspath(os.p
-00001e10: 6174 682e 6469 726e 616d 6528 225f 5f66  ath.dirname("__f
-00001e20: 696c 655f 5f22 2929 290a 0a23 2054 7279  ile__")))..# Try
-00001e30: 2061 6e64 2069 6d70 6f72 7420 6f75 7420   and import out 
-00001e40: 7072 6f74 6f62 7566 2064 6566 696e 6974  protobuf definit
-00001e50: 696f 6e73 2e0a 2320 5768 696c 6520 7765  ions..# While we
-00001e60: 2074 7261 6e73 6974 696f 6e20 746f 2062   transition to b
-00001e70: 617a 656c 2077 6520 7761 6e74 2074 6f20  azel we want to 
-00001e80: 7375 7070 6f72 7420 626f 7468 2074 6865  support both the
-00001e90: 206d 616b 6566 696c 6520 7761 7920 616e   makefile way an
-00001ea0: 6420 7468 6520 6e65 7720 7761 7920 2844  d the new way (D
-00001eb0: 422d 3133 3934 3729 0a74 7279 3a0a 2020  B-13947).try:.  
-00001ec0: 2020 696d 706f 7274 2043 6c69 656e 7457    import ClientW
-00001ed0: 6972 6550 726f 746f 636f 6c5f 7062 3220  ireProtocol_pb2 
-00001ee0: 6173 2070 726f 746f 2020 2320 7079 6c69  as proto  # pyli
-00001ef0: 6e74 3a20 6469 7361 626c 653d 696d 706f  nt: disable=impo
-00001f00: 7274 2d65 7272 6f72 2c77 726f 6e67 2d69  rt-error,wrong-i
-00001f10: 6d70 6f72 742d 706f 7369 7469 6f6e 0a65  mport-position.e
-00001f20: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
-00001f30: 7220 6173 2065 7863 3a0a 2020 2020 6672  r as exc:.    fr
-00001f40: 6f6d 2073 6861 7265 644d 6573 7361 6765  om sharedMessage
-00001f50: 7320 696d 706f 7274 2063 6c69 656e 7457  s import clientW
-00001f60: 6972 6550 726f 746f 636f 6c5f 7062 3220  ireProtocol_pb2 
-00001f70: 6173 2070 726f 746f 2020 2320 7079 6c69  as proto  # pyli
-00001f80: 6e74 3a20 6469 7361 626c 653d 696d 706f  nt: disable=impo
-00001f90: 7274 2d65 7272 6f72 2c77 726f 6e67 2d69  rt-error,wrong-i
-00001fa0: 6d70 6f72 742d 706f 7369 7469 6f6e 0a0a  mport-position..
-00001fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001fc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001fd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001fe0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001ff0: 2323 2323 2323 2323 230a 2320 4275 696c  #########.# Buil
-00002000: 6420 7375 7070 6f72 7465 6420 7265 7175  d supported requ
-00002010: 6573 742f 7265 7370 6f6e 7365 2074 7970  est/response typ
-00002020: 6520 6d61 7070 696e 6773 0a23 2323 2323  e mappings.#####
+00001af0: 737d 2229 0a0a 0a23 2042 7920 696e 7374  s}")...# By inst
+00001b00: 616e 7469 6174 696e 6720 7468 6573 6520  antiating these 
+00001b10: 6865 7265 2077 6520 7265 6475 6365 2074  here we reduce t
+00001b20: 6865 206f 7665 7268 6561 6420 6f66 2073  he overhead of s
+00001b30: 6574 7469 6e67 2074 6869 7320 7570 0a23  etting this up.#
+00001b40: 2065 6163 6820 7469 6d65 2077 6520 6361   each time we ca
+00001b50: 6c6c 2069 740a 5f75 6e70 6163 6b5f 7368  ll it._unpack_sh
+00001b60: 6f72 7420 3d20 7374 7275 6374 2e53 7472  ort = struct.Str
+00001b70: 7563 7428 2221 6822 292e 756e 7061 636b  uct("!h").unpack
+00001b80: 5f66 726f 6d0a 5f75 6e70 6163 6b5f 696e  _from._unpack_in
+00001b90: 7420 3d20 7374 7275 6374 2e53 7472 7563  t = struct.Struc
+00001ba0: 7428 2221 6922 292e 756e 7061 636b 5f66  t("!i").unpack_f
+00001bb0: 726f 6d0a 5f75 6e70 6163 6b5f 6c6f 6e67  rom._unpack_long
+00001bc0: 203d 2073 7472 7563 742e 5374 7275 6374   = struct.Struct
+00001bd0: 2822 2171 2229 2e75 6e70 6163 6b5f 6672  ("!q").unpack_fr
+00001be0: 6f6d 0a5f 756e 7061 636b 5f66 6c6f 6174  om._unpack_float
+00001bf0: 203d 2073 7472 7563 742e 5374 7275 6374   = struct.Struct
+00001c00: 2822 2166 2229 2e75 6e70 6163 6b5f 6672  ("!f").unpack_fr
+00001c10: 6f6d 0a5f 756e 7061 636b 5f64 6f75 626c  om._unpack_doubl
+00001c20: 6520 3d20 7374 7275 6374 2e53 7472 7563  e = struct.Struc
+00001c30: 7428 2221 6422 292e 756e 7061 636b 5f66  t("!d").unpack_f
+00001c40: 726f 6d0a 5f75 6e70 6163 6b5f 626f 6f6c  rom._unpack_bool
+00001c50: 203d 2073 7472 7563 742e 5374 7275 6374   = struct.Struct
+00001c60: 2822 3f22 292e 756e 7061 636b 5f66 726f  ("?").unpack_fro
+00001c70: 6d0a 5f75 6e70 6163 6b5f 6368 6172 203d  m._unpack_char =
+00001c80: 2073 7472 7563 742e 5374 7275 6374 2822   struct.Struct("
+00001c90: 6322 292e 756e 7061 636b 5f66 726f 6d0a  c").unpack_from.
+00001ca0: 0a23 2065 6173 7920 636f 6e76 6572 7369  .# easy conversi
+00001cb0: 6f6e 7320 7765 2063 616e 2064 6f20 7769  ons we can do wi
+00001cc0: 7468 2073 7472 7563 7473 0a5f 7479 7065  th structs._type
+00001cd0: 5f6d 6170 203d 207b 0a20 2020 2054 7970  _map = {.    Typ
+00001ce0: 6543 6f64 6573 2e49 4e54 3a20 2873 7472  eCodes.INT: (str
+00001cf0: 7563 742e 6361 6c63 7369 7a65 2822 2169  uct.calcsize("!i
+00001d00: 2229 2c20 5f75 6e70 6163 6b5f 696e 7429  "), _unpack_int)
+00001d10: 2c0a 2020 2020 5479 7065 436f 6465 732e  ,.    TypeCodes.
+00001d20: 4c4f 4e47 3a20 2873 7472 7563 742e 6361  LONG: (struct.ca
+00001d30: 6c63 7369 7a65 2822 2171 2229 2c20 5f75  lcsize("!q"), _u
+00001d40: 6e70 6163 6b5f 6c6f 6e67 292c 0a20 2020  npack_long),.   
+00001d50: 2054 7970 6543 6f64 6573 2e46 4c4f 4154   TypeCodes.FLOAT
+00001d60: 3a20 2873 7472 7563 742e 6361 6c63 7369  : (struct.calcsi
+00001d70: 7a65 2822 2166 2229 2c20 5f75 6e70 6163  ze("!f"), _unpac
+00001d80: 6b5f 666c 6f61 7429 2c0a 2020 2020 5479  k_float),.    Ty
+00001d90: 7065 436f 6465 732e 444f 5542 4c45 3a20  peCodes.DOUBLE: 
+00001da0: 2873 7472 7563 742e 6361 6c63 7369 7a65  (struct.calcsize
+00001db0: 2822 2164 2229 2c20 5f75 6e70 6163 6b5f  ("!d"), _unpack_
+00001dc0: 646f 7562 6c65 292c 0a20 2020 2054 7970  double),.    Typ
+00001dd0: 6543 6f64 6573 2e42 4f4f 4c45 414e 3a20  eCodes.BOOLEAN: 
+00001de0: 2873 7472 7563 742e 6361 6c63 7369 7a65  (struct.calcsize
+00001df0: 2822 3f22 292c 205f 756e 7061 636b 5f62  ("?"), _unpack_b
+00001e00: 6f6f 6c29 2c0a 2020 2020 5479 7065 436f  ool),.    TypeCo
+00001e10: 6465 732e 5348 4f52 543a 2028 7374 7275  des.SHORT: (stru
+00001e20: 6374 2e63 616c 6373 697a 6528 2221 6822  ct.calcsize("!h"
+00001e30: 292c 205f 756e 7061 636b 5f73 686f 7274  ), _unpack_short
+00001e40: 292c 0a7d 0a0a 0a23 2323 2323 2323 2323  ),.}...#########
+00001e50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001e60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001e70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001e80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001e90: 0a23 2044 6174 6162 6173 6520 4150 4920  .# Database API 
+00001ea0: 322e 3020 7479 7065 732e 2020 5468 6573  2.0 types.  Thes
+00001eb0: 6520 6172 6520 7265 7175 6972 6564 2062  e are required b
+00001ec0: 7920 5045 4d20 3234 390a 2323 2323 2323  y PEM 249.######
+00001ed0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001f10: 2323 230a 4269 6e61 7279 203d 2062 7974  ###.Binary = byt
+00001f20: 6573 2020 2320 3a20 3a6d 6574 6120 7072  es  # : :meta pr
+00001f30: 6976 6174 653a 0a53 5452 494e 4720 3d20  ivate:.STRING = 
+00001f40: 5479 7065 436f 6465 732e 5354 5249 4e47  TypeCodes.STRING
+00001f50: 2020 2320 3a20 3a6d 6574 6120 7072 6976    # : :meta priv
+00001f60: 6174 653a 0a42 494e 4152 5920 3d20 5479  ate:.BINARY = Ty
+00001f70: 7065 436f 6465 732e 4249 4e41 5259 2020  peCodes.BINARY  
+00001f80: 2320 3a20 3a6d 6574 6120 7072 6976 6174  # : :meta privat
+00001f90: 653a 0a4e 554d 4245 5220 3d20 5479 7065  e:.NUMBER = Type
+00001fa0: 436f 6465 732e 494e 5420 2023 203a 203a  Codes.INT  # : :
+00001fb0: 6d65 7461 2070 7269 7661 7465 3a0a 4441  meta private:.DA
+00001fc0: 5445 5449 4d45 203d 2054 7970 6543 6f64  TETIME = TypeCod
+00001fd0: 6573 2e54 494d 4553 5441 4d50 2020 2320  es.TIMESTAMP  # 
+00001fe0: 3a20 3a6d 6574 6120 7072 6976 6174 653a  : :meta private:
+00001ff0: 0a52 4f57 4944 203d 2054 7970 6543 6f64  .ROWID = TypeCod
+00002000: 6573 2e49 4e54 2020 2320 3a20 3a6d 6574  es.INT  # : :met
+00002010: 6120 7072 6976 6174 653a 0a0a 2323 2323  a private:..####
+00002020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00002030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00002040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00002050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002060: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002070: 2323 2323 0a0a 0a63 6c61 7373 205f 4f63  ####...class _Oc
-00002080: 6965 6e74 5265 7175 6573 7446 6163 746f  ientRequestFacto
-00002090: 7279 3a0a 2020 2020 6465 6620 7265 7175  ry:.    def requ
-000020a0: 6573 7428 7365 6c66 2c20 6f70 6572 6174  est(self, operat
-000020b0: 696f 6e3a 2073 7472 293a 0a20 2020 2020  ion: str):.     
-000020c0: 2020 2022 2222 4765 6e65 7261 7465 7320     """Generates 
-000020d0: 6120 6675 6c6c 7920 706f 7075 6c61 7465  a fully populate
-000020e0: 6420 7265 7175 6573 7420 7072 6f74 6f62  d request protob
-000020f0: 7566 2222 220a 2020 2020 2020 2020 7261  uf""".        ra
-00002100: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
-00002110: 6564 4572 726f 720a 0a20 2020 2064 6566  edError..    def
-00002120: 2072 6573 706f 6e73 6528 7365 6c66 293a   response(self):
-00002130: 0a20 2020 2020 2020 2022 2222 4765 6e65  .        """Gene
-00002140: 7261 7465 7320 6120 6675 6c6c 7920 706f  rates a fully po
-00002150: 7075 6c61 7465 6420 7265 7370 6f6e 7365  pulated response
-00002160: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
-00002170: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
-00002180: 706c 656d 656e 7465 6445 7272 6f72 0a0a  plementedError..
-00002190: 2020 2020 6465 6620 7072 6f63 6573 7328      def process(
-000021a0: 7365 6c66 2c20 7273 7029 202d 3e20 416e  self, rsp) -> An
-000021b0: 793a 0a20 2020 2020 2020 2022 2222 5072  y:.        """Pr
-000021c0: 6f63 6573 7320 7468 6520 636c 6965 6e74  ocess the client
-000021d0: 2072 6573 706f 6e73 6522 2222 0a20 2020   response""".   
-000021e0: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
-000021f0: 706c 656d 656e 7465 6445 7272 6f72 0a0a  plementedError..
-00002200: 0a63 6c61 7373 205f 4578 6563 7574 6551  .class _ExecuteQ
-00002210: 7565 7279 4661 6374 6f72 7928 5f4f 6369  ueryFactory(_Oci
-00002220: 656e 7452 6571 7565 7374 4661 6374 6f72  entRequestFactor
-00002230: 7929 3a0a 2020 2020 6465 6620 7265 7175  y):.    def requ
-00002240: 6573 7428 7365 6c66 2c20 6f70 6572 6174  est(self, operat
-00002250: 696f 6e3a 2073 7472 293a 0a20 2020 2020  ion: str):.     
-00002260: 2020 2022 2222 4765 6e65 7261 7465 7320     """Generates 
-00002270: 6120 6675 6c6c 7920 706f 7075 6c61 7465  a fully populate
-00002280: 6420 4558 4543 5554 455f 5155 4552 5920  d EXECUTE_QUERY 
-00002290: 7265 7175 6573 7420 7072 6f74 6f62 7566  request protobuf
-000022a0: 2222 220a 2020 2020 2020 2020 7265 7120  """.        req 
-000022b0: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
-000022c0: 290a 2020 2020 2020 2020 7265 712e 7479  ).        req.ty
-000022d0: 7065 203d 2070 726f 746f 2e52 6571 7565  pe = proto.Reque
-000022e0: 7374 2e52 6571 7565 7374 5479 7065 2e56  st.RequestType.V
-000022f0: 616c 7565 2822 4558 4543 5554 455f 5155  alue("EXECUTE_QU
-00002300: 4552 5922 290a 2020 2020 2020 2020 7265  ERY").        re
-00002310: 712e 6578 6563 7574 655f 7175 6572 792e  q.execute_query.
-00002320: 7371 6c20 3d20 6f70 6572 6174 696f 6e0a  sql = operation.
-00002330: 2020 2020 2020 2020 7265 712e 6578 6563          req.exec
-00002340: 7574 655f 7175 6572 792e 666f 7263 6520  ute_query.force 
-00002350: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00002360: 7265 7475 726e 2072 6571 0a0a 2020 2020  return req..    
-00002370: 6465 6620 7265 7370 6f6e 7365 2873 656c  def response(sel
-00002380: 6629 3a0a 2020 2020 2020 2020 2222 2247  f):.        """G
-00002390: 656e 6572 6174 6573 2061 2066 756c 6c79  enerates a fully
-000023a0: 2070 6f70 756c 6174 6564 2045 5845 4355   populated EXECU
-000023b0: 5445 5f51 5545 5259 2072 6573 706f 6e73  TE_QUERY respons
-000023c0: 6520 7072 6f74 6f62 7566 2222 220a 2020  e protobuf""".  
-000023d0: 2020 2020 2020 7265 7475 726e 2070 726f        return pro
-000023e0: 746f 2e45 7865 6375 7465 5175 6572 7952  to.ExecuteQueryR
-000023f0: 6573 706f 6e73 6528 290a 0a0a 636c 6173  esponse()...clas
-00002400: 7320 5f45 7865 6375 7465 4578 706c 6169  s _ExecuteExplai
-00002410: 6e46 6163 746f 7279 285f 4f63 6965 6e74  nFactory(_Ocient
-00002420: 5265 7175 6573 7446 6163 746f 7279 293a  RequestFactory):
-00002430: 0a20 2020 2064 6566 2072 6571 7565 7374  .    def request
-00002440: 2873 656c 662c 206f 7065 7261 7469 6f6e  (self, operation
-00002450: 3a20 7374 7229 3a0a 2020 2020 2020 2020  : str):.        
-00002460: 2222 2247 656e 6572 6174 6573 2061 2066  """Generates a f
-00002470: 756c 6c79 2070 6f70 756c 6174 6564 2045  ully populated E
-00002480: 5845 4355 5445 5f45 5850 4c41 494e 2072  XECUTE_EXPLAIN r
-00002490: 6571 7565 7374 2070 726f 746f 6275 6622  equest protobuf"
-000024a0: 2222 0a20 2020 2020 2020 2072 6571 203d  "".        req =
-000024b0: 2070 726f 746f 2e52 6571 7565 7374 2829   proto.Request()
-000024c0: 0a20 2020 2020 2020 2072 6571 2e74 7970  .        req.typ
-000024d0: 6520 3d20 7072 6f74 6f2e 5265 7175 6573  e = proto.Reques
-000024e0: 742e 5265 7175 6573 7454 7970 652e 5661  t.RequestType.Va
-000024f0: 6c75 6528 2245 5845 4355 5445 5f45 5850  lue("EXECUTE_EXP
-00002500: 4c41 494e 2229 0a20 2020 2020 2020 2072  LAIN").        r
-00002510: 6571 2e65 7865 6375 7465 5f65 7870 6c61  eq.execute_expla
-00002520: 696e 2e66 6f72 6d61 7420 3d20 7072 6f74  in.format = prot
-00002530: 6f2e 4578 706c 6169 6e46 6f72 6d61 742e  o.ExplainFormat.
-00002540: 4a53 4f4e 0a20 2020 2020 2020 2073 706c  JSON.        spl
-00002550: 6974 7465 6420 3d20 6f70 6572 6174 696f  itted = operatio
-00002560: 6e2e 7370 6c69 7428 6d61 7873 706c 6974  n.split(maxsplit
-00002570: 3d31 290a 2020 2020 2020 2020 6966 206c  =1).        if l
-00002580: 656e 2873 706c 6974 7465 6429 203d 3d20  en(splitted) == 
-00002590: 323a 0a20 2020 2020 2020 2020 2020 2072  2:.            r
-000025a0: 6571 2e65 7865 6375 7465 5f65 7870 6c61  eq.execute_expla
-000025b0: 696e 2e73 716c 203d 2073 706c 6974 7465  in.sql = splitte
-000025c0: 645b 315d 0a20 2020 2020 2020 2072 6574  d[1].        ret
-000025d0: 7572 6e20 7265 710a 0a20 2020 2064 6566  urn req..    def
-000025e0: 2072 6573 706f 6e73 6528 7365 6c66 293a   response(self):
-000025f0: 0a20 2020 2020 2020 2022 2222 4765 6e65  .        """Gene
-00002600: 7261 7465 7320 6120 6675 6c6c 7920 706f  rates a fully po
-00002610: 7075 6c61 7465 6420 4558 4543 5554 455f  pulated EXECUTE_
-00002620: 4558 504c 4149 4e20 7265 7370 6f6e 7365  EXPLAIN response
-00002630: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
-00002640: 2020 2020 2072 6574 7572 6e20 7072 6f74       return prot
-00002650: 6f2e 4578 706c 6169 6e52 6573 706f 6e73  o.ExplainRespons
-00002660: 6553 7472 696e 6750 6c61 6e28 290a 0a0a  eStringPlan()...
-00002670: 636c 6173 7320 5f45 7865 6375 7465 4578  class _ExecuteEx
-00002680: 706f 7274 4661 6374 6f72 7928 5f4f 6369  portFactory(_Oci
-00002690: 656e 7452 6571 7565 7374 4661 6374 6f72  entRequestFactor
-000026a0: 7929 3a0a 2020 2020 6465 6620 7265 7175  y):.    def requ
-000026b0: 6573 7428 7365 6c66 2c20 6f70 6572 6174  est(self, operat
-000026c0: 696f 6e3a 2073 7472 293a 0a20 2020 2020  ion: str):.     
-000026d0: 2020 2022 2222 4765 6e65 7261 7465 7320     """Generates 
-000026e0: 6120 6675 6c6c 7920 706f 7075 6c61 7465  a fully populate
-000026f0: 6420 4558 4543 5554 455f 4558 504f 5254  d EXECUTE_EXPORT
-00002700: 2072 6571 7565 7374 2070 726f 746f 6275   request protobu
-00002710: 6622 2222 0a20 2020 2020 2020 2072 6571  f""".        req
-00002720: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
-00002730: 2829 0a20 2020 2020 2020 2072 6571 2e74  ().        req.t
-00002740: 7970 6520 3d20 7072 6f74 6f2e 5265 7175  ype = proto.Requ
-00002750: 6573 742e 5265 7175 6573 7454 7970 652e  est.RequestType.
-00002760: 5661 6c75 6528 2245 5845 4355 5445 5f45  Value("EXECUTE_E
-00002770: 5850 4f52 5422 290a 2020 2020 2020 2020  XPORT").        
-00002780: 7265 712e 6578 6563 7574 655f 6578 706f  req.execute_expo
-00002790: 7274 2e73 716c 203d 206f 7065 7261 7469  rt.sql = operati
-000027a0: 6f6e 0a20 2020 2020 2020 2072 6574 7572  on.        retur
-000027b0: 6e20 7265 710a 0a20 2020 2064 6566 2072  n req..    def r
-000027c0: 6573 706f 6e73 6528 7365 6c66 293a 0a20  esponse(self):. 
-000027d0: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
-000027e0: 7465 7320 6120 6675 6c6c 7920 706f 7075  tes a fully popu
-000027f0: 6c61 7465 6420 4558 4543 5554 455f 4558  lated EXECUTE_EX
-00002800: 504f 5254 2072 6573 706f 6e73 6520 7072  PORT response pr
-00002810: 6f74 6f62 7566 2222 220a 2020 2020 2020  otobuf""".      
-00002820: 2020 7265 7475 726e 2070 726f 746f 2e45    return proto.E
-00002830: 7865 6375 7465 4578 706f 7274 5265 7370  xecuteExportResp
-00002840: 6f6e 7365 2829 0a0a 0a63 6c61 7373 205f  onse()...class _
-00002850: 4578 706c 6169 6e50 6970 656c 696e 6546  ExplainPipelineF
-00002860: 6163 746f 7279 285f 4f63 6965 6e74 5265  actory(_OcientRe
-00002870: 7175 6573 7446 6163 746f 7279 293a 0a20  questFactory):. 
-00002880: 2020 2064 6566 2072 6571 7565 7374 2873     def request(s
-00002890: 656c 662c 206f 7065 7261 7469 6f6e 3a20  elf, operation: 
-000028a0: 7374 7229 3a0a 2020 2020 2020 2020 2222  str):.        ""
-000028b0: 2247 656e 6572 6174 6573 2061 2066 756c  "Generates a ful
-000028c0: 6c79 2070 6f70 756c 6174 6564 2045 5850  ly populated EXP
-000028d0: 4c41 494e 5f50 4950 454c 494e 4520 7265  LAIN_PIPELINE re
-000028e0: 7175 6573 7420 7072 6f74 6f62 7566 2222  quest protobuf""
-000028f0: 220a 2020 2020 2020 2020 7265 7120 3d20  ".        req = 
-00002900: 7072 6f74 6f2e 5265 7175 6573 7428 290a  proto.Request().
-00002910: 2020 2020 2020 2020 7265 712e 7479 7065          req.type
-00002920: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
-00002930: 2e52 6571 7565 7374 5479 7065 2e56 616c  .RequestType.Val
-00002940: 7565 2822 4558 504c 4149 4e5f 5049 5045  ue("EXPLAIN_PIPE
-00002950: 4c49 4e45 2229 0a20 2020 2020 2020 2072  LINE").        r
-00002960: 6571 2e65 7870 6c61 696e 5f70 6970 656c  eq.explain_pipel
-00002970: 696e 652e 7371 6c20 3d20 6f70 6572 6174  ine.sql = operat
-00002980: 696f 6e0a 2020 2020 2020 2020 7265 7475  ion.        retu
-00002990: 726e 2072 6571 0a0a 2020 2020 6465 6620  rn req..    def 
-000029a0: 7265 7370 6f6e 7365 2873 656c 6629 3a0a  response(self):.
-000029b0: 2020 2020 2020 2020 2222 2247 656e 6572          """Gener
-000029c0: 6174 6573 2061 2066 756c 6c79 2070 6f70  ates a fully pop
-000029d0: 756c 6174 6564 2045 5850 4c41 494e 5f50  ulated EXPLAIN_P
-000029e0: 4950 454c 494e 4520 7265 7370 6f6e 7365  IPELINE response
-000029f0: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
-00002a00: 2020 2020 2072 6574 7572 6e20 7072 6f74       return prot
-00002a10: 6f2e 4578 706c 6169 6e50 6970 656c 696e  o.ExplainPipelin
-00002a20: 6552 6573 706f 6e73 6528 290a 0a0a 636c  eResponse()...cl
-00002a30: 6173 7320 5f43 6865 636b 4461 7461 4661  ass _CheckDataFa
-00002a40: 6374 6f72 7928 5f4f 6369 656e 7452 6571  ctory(_OcientReq
-00002a50: 7565 7374 4661 6374 6f72 7929 3a0a 2020  uestFactory):.  
-00002a60: 2020 6465 6620 7265 7175 6573 7428 7365    def request(se
-00002a70: 6c66 2c20 6f70 6572 6174 696f 6e3a 2073  lf, operation: s
-00002a80: 7472 293a 0a20 2020 2020 2020 2022 2222  tr):.        """
-00002a90: 4765 6e65 7261 7465 7320 6120 6675 6c6c  Generates a full
-00002aa0: 7920 706f 7075 6c61 7465 6420 4348 4543  y populated CHEC
-00002ab0: 4b5f 4441 5441 2072 6571 7565 7374 2070  K_DATA request p
-00002ac0: 726f 746f 6275 6622 2222 0a20 2020 2020  rotobuf""".     
-00002ad0: 2020 2072 6571 203d 2070 726f 746f 2e52     req = proto.R
-00002ae0: 6571 7565 7374 2829 0a20 2020 2020 2020  equest().       
-00002af0: 2072 6571 2e74 7970 6520 3d20 7072 6f74   req.type = prot
-00002b00: 6f2e 5265 7175 6573 742e 5265 7175 6573  o.Request.Reques
-00002b10: 7454 7970 652e 5661 6c75 6528 2243 4845  tType.Value("CHE
-00002b20: 434b 5f44 4154 4122 290a 2020 2020 2020  CK_DATA").      
-00002b30: 2020 7265 712e 6368 6563 6b5f 6461 7461    req.check_data
-00002b40: 2e73 716c 203d 206f 7065 7261 7469 6f6e  .sql = operation
-00002b50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002b60: 7265 710a 0a20 2020 2064 6566 2072 6573  req..    def res
-00002b70: 706f 6e73 6528 7365 6c66 293a 0a20 2020  ponse(self):.   
-00002b80: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-00002b90: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
-00002ba0: 7465 6420 4348 4543 4b5f 4441 5441 2072  ted CHECK_DATA r
-00002bb0: 6573 706f 6e73 6520 7072 6f74 6f62 7566  esponse protobuf
-00002bc0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00002bd0: 726e 2070 726f 746f 2e43 6865 636b 4461  rn proto.CheckDa
-00002be0: 7461 5265 7370 6f6e 7365 2829 0a0a 0a63  taResponse()...c
-00002bf0: 6c61 7373 205f 466f 7263 6545 7874 6572  lass _ForceExter
-00002c00: 6e61 6c46 6163 746f 7279 285f 4f63 6965  nalFactory(_Ocie
-00002c10: 6e74 5265 7175 6573 7446 6163 746f 7279  ntRequestFactory
-00002c20: 293a 0a20 2020 2064 6566 2072 6571 7565  ):.    def reque
-00002c30: 7374 2873 656c 662c 206f 7065 7261 7469  st(self, operati
-00002c40: 6f6e 3a20 7374 7229 3a0a 2020 2020 2020  on: str):.      
-00002c50: 2020 2222 2247 656e 6572 6174 6573 2061    """Generates a
-00002c60: 2066 756c 6c79 2070 6f70 756c 6174 6564   fully populated
-00002c70: 2046 4f52 4345 5f45 5854 4552 4e41 4c20   FORCE_EXTERNAL 
-00002c80: 7265 7175 6573 7420 7072 6f74 6f62 7566  request protobuf
-00002c90: 2222 220a 2020 2020 2020 2020 7265 7120  """.        req 
-00002ca0: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
-00002cb0: 290a 2020 2020 2020 2020 7265 712e 7479  ).        req.ty
-00002cc0: 7065 203d 2070 726f 746f 2e52 6571 7565  pe = proto.Reque
-00002cd0: 7374 2e52 6571 7565 7374 5479 7065 2e56  st.RequestType.V
-00002ce0: 616c 7565 2822 5345 545f 5041 5241 4d45  alue("SET_PARAME
-00002cf0: 5445 5222 290a 2020 2020 2020 2020 7370  TER").        sp
-00002d00: 203d 2072 6571 2e73 6574 5f70 6172 616d   = req.set_param
-00002d10: 6574 6572 0a20 2020 2020 2020 2069 6620  eter.        if 
-00002d20: 6f70 6572 6174 696f 6e2e 656e 6473 7769  operation.endswi
-00002d30: 7468 2822 6f6e 2229 3a0a 2020 2020 2020  th("on"):.      
-00002d40: 2020 2020 2020 7370 2e66 6f72 6365 5f65        sp.force_e
-00002d50: 7874 6572 6e61 6c2e 6973 5f6f 6e20 3d20  xternal.is_on = 
-00002d60: 5472 7565 0a20 2020 2020 2020 2065 6c69  True.        eli
-00002d70: 6620 6f70 6572 6174 696f 6e2e 656e 6473  f operation.ends
-00002d80: 7769 7468 2822 6f66 6622 293a 0a20 2020  with("off"):.   
-00002d90: 2020 2020 2020 2020 2073 702e 666f 7263           sp.forc
-00002da0: 655f 6578 7465 726e 616c 2e69 735f 6f6e  e_external.is_on
-00002db0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00002dc0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00002dd0: 2020 2072 6169 7365 2053 796e 7461 7845     raise SyntaxE
-00002de0: 7272 6f72 2827 466f 726d 6174 206d 7573  rror('Format mus
-00002df0: 7420 6265 2022 464f 5243 4520 4558 5445  t be "FORCE EXTE
-00002e00: 524e 414c 2028 6f6e 7c6f 6666 2922 2729  RNAL (on|off)"')
-00002e10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002e20: 7265 710a 0a20 2020 2064 6566 2072 6573  req..    def res
-00002e30: 706f 6e73 6528 7365 6c66 293a 0a20 2020  ponse(self):.   
-00002e40: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-00002e50: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
-00002e60: 7465 6420 464f 5243 455f 4558 5445 524e  ted FORCE_EXTERN
-00002e70: 414c 2072 6573 706f 6e73 6520 7072 6f74  AL response prot
-00002e80: 6f62 7566 2222 220a 2020 2020 2020 2020  obuf""".        
-00002e90: 7265 7475 726e 2070 726f 746f 2e43 6f6e  return proto.Con
-00002ea0: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
-00002eb0: 6528 290a 0a0a 636c 6173 7320 5f53 6574  e()...class _Set
-00002ec0: 5363 6865 6d61 4661 6374 6f72 7928 5f4f  SchemaFactory(_O
-00002ed0: 6369 656e 7452 6571 7565 7374 4661 6374  cientRequestFact
-00002ee0: 6f72 7929 3a0a 2020 2020 6465 6620 7265  ory):.    def re
-00002ef0: 7175 6573 7428 7365 6c66 2c20 7363 6865  quest(self, sche
-00002f00: 6d61 3a20 7374 7229 3a0a 2020 2020 2020  ma: str):.      
-00002f10: 2020 2222 2247 656e 6572 6174 6573 2061    """Generates a
-00002f20: 2066 756c 6c79 2070 6f70 756c 6174 6564   fully populated
-00002f30: 2053 4554 2053 4348 454d 4120 7265 7175   SET SCHEMA requ
-00002f40: 6573 7420 7072 6f74 6f62 7566 2222 220a  est protobuf""".
-00002f50: 2020 2020 2020 2020 7265 7120 3d20 7072          req = pr
-00002f60: 6f74 6f2e 5265 7175 6573 7428 290a 2020  oto.Request().  
-00002f70: 2020 2020 2020 7265 712e 7479 7065 203d        req.type =
-00002f80: 2070 726f 746f 2e52 6571 7565 7374 2e52   proto.Request.R
-00002f90: 6571 7565 7374 5479 7065 2e56 616c 7565  equestType.Value
-00002fa0: 2822 5345 545f 5343 4845 4d41 2229 0a20  ("SET_SCHEMA"). 
-00002fb0: 2020 2020 2020 2072 6571 2e73 6574 5f73         req.set_s
-00002fc0: 6368 656d 612e 7363 6865 6d61 203d 2073  chema.schema = s
-00002fd0: 6368 656d 610a 2020 2020 2020 2020 7265  chema.        re
-00002fe0: 7475 726e 2072 6571 0a0a 2020 2020 6465  turn req..    de
-00002ff0: 6620 7265 7370 6f6e 7365 2873 656c 6629  f response(self)
-00003000: 3a0a 2020 2020 2020 2020 2222 2247 656e  :.        """Gen
-00003010: 6572 6174 6573 2053 4554 5f53 4348 454d  erates SET_SCHEM
-00003020: 4120 7265 7370 6f6e 7365 2070 726f 746f  A response proto
-00003030: 6275 6622 2222 0a20 2020 2020 2020 2072  buf""".        r
-00003040: 6574 7572 6e20 7072 6f74 6f2e 436f 6e66  eturn proto.Conf
-00003050: 6972 6d61 7469 6f6e 5265 7370 6f6e 7365  irmationResponse
-00003060: 2829 0a0a 0a63 6c61 7373 205f 4765 7453  ()...class _GetS
-00003070: 6368 656d 6146 6163 746f 7279 285f 4f63  chemaFactory(_Oc
-00003080: 6965 6e74 5265 7175 6573 7446 6163 746f  ientRequestFacto
-00003090: 7279 293a 0a20 2020 2064 6566 2072 6571  ry):.    def req
-000030a0: 7565 7374 2873 656c 6629 3a0a 2020 2020  uest(self):.    
-000030b0: 2020 2020 2222 2247 656e 6572 6174 6573      """Generates
-000030c0: 2061 2066 756c 6c79 2070 6f70 756c 6174   a fully populat
-000030d0: 6564 2047 4554 2053 4348 454d 4120 7265  ed GET SCHEMA re
-000030e0: 7175 6573 7420 7072 6f74 6f62 7566 2222  quest protobuf""
-000030f0: 220a 2020 2020 2020 2020 7265 7120 3d20  ".        req = 
-00003100: 7072 6f74 6f2e 5265 7175 6573 7428 290a  proto.Request().
-00003110: 2020 2020 2020 2020 7265 712e 7479 7065          req.type
-00003120: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
-00003130: 2e52 6571 7565 7374 5479 7065 2e56 616c  .RequestType.Val
-00003140: 7565 2822 4745 545f 5343 4845 4d41 2229  ue("GET_SCHEMA")
-00003150: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003160: 7265 710a 0a20 2020 2064 6566 2072 6573  req..    def res
-00003170: 706f 6e73 6528 7365 6c66 293a 0a20 2020  ponse(self):.   
-00003180: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-00003190: 7320 5345 545f 5343 4845 4d41 2072 6573  s SET_SCHEMA res
-000031a0: 706f 6e73 6520 7072 6f74 6f62 7566 2222  ponse protobuf""
-000031b0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-000031c0: 2070 726f 746f 2e47 6574 5363 6865 6d61   proto.GetSchema
-000031d0: 5265 7370 6f6e 7365 2829 0a0a 0a63 6c61  Response()...cla
-000031e0: 7373 205f 436c 6561 7243 6163 6865 4661  ss _ClearCacheFa
-000031f0: 6374 6f72 7928 5f4f 6369 656e 7452 6571  ctory(_OcientReq
-00003200: 7565 7374 4661 6374 6f72 7929 3a0a 2020  uestFactory):.  
-00003210: 2020 6465 6620 7265 7175 6573 7428 7365    def request(se
-00003220: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00003230: 4765 6e65 7261 7465 7320 6120 6675 6c6c  Generates a full
-00003240: 7920 706f 7075 6c61 7465 6420 434c 4541  y populated CLEA
-00003250: 5220 4341 4348 4520 7265 7175 6573 7420  R CACHE request 
-00003260: 7072 6f74 6f62 7566 2222 220a 2020 2020  protobuf""".    
-00003270: 2020 2020 7265 7120 3d20 7072 6f74 6f2e      req = proto.
-00003280: 5265 7175 6573 7428 290a 2020 2020 2020  Request().      
-00003290: 2020 7265 712e 7479 7065 203d 2070 726f    req.type = pro
-000032a0: 746f 2e52 6571 7565 7374 2e52 6571 7565  to.Request.Reque
-000032b0: 7374 5479 7065 2e56 616c 7565 2822 434c  stType.Value("CL
-000032c0: 4541 525f 4341 4348 4522 290a 2020 2020  EAR_CACHE").    
-000032d0: 2020 2020 7265 712e 636c 6561 725f 6361      req.clear_ca
-000032e0: 6368 652e 616c 6c5f 6e6f 6465 7320 3d20  che.all_nodes = 
-000032f0: 5472 7565 0a20 2020 2020 2020 2072 6574  True.        ret
-00003300: 7572 6e20 7265 710a 0a20 2020 2064 6566  urn req..    def
-00003310: 2072 6573 706f 6e73 6528 7365 6c66 293a   response(self):
-00003320: 0a20 2020 2020 2020 2022 2222 4765 6e65  .        """Gene
-00003330: 7261 7465 7320 5345 545f 5343 4845 4d41  rates SET_SCHEMA
-00003340: 2072 6573 706f 6e73 6520 7072 6f74 6f62   response protob
-00003350: 7566 2222 220a 2020 2020 2020 2020 7265  uf""".        re
-00003360: 7475 726e 2070 726f 746f 2e43 6f6e 6669  turn proto.Confi
-00003370: 726d 6174 696f 6e52 6573 706f 6e73 6528  rmationResponse(
-00003380: 290a 0a0a 636c 6173 7320 5f53 6574 5061  )...class _SetPa
-00003390: 7261 6d65 7465 7246 6163 746f 7279 285f  rameterFactory(_
-000033a0: 4f63 6965 6e74 5265 7175 6573 7446 6163  OcientRequestFac
-000033b0: 746f 7279 293a 0a20 2020 2064 6566 2072  tory):.    def r
-000033c0: 6571 7565 7374 2873 656c 662c 206f 703a  equest(self, op:
-000033d0: 2073 7472 2c20 7661 6c3a 2069 6e74 293a   str, val: int):
-000033e0: 0a20 2020 2020 2020 2022 2222 4765 6e65  .        """Gene
-000033f0: 7261 7465 7320 6120 6675 6c6c 7920 706f  rates a fully po
-00003400: 7075 6c61 7465 6420 5345 5420 5041 5241  pulated SET PARA
-00003410: 4d45 5445 5220 7265 7175 6573 7420 7072  METER request pr
-00003420: 6f74 6f62 7566 2222 220a 2020 2020 2020  otobuf""".      
-00003430: 2020 7265 7120 3d20 7072 6f74 6f2e 5265    req = proto.Re
-00003440: 7175 6573 7428 290a 2020 2020 2020 2020  quest().        
-00003450: 7265 712e 7479 7065 203d 2070 726f 746f  req.type = proto
-00003460: 2e52 6571 7565 7374 2e52 6571 7565 7374  .Request.Request
-00003470: 5479 7065 2e56 616c 7565 2822 5345 545f  Type.Value("SET_
-00003480: 5041 5241 4d45 5445 5222 290a 0a20 2020  PARAMETER")..   
-00003490: 2020 2020 2073 7020 3d20 7265 712e 7365       sp = req.se
-000034a0: 745f 7061 7261 6d65 7465 720a 0a20 2020  t_parameter..   
-000034b0: 2020 2020 2069 6620 6f70 203d 3d20 224d       if op == "M
-000034c0: 4158 524f 5753 223a 0a20 2020 2020 2020  AXROWS":.       
-000034d0: 2020 2020 2073 702e 726f 775f 6c69 6d69       sp.row_limi
-000034e0: 742e 726f 774c 696d 6974 203d 2076 616c  t.rowLimit = val
-000034f0: 0a20 2020 2020 2020 2065 6c69 6620 6f70  .        elif op
-00003500: 203d 3d20 224d 4158 5449 4d45 223a 0a20   == "MAXTIME":. 
-00003510: 2020 2020 2020 2020 2020 2073 702e 7469             sp.ti
-00003520: 6d65 5f6c 696d 6974 2e74 696d 654c 696d  me_limit.timeLim
-00003530: 6974 203d 2076 616c 0a20 2020 2020 2020  it = val.       
-00003540: 2065 6c69 6620 6f70 203d 3d20 224d 4158   elif op == "MAX
-00003550: 5445 4d50 4449 534b 223a 0a20 2020 2020  TEMPDISK":.     
-00003560: 2020 2020 2020 2073 702e 7465 6d70 5f64         sp.temp_d
-00003570: 6973 6b5f 6c69 6d69 742e 7465 6d70 4469  isk_limit.tempDi
-00003580: 736b 4c69 6d69 7420 3d20 7661 6c0a 2020  skLimit = val.  
-00003590: 2020 2020 2020 656c 6966 206f 7020 3d3d        elif op ==
-000035a0: 2022 5052 494f 5249 5459 223a 0a20 2020   "PRIORITY":.   
-000035b0: 2020 2020 2020 2020 2073 702e 7072 696f           sp.prio
-000035c0: 7269 7479 2e70 7269 6f72 6974 7920 3d20  rity.priority = 
-000035d0: 7661 6c0a 2020 2020 2020 2020 656c 6966  val.        elif
-000035e0: 206f 7020 3d3d 2022 5041 5241 4c4c 454c   op == "PARALLEL
-000035f0: 4953 4d22 3a0a 2020 2020 2020 2020 2020  ISM":.          
-00003600: 2020 7370 2e63 6f6e 6375 7272 656e 6379    sp.concurrency
-00003610: 2e63 6f6e 6375 7272 656e 6379 203d 2076  .concurrency = v
-00003620: 616c 0a20 2020 2020 2020 2065 6c73 653a  al.        else:
-00003630: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00003640: 7365 2050 726f 6772 616d 6d69 6e67 4572  se ProgrammingEr
-00003650: 726f 7228 7265 6173 6f6e 3d66 2253 796e  ror(reason=f"Syn
-00003660: 7461 7820 6572 726f 722e 2049 6e76 616c  tax error. Inval
-00003670: 6964 2053 4554 207b 6f70 7d22 290a 0a20  id SET {op}").. 
-00003680: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00003690: 710a 0a20 2020 2064 6566 2072 6573 706f  q..    def respo
-000036a0: 6e73 6528 7365 6c66 293a 0a20 2020 2020  nse(self):.     
-000036b0: 2020 2022 2222 4765 6e65 7261 7465 7320     """Generates 
-000036c0: 6120 5345 545f 5041 5241 4d45 5445 5220  a SET_PARAMETER 
-000036d0: 7265 7370 6f6e 7365 2070 726f 746f 6275  response protobu
-000036e0: 6622 2222 0a20 2020 2020 2020 2072 6574  f""".        ret
-000036f0: 7572 6e20 7072 6f74 6f2e 436f 6e66 6972  urn proto.Confir
-00003700: 6d61 7469 6f6e 5265 7370 6f6e 7365 2829  mationResponse()
-00003710: 0a0a 0a63 6c61 7373 205f 4361 6e63 656c  ...class _Cancel
-00003720: 5175 6572 7946 6163 746f 7279 285f 4f63  QueryFactory(_Oc
-00003730: 6965 6e74 5265 7175 6573 7446 6163 746f  ientRequestFacto
-00003740: 7279 293a 0a20 2020 2064 6566 2072 6571  ry):.    def req
-00003750: 7565 7374 2873 656c 662c 2069 643a 2073  uest(self, id: s
-00003760: 7472 293a 0a20 2020 2020 2020 2022 2222  tr):.        """
-00003770: 4765 6e65 7261 7465 7320 6120 6675 6c6c  Generates a full
-00003780: 7920 706f 7075 6c61 7465 6420 4341 4e43  y populated CANC
-00003790: 454c 2051 5545 5259 2072 6571 7565 7374  EL QUERY request
-000037a0: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
-000037b0: 2020 2020 2072 6571 203d 2070 726f 746f       req = proto
-000037c0: 2e52 6571 7565 7374 2829 0a20 2020 2020  .Request().     
-000037d0: 2020 2072 6571 2e74 7970 6520 3d20 7072     req.type = pr
-000037e0: 6f74 6f2e 5265 7175 6573 742e 5265 7175  oto.Request.Requ
-000037f0: 6573 7454 7970 652e 5661 6c75 6528 2243  estType.Value("C
-00003800: 414e 4345 4c5f 5155 4552 5922 290a 2020  ANCEL_QUERY").  
-00003810: 2020 2020 2020 7265 712e 6361 6e63 656c        req.cancel
-00003820: 5f71 7565 7279 2e73 716c 203d 2069 640a  _query.sql = id.
-00003830: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00003840: 6571 0a0a 2020 2020 6465 6620 7265 7370  eq..    def resp
-00003850: 6f6e 7365 2873 656c 6629 3a0a 2020 2020  onse(self):.    
-00003860: 2020 2020 2222 2247 656e 6572 6174 6573      """Generates
-00003870: 2061 2043 414e 4345 4c5f 5155 4552 5920   a CANCEL_QUERY 
-00003880: 7265 7370 6f6e 7365 2070 726f 746f 6275  response protobu
-00003890: 6622 2222 0a20 2020 2020 2020 2072 6574  f""".        ret
-000038a0: 7572 6e20 7072 6f74 6f2e 4361 6e63 656c  urn proto.Cancel
-000038b0: 5175 6572 7952 6573 706f 6e73 6528 290a  QueryResponse().
-000038c0: 0a0a 636c 6173 7320 5f4b 696c 6c51 7565  ..class _KillQue
-000038d0: 7279 4661 6374 6f72 7928 5f4f 6369 656e  ryFactory(_Ocien
-000038e0: 7452 6571 7565 7374 4661 6374 6f72 7929  tRequestFactory)
-000038f0: 3a0a 2020 2020 6465 6620 7265 7175 6573  :.    def reques
-00003900: 7428 7365 6c66 2c20 6964 3a20 7374 7229  t(self, id: str)
-00003910: 3a0a 2020 2020 2020 2020 2222 2247 656e  :.        """Gen
-00003920: 6572 6174 6573 2061 2066 756c 6c79 2070  erates a fully p
-00003930: 6f70 756c 6174 6564 204b 494c 4c20 5155  opulated KILL QU
-00003940: 4552 5920 7265 7175 6573 7420 7072 6f74  ERY request prot
-00003950: 6f62 7566 2222 220a 2020 2020 2020 2020  obuf""".        
-00003960: 7265 7120 3d20 7072 6f74 6f2e 5265 7175  req = proto.Requ
-00003970: 6573 7428 290a 2020 2020 2020 2020 7265  est().        re
-00003980: 712e 7479 7065 203d 2070 726f 746f 2e52  q.type = proto.R
-00003990: 6571 7565 7374 2e52 6571 7565 7374 5479  equest.RequestTy
-000039a0: 7065 2e56 616c 7565 2822 4b49 4c4c 5f51  pe.Value("KILL_Q
-000039b0: 5545 5259 2229 0a20 2020 2020 2020 2072  UERY").        r
-000039c0: 6571 2e6b 696c 6c5f 7175 6572 792e 7371  eq.kill_query.sq
-000039d0: 6c20 3d20 6964 0a20 2020 2020 2020 2072  l = id.        r
-000039e0: 6574 7572 6e20 7265 710a 0a20 2020 2064  eturn req..    d
-000039f0: 6566 2072 6573 706f 6e73 6528 7365 6c66  ef response(self
-00003a00: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-00003a10: 6e65 7261 7465 7320 6120 4b49 4c4c 5f51  nerates a KILL_Q
-00003a20: 5545 5259 2072 6573 706f 6e73 6520 7072  UERY response pr
-00003a30: 6f74 6f62 7566 2222 220a 2020 2020 2020  otobuf""".      
-00003a40: 2020 7265 7475 726e 2070 726f 746f 2e4b    return proto.K
-00003a50: 696c 6c51 7565 7279 5265 7370 6f6e 7365  illQueryResponse
-00003a60: 2829 0a0a 0a63 6c61 7373 205f 4765 7453  ()...class _GetS
-00003a70: 7973 7465 6d4d 6574 6164 6174 6146 6163  ystemMetadataFac
-00003a80: 746f 7279 285f 4f63 6965 6e74 5265 7175  tory(_OcientRequ
-00003a90: 6573 7446 6163 746f 7279 293a 0a20 2020  estFactory):.   
-00003aa0: 2064 6566 2072 6571 7565 7374 2873 656c   def request(sel
-00003ab0: 662c 206f 702c 2073 6368 656d 612c 2074  f, op, schema, t
-00003ac0: 6162 6c65 2c20 636f 6c75 6d6e 2c20 7669  able, column, vi
-00003ad0: 6577 293a 0a20 2020 2020 2020 2022 2222  ew):.        """
-00003ae0: 4765 6e65 7261 7465 7320 6120 6675 6c6c  Generates a full
-00003af0: 7920 706f 7075 6c61 7465 6420 4745 545f  y populated GET_
-00003b00: 5359 5354 454d 5f4d 4554 4144 4154 4120  SYSTEM_METADATA 
-00003b10: 7265 7175 6573 7420 7072 6f74 6f62 7566  request protobuf
-00003b20: 2222 220a 2020 2020 2020 2020 7265 7120  """.        req 
-00003b30: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
-00003b40: 290a 2020 2020 2020 2020 7265 712e 7479  ).        req.ty
-00003b50: 7065 203d 2070 726f 746f 2e52 6571 7565  pe = proto.Reque
-00003b60: 7374 2e52 6571 7565 7374 5479 7065 2e56  st.RequestType.V
-00003b70: 616c 7565 2822 4645 5443 485f 5359 5354  alue("FETCH_SYST
-00003b80: 454d 5f4d 4554 4144 4154 4122 290a 2020  EM_METADATA").  
-00003b90: 2020 2020 2020 7265 712e 6665 7463 685f        req.fetch_
-00003ba0: 7379 7374 656d 5f6d 6574 6164 6174 612e  system_metadata.
-00003bb0: 6361 6c6c 203d 206f 700a 0a20 2020 2020  call = op..     
-00003bc0: 2020 2069 6620 7363 6865 6d61 2069 7320     if schema is 
-00003bd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00003be0: 2020 2020 2020 7265 712e 6665 7463 685f        req.fetch_
-00003bf0: 7379 7374 656d 5f6d 6574 6164 6174 612e  system_metadata.
-00003c00: 7363 6865 6d61 203d 2073 6368 656d 610a  schema = schema.
-00003c10: 2020 2020 2020 2020 6966 2074 6162 6c65          if table
-00003c20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00003c30: 2020 2020 2020 2020 2020 7265 712e 6665            req.fe
-00003c40: 7463 685f 7379 7374 656d 5f6d 6574 6164  tch_system_metad
-00003c50: 6174 612e 7461 626c 6520 3d20 7461 626c  ata.table = tabl
-00003c60: 650a 2020 2020 2020 2020 6966 2063 6f6c  e.        if col
-00003c70: 756d 6e20 6973 206e 6f74 204e 6f6e 653a  umn is not None:
-00003c80: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-00003c90: 2e66 6574 6368 5f73 7973 7465 6d5f 6d65  .fetch_system_me
-00003ca0: 7461 6461 7461 2e63 6f6c 756d 6e20 3d20  tadata.column = 
-00003cb0: 636f 6c75 6d6e 0a20 2020 2020 2020 2069  column.        i
-00003cc0: 6620 7669 6577 2069 7320 6e6f 7420 4e6f  f view is not No
-00003cd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00003ce0: 7265 712e 6665 7463 685f 7379 7374 656d  req.fetch_system
-00003cf0: 5f6d 6574 6164 6174 612e 7669 6577 203d  _metadata.view =
-00003d00: 2076 6965 770a 0a20 2020 2020 2020 2072   view..        r
-00003d10: 6574 7572 6e20 7265 710a 0a20 2020 2064  eturn req..    d
-00003d20: 6566 2072 6573 706f 6e73 6528 7365 6c66  ef response(self
-00003d30: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-00003d40: 6e65 7261 7465 7320 6120 6675 6c6c 7920  nerates a fully 
-00003d50: 706f 7075 6c61 7465 6420 4348 4543 4b5f  populated CHECK_
-00003d60: 4441 5441 2072 6573 706f 6e73 6520 7072  DATA response pr
-00003d70: 6f74 6f62 7566 2222 220a 2020 2020 2020  otobuf""".      
-00003d80: 2020 7265 7475 726e 2070 726f 746f 2e46    return proto.F
-00003d90: 6574 6368 5379 7374 656d 4d65 7461 6461  etchSystemMetada
-00003da0: 7461 5265 7370 6f6e 7365 2829 0a0a 0a22  taResponse()..."
-00003db0: 2222 4d61 7070 696e 6720 6672 6f6d 2071  ""Mapping from q
-00003dc0: 7565 7279 2074 7970 6520 746f 2069 7473  uery type to its
-00003dd0: 2072 6571 7565 7374 2066 6163 746f 7279   request factory
-00003de0: 2222 220a 5f4f 4349 454e 545f 5245 5155  """._OCIENT_REQU
-00003df0: 4553 545f 4641 4354 4f52 4945 5320 3d20  EST_FACTORIES = 
-00003e00: 7b0a 2020 2020 2253 454c 4543 5422 3a20  {.    "SELECT": 
-00003e10: 5f45 7865 6375 7465 5175 6572 7946 6163  _ExecuteQueryFac
-00003e20: 746f 7279 2829 2c0a 2020 2020 2257 4954  tory(),.    "WIT
-00003e30: 4822 3a20 5f45 7865 6375 7465 5175 6572  H": _ExecuteQuer
-00003e40: 7946 6163 746f 7279 2829 2c0a 2020 2020  yFactory(),.    
-00003e50: 2245 5850 4c41 494e 2050 4950 454c 494e  "EXPLAIN PIPELIN
-00003e60: 4522 3a20 5f45 7870 6c61 696e 5069 7065  E": _ExplainPipe
-00003e70: 6c69 6e65 4661 6374 6f72 7928 292c 0a20  lineFactory(),. 
-00003e80: 2020 2022 4558 504c 4149 4e22 3a20 5f45     "EXPLAIN": _E
-00003e90: 7865 6375 7465 4578 706c 6169 6e46 6163  xecuteExplainFac
-00003ea0: 746f 7279 2829 2c0a 2020 2020 2245 5850  tory(),.    "EXP
-00003eb0: 4f52 5422 3a20 5f45 7865 6375 7465 4578  ORT": _ExecuteEx
-00003ec0: 706f 7274 4661 6374 6f72 7928 292c 0a20  portFactory(),. 
-00003ed0: 2020 2022 4348 4543 4b22 3a20 5f43 6865     "CHECK": _Che
-00003ee0: 636b 4461 7461 4661 6374 6f72 7928 292c  ckDataFactory(),
-00003ef0: 0a20 2020 2022 464f 5243 4522 3a20 5f46  .    "FORCE": _F
-00003f00: 6f72 6365 4578 7465 726e 616c 4661 6374  orceExternalFact
-00003f10: 6f72 7928 292c 0a20 2020 2022 5345 5420  ory(),.    "SET 
-00003f20: 5343 4845 4d41 223a 205f 5365 7453 6368  SCHEMA": _SetSch
-00003f30: 656d 6146 6163 746f 7279 2829 2c0a 2020  emaFactory(),.  
-00003f40: 2020 2247 4554 2053 4348 454d 4122 3a20    "GET SCHEMA": 
-00003f50: 5f47 6574 5363 6865 6d61 4661 6374 6f72  _GetSchemaFactor
-00003f60: 7928 292c 0a20 2020 2022 434c 4541 5220  y(),.    "CLEAR 
-00003f70: 4341 4348 4522 3a20 5f43 6c65 6172 4361  CACHE": _ClearCa
-00003f80: 6368 6546 6163 746f 7279 2829 2c0a 2020  cheFactory(),.  
-00003f90: 2020 2253 4554 223a 205f 5365 7450 6172    "SET": _SetPar
-00003fa0: 616d 6574 6572 4661 6374 6f72 7928 292c  ameterFactory(),
-00003fb0: 0a20 2020 2022 4341 4e43 454c 223a 205f  .    "CANCEL": _
-00003fc0: 4361 6e63 656c 5175 6572 7946 6163 746f  CancelQueryFacto
-00003fd0: 7279 2829 2c0a 2020 2020 224b 494c 4c22  ry(),.    "KILL"
-00003fe0: 3a20 5f4b 696c 6c51 7565 7279 4661 6374  : _KillQueryFact
-00003ff0: 6f72 7928 292c 0a20 2020 2022 4745 5420  ory(),.    "GET 
-00004000: 5359 5354 454d 204d 4554 4144 4154 4122  SYSTEM METADATA"
-00004010: 3a20 5f47 6574 5379 7374 656d 4d65 7461  : _GetSystemMeta
-00004020: 6461 7461 4661 6374 6f72 7928 292c 0a7d  dataFactory(),.}
-00004030: 0a0a 0a64 6566 205f 636f 6e76 6572 745f  ...def _convert_
-00004040: 6578 6365 7074 696f 6e28 6d73 6729 3a0a  exception(msg):.
-00004050: 2020 2020 2222 2249 6e74 6572 6e61 6c20      """Internal 
-00004060: 726f 7574 696e 6520 746f 2063 6f6e 7665  routine to conve
-00004070: 7274 2074 6865 2067 6f6f 676c 6520 7072  rt the google pr
-00004080: 6f74 6f62 7566 2043 6f6e 6669 726d 6174  otobuf Confirmat
-00004090: 696f 6e52 6573 706f 6e73 650a 2020 2020  ionResponse.    
-000040a0: 746f 2061 6e20 6578 6365 7074 696f 6e0a  to an exception.
-000040b0: 2020 2020 2222 220a 2020 2020 6966 206d      """.    if m
-000040c0: 7367 2e76 656e 646f 725f 636f 6465 203c  sg.vendor_code <
-000040d0: 2030 3a0a 2020 2020 2020 2020 7265 7475   0:.        retu
-000040e0: 726e 2045 7272 6f72 2873 716c 5f73 7461  rn Error(sql_sta
-000040f0: 7465 3d6d 7367 2e73 716c 5f73 7461 7465  te=msg.sql_state
-00004100: 2c20 7265 6173 6f6e 3d6d 7367 2e72 6561  , reason=msg.rea
-00004110: 736f 6e2c 2076 656e 646f 725f 636f 6465  son, vendor_code
-00004120: 3d6d 7367 2e76 656e 646f 725f 636f 6465  =msg.vendor_code
-00004130: 290a 0a20 2020 2072 6574 7572 6e20 5761  )..    return Wa
-00004140: 726e 696e 6728 7371 6c5f 7374 6174 653d  rning(sql_state=
-00004150: 6d73 672e 7371 6c5f 7374 6174 652c 2072  msg.sql_state, r
-00004160: 6561 736f 6e3d 6d73 672e 7265 6173 6f6e  eason=msg.reason
-00004170: 2c20 7665 6e64 6f72 5f63 6f64 653d 6d73  , vendor_code=ms
-00004180: 672e 7665 6e64 6f72 5f63 6f64 6529 0a0a  g.vendor_code)..
-00004190: 0a64 6566 205f 7365 6e64 5f6d 7367 2863  .def _send_msg(c
-000041a0: 6f6e 6e2c 2070 726f 746f 6275 665f 6d73  onn, protobuf_ms
-000041b0: 6729 3a0a 2020 2020 2222 2249 6e74 6572  g):.    """Inter
-000041c0: 6e61 6c20 726f 7574 696e 6520 746f 2073  nal routine to s
-000041d0: 656e 6420 6120 7072 6f74 6f62 7566 206d  end a protobuf m
-000041e0: 6573 7361 6765 206f 6e20 6120 636f 6e6e  essage on a conn
-000041f0: 6563 7469 6f6e 2222 220a 2020 2020 6966  ection""".    if
-00004200: 206e 6f74 2063 6f6e 6e2e 736f 636b 3a0a   not conn.sock:.
-00004210: 2020 2020 2020 2020 7261 6973 6520 5072          raise Pr
-00004220: 6f67 7261 6d6d 696e 6745 7272 6f72 2822  ogrammingError("
-00004230: 436f 6e6e 6563 7469 6f6e 206e 6f74 2061  Connection not a
-00004240: 7661 696c 6162 6c65 2229 0a0a 2020 2020  vailable")..    
-00004250: 6c6f 6767 6572 2e64 6562 7567 2866 2253  logger.debug(f"S
-00004260: 656e 6469 6e67 206d 6573 7361 6765 206f  ending message o
-00004270: 6e20 736f 636b 6574 207b 636f 6e6e 2e73  n socket {conn.s
-00004280: 6f63 6b7d 3a20 7b70 726f 746f 6275 665f  ock}: {protobuf_
-00004290: 6d73 677d 2229 0a0a 2020 2020 7472 793a  msg}")..    try:
-000042a0: 0a20 2020 2020 2020 2063 6f6e 6e2e 736f  .        conn.so
-000042b0: 636b 2e73 656e 6461 6c6c 2873 7472 7563  ck.sendall(struc
-000042c0: 742e 7061 636b 2822 2169 222c 2070 726f  t.pack("!i", pro
-000042d0: 746f 6275 665f 6d73 672e 4279 7465 5369  tobuf_msg.ByteSi
-000042e0: 7a65 2829 2920 2b20 7072 6f74 6f62 7566  ze()) + protobuf
-000042f0: 5f6d 7367 2e53 6572 6961 6c69 7a65 546f  _msg.SerializeTo
-00004300: 5374 7269 6e67 2829 290a 2020 2020 6578  String()).    ex
-00004310: 6365 7074 2049 4f45 7272 6f72 3a0a 2020  cept IOError:.  
-00004320: 2020 2020 2020 7261 6973 6520 494f 4572        raise IOEr
-00004330: 726f 7228 224e 6574 776f 726b 2073 656e  ror("Network sen
-00004340: 6420 6572 726f 7222 290a 0a0a 6465 6620  d error")...def 
-00004350: 5f72 6563 765f 616c 6c28 636f 6e6e 2c20  _recv_all(conn, 
-00004360: 7369 7a65 293a 0a20 2020 2022 2222 496e  size):.    """In
-00004370: 7465 726e 616c 2072 6f75 7469 6e65 2074  ternal routine t
-00004380: 6f20 7265 6365 6976 6520 6073 697a 6560  o receive `size`
-00004390: 2062 7974 6573 206f 6620 6461 7461 2066   bytes of data f
-000043a0: 726f 6d20 6120 636f 6e6e 6563 7469 6f6e  rom a connection
-000043b0: 2222 220a 2020 2020 6966 206e 6f74 2063  """.    if not c
-000043c0: 6f6e 6e2e 736f 636b 3a0a 2020 2020 2020  onn.sock:.      
-000043d0: 2020 7261 6973 6520 4572 726f 7228 2243    raise Error("C
-000043e0: 6f6e 6e65 6374 696f 6e20 6e6f 7420 6176  onnection not av
-000043f0: 6169 6c61 626c 6522 290a 0a20 2020 2077  ailable")..    w
-00004400: 6869 6c65 206c 656e 2863 6f6e 6e2e 5f62  hile len(conn._b
-00004410: 7566 6665 7229 203c 2073 697a 653a 0a20  uffer) < size:. 
-00004420: 2020 2020 2020 2072 6563 6569 7665 6420         received 
-00004430: 3d20 636f 6e6e 2e73 6f63 6b2e 7265 6376  = conn.sock.recv
-00004440: 2831 3637 3737 3231 3629 2020 2320 3136  (16777216)  # 16
-00004450: 4d42 2062 7566 6665 720a 2020 2020 2020  MB buffer.      
-00004460: 2020 6966 206e 6f74 2072 6563 6569 7665    if not receive
-00004470: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
-00004480: 6169 7365 2049 4f45 7272 6f72 2822 4e65  aise IOError("Ne
-00004490: 7477 6f72 6b20 7265 6365 6976 6520 6572  twork receive er
-000044a0: 726f 7222 290a 2020 2020 2020 2020 636f  ror").        co
-000044b0: 6e6e 2e5f 6275 6666 6572 202b 3d20 7265  nn._buffer += re
-000044c0: 6365 6976 6564 0a0a 2020 2020 7265 7420  ceived..    ret 
-000044d0: 3d20 636f 6e6e 2e5f 6275 6666 6572 5b3a  = conn._buffer[:
-000044e0: 7369 7a65 5d0a 2020 2020 636f 6e6e 2e5f  size].    conn._
-000044f0: 6275 6666 6572 203d 2063 6f6e 6e2e 5f62  buffer = conn._b
-00004500: 7566 6665 725b 7369 7a65 3a5d 0a0a 2020  uffer[size:]..  
-00004510: 2020 7265 7475 726e 2072 6574 0a0a 0a64    return ret...d
-00004520: 6566 205f 7265 6376 5f6d 7367 2863 6f6e  ef _recv_msg(con
-00004530: 6e2c 2070 726f 746f 6275 665f 6d73 6729  n, protobuf_msg)
-00004540: 3a0a 2020 2020 2222 2249 6e74 6572 6e61  :.    """Interna
-00004550: 6c20 726f 7574 696e 6520 746f 2072 6563  l routine to rec
-00004560: 6569 7665 2061 2070 726f 746f 6275 6620  eive a protobuf 
-00004570: 6d65 7373 6167 6520 6f6e 2061 2063 6f6e  message on a con
-00004580: 6e65 6374 696f 6e22 2222 0a20 2020 2068  nection""".    h
-00004590: 6472 203d 205f 7265 6376 5f61 6c6c 2863  dr = _recv_all(c
-000045a0: 6f6e 6e2c 2034 290a 2020 2020 6d73 6773  onn, 4).    msgs
-000045b0: 697a 6520 3d20 7374 7275 6374 2e75 6e70  ize = struct.unp
-000045c0: 6163 6b28 2221 6922 2c20 6864 7229 5b30  ack("!i", hdr)[0
-000045d0: 5d0a 0a20 2020 206d 7367 203d 205f 7265  ]..    msg = _re
-000045e0: 6376 5f61 6c6c 2863 6f6e 6e2c 206d 7367  cv_all(conn, msg
-000045f0: 7369 7a65 290a 0a20 2020 2070 726f 746f  size)..    proto
-00004600: 6275 665f 6d73 672e 5061 7273 6546 726f  buf_msg.ParseFro
-00004610: 6d53 7472 696e 6728 6d73 6729 0a0a 2020  mString(msg)..  
-00004620: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
-00004630: 2252 6563 6569 7665 6420 6d65 7373 6167  "Received messag
-00004640: 6520 6f6e 2063 6f6e 6e65 6374 696f 6e20  e on connection 
-00004650: 7b63 6f6e 6e2e 736f 636b 7d3a 207b 7072  {conn.sock}: {pr
-00004660: 6f74 6f62 7566 5f6d 7367 7d22 290a 0a20  otobuf_msg}").. 
-00004670: 2020 2072 6574 7572 6e20 7072 6f74 6f62     return protob
-00004680: 7566 5f6d 7367 0a0a 0a64 6566 2044 6174  uf_msg...def Dat
-00004690: 6528 7965 6172 2c20 6d6f 6e74 682c 2064  e(year, month, d
-000046a0: 6179 293a 2020 2320 7079 6c69 6e74 3a20  ay):  # pylint: 
-000046b0: 6469 7361 626c 653d 696e 7661 6c69 642d  disable=invalid-
-000046c0: 6e61 6d65 0a20 2020 2022 2222 5479 7065  name.    """Type
-000046d0: 2063 6f6e 7374 7275 6374 6f72 2072 6571   constructor req
-000046e0: 7569 7265 6420 696e 2050 4550 2032 3439  uired in PEP 249
-000046f0: 2074 6f20 636f 6e73 7472 7563 7420 610a   to construct a.
-00004700: 2020 2020 4461 7465 206f 626a 6563 7420      Date object 
-00004710: 6672 6f6d 2079 6561 722c 206d 6f6e 7468  from year, month
-00004720: 2c20 6461 790a 2020 2020 2222 220a 2020  , day.    """.  
-00004730: 2020 7265 7475 726e 2064 6174 6574 696d    return datetim
-00004740: 652e 6461 7465 7469 6d65 2879 6561 722c  e.datetime(year,
-00004750: 206d 6f6e 7468 2c20 6461 7929 0a0a 0a64   month, day)...d
-00004760: 6566 2054 696d 6528 686f 7572 2c20 6d69  ef Time(hour, mi
-00004770: 6e75 7465 2c20 7365 636f 6e64 293a 2020  nute, second):  
-00004780: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-00004790: 653d 696e 7661 6c69 642d 6e61 6d65 0a20  e=invalid-name. 
-000047a0: 2020 2022 2222 5479 7065 2063 6f6e 7374     """Type const
-000047b0: 7275 6374 6f72 2072 6571 7569 7265 6420  ructor required 
-000047c0: 696e 2050 4550 2032 3439 2074 6f20 636f  in PEP 249 to co
-000047d0: 6e73 7472 7563 7420 610a 2020 2020 5469  nstruct a.    Ti
-000047e0: 6d65 206f 626a 6563 7420 6672 6f6d 2068  me object from h
-000047f0: 6f75 722c 206d 696e 7574 652c 2073 6563  our, minute, sec
-00004800: 6f6e 640a 2020 2020 2222 220a 2020 2020  ond.    """.    
-00004810: 7265 7475 726e 2064 6174 6574 696d 652e  return datetime.
-00004820: 7469 6d65 2868 6f75 722c 206d 696e 7574  time(hour, minut
-00004830: 652c 2073 6563 6f6e 6429 0a0a 0a64 6566  e, second)...def
-00004840: 2054 696d 6573 7461 6d70 2879 6561 722c   Timestamp(year,
-00004850: 206d 6f6e 7468 2c20 6461 792c 2068 6f75   month, day, hou
-00004860: 722c 206d 696e 7574 652c 2073 6563 6f6e  r, minute, secon
-00004870: 6429 3a20 2023 2070 796c 696e 743a 2064  d):  # pylint: d
-00004880: 6973 6162 6c65 3d69 6e76 616c 6964 2d6e  isable=invalid-n
-00004890: 616d 652c 746f 6f2d 6d61 6e79 2d61 7267  ame,too-many-arg
-000048a0: 756d 656e 7473 0a20 2020 2022 2222 5479  uments.    """Ty
-000048b0: 7065 2063 6f6e 7374 7275 6374 6f72 2072  pe constructor r
-000048c0: 6571 7569 7265 6420 696e 2050 4550 2032  equired in PEP 2
-000048d0: 3439 2074 6f20 636f 6e73 7472 7563 740a  49 to construct.
-000048e0: 2020 2020 6120 5469 6d65 7374 616d 7020      a Timestamp 
-000048f0: 6f62 6a65 6374 2066 726f 6d20 7965 6172  object from year
-00004900: 2c20 6d6f 6e74 682c 2064 6179 2c20 686f  , month, day, ho
-00004910: 7572 2c20 6d69 6e75 7465 2c20 7365 636f  ur, minute, seco
-00004920: 6e64 0a20 2020 2022 2222 0a20 2020 2072  nd.    """.    r
-00004930: 6574 7572 6e20 6461 7465 7469 6d65 2e64  eturn datetime.d
-00004940: 6174 6574 696d 6528 7965 6172 2c20 6d6f  atetime(year, mo
-00004950: 6e74 682c 2064 6179 2c20 686f 7572 2c20  nth, day, hour, 
-00004960: 6d69 6e75 7465 2c20 7365 636f 6e64 292e  minute, second).
-00004970: 7469 6d65 7374 616d 7028 290a 0a0a 6465  timestamp()...de
-00004980: 6620 4461 7465 4672 6f6d 5469 636b 7328  f DateFromTicks(
-00004990: 7469 636b 7329 3a20 2023 2070 796c 696e  ticks):  # pylin
-000049a0: 743a 2064 6973 6162 6c65 3d69 6e76 616c  t: disable=inval
-000049b0: 6964 2d6e 616d 650a 2020 2020 2222 2254  id-name.    """T
-000049c0: 7970 6520 636f 6e73 7472 7563 746f 7220  ype constructor 
-000049d0: 7265 7175 6972 6564 2069 6e20 5045 5020  required in PEP 
-000049e0: 3234 3920 746f 2063 6f6e 7374 7275 6374  249 to construct
-000049f0: 0a20 2020 2061 2044 6174 6520 6f62 6a65  .    a Date obje
-00004a00: 6374 2066 726f 6d20 6120 7469 6d65 7374  ct from a timest
-00004a10: 616d 7020 6f66 2073 6563 6f6e 6473 2073  amp of seconds s
-00004a20: 696e 6365 2065 706f 6368 0a20 2020 2022  ince epoch.    "
-00004a30: 2222 0a20 2020 2072 6574 7572 6e20 6461  "".    return da
-00004a40: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
-00004a50: 7574 6366 726f 6d74 696d 6573 7461 6d70  utcfromtimestamp
-00004a60: 2874 6963 6b73 290a 0a0a 6465 6620 5469  (ticks)...def Ti
-00004a70: 6d65 4672 6f6d 5469 636b 7328 7469 636b  meFromTicks(tick
-00004a80: 7329 3a20 2023 2070 796c 696e 743a 2064  s):  # pylint: d
-00004a90: 6973 6162 6c65 3d69 6e76 616c 6964 2d6e  isable=invalid-n
-00004aa0: 616d 650a 2020 2020 2222 2254 7970 6520  ame.    """Type 
-00004ab0: 636f 6e73 7472 7563 746f 7220 7265 7175  constructor requ
-00004ac0: 6972 6564 2069 6e20 5045 5020 3234 3920  ired in PEP 249 
-00004ad0: 746f 2063 6f6e 7374 7275 6374 0a20 2020  to construct.   
-00004ae0: 2061 2054 696d 6520 6f62 6a65 6374 2066   a Time object f
-00004af0: 726f 6d20 6120 7469 6d65 7374 616d 7020  rom a timestamp 
-00004b00: 6f66 2073 6563 6f6e 6473 2073 696e 6365  of seconds since
-00004b10: 2065 706f 6368 0a20 2020 2022 2222 0a20   epoch.    """. 
-00004b20: 2020 2064 6174 655f 7469 6d65 203d 2064     date_time = d
-00004b30: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
-00004b40: 2e75 7463 6672 6f6d 7469 6d65 7374 616d  .utcfromtimestam
-00004b50: 7028 7469 636b 7329 0a20 2020 2072 6574  p(ticks).    ret
-00004b60: 7572 6e20 6461 7465 7469 6d65 2e74 696d  urn datetime.tim
-00004b70: 6528 6461 7465 5f74 696d 652e 686f 7572  e(date_time.hour
-00004b80: 2c20 6461 7465 5f74 696d 652e 6d69 6e75  , date_time.minu
-00004b90: 7465 2c20 6461 7465 5f74 696d 652e 7365  te, date_time.se
-00004ba0: 636f 6e64 290a 0a0a 6465 6620 5469 6d65  cond)...def Time
-00004bb0: 7374 616d 7046 726f 6d54 6963 6b73 2874  stampFromTicks(t
-00004bc0: 6963 6b73 293a 2020 2320 7079 6c69 6e74  icks):  # pylint
-00004bd0: 3a20 6469 7361 626c 653d 696e 7661 6c69  : disable=invali
-00004be0: 642d 6e61 6d65 0a20 2020 2022 2222 5479  d-name.    """Ty
-00004bf0: 7065 2063 6f6e 7374 7275 6374 6f72 2072  pe constructor r
-00004c00: 6571 7569 7265 6420 696e 2050 4550 2032  equired in PEP 2
-00004c10: 3439 2074 6f20 636f 6e73 7472 7563 740a  49 to construct.
-00004c20: 2020 2020 6120 5469 6d65 7374 616d 7020      a Timestamp 
-00004c30: 6f62 6a65 6374 2066 726f 6d20 6120 7469  object from a ti
-00004c40: 6d65 7374 616d 7020 6f66 2073 6563 6f6e  mestamp of secon
-00004c50: 6473 2073 696e 6365 2065 706f 6368 0a20  ds since epoch. 
-00004c60: 2020 2022 2222 0a20 2020 2072 6574 7572     """.    retur
-00004c70: 6e20 7469 636b 730a 0a0a 6465 6620 5f68  n ticks...def _h
-00004c80: 6173 685f 6b65 7928 7368 6172 6564 5f6b  ash_key(shared_k
-00004c90: 6579 2c20 7361 6c74 293a 0a20 2020 2022  ey, salt):.    "
-00004ca0: 2222 496e 7465 726e 616c 206b 6579 2068  ""Internal key h
-00004cb0: 6173 6820 6675 6e63 7469 6f6e 2222 220a  ash function""".
-00004cc0: 2020 2020 2320 4e6f 2069 6465 6120 7768      # No idea wh
-00004cd0: 6572 6520 7468 6973 2061 6c67 6f72 6974  ere this algorit
-00004ce0: 686d 2063 616d 6520 6672 6f6d 2c20 6275  hm came from, bu
-00004cf0: 7420 646f 2061 2068 6f6d 6520 6772 6f77  t do a home grow
-00004d00: 6e20 6b65 790a 2020 2020 2320 6465 7269  n key.    # deri
-00004d10: 7669 6174 696f 6e20 6675 6e63 7469 6f6e  viation function
-00004d20: 0a20 2020 2062 7566 6665 7220 3d20 7374  .    buffer = st
-00004d30: 7275 6374 2e70 6163 6b28 2221 6922 2c20  ruct.pack("!i", 
-00004d40: 6c65 6e28 7368 6172 6564 5f6b 6579 2929  len(shared_key))
-00004d50: 0a20 2020 2062 7566 6665 7220 3d20 6275  .    buffer = bu
-00004d60: 6666 6572 202b 2073 616c 740a 2020 2020  ffer + salt.    
-00004d70: 6275 6666 6572 203d 2062 7566 6665 7220  buffer = buffer 
-00004d80: 2b20 7368 6172 6564 5f6b 6579 0a20 2020  + shared_key.   
-00004d90: 2068 6173 6865 7220 3d20 6861 7368 6573   hasher = hashes
-00004da0: 2e48 6173 6828 6861 7368 6573 2e53 4841  .Hash(hashes.SHA
-00004db0: 3235 3628 292c 2062 6163 6b65 6e64 3d64  256(), backend=d
-00004dc0: 6566 6175 6c74 5f62 6163 6b65 6e64 2829  efault_backend()
-00004dd0: 290a 2020 2020 6861 7368 6572 2e75 7064  ).    hasher.upd
-00004de0: 6174 6528 6275 6666 6572 290a 2020 2020  ate(buffer).    
-00004df0: 7265 7475 726e 2068 6173 6865 722e 6669  return hasher.fi
-00004e00: 6e61 6c69 7a65 2829 0a0a 0a23 2053 6573  nalize()...# Ses
-00004e10: 7369 6f6e 7320 636f 6465 0a0a 2320 5573  sions code..# Us
-00004e20: 6564 2066 6f72 2072 6570 7265 7365 6e74  ed for represent
-00004e30: 696e 6720 6120 7365 7373 696f 6e20 6372  ing a session cr
-00004e40: 6561 7465 6420 7769 7468 2061 2073 6563  eated with a sec
-00004e50: 7572 6974 7920 746f 6b65 6e20 7369 676e  urity token sign
-00004e60: 2069 6e0a 0a0a 636c 6173 7320 5365 6375   in...class Secu
-00004e70: 7269 7479 546f 6b65 6e3a 0a20 2020 2064  rityToken:.    d
-00004e80: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00004e90: 2c20 746f 6b65 6e44 6174 613a 2073 7472  , tokenData: str
-00004ea0: 2c20 746f 6b65 6e53 6967 6e61 7475 7265  , tokenSignature
-00004eb0: 3a20 7374 722c 2069 7373 7565 7246 696e  : str, issuerFin
-00004ec0: 6765 7270 7269 6e74 3a20 7374 7229 3a0a  gerprint: str):.
-00004ed0: 2020 2020 2020 2020 7365 6c66 2e74 6f6b          self.tok
-00004ee0: 656e 4461 7461 203d 2074 6f6b 656e 4461  enData = tokenDa
-00004ef0: 7461 0a20 2020 2020 2020 2073 656c 662e  ta.        self.
-00004f00: 746f 6b65 6e53 6967 6e61 7475 7265 203d  tokenSignature =
-00004f10: 2074 6f6b 656e 5369 676e 6174 7572 650a   tokenSignature.
-00004f20: 2020 2020 2020 2020 7365 6c66 2e69 7373          self.iss
-00004f30: 7565 7246 696e 6765 7270 7269 6e74 203d  uerFingerprint =
-00004f40: 2069 7373 7565 7246 696e 6765 7270 7269   issuerFingerpri
-00004f50: 6e74 0a0a 0a23 2055 7365 6420 666f 7220  nt...# Used for 
-00004f60: 7265 7072 6573 656e 7469 6e67 2061 2073  representing a s
-00004f70: 6573 7369 6f6e 2063 7265 6174 6564 2077  ession created w
-00004f80: 6974 6820 6120 7573 6572 2061 6e64 2070  ith a user and p
-00004f90: 6173 7377 6f72 6420 7369 676e 2069 6e2e  assword sign in.
-00004fa0: 0a0a 0a63 6c61 7373 2055 7365 7241 6e64  ...class UserAnd
-00004fb0: 5061 7373 776f 7264 3a0a 2020 2020 6465  Password:.    de
-00004fc0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00004fd0: 2075 7365 723a 2073 7472 2c20 7061 7373   user: str, pass
-00004fe0: 776f 7264 3a20 7374 7229 3a0a 2020 2020  word: str):.    
-00004ff0: 2020 2020 7365 6c66 2e75 7365 7220 3d20      self.user = 
-00005000: 7573 6572 0a20 2020 2020 2020 2073 656c  user.        sel
-00005010: 662e 7061 7373 776f 7264 203d 2070 6173  f.password = pas
-00005020: 7377 6f72 640a 0a0a 636c 6173 7320 5365  sword...class Se
-00005030: 7373 696f 6e3a 0a20 2020 2064 6566 205f  ssion:.    def _
-00005040: 5f69 6e69 745f 5f28 7365 6c66 2c20 7365  _init__(self, se
-00005050: 6375 7269 7479 546f 6b65 6e3d 4e6f 6e65  curityToken=None
-00005060: 2c20 7573 6572 416e 6450 6173 7377 6f72  , userAndPasswor
-00005070: 643d 4e6f 6e65 293a 0a20 2020 2020 2020  d=None):.       
-00005080: 2023 204f 6e6c 7920 6f6e 6520 6f66 2074   # Only one of t
-00005090: 6865 7365 2073 686f 756c 6420 6265 2069  hese should be i
-000050a0: 6e73 7461 6e74 6961 7465 642e 2054 6865  nstantiated. The
-000050b0: 206f 7468 6572 204d 5553 5420 6265 206e   other MUST be n
-000050c0: 6f6e 652e 0a20 2020 2020 2020 2073 656c  one..        sel
-000050d0: 662e 7365 6375 7269 7479 546f 6b65 6e20  f.securityToken 
-000050e0: 3d20 7365 6375 7269 7479 546f 6b65 6e0a  = securityToken.
-000050f0: 2020 2020 2020 2020 7365 6c66 2e75 7365          self.use
-00005100: 7241 6e64 5061 7373 776f 7264 203d 2075  rAndPassword = u
-00005110: 7365 7241 6e64 5061 7373 776f 7264 0a0a  serAndPassword..
-00005120: 0a63 6c61 7373 2043 6f6e 6e65 6374 696f  .class Connectio
-00005130: 6e3a 0a20 2020 2022 2222 4120 636f 6e6e  n:.    """A conn
-00005140: 6563 7469 6f6e 2074 6f20 7468 6520 4f63  ection to the Oc
-00005150: 6965 6e74 2064 6174 6162 6173 652e 204e  ient database. N
-00005160: 6f72 6d61 6c6c 7920 636f 6e73 7472 7563  ormally construc
-00005170: 7465 6420 6279 0a20 2020 2063 616c 6c69  ted by.    calli
-00005180: 6e67 2074 6865 206d 6f64 756c 6520 6063  ng the module `c
-00005190: 6f6e 6e65 6374 2829 6020 6361 6c6c 2c20  onnect()` call, 
-000051a0: 6275 7420 6361 6e20 6265 2063 6f6e 7374  but can be const
-000051b0: 7275 6374 6564 0a20 2020 2064 6972 6563  ructed.    direc
-000051c0: 746c 790a 2020 2020 2222 220a 0a20 2020  tly.    """..   
-000051d0: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-000051e0: 6c65 3d74 6f6f 2d6d 616e 792d 696e 7374  le=too-many-inst
-000051f0: 616e 6365 2d61 7474 7269 6275 7465 730a  ance-attributes.
-00005200: 2020 2020 544c 535f 4e4f 4e45 203d 2031      TLS_NONE = 1
-00005210: 2020 2320 3a20 3a6d 6574 6120 7072 6976    # : :meta priv
-00005220: 6174 653a 0a20 2020 2054 4c53 5f55 4e56  ate:.    TLS_UNV
-00005230: 4552 4946 4945 4420 3d20 3220 2023 203a  ERIFIED = 2  # :
-00005240: 203a 6d65 7461 2070 7269 7661 7465 3a0a   :meta private:.
-00005250: 2020 2020 544c 535f 4f4e 203d 2033 2020      TLS_ON = 3  
-00005260: 2320 3a20 3a6d 6574 6120 7072 6976 6174  # : :meta privat
-00005270: 653a 0a0a 2020 2020 4841 4e44 5348 414b  e:..    HANDSHAK
-00005280: 455f 4342 4320 3d20 310a 2020 2020 4841  E_CBC = 1.    HA
-00005290: 4e44 5348 414b 455f 4743 4d20 3d20 320a  NDSHAKE_GCM = 2.
-000052a0: 2020 2020 4841 4e44 5348 414b 455f 5353      HANDSHAKE_SS
-000052b0: 4f20 3d20 330a 0a20 2020 2044 4546 4155  O = 3..    DEFAU
-000052c0: 4c54 5f48 4f53 5420 3d20 226c 6f63 616c  LT_HOST = "local
-000052d0: 686f 7374 220a 2020 2020 4445 4641 554c  host".    DEFAUL
-000052e0: 545f 504f 5254 203d 2034 3035 300a 2020  T_PORT = 4050.  
-000052f0: 2020 4445 4641 554c 545f 4441 5441 4241    DEFAULT_DATABA
-00005300: 5345 203d 2022 7379 7374 656d 220a 0a20  SE = "system".. 
-00005310: 2020 2068 6f73 7473 203d 205b 5d0a 2020     hosts = [].  
-00005320: 2020 706f 7274 203d 204e 6f6e 650a 2020    port = None.  
-00005330: 2020 6461 7461 6261 7365 203d 204e 6f6e    database = Non
-00005340: 650a 2020 2020 746c 7320 3d20 4e6f 6e65  e.    tls = None
-00005350: 0a20 2020 2066 6f72 6365 203d 204e 6f6e  .    force = Non
-00005360: 650a 2020 2020 6861 6e64 7368 616b 6520  e.    handshake 
-00005370: 3d20 4e6f 6e65 0a20 2020 2075 7365 7220  = None.    user 
-00005380: 3d20 4e6f 6e65 0a20 2020 2070 6173 7377  = None.    passw
-00005390: 6f72 6420 3d20 4e6f 6e65 0a20 2020 2073  ord = None.    s
-000053a0: 6563 6f6e 6461 7279 5f69 6e74 6572 6661  econdary_interfa
-000053b0: 6365 7320 3d20 4e6f 6e65 0a20 2020 2073  ces = None.    s
-000053c0: 6563 6f6e 6461 7279 5f69 6e64 6578 203d  econdary_index =
-000053d0: 202d 310a 2020 2020 736f 636b 203d 204e   -1.    sock = N
-000053e0: 6f6e 650a 2020 2020 7365 7373 696f 6e5f  one.    session_
-000053f0: 6964 203d 2073 7472 2875 7569 642e 7575  id = str(uuid.uu
-00005400: 6964 3128 2929 0a0a 2020 2020 7365 7373  id1())..    sess
-00005410: 696f 6e20 3d20 4e6f 6e65 0a20 2020 2073  ion = None.    s
-00005420: 6572 7665 7253 6573 7369 6f6e 4964 203d  erverSessionId =
-00005430: 204e 6f6e 650a 0a20 2020 2023 2057 6865   None..    # Whe
-00005440: 7468 6572 2074 6865 206e 6578 7420 6578  ther the next ex
-00005450: 6563 7574 6520 7175 6572 7920 7275 6e20  ecute query run 
-00005460: 6f6e 2074 6869 7320 636f 6e6e 6563 7469  on this connecti
-00005470: 6f6e 2077 696c 6c20 6265 2072 6564 6972  on will be redir
-00005480: 6563 7465 642e 2044 6f65 7320 6e6f 7468  ected. Does noth
-00005490: 696e 6720 6966 2066 6f72 6365 2069 7320  ing if force is 
-000054a0: 7365 7420 746f 2074 7275 650a 2020 2020  set to true.    
-000054b0: 666f 7263 655f 6e65 7874 5f72 6564 6972  force_next_redir
-000054c0: 6563 7420 3d20 4661 6c73 650a 0a20 2020  ect = False..   
-000054d0: 2023 2053 6573 7369 6f6e 7320 636f 6465   # Sessions code
-000054e0: 2065 6e64 0a0a 2020 2020 2320 7468 6520   end..    # the 
-000054f0: 5045 5020 3234 3920 7374 616e 6461 7264  PEP 249 standard
-00005500: 2072 6563 6f6d 6d65 6e74 7320 6d61 6b69   recomments maki
-00005510: 6e67 2074 6865 206d 6f64 756c 6520 6c65  ng the module le
-00005520: 7665 6c20 6578 6365 7074 696f 6e73 0a20  vel exceptions. 
-00005530: 2020 2023 2061 6c73 6f20 6174 7472 6962     # also attrib
-00005540: 7574 6573 206f 6e20 7468 6520 436f 6e6e  utes on the Conn
-00005550: 6563 7469 6f6e 2063 6c61 7373 0a20 2020  ection class.   
-00005560: 2045 7272 6f72 203d 2045 7272 6f72 0a20   Error = Error. 
-00005570: 2020 2057 6172 6e69 6e67 203d 2057 6172     Warning = War
-00005580: 6e69 6e67 0a20 2020 2049 6e74 6572 6661  ning.    Interfa
-00005590: 6365 4572 726f 7220 3d20 496e 7465 7266  ceError = Interf
-000055a0: 6163 6545 7272 6f72 0a20 2020 2044 6174  aceError.    Dat
-000055b0: 6162 6173 6545 7272 6f72 203d 2044 6174  abaseError = Dat
-000055c0: 6162 6173 6545 7272 6f72 0a20 2020 2049  abaseError.    I
-000055d0: 6e74 6572 6e61 6c45 7272 6f72 203d 2049  nternalError = I
-000055e0: 6e74 6572 6e61 6c45 7272 6f72 0a20 2020  nternalError.   
-000055f0: 204f 7065 7261 7469 6f6e 616c 4572 726f   OperationalErro
-00005600: 7220 3d20 4f70 6572 6174 696f 6e61 6c45  r = OperationalE
-00005610: 7272 6f72 0a20 2020 2050 726f 6772 616d  rror.    Program
-00005620: 6d69 6e67 4572 726f 7220 3d20 5072 6f67  mingError = Prog
-00005630: 7261 6d6d 696e 6745 7272 6f72 0a20 2020  rammingError.   
-00005640: 2049 6e74 6567 7269 7479 4572 726f 7220   IntegrityError 
-00005650: 3d20 496e 7465 6772 6974 7945 7272 6f72  = IntegrityError
-00005660: 0a20 2020 2044 6174 6145 7272 6f72 203d  .    DataError =
-00005670: 2044 6174 6145 7272 6f72 0a20 2020 204e   DataError.    N
-00005680: 6f74 5375 7070 6f72 7465 6445 7272 6f72  otSupportedError
-00005690: 203d 204e 6f74 5375 7070 6f72 7465 6445   = NotSupportedE
-000056a0: 7272 6f72 0a0a 2020 2020 6465 6620 5f73  rror..    def _s
-000056b0: 736c 697a 655f 636f 6e6e 6563 7469 6f6e  slize_connection
-000056c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000056d0: 2222 220a 2020 2020 2020 2020 4966 2053  """.        If S
-000056e0: 534c 2069 7320 7370 6563 6966 6965 642c  SL is specified,
-000056f0: 2077 7261 7020 7468 6520 736f 636b 6574   wrap the socket
-00005700: 2069 6e20 616e 2053 534c 2063 6f6e 6e65   in an SSL conne
-00005710: 6374 696f 6e0a 2020 2020 2020 2020 2222  ction.        ""
-00005720: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-00005730: 662e 746c 7320 213d 2073 656c 662e 544c  f.tls != self.TL
-00005740: 535f 4e4f 4e45 3a0a 2020 2020 2020 2020  S_NONE:.        
-00005750: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00005760: 2822 4372 6561 7469 6e67 2054 4c53 2063  ("Creating TLS c
-00005770: 6f6e 6e65 6374 696f 6e22 290a 2020 2020  onnection").    
-00005780: 2020 2020 2020 2020 636f 6e74 6578 7420          context 
-00005790: 3d20 7373 6c2e 6372 6561 7465 5f64 6566  = ssl.create_def
-000057a0: 6175 6c74 5f63 6f6e 7465 7874 2829 0a20  ault_context(). 
-000057b0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-000057c0: 7874 2e63 6865 636b 5f68 6f73 746e 616d  xt.check_hostnam
-000057d0: 6520 3d20 4661 6c73 650a 2020 2020 2020  e = False.      
-000057e0: 2020 2020 2020 6966 2073 656c 662e 746c        if self.tl
-000057f0: 7320 213d 2073 656c 662e 544c 535f 4f4e  s != self.TLS_ON
-00005800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005810: 2020 636f 6e74 6578 742e 7665 7269 6679    context.verify
-00005820: 5f6d 6f64 6520 3d20 7373 6c2e 4345 5254  _mode = ssl.CERT
-00005830: 5f4e 4f4e 450a 2020 2020 2020 2020 2020  _NONE.          
-00005840: 2020 7365 6c66 2e73 6f63 6b20 3d20 636f    self.sock = co
-00005850: 6e74 6578 742e 7772 6170 5f73 6f63 6b65  ntext.wrap_socke
-00005860: 7428 7365 6c66 2e73 6f63 6b29 0a0a 2020  t(self.sock)..  
-00005870: 2020 2320 4e6f 7465 2074 6861 7420 7468    # Note that th
-00005880: 6572 6520 6172 6520 6120 636f 7570 6c65  ere are a couple
-00005890: 206f 6620 706c 6163 6573 2069 6e20 7468   of places in th
-000058a0: 6520 636f 6465 2077 6865 7265 2077 6520  e code where we 
-000058b0: 7265 636f 6e73 7472 7563 7420 7468 6520  reconstruct the 
-000058c0: 436f 6e6e 6563 7469 6f6e 2e20 2049 6620  Connection.  If 
-000058d0: 796f 7520 6164 6420 6120 7061 7261 6d65  you add a parame
-000058e0: 7465 7220 6865 7265 2c20 6d61 6b65 2073  ter here, make s
-000058f0: 7572 6520 746f 2075 7064 6174 6520 7468  ure to update th
-00005900: 6f73 650a 2020 2020 2320 706c 6163 6573  ose.    # places
-00005910: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00005920: 5f28 7365 6c66 2c20 6473 6e3d 4e6f 6e65  _(self, dsn=None
-00005930: 2c20 7573 6572 3d4e 6f6e 652c 2070 6173  , user=None, pas
-00005940: 7377 6f72 643d 4e6f 6e65 2c20 686f 7374  sword=None, host
-00005950: 3d4e 6f6e 652c 2064 6174 6162 6173 653d  =None, database=
-00005960: 4e6f 6e65 2c20 746c 733d 4e6f 6e65 2c20  None, tls=None, 
-00005970: 6861 6e64 7368 616b 653d 4e6f 6e65 2c20  handshake=None, 
-00005980: 666f 7263 653d 4e6f 6e65 2c20 636f 6e66  force=None, conf
-00005990: 6967 6669 6c65 3d4e 6f6e 652c 2073 6573  igfile=None, ses
-000059a0: 7369 6f6e 3d4e 6f6e 6529 3a0a 2020 2020  sion=None):.    
-000059b0: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
-000059c0: 7361 626c 653d 746f 6f2d 6d61 6e79 2d61  sable=too-many-a
-000059d0: 7267 756d 656e 7473 2c6e 6f2d 6d65 6d62  rguments,no-memb
-000059e0: 6572 0a20 2020 2020 2020 2022 2222 436f  er.        """Co
-000059f0: 6e6e 6563 7469 6f6e 2070 6172 616d 6574  nnection paramet
-00005a00: 6572 7320 6361 6e20 6265 2073 7065 6369  ers can be speci
-00005a10: 6669 6564 2061 7320 7061 7274 206f 6620  fied as part of 
-00005a20: 7468 6520 6473 6e2c 0a20 2020 2020 2020  the dsn,.       
-00005a30: 2075 7369 6e67 206b 6579 776f 7264 2061   using keyword a
-00005a40: 7267 756d 656e 7473 206f 7220 626f 7468  rguments or both
-00005a50: 2e20 2049 6620 626f 7468 2061 7265 2073  .  If both are s
-00005a60: 7065 6369 6669 6564 2c20 7468 6520 6b65  pecified, the ke
-00005a70: 7977 6f72 640a 2020 2020 2020 2020 7061  yword.        pa
-00005a80: 7261 6d65 7465 7220 6f76 6572 7269 6465  rameter override
-00005a90: 7320 7468 6520 7661 6c75 6520 696e 2074  s the value in t
-00005aa0: 6865 2064 736e 2e0a 0a20 2020 2020 2020  he dsn...       
-00005ab0: 2054 6865 204f 6369 656e 7420 4453 4e20   The Ocient DSN 
-00005ac0: 6973 206f 6620 7468 6520 666f 726d 6174  is of the format
-00005ad0: 3a0a 2020 2020 2020 2020 606f 6369 656e  :.        `ocien
-00005ae0: 743a 2f2f 7573 6572 3a70 6173 7377 6f72  t://user:passwor
-00005af0: 6440 5b68 6f73 745d 5b3a 706f 7274 5d5b  d@[host][:port][
-00005b00: 2f64 6174 6162 6173 655d 5b3f 7061 7261  /database][?para
-00005b10: 6d31 3d76 616c 7565 3126 2e2e 2e5d 600a  m1=value1&...]`.
-00005b20: 0a20 2020 2020 2020 2060 7573 6572 6020  .        `user` 
-00005b30: 616e 6420 6070 6173 7377 6f72 6460 206d  and `password` m
-00005b40: 7573 7420 6265 2073 7570 706c 6965 642e  ust be supplied.
-00005b50: 2020 6068 6f73 7460 2064 6566 6175 6c74    `host` default
-00005b60: 7320 746f 206c 6f63 616c 686f 7374 2c0a  s to localhost,.
-00005b70: 2020 2020 2020 2020 706f 7274 2064 6566          port def
-00005b80: 6175 6c74 7320 746f 2034 3035 302c 2064  aults to 4050, d
-00005b90: 6174 6162 6173 6520 6465 6661 756c 7473  atabase defaults
-00005ba0: 2074 6f20 6073 7973 7465 6d60 2061 6e64   to `system` and
-00005bb0: 2060 746c 7360 2064 6566 6175 6c74 730a   `tls` defaults.
-00005bc0: 2020 2020 2020 2020 746f 2060 6f66 6660          to `off`
-00005bd0: 2e0a 0a20 2020 2020 2020 204d 756c 7469  ...        Multi
-00005be0: 706c 6520 686f 7374 7320 6d61 7920 6265  ple hosts may be
-00005bf0: 2073 7065 6369 6669 6564 2c20 7365 7061   specified, sepa
-00005c00: 7261 7465 6420 6279 2061 2063 6f6d 6d61  rated by a comma
-00005c10: 2c20 696e 2077 6869 6368 2063 6173 6520  , in which case 
-00005c20: 7468 650a 2020 2020 2020 2020 686f 7374  the.        host
-00005c30: 7320 7769 6c6c 2062 6520 7472 6965 6420  s will be tried 
-00005c40: 696e 206f 7264 6572 2020 5468 7573 2061  in order  Thus a
-00005c50: 6e20 6578 616d 706c 6520 4453 4e20 6d69  n example DSN mi
-00005c60: 6768 7420 6265 0a20 2020 2020 2020 2060  ght be.        `
-00005c70: 6f63 6965 6e74 3a2f 2f73 6f6d 656f 6e65  ocient://someone
-00005c80: 3a73 6f6d 6570 6173 7377 6f72 6440 686f  :somepassword@ho
-00005c90: 7374 312c 686f 7374 323a 3430 3531 2f6d  st1,host2:4051/m
-00005ca0: 7964 6260 0a0a 2020 2020 2020 2020 636f  ydb`..        co
-00005cb0: 6e66 6967 6669 6c65 2069 7320 7468 6520  nfigfile is the 
-00005cc0: 6e61 6d65 206f 6620 6120 636f 6e66 6967  name of a config
-00005cd0: 7572 6174 696f 6e20 6669 6c65 2069 6e20  uration file in 
-00005ce0: 494e 4920 666f 726d 6174 2c20 7768 6572  INI format, wher
-00005cf0: 6520 6561 6368 0a20 2020 2020 2020 2073  e each.        s
-00005d00: 6563 7469 6f6e 2069 7320 6569 7468 6572  ection is either
-00005d10: 2064 6566 6175 6c74 2c20 6f72 2061 2070   default, or a p
-00005d20: 6174 7465 726e 2074 6861 7420 6d61 7463  attern that matc
-00005d30: 6865 7320 7468 6520 686f 7374 2061 6e64  hes the host and
-00005d40: 206f 7074 696f 6e61 6c6c 790a 2020 2020   optionally.    
-00005d50: 2020 2020 6461 7461 6261 7365 2e20 7365      database. se
-00005d60: 6374 696f 6e73 2061 7265 206d 6174 6368  ctions are match
-00005d70: 6564 2069 6e20 6f72 6465 722c 2073 6f20  ed in order, so 
-00005d80: 6d6f 7265 2073 7065 6369 6669 6320 7365  more specific se
-00005d90: 6374 696f 6e73 2073 686f 756c 640a 2020  ctions should.  
-00005da0: 2020 2020 2020 7072 6563 6564 6520 6c65        precede le
-00005db0: 7373 2073 7065 6369 6669 6320 7365 6374  ss specific sect
-00005dc0: 696f 6e73 3a3a 0a0a 2020 2020 2020 2020  ions::..        
-00005dd0: 2020 2020 5b44 4546 4155 4c54 5d0a 2020      [DEFAULT].  
-00005de0: 2020 2020 2020 2020 2020 746c 7320 3d20            tls = 
-00005df0: 756e 7665 7269 6669 6564 0a0a 2020 2020  unverified..    
-00005e00: 2020 2020 2020 2020 2320 5468 6973 2077          # This w
-00005e10: 696c 6c20 6d61 7463 6820 7468 6520 7370  ill match the sp
-00005e20: 6563 6966 6963 2068 6f73 7420 616e 6420  ecific host and 
-00005e30: 6461 7461 6261 7365 0a20 2020 2020 2020  database.       
-00005e40: 2020 2020 205b 666f 6f2e 6f63 6965 6e74       [foo.ocient
-00005e50: 2e63 6f6d 2f73 6f6d 6564 625d 0a20 2020  .com/somedb].   
-00005e60: 2020 2020 2020 2020 2075 7365 7220 3d20           user = 
-00005e70: 7061 6e74 6865 720a 2020 2020 2020 2020  panther.        
-00005e80: 2020 2020 7061 7373 776f 7264 203d 2070      password = p
-00005e90: 696e 6b0a 0a20 2020 2020 2020 2020 2020  ink..           
-00005ea0: 2023 2054 6869 7320 7769 6c6c 206d 6174   # This will mat
-00005eb0: 6368 2074 6865 2073 7065 6369 6669 6320  ch the specific 
-00005ec0: 686f 7374 0a20 2020 2020 2020 2020 2020  host.           
-00005ed0: 205b 666f 6f2e 6f63 6965 6e74 2e63 6f6d   [foo.ocient.com
-00005ee0: 5d0a 2020 2020 2020 2020 2020 2020 7573  ].            us
-00005ef0: 6572 203d 2070 616e 7468 6572 0a20 2020  er = panther.   
-00005f00: 2020 2020 2020 2020 2070 6173 7377 6f72           passwor
-00005f10: 6420 3d20 7069 6e6b 0a0a 2020 2020 2020  d = pink..      
-00005f20: 2020 2020 2020 2320 5468 6973 2077 696c        # This wil
-00005f30: 6c20 6d61 7463 6820 616e 7920 686f 7374  l match any host
-00005f40: 2069 6e20 7468 6520 6f63 6965 6e74 2e63   in the ocient.c
-00005f50: 6f6d 2064 6f6d 6169 6e0a 2020 2020 2020  om domain.      
-00005f60: 2020 2020 2020 5b2a 2e6f 6369 656e 742e        [*.ocient.
-00005f70: 636f 6d5d 0a20 2020 2020 2020 2020 2020  com].           
-00005f80: 2075 7365 7220 3d20 746f 6d0a 2020 2020   user = tom.    
-00005f90: 2020 2020 2020 2020 7061 7373 776f 7264          password
-00005fa0: 203d 206a 6572 7279 0a20 2020 2020 2020   = jerry.       
-00005fb0: 2020 2020 2064 6174 6162 6173 6520 3d20       database = 
-00005fc0: 6d69 6365 0a0a 2020 2020 2020 2020 2020  mice..          
-00005fd0: 2020 2320 5468 6973 2077 696c 6c20 6d61    # This will ma
-00005fe0: 7463 6820 616e 7920 686f 7374 2069 6e20  tch any host in 
-00005ff0: 7468 6520 6f63 6965 6e74 2e63 6f6d 2064  the ocient.com d
-00006000: 6f6d 6169 6e0a 2020 2020 2020 2020 2020  omain.          
-00006010: 2020 5b2a 2e6f 6369 656e 742e 636f 6d5d    [*.ocient.com]
-00006020: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
-00006030: 7220 3d20 746f 6d0a 2020 2020 2020 2020  r = tom.        
-00006040: 2020 2020 7061 7373 776f 7264 203d 206a      password = j
-00006050: 6572 7279 0a0a 2020 2020 2020 2020 4375  erry..        Cu
-00006060: 7272 656e 746c 7920 7375 7070 6f72 7465  rrently supporte
-00006070: 6420 7061 7261 6d65 7465 7273 2061 7265  d parameters are
-00006080: 3a0a 0a20 2020 2020 2020 202d 2074 6c73  :..        - tls
-00006090: 3a20 5768 6963 6820 6361 6e20 6861 7665  : Which can have
-000060a0: 2074 6865 2076 616c 7565 7320 226f 6666   the values "off
-000060b0: 222c 2022 756e 7665 7269 6669 6564 222c  ", "unverified",
-000060c0: 206f 7220 226f 6e22 2069 6e20 7468 6520   or "on" in the 
-000060d0: 6473 6e2c 0a20 2020 2020 2020 2020 2020  dsn,.           
-000060e0: 206f 7220 436f 6e6e 6563 7469 6f6e 2e54   or Connection.T
-000060f0: 4c53 5f4e 4f4e 452c 2043 6f6e 6e65 6374  LS_NONE, Connect
-00006100: 696f 6e2e 544c 535f 554e 5645 5249 4649  ion.TLS_UNVERIFI
-00006110: 4544 2c20 6f72 0a20 2020 2020 2020 2020  ED, or.         
-00006120: 2020 2043 6f6e 6e65 6374 696f 6e2e 544c     Connection.TL
-00006130: 535f 4f4e 2061 7320 6120 6b65 7977 6f72  S_ON as a keywor
-00006140: 6420 7061 7261 6d65 7465 722e 0a20 2020  d parameter..   
-00006150: 2020 2020 202d 2066 6f72 6365 3a20 5472       - force: Tr
-00006160: 7565 206f 7220 4661 6c73 652c 2077 6865  ue or False, whe
-00006170: 7468 6572 2074 6f20 666f 7263 6520 7468  ther to force th
-00006180: 6520 636f 6e6e 6563 7469 6f6e 2074 6f20  e connection to 
-00006190: 7265 6d61 696e 206f 6e20 7468 6973 0a20  remain on this. 
-000061a0: 2020 2020 2020 2020 2020 2073 6572 7665             serve
-000061b0: 720a 2020 2020 2020 2020 2222 220a 2020  r.        """.  
-000061c0: 2020 2020 2020 2320 7079 6c69 6e74 3a20        # pylint: 
-000061d0: 6469 7361 626c 653d 6e6f 2d6d 656d 6265  disable=no-membe
-000061e0: 720a 2020 2020 2020 2020 7365 6c66 2e5f  r.        self._
-000061f0: 7061 7273 655f 6172 6773 2864 736e 2c20  parse_args(dsn, 
-00006200: 7573 6572 2c20 7061 7373 776f 7264 2c20  user, password, 
-00006210: 686f 7374 2c20 6461 7461 6261 7365 2c20  host, database, 
-00006220: 746c 732c 2068 616e 6473 6861 6b65 2c20  tls, handshake, 
-00006230: 666f 7263 652c 2063 6f6e 6669 6766 696c  force, configfil
-00006240: 6529 0a0a 2020 2020 2020 2020 7361 7665  e)..        save
-00006250: 645f 6578 6320 3d20 4e6f 6e65 0a20 2020  d_exc = None.   
-00006260: 2020 2020 2066 6f72 206f 6e65 5f68 6f73       for one_hos
-00006270: 7420 696e 2073 656c 662e 686f 7374 733a  t in self.hosts:
-00006280: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-00006290: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000062a0: 2020 6c6f 6767 6572 2e69 6e66 6f28 6622    logger.info(f"
-000062b0: 5472 7969 6e67 2074 6f20 636f 6e6e 6563  Trying to connec
-000062c0: 7420 746f 207b 6f6e 655f 686f 7374 7d3a  t to {one_host}:
-000062d0: 7b73 656c 662e 706f 7274 7d22 290a 2020  {self.port}").  
-000062e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000062f0: 6c66 2e73 6f63 6b20 3d20 736f 636b 6574  lf.sock = socket
-00006300: 2e63 7265 6174 655f 636f 6e6e 6563 7469  .create_connecti
-00006310: 6f6e 2828 6f6e 655f 686f 7374 2c20 7365  on((one_host, se
-00006320: 6c66 2e70 6f72 7429 290a 2020 2020 2020  lf.port)).      
-00006330: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00006340: 2e69 6e66 6f28 6622 436f 6e6e 6563 7465  .info(f"Connecte
-00006350: 6420 746f 207b 6f6e 655f 686f 7374 7d3a  d to {one_host}:
-00006360: 7b73 656c 662e 706f 7274 7d20 6f6e 2073  {self.port} on s
-00006370: 6f63 6b65 7420 7b73 656c 662e 736f 636b  ocket {self.sock
-00006380: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00006390: 2020 2020 7361 7665 645f 6578 6320 3d20      saved_exc = 
-000063a0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-000063b0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-000063c0: 2020 2020 2020 2065 7863 6570 7420 436f         except Co
-000063d0: 6e6e 6563 7469 6f6e 4572 726f 7220 6173  nnectionError as
-000063e0: 2065 7863 3a0a 2020 2020 2020 2020 2020   exc:.          
-000063f0: 2020 2020 2020 7361 7665 645f 6578 6320        saved_exc 
-00006400: 3d20 6578 630a 2020 2020 2020 2020 2020  = exc.          
-00006410: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00006420: 6f6e 2061 7320 6578 633a 0a20 2020 2020  on as exc:.     
-00006430: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-00006440: 5f65 7863 203d 2065 7863 0a0a 2020 2020  _exc = exc..    
-00006450: 2020 2020 6966 2073 6176 6564 5f65 7863      if saved_exc
-00006460: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00006470: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00006480: 4572 726f 7228 6622 556e 6162 6c65 2074  Error(f"Unable t
-00006490: 6f20 636f 6e6e 6563 7420 746f 207b 272c  o connect to {',
-000064a0: 272e 6a6f 696e 2873 656c 662e 686f 7374  '.join(self.host
-000064b0: 7329 7d3a 7b73 656c 662e 706f 7274 7d3a  s)}:{self.port}:
-000064c0: 207b 7374 7228 7361 7665 645f 6578 6329   {str(saved_exc)
-000064d0: 7d22 2920 6672 6f6d 2073 6176 6564 5f65  }") from saved_e
-000064e0: 7863 0a0a 2020 2020 2020 2020 7365 6c66  xc..        self
-000064f0: 2e5f 7373 6c69 7a65 5f63 6f6e 6e65 6374  ._sslize_connect
-00006500: 696f 6e28 290a 0a20 2020 2020 2020 2073  ion()..        s
-00006510: 656c 662e 5f62 7566 6665 7220 3d20 6222  elf._buffer = b"
-00006520: 220a 2020 2020 2020 2020 7365 6c66 2e73  ".        self.s
-00006530: 6573 7369 6f6e 203d 2073 6573 7369 6f6e  ession = session
-00006540: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00006550: 2e68 616e 6473 6861 6b65 203d 3d20 7365  .handshake == se
-00006560: 6c66 2e48 414e 4453 4841 4b45 5f53 534f  lf.HANDSHAKE_SSO
-00006570: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00006580: 2073 656c 662e 7573 6572 2e6c 6f77 6572   self.user.lower
-00006590: 2829 2021 3d20 2222 206f 7220 7365 6c66  () != "" or self
-000065a0: 2e70 6173 7377 6f72 642e 6c6f 7765 7228  .password.lower(
-000065b0: 2920 213d 2022 223a 0a20 2020 2020 2020  ) != "":.       
-000065c0: 2020 2020 2020 2020 2023 2049 6620 6569           # If ei
-000065d0: 7468 6572 2061 7265 206e 6f6e 2d65 6d70  ther are non-emp
-000065e0: 7479 2c20 7573 6520 7468 6520 4342 435f  ty, use the CBC_
-000065f0: 4743 4d2e 0a20 2020 2020 2020 2020 2020  GCM..           
-00006600: 2020 2020 2073 656c 662e 5f63 6c69 656e       self._clien
-00006610: 745f 6861 6e64 7368 616b 655f 4342 435f  t_handshake_CBC_
-00006620: 4743 4d28 6973 5f65 7870 6c69 6369 745f  GCM(is_explicit_
-00006630: 7373 6f3d 5472 7565 2c20 666f 7263 653d  sso=True, force=
-00006640: 7365 6c66 2e66 6f72 6365 290a 2020 2020  self.force).    
-00006650: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00006660: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00006670: 2073 656c 662e 7365 7373 696f 6e20 6973   self.session is
-00006680: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00006690: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000066a0: 656c 662e 5f63 6c69 656e 745f 6861 6e64  elf._client_hand
-000066b0: 7368 616b 655f 7365 6375 7269 7479 5f74  shake_security_t
-000066c0: 6f6b 656e 2829 0a20 2020 2020 2020 2020  oken().         
-000066d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066f0: 2073 656c 662e 5f63 6c69 656e 745f 6861   self._client_ha
-00006700: 6e64 7368 616b 655f 5353 4f28 290a 2020  ndshake_SSO().  
-00006710: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00006720: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
-00006730: 6965 6e74 5f68 616e 6473 6861 6b65 5f43  ient_handshake_C
-00006740: 4243 5f47 434d 2869 735f 6578 706c 6963  BC_GCM(is_explic
-00006750: 6974 5f73 736f 3d46 616c 7365 2c20 666f  it_sso=False, fo
-00006760: 7263 653d 7365 6c66 2e66 6f72 6365 290a  rce=self.force).
-00006770: 0a20 2020 2064 6566 205f 696e 6974 6961  .    def _initia
-00006780: 6c69 7a65 5f63 6c69 656e 745f 636f 6e6e  lize_client_conn
-00006790: 6563 7469 6f6e 2873 656c 662c 2063 6c69  ection(self, cli
-000067a0: 656e 745f 636f 6e6e 6563 7469 6f6e 5f6d  ent_connection_m
-000067b0: 6573 7361 6765 293a 0a20 2020 2020 2020  essage):.       
-000067c0: 2022 2222 496e 6974 6961 6c69 7a65 7320   """Initializes 
-000067d0: 6669 656c 6473 2075 7365 6420 696e 2069  fields used in i
-000067e0: 6e69 7469 616c 2063 6c69 656e 7420 6861  nitial client ha
-000067f0: 6e64 7368 616b 6520 7265 7175 6573 7473  ndshake requests
-00006800: 2e0a 2020 2020 2020 2020 312e 2064 6174  ..        1. dat
-00006810: 6162 6173 650a 2020 2020 2020 2020 322e  abase.        2.
-00006820: 2063 6c69 656e 7469 6420 2870 796f 6369   clientid (pyoci
-00006830: 656e 7429 0a20 2020 2020 2020 2033 2e20  ent).        3. 
-00006840: 7072 6f74 6f63 6f6c 2076 6572 7369 6f6e  protocol version
-00006850: 0a20 2020 2020 2020 2034 2e20 7665 7273  .        4. vers
-00006860: 696f 6e5f 6d61 6a6f 720a 2020 2020 2020  ion_major.      
-00006870: 2020 352e 2076 6572 7369 6f6e 5f6d 696e    5. version_min
-00006880: 6f72 0a20 2020 2020 2020 2036 2e20 7365  or.        6. se
-00006890: 7373 696f 6e20 6964 0a0a 2020 2020 2020  ssion id..      
-000068a0: 2020 4e6f 7465 2c20 6e6f 7420 616c 6c20    Note, not all 
-000068b0: 6669 656c 6473 2061 7265 2069 6e69 7469  fields are initi
-000068c0: 616c 697a 6564 2e20 536f 6d65 2066 6965  alized. Some fie
-000068d0: 6c64 7320 6172 6520 7370 6563 6961 6c20  lds are special 
-000068e0: 746f 2063 6572 7461 696e 2063 6c69 656e  to certain clien
-000068f0: 7420 6861 6e64 7368 616b 6573 2e0a 2020  t handshakes..  
-00006900: 2020 2020 2020 466f 7220 6578 616d 706c        For exampl
-00006910: 652c 2074 6865 2053 534f 2068 616e 6473  e, the SSO hands
-00006920: 6861 6b65 2077 6974 6820 746f 6b65 6e20  hake with token 
-00006930: 646f 6573 206e 6f74 2074 616b 6520 7573  does not take us
-00006940: 6572 2061 6e64 2069 6e73 7465 6164 2074  er and instead t
-00006950: 616b 6573 2061 2073 6563 7572 6974 7920  akes a security 
-00006960: 746f 6b65 6e2e 0a0a 2020 2020 2020 2020  token...        
-00006970: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00006980: 2020 636c 6965 6e74 5f63 6f6e 6e65 6374    client_connect
-00006990: 696f 6e5f 6d65 7373 6167 6520 285b 7072  ion_message ([pr
-000069a0: 6f74 6f20 6d65 7373 6167 655d 293a 2074  oto message]): t
-000069b0: 6865 2063 6c69 656e 7420 6861 6e64 7368  he client handsh
-000069c0: 616b 6520 7265 7175 6573 7420 746f 2069  ake request to i
-000069d0: 6e69 7469 616c 697a 650a 2020 2020 2020  nitialize.      
-000069e0: 2020 2222 220a 2020 2020 2020 2020 636c    """.        cl
-000069f0: 6965 6e74 5f63 6f6e 6e65 6374 696f 6e5f  ient_connection_
-00006a00: 6d65 7373 6167 652e 6461 7461 6261 7365  message.database
-00006a10: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
-00006a20: 0a20 2020 2020 2020 2063 6c69 656e 745f  .        client_
-00006a30: 636f 6e6e 6563 7469 6f6e 5f6d 6573 7361  connection_messa
-00006a40: 6765 2e63 6c69 656e 7469 6420 3d20 4452  ge.clientid = DR
-00006a50: 4956 4552 5f49 440a 2020 2020 2020 2020  IVER_ID.        
-00006a60: 636c 6965 6e74 5f63 6f6e 6e65 6374 696f  client_connectio
-00006a70: 6e5f 6d65 7373 6167 652e 7665 7273 696f  n_message.versio
-00006a80: 6e20 3d20 5052 4f54 4f43 4f4c 5f56 4552  n = PROTOCOL_VER
-00006a90: 5349 4f4e 0a20 2020 2020 2020 2063 6c69  SION.        cli
-00006aa0: 656e 745f 636f 6e6e 6563 7469 6f6e 5f6d  ent_connection_m
-00006ab0: 6573 7361 6765 2e6d 616a 6f72 436c 6965  essage.majorClie
-00006ac0: 6e74 5665 7273 696f 6e20 3d20 7665 7273  ntVersion = vers
-00006ad0: 696f 6e5f 6d61 6a6f 720a 2020 2020 2020  ion_major.      
-00006ae0: 2020 636c 6965 6e74 5f63 6f6e 6e65 6374    client_connect
-00006af0: 696f 6e5f 6d65 7373 6167 652e 6d69 6e6f  ion_message.mino
-00006b00: 7243 6c69 656e 7456 6572 7369 6f6e 203d  rClientVersion =
-00006b10: 2076 6572 7369 6f6e 5f6d 696e 6f72 0a20   version_minor. 
-00006b20: 2020 2020 2020 2063 6c69 656e 745f 636f         client_co
-00006b30: 6e6e 6563 7469 6f6e 5f6d 6573 7361 6765  nnection_message
-00006b40: 2e73 6573 7369 6f6e 4944 203d 2073 656c  .sessionID = sel
-00006b50: 662e 7365 7373 696f 6e5f 6964 0a0a 2020  f.session_id..  
-00006b60: 2020 6465 6620 5f63 6c69 656e 745f 6861    def _client_ha
-00006b70: 6e64 7368 616b 655f 4342 435f 4743 4d28  ndshake_CBC_GCM(
-00006b80: 7365 6c66 2c20 6973 5f65 7870 6c69 6369  self, is_explici
-00006b90: 745f 7373 6f3d 4661 6c73 652c 2066 6f72  t_sso=False, for
-00006ba0: 6365 3d46 616c 7365 293a 0a20 2020 2020  ce=False):.     
-00006bb0: 2020 2077 6869 6c65 2054 7275 653a 0a20     while True:. 
-00006bc0: 2020 2020 2020 2020 2020 2023 2323 2323             #####
-00006bd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006be0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006bf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006c00: 2323 2323 2323 2323 2323 2323 230a 2020  #############.  
-00006c10: 2020 2020 2020 2020 2020 2320 5365 6e64            # Send
-00006c20: 2074 6865 2043 4c49 454e 545f 434f 4e4e   the CLIENT_CONN
-00006c30: 4543 5449 4f4e 2072 6571 7565 7374 0a20  ECTION request. 
-00006c40: 2020 2020 2020 2020 2020 2023 2323 2323             #####
-00006c50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006c60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006c70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006c80: 2323 2323 2323 2323 2323 2323 230a 2020  #############.  
-00006c90: 2020 2020 2020 2020 2020 7265 7120 3d20            req = 
-00006ca0: 7072 6f74 6f2e 5265 7175 6573 7428 290a  proto.Request().
-00006cb0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00006cc0: 656c 662e 6861 6e64 7368 616b 6520 3d3d  elf.handshake ==
-00006cd0: 2073 656c 662e 4841 4e44 5348 414b 455f   self.HANDSHAKE_
-00006ce0: 4342 433a 0a20 2020 2020 2020 2020 2020  CBC:.           
-00006cf0: 2020 2020 2072 6571 2e74 7970 6520 3d20       req.type = 
-00006d00: 7265 712e 434c 4945 4e54 5f43 4f4e 4e45  req.CLIENT_CONNE
-00006d10: 4354 494f 4e0a 2020 2020 2020 2020 2020  CTION.          
-00006d20: 2020 2020 2020 636c 6965 6e74 5f63 6f6e        client_con
-00006d30: 6e65 6374 696f 6e20 3d20 7265 712e 636c  nection = req.cl
-00006d40: 6965 6e74 5f63 6f6e 6e65 6374 696f 6e0a  ient_connection.
-00006d50: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00006d60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006d70: 2020 2320 5368 6f75 6c64 2062 6520 4743    # Should be GC
-00006d80: 4d0a 2020 2020 2020 2020 2020 2020 2020  M.              
-00006d90: 2020 7265 712e 7479 7065 203d 2072 6571    req.type = req
-00006da0: 2e43 4c49 454e 545f 434f 4e4e 4543 5449  .CLIENT_CONNECTI
-00006db0: 4f4e 5f47 434d 0a20 2020 2020 2020 2020  ON_GCM.         
-00006dc0: 2020 2020 2020 2063 6c69 656e 745f 636f         client_co
-00006dd0: 6e6e 6563 7469 6f6e 203d 2072 6571 2e63  nnection = req.c
-00006de0: 6c69 656e 745f 636f 6e6e 6563 7469 6f6e  lient_connection
-00006df0: 5f67 636d 0a20 2020 2020 2020 2020 2020  _gcm.           
-00006e00: 2020 2020 2063 6c69 656e 745f 636f 6e6e       client_conn
-00006e10: 6563 7469 6f6e 2e65 7870 6c69 6369 7453  ection.explicitS
-00006e20: 534f 203d 2069 735f 6578 706c 6963 6974  SO = is_explicit
-00006e30: 5f73 736f 0a20 2020 2020 2020 2020 2020  _sso.           
-00006e40: 2063 6c69 656e 745f 636f 6e6e 6563 7469   client_connecti
-00006e50: 6f6e 2e75 7365 7269 6420 3d20 7365 6c66  on.userid = self
-00006e60: 2e75 7365 720a 2020 2020 2020 2020 2020  .user.          
-00006e70: 2020 7365 6c66 2e5f 696e 6974 6961 6c69    self._initiali
-00006e80: 7a65 5f63 6c69 656e 745f 636f 6e6e 6563  ze_client_connec
-00006e90: 7469 6f6e 2863 6c69 656e 745f 636f 6e6e  tion(client_conn
-00006ea0: 6563 7469 6f6e 290a 0a20 2020 2020 2020  ection)..       
-00006eb0: 2020 2020 205f 7365 6e64 5f6d 7367 2873       _send_msg(s
-00006ec0: 656c 662c 2072 6571 290a 0a20 2020 2020  elf, req)..     
-00006ed0: 2020 2020 2020 2023 2323 2323 2323 2323         #########
-00006ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006f10: 2323 2323 2323 2323 230a 2020 2020 2020  #########.      
-00006f20: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
-00006f30: 434c 4945 4e54 5f43 4f4e 4e45 4354 494f  CLIENT_CONNECTIO
-00006f40: 4e20 7265 7370 6f6e 7365 2061 6e64 2070  N response and p
-00006f50: 726f 6365 7373 2069 740a 2020 2020 2020  rocess it.      
-00006f60: 2020 2020 2020 2323 2323 2323 2323 2323        ##########
-00006f70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006f80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006f90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006fa0: 2323 2323 2323 2323 0a20 2020 2020 2020  ########.       
-00006fb0: 2020 2020 2069 6620 7365 6c66 2e68 616e       if self.han
-00006fc0: 6473 6861 6b65 203d 3d20 7365 6c66 2e48  dshake == self.H
-00006fd0: 414e 4453 4841 4b45 5f43 4243 3a0a 2020  ANDSHAKE_CBC:.  
-00006fe0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00006ff0: 4342 430a 2020 2020 2020 2020 2020 2020  CBC.            
-00007000: 2020 2020 7273 7020 3d20 5f72 6563 765f      rsp = _recv_
-00007010: 6d73 6728 7365 6c66 2c20 7072 6f74 6f2e  msg(self, proto.
-00007020: 436c 6965 6e74 436f 6e6e 6563 7469 6f6e  ClientConnection
-00007030: 5265 7370 6f6e 7365 2829 290a 2020 2020  Response()).    
-00007040: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00007050: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00007060: 4743 4d20 6f72 2065 7870 6c69 6369 7420  GCM or explicit 
-00007070: 5353 4f0a 2020 2020 2020 2020 2020 2020  SSO.            
-00007080: 2020 2020 7273 7020 3d20 5f72 6563 765f      rsp = _recv_
-00007090: 6d73 6728 7365 6c66 2c20 7072 6f74 6f2e  msg(self, proto.
-000070a0: 436c 6965 6e74 436f 6e6e 6563 7469 6f6e  ClientConnection
-000070b0: 4743 4d52 6573 706f 6e73 6528 2929 0a0a  GCMResponse())..
-000070c0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-000070d0: 7370 2e72 6573 706f 6e73 652e 7479 7065  sp.response.type
-000070e0: 203d 3d20 7072 6f74 6f2e 436f 6e66 6972   == proto.Confir
-000070f0: 6d61 7469 6f6e 5265 7370 6f6e 7365 2e52  mationResponse.R
-00007100: 4553 504f 4e53 455f 5741 524e 3a0a 2020  ESPONSE_WARN:.  
-00007110: 2020 2020 2020 2020 2020 2020 2020 7761                wa
-00007120: 726e 2872 7370 2e72 6573 706f 6e73 652e  rn(rsp.response.
-00007130: 7265 6173 6f6e 290a 2020 2020 2020 2020  reason).        
-00007140: 2020 2020 656c 6966 206e 6f74 2072 7370      elif not rsp
-00007150: 2e72 6573 706f 6e73 652e 7479 7065 203d  .response.type =
-00007160: 3d20 7072 6f74 6f2e 436f 6e66 6972 6d61  = proto.Confirma
-00007170: 7469 6f6e 5265 7370 6f6e 7365 2e52 4553  tionResponse.RES
-00007180: 504f 4e53 455f 4f4b 3a0a 2020 2020 2020  PONSE_OK:.      
-00007190: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000071a0: 5f63 6f6e 7665 7274 5f65 7863 6570 7469  _convert_excepti
-000071b0: 6f6e 2872 7370 2e72 6573 706f 6e73 6529  on(rsp.response)
-000071c0: 0a0a 2020 2020 2020 2020 2020 2020 7065  ..            pe
-000071d0: 6572 5f6b 6579 203d 206c 6f61 645f 7065  er_key = load_pe
-000071e0: 6d5f 7075 626c 6963 5f6b 6579 2872 7370  m_public_key(rsp
-000071f0: 2e70 7562 4b65 792e 656e 636f 6465 2865  .pubKey.encode(e
-00007200: 6e63 6f64 696e 673d 2255 5446 2d38 222c  ncoding="UTF-8",
-00007210: 2065 7272 6f72 733d 2273 7472 6963 7422   errors="strict"
-00007220: 292c 2062 6163 6b65 6e64 3d64 6566 6175  ), backend=defau
-00007230: 6c74 5f62 6163 6b65 6e64 2829 290a 2020  lt_backend()).  
-00007240: 2020 2020 2020 2020 2020 2863 6970 6865            (ciphe
-00007250: 722c 2067 656e 6572 6174 6564 5f68 6d61  r, generated_hma
-00007260: 632c 2070 7562 6c69 635f 6b65 7929 203d  c, public_key) =
-00007270: 2073 656c 662e 5f65 6e63 7279 7074 696f   self._encryptio
-00007280: 6e5f 726f 7574 696e 6528 7273 702e 6976  n_routine(rsp.iv
-00007290: 2c20 7065 6572 5f6b 6579 290a 0a20 2020  , peer_key)..   
-000072a0: 2020 2020 2020 2020 2023 2323 2323 2323           #######
-000072b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000072c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000072d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000072e0: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
-000072f0: 2020 2020 2020 2020 2320 5365 6e64 2074          # Send t
-00007300: 6865 2043 4c49 454e 545f 434f 4e4e 4543  he CLIENT_CONNEC
-00007310: 5449 4f4e 3220 7265 7175 6573 740a 2020  TION2 request.  
-00007320: 2020 2020 2020 2020 2020 2323 2323 2323            ######
-00007330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007360: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
-00007370: 2020 2020 2020 2020 2072 6571 203d 2070           req = p
-00007380: 726f 746f 2e52 6571 7565 7374 2829 0a20  roto.Request(). 
-00007390: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000073a0: 6c66 2e68 616e 6473 6861 6b65 203d 3d20  lf.handshake == 
-000073b0: 7365 6c66 2e48 414e 4453 4841 4b45 5f43  self.HANDSHAKE_C
-000073c0: 4243 3a0a 2020 2020 2020 2020 2020 2020  BC:.            
-000073d0: 2020 2020 7265 712e 7479 7065 203d 2072      req.type = r
-000073e0: 6571 2e43 4c49 454e 545f 434f 4e4e 4543  eq.CLIENT_CONNEC
-000073f0: 5449 4f4e 320a 2020 2020 2020 2020 2020  TION2.          
-00007400: 2020 2020 2020 7265 712e 636c 6965 6e74        req.client
-00007410: 5f63 6f6e 6e65 6374 696f 6e32 2e63 6970  _connection2.cip
-00007420: 6865 7220 3d20 6369 7068 6572 0a20 2020  her = cipher.   
-00007430: 2020 2020 2020 2020 2020 2020 2072 6571               req
-00007440: 2e63 6c69 656e 745f 636f 6e6e 6563 7469  .client_connecti
-00007450: 6f6e 322e 666f 7263 6520 3d20 666f 7263  on2.force = forc
-00007460: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00007470: 2020 7265 712e 636c 6965 6e74 5f63 6f6e    req.client_con
-00007480: 6e65 6374 696f 6e32 2e68 6d61 6320 3d20  nection2.hmac = 
-00007490: 6765 6e65 7261 7465 645f 686d 6163 0a20  generated_hmac. 
-000074a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000074b0: 6571 2e63 6c69 656e 745f 636f 6e6e 6563  eq.client_connec
-000074c0: 7469 6f6e 322e 7075 624b 6579 203d 2070  tion2.pubKey = p
-000074d0: 7562 6c69 635f 6b65 792e 7075 626c 6963  ublic_key.public
-000074e0: 5f62 7974 6573 2865 6e63 6f64 696e 673d  _bytes(encoding=
-000074f0: 7365 7269 616c 697a 6174 696f 6e2e 456e  serialization.En
-00007500: 636f 6469 6e67 2e50 454d 2c20 666f 726d  coding.PEM, form
-00007510: 6174 3d73 6572 6961 6c69 7a61 7469 6f6e  at=serialization
-00007520: 2e50 7562 6c69 6346 6f72 6d61 742e 5375  .PublicFormat.Su
-00007530: 626a 6563 7450 7562 6c69 634b 6579 496e  bjectPublicKeyIn
-00007540: 666f 290a 2020 2020 2020 2020 2020 2020  fo).            
-00007550: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00007560: 2020 2020 2020 7265 712e 7479 7065 203d        req.type =
-00007570: 2072 6571 2e43 4c49 454e 545f 434f 4e4e   req.CLIENT_CONN
-00007580: 4543 5449 4f4e 5f47 434d 320a 2020 2020  ECTION_GCM2.    
-00007590: 2020 2020 2020 2020 2020 2020 7265 712e              req.
-000075a0: 636c 6965 6e74 5f63 6f6e 6e65 6374 696f  client_connectio
-000075b0: 6e5f 6763 6d32 2e63 6970 6865 7220 3d20  n_gcm2.cipher = 
-000075c0: 6369 7068 6572 0a20 2020 2020 2020 2020  cipher.         
-000075d0: 2020 2020 2020 2072 6571 2e63 6c69 656e         req.clien
-000075e0: 745f 636f 6e6e 6563 7469 6f6e 5f67 636d  t_connection_gcm
-000075f0: 322e 666f 7263 6520 3d20 666f 7263 650a  2.force = force.
-00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007610: 7265 712e 636c 6965 6e74 5f63 6f6e 6e65  req.client_conne
-00007620: 6374 696f 6e5f 6763 6d32 2e68 6d61 6320  ction_gcm2.hmac 
-00007630: 3d20 6765 6e65 7261 7465 645f 686d 6163  = generated_hmac
-00007640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007650: 2072 6571 2e63 6c69 656e 745f 636f 6e6e   req.client_conn
-00007660: 6563 7469 6f6e 5f67 636d 322e 6578 706c  ection_gcm2.expl
-00007670: 6963 6974 5353 4f20 3d20 6973 5f65 7870  icitSSO = is_exp
-00007680: 6c69 6369 745f 7373 6f0a 2020 2020 2020  licit_sso.      
-00007690: 2020 2020 2020 2020 2020 7265 712e 636c            req.cl
-000076a0: 6965 6e74 5f63 6f6e 6e65 6374 696f 6e5f  ient_connection_
-000076b0: 6763 6d32 2e70 7562 4b65 7920 3d20 7075  gcm2.pubKey = pu
-000076c0: 626c 6963 5f6b 6579 2e70 7562 6c69 635f  blic_key.public_
-000076d0: 6279 7465 7328 656e 636f 6469 6e67 3d73  bytes(encoding=s
-000076e0: 6572 6961 6c69 7a61 7469 6f6e 2e45 6e63  erialization.Enc
-000076f0: 6f64 696e 672e 5045 4d2c 2066 6f72 6d61  oding.PEM, forma
-00007700: 743d 7365 7269 616c 697a 6174 696f 6e2e  t=serialization.
-00007710: 5075 626c 6963 466f 726d 6174 2e53 7562  PublicFormat.Sub
-00007720: 6a65 6374 5075 626c 6963 4b65 7949 6e66  jectPublicKeyInf
-00007730: 6f29 0a0a 2020 2020 2020 2020 2020 2020  o)..            
-00007740: 5f73 656e 645f 6d73 6728 7365 6c66 2c20  _send_msg(self, 
-00007750: 7265 7129 0a0a 2020 2020 2020 2020 2020  req)..          
-00007760: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
-00007770: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007780: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007790: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000077a0: 2323 2323 0a20 2020 2020 2020 2020 2020  ####.           
-000077b0: 2023 2047 6574 2074 6865 2043 4c49 454e   # Get the CLIEN
-000077c0: 545f 434f 4e4e 4543 5449 4f4e 2072 6573  T_CONNECTION res
-000077d0: 706f 6e73 6520 616e 6420 7072 6f63 6573  ponse and proces
-000077e0: 7320 6974 0a20 2020 2020 2020 2020 2020  s it.           
-000077f0: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00002060: 2323 2323 230a 2320 496d 706f 7274 206f  #####.# Import o
+00002070: 7572 2067 6f6f 676c 6520 7072 6f74 6f62  ur google protob
+00002080: 7566 206d 6573 7361 6765 2064 6566 696e  uf message defin
+00002090: 6974 696f 6e73 0a23 2057 6520 6173 7375  itions.# We assu
+000020a0: 6d65 2074 6861 7420 7468 6520 436c 6965  me that the Clie
+000020b0: 6e74 5769 7265 5072 6f74 6f63 6f6c 5f70  ntWireProtocol_p
+000020c0: 622e 7079 2066 696c 6520 6973 2069 6e20  b.py file is in 
+000020d0: 7468 6520 7361 6d65 2064 6972 6563 746f  the same directo
+000020e0: 7279 0a23 2061 7320 7468 6973 2066 696c  ry.# as this fil
+000020f0: 650a 2323 2323 2323 2323 2323 2323 2323  e.##############
+00002100: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002110: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002130: 2323 2323 2323 2323 2323 230a 7379 732e  ###########.sys.
+00002140: 7061 7468 2e61 7070 656e 6428 6f73 2e70  path.append(os.p
+00002150: 6174 682e 6162 7370 6174 6828 6f73 2e70  ath.abspath(os.p
+00002160: 6174 682e 6469 726e 616d 6528 225f 5f66  ath.dirname("__f
+00002170: 696c 655f 5f22 2929 290a 0a23 2054 7279  ile__")))..# Try
+00002180: 2061 6e64 2069 6d70 6f72 7420 6f75 7420   and import out 
+00002190: 7072 6f74 6f62 7566 2064 6566 696e 6974  protobuf definit
+000021a0: 696f 6e73 2e0a 2320 5768 696c 6520 7765  ions..# While we
+000021b0: 2074 7261 6e73 6974 696f 6e20 746f 2062   transition to b
+000021c0: 617a 656c 2077 6520 7761 6e74 2074 6f20  azel we want to 
+000021d0: 7375 7070 6f72 7420 626f 7468 2074 6865  support both the
+000021e0: 206d 616b 6566 696c 6520 7761 7920 616e   makefile way an
+000021f0: 6420 7468 6520 6e65 7720 7761 7920 2844  d the new way (D
+00002200: 422d 3133 3934 3729 0a74 7279 3a0a 2020  B-13947).try:.  
+00002210: 2020 696d 706f 7274 2043 6c69 656e 7457    import ClientW
+00002220: 6972 6550 726f 746f 636f 6c5f 7062 3220  ireProtocol_pb2 
+00002230: 6173 2070 726f 746f 2020 2320 7079 6c69  as proto  # pyli
+00002240: 6e74 3a20 6469 7361 626c 653d 696d 706f  nt: disable=impo
+00002250: 7274 2d65 7272 6f72 2c77 726f 6e67 2d69  rt-error,wrong-i
+00002260: 6d70 6f72 742d 706f 7369 7469 6f6e 0a65  mport-position.e
+00002270: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
+00002280: 7220 6173 2065 7863 3a0a 2020 2020 6672  r as exc:.    fr
+00002290: 6f6d 2073 6861 7265 644d 6573 7361 6765  om sharedMessage
+000022a0: 7320 696d 706f 7274 2063 6c69 656e 7457  s import clientW
+000022b0: 6972 6550 726f 746f 636f 6c5f 7062 3220  ireProtocol_pb2 
+000022c0: 6173 2070 726f 746f 2020 2320 7079 6c69  as proto  # pyli
+000022d0: 6e74 3a20 6469 7361 626c 653d 696d 706f  nt: disable=impo
+000022e0: 7274 2d65 7272 6f72 2c77 726f 6e67 2d69  rt-error,wrong-i
+000022f0: 6d70 6f72 742d 706f 7369 7469 6f6e 0a0a  mport-position..
+00002300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002340: 2323 2323 2323 2323 230a 2320 4c69 6768  #########.# Ligh
+00002350: 7477 6569 6768 7420 4749 5320 636c 6173  tweight GIS clas
+00002360: 7365 730a 2323 2323 2323 2323 2323 2323  ses.############
+00002370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000023a0: 2323 2323 2323 2323 2323 2323 230a 0a0a  #############...
+000023b0: 636c 6173 7320 5f53 5450 6f69 6e74 3a0a  class _STPoint:.
+000023c0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000023d0: 2873 656c 662c 206c 6f6e 673a 2066 6c6f  (self, long: flo
+000023e0: 6174 2c20 6c61 743a 2066 6c6f 6174 293a  at, lat: float):
+000023f0: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
+00002400: 6e67 203d 206c 6f6e 670a 2020 2020 2020  ng = long.      
+00002410: 2020 7365 6c66 2e6c 6174 203d 206c 6174    self.lat = lat
+00002420: 0a0a 2020 2020 6465 6620 776b 745f 696e  ..    def wkt_in
+00002430: 6e65 7228 7365 6c66 2920 2d3e 2073 7472  ner(self) -> str
+00002440: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00002450: 2073 7472 2873 656c 662e 6c6f 6e67 2920   str(self.long) 
+00002460: 2b20 2220 2220 2b20 7374 7228 7365 6c66  + " " + str(self
+00002470: 2e6c 6174 290a 0a20 2020 2064 6566 205f  .lat)..    def _
+00002480: 5f72 6570 725f 5f28 7365 6c66 293a 0a20  _repr__(self):. 
+00002490: 2020 2020 2020 2069 6620 6973 696e 6628         if isinf(
+000024a0: 7365 6c66 2e6c 6f6e 6729 206f 7220 6973  self.long) or is
+000024b0: 696e 6628 7365 6c66 2e6c 6174 293a 0a20  inf(self.lat):. 
+000024c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000024d0: 6e20 2250 4f49 4e54 2045 4d50 5459 220a  n "POINT EMPTY".
+000024e0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
+000024f0: 504f 494e 5428 2220 2b20 7365 6c66 2e77  POINT(" + self.w
+00002500: 6b74 5f69 6e6e 6572 2829 202b 2022 2922  kt_inner() + ")"
+00002510: 0a0a 2020 2020 6465 6620 5f5f 6571 5f5f  ..    def __eq__
+00002520: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
+00002530: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00002540: 616e 6365 286f 7468 6572 2c20 5f53 5450  ance(other, _STP
+00002550: 6f69 6e74 293a 0a20 2020 2020 2020 2020  oint):.         
+00002560: 2020 2072 6574 7572 6e20 7365 6c66 2e6c     return self.l
+00002570: 6f6e 6720 3d3d 206f 7468 6572 2e6c 6f6e  ong == other.lon
+00002580: 6720 616e 6420 7365 6c66 2e6c 6174 203d  g and self.lat =
+00002590: 3d20 6f74 6865 722e 6c61 740a 2020 2020  = other.lat.    
+000025a0: 2020 2020 7265 7475 726e 204e 6f74 496d      return NotIm
+000025b0: 706c 656d 656e 7465 640a 0a0a 6465 6620  plemented...def 
+000025c0: 5f6c 696e 6573 7472 696e 675f 776b 745f  _linestring_wkt_
+000025d0: 696e 6e65 7228 706f 696e 7473 3a20 4c69  inner(points: Li
+000025e0: 7374 5b5f 5354 506f 696e 745d 2920 2d3e  st[_STPoint]) ->
+000025f0: 2073 7472 3a0a 2020 2020 7265 7475 726e   str:.    return
+00002600: 2022 2822 202b 2022 2c20 222e 6a6f 696e   "(" + ", ".join
+00002610: 2828 702e 776b 745f 696e 6e65 7228 2920  ((p.wkt_inner() 
+00002620: 666f 7220 7020 696e 2070 6f69 6e74 7329  for p in points)
+00002630: 2920 2b20 2229 220a 0a0a 636c 6173 7320  ) + ")"...class 
+00002640: 5f53 544c 696e 6573 7472 696e 673a 0a20  _STLinestring:. 
+00002650: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00002660: 7365 6c66 2c20 706f 696e 7473 3a20 4c69  self, points: Li
+00002670: 7374 5b5f 5354 506f 696e 745d 293a 0a20  st[_STPoint]):. 
+00002680: 2020 2020 2020 2073 656c 662e 706f 696e         self.poin
+00002690: 7473 203d 2070 6f69 6e74 730a 0a20 2020  ts = points..   
+000026a0: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
+000026b0: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+000026c0: 6e6f 7420 7365 6c66 2e70 6f69 6e74 733a  not self.points:
+000026d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000026e0: 7572 6e20 224c 494e 4553 5452 494e 4720  urn "LINESTRING 
+000026f0: 454d 5054 5922 0a20 2020 2020 2020 2072  EMPTY".        r
+00002700: 6574 7572 6e20 224c 494e 4553 5452 494e  eturn "LINESTRIN
+00002710: 4722 202b 205f 6c69 6e65 7374 7269 6e67  G" + _linestring
+00002720: 5f77 6b74 5f69 6e6e 6572 2873 656c 662e  _wkt_inner(self.
+00002730: 706f 696e 7473 290a 0a20 2020 2064 6566  points)..    def
+00002740: 205f 5f65 715f 5f28 7365 6c66 2c20 6f74   __eq__(self, ot
+00002750: 6865 7229 3a0a 2020 2020 2020 2020 2320  her):.        # 
+00002760: 7374 7269 6374 2065 7175 616c 6974 792c  strict equality,
+00002770: 206e 6f74 2073 656d 616e 7469 630a 2020   not semantic.  
+00002780: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00002790: 6e63 6528 6f74 6865 722c 205f 5354 4c69  nce(other, _STLi
+000027a0: 6e65 7374 7269 6e67 293a 0a20 2020 2020  nestring):.     
+000027b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000027c0: 6c66 2e70 6f69 6e74 7320 3d3d 206f 7468  lf.points == oth
+000027d0: 6572 2e70 6f69 6e74 730a 2020 2020 2020  er.points.      
+000027e0: 2020 7265 7475 726e 204e 6f74 496d 706c    return NotImpl
+000027f0: 656d 656e 7465 640a 0a0a 636c 6173 7320  emented...class 
+00002800: 5f53 5450 6f6c 7967 6f6e 3a0a 2020 2020  _STPolygon:.    
+00002810: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00002820: 662c 2065 7874 6572 696f 723a 204c 6973  f, exterior: Lis
+00002830: 745b 5f53 5450 6f69 6e74 5d2c 2068 6f6c  t[_STPoint], hol
+00002840: 6573 3a20 4c69 7374 5b4c 6973 745b 5f53  es: List[List[_S
+00002850: 5450 6f69 6e74 5d5d 293a 0a20 2020 2020  TPoint]]):.     
+00002860: 2020 2073 656c 662e 6578 7465 7269 6f72     self.exterior
+00002870: 203d 2065 7874 6572 696f 720a 2020 2020   = exterior.    
+00002880: 2020 2020 7365 6c66 2e68 6f6c 6573 203d      self.holes =
+00002890: 2068 6f6c 6573 0a0a 2020 2020 6465 6620   holes..    def 
+000028a0: 5f5f 7265 7072 5f5f 2873 656c 6629 3a0a  __repr__(self):.
+000028b0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+000028c0: 656c 662e 6578 7465 7269 6f72 3a0a 2020  elf.exterior:.  
+000028d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000028e0: 2022 504f 4c59 474f 4e20 454d 5054 5922   "POLYGON EMPTY"
+000028f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002900: 2250 4f4c 5947 4f4e 2822 202b 2022 2c20  "POLYGON(" + ", 
+00002910: 222e 6a6f 696e 2828 5f6c 696e 6573 7472  ".join((_linestr
+00002920: 696e 675f 776b 745f 696e 6e65 7228 706c  ing_wkt_inner(pl
+00002930: 2920 666f 7220 706c 2069 6e20 5b73 656c  ) for pl in [sel
+00002940: 662e 6578 7465 7269 6f72 5d20 2b20 7365  f.exterior] + se
+00002950: 6c66 2e68 6f6c 6573 2929 202b 2022 2922  lf.holes)) + ")"
+00002960: 0a0a 2020 2020 6465 6620 5f5f 6571 5f5f  ..    def __eq__
+00002970: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
+00002980: 2020 2020 2020 2023 2073 7472 6963 7420         # strict 
+00002990: 6571 7561 6c69 7479 2c20 6e6f 7420 7365  equality, not se
+000029a0: 6d61 6e74 6963 0a20 2020 2020 2020 2069  mantic.        i
+000029b0: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
+000029c0: 6572 2c20 5f53 5450 6f6c 7967 6f6e 293a  er, _STPolygon):
+000029d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000029e0: 7572 6e20 7365 6c66 2e65 7874 6572 696f  urn self.exterio
+000029f0: 7220 3d3d 206f 7468 6572 2e65 7874 6572  r == other.exter
+00002a00: 696f 7220 616e 6420 7365 6c66 2e68 6f6c  ior and self.hol
+00002a10: 6573 203d 3d20 6f74 6865 722e 686f 6c65  es == other.hole
+00002a20: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
+00002a30: 204e 6f74 496d 706c 656d 656e 7465 640a   NotImplemented.
+00002a40: 0a0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+00002a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002a60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002a70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002a80: 2323 2323 2323 2323 2323 230a 2320 4275  ###########.# Bu
+00002a90: 696c 6420 7375 7070 6f72 7465 6420 7265  ild supported re
+00002aa0: 7175 6573 742f 7265 7370 6f6e 7365 2074  quest/response t
+00002ab0: 7970 6520 6d61 7070 696e 6773 0a23 2323  ype mappings.###
+00002ac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002ad0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002ae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002af0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002b00: 2323 2323 2323 0a0a 0a63 6c61 7373 205f  ######...class _
+00002b10: 4f63 6965 6e74 5265 7175 6573 7446 6163  OcientRequestFac
+00002b20: 746f 7279 3a0a 2020 2020 6465 6620 7265  tory:.    def re
+00002b30: 7175 6573 7428 7365 6c66 2c20 6f70 6572  quest(self, oper
+00002b40: 6174 696f 6e3a 2073 7472 293a 0a20 2020  ation: str):.   
+00002b50: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
+00002b60: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
+00002b70: 7465 6420 7265 7175 6573 7420 7072 6f74  ted request prot
+00002b80: 6f62 7566 2222 220a 2020 2020 2020 2020  obuf""".        
+00002b90: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+00002ba0: 6e74 6564 4572 726f 720a 0a20 2020 2064  ntedError..    d
+00002bb0: 6566 2072 6573 706f 6e73 6528 7365 6c66  ef response(self
+00002bc0: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
+00002bd0: 6e65 7261 7465 7320 6120 6675 6c6c 7920  nerates a fully 
+00002be0: 706f 7075 6c61 7465 6420 7265 7370 6f6e  populated respon
+00002bf0: 7365 2070 726f 746f 6275 6622 2222 0a20  se protobuf""". 
+00002c00: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+00002c10: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00002c20: 0a0a 2020 2020 6465 6620 7072 6f63 6573  ..    def proces
+00002c30: 7328 7365 6c66 2c20 7273 7029 202d 3e20  s(self, rsp) -> 
+00002c40: 416e 793a 0a20 2020 2020 2020 2022 2222  Any:.        """
+00002c50: 5072 6f63 6573 7320 7468 6520 636c 6965  Process the clie
+00002c60: 6e74 2072 6573 706f 6e73 6522 2222 0a20  nt response""". 
+00002c70: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+00002c80: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00002c90: 0a0a 0a63 6c61 7373 205f 4578 6563 7574  ...class _Execut
+00002ca0: 6551 7565 7279 4661 6374 6f72 7928 5f4f  eQueryFactory(_O
+00002cb0: 6369 656e 7452 6571 7565 7374 4661 6374  cientRequestFact
+00002cc0: 6f72 7929 3a0a 2020 2020 6465 6620 7265  ory):.    def re
+00002cd0: 7175 6573 7428 7365 6c66 2c20 6f70 6572  quest(self, oper
+00002ce0: 6174 696f 6e3a 2073 7472 293a 0a20 2020  ation: str):.   
+00002cf0: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
+00002d00: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
+00002d10: 7465 6420 4558 4543 5554 455f 5155 4552  ted EXECUTE_QUER
+00002d20: 5920 7265 7175 6573 7420 7072 6f74 6f62  Y request protob
+00002d30: 7566 2222 220a 2020 2020 2020 2020 7265  uf""".        re
+00002d40: 7120 3d20 7072 6f74 6f2e 5265 7175 6573  q = proto.Reques
+00002d50: 7428 290a 2020 2020 2020 2020 7265 712e  t().        req.
+00002d60: 7479 7065 203d 2070 726f 746f 2e52 6571  type = proto.Req
+00002d70: 7565 7374 2e52 6571 7565 7374 5479 7065  uest.RequestType
+00002d80: 2e56 616c 7565 2822 4558 4543 5554 455f  .Value("EXECUTE_
+00002d90: 5155 4552 5922 290a 2020 2020 2020 2020  QUERY").        
+00002da0: 7265 712e 6578 6563 7574 655f 7175 6572  req.execute_quer
+00002db0: 792e 7371 6c20 3d20 6f70 6572 6174 696f  y.sql = operatio
+00002dc0: 6e0a 2020 2020 2020 2020 7265 712e 6578  n.        req.ex
+00002dd0: 6563 7574 655f 7175 6572 792e 666f 7263  ecute_query.forc
+00002de0: 6520 3d20 4661 6c73 650a 2020 2020 2020  e = False.      
+00002df0: 2020 7265 7475 726e 2072 6571 0a0a 2020    return req..  
+00002e00: 2020 6465 6620 7265 7370 6f6e 7365 2873    def response(s
+00002e10: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00002e20: 2247 656e 6572 6174 6573 2061 2066 756c  "Generates a ful
+00002e30: 6c79 2070 6f70 756c 6174 6564 2045 5845  ly populated EXE
+00002e40: 4355 5445 5f51 5545 5259 2072 6573 706f  CUTE_QUERY respo
+00002e50: 6e73 6520 7072 6f74 6f62 7566 2222 220a  nse protobuf""".
+00002e60: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+00002e70: 726f 746f 2e45 7865 6375 7465 5175 6572  roto.ExecuteQuer
+00002e80: 7952 6573 706f 6e73 6528 290a 0a0a 636c  yResponse()...cl
+00002e90: 6173 7320 5f45 7865 6375 7465 4578 706c  ass _ExecuteExpl
+00002ea0: 6169 6e46 6163 746f 7279 285f 4f63 6965  ainFactory(_Ocie
+00002eb0: 6e74 5265 7175 6573 7446 6163 746f 7279  ntRequestFactory
+00002ec0: 293a 0a20 2020 2064 6566 2072 6571 7565  ):.    def reque
+00002ed0: 7374 2873 656c 662c 206f 7065 7261 7469  st(self, operati
+00002ee0: 6f6e 3a20 7374 7229 3a0a 2020 2020 2020  on: str):.      
+00002ef0: 2020 2222 2247 656e 6572 6174 6573 2061    """Generates a
+00002f00: 2066 756c 6c79 2070 6f70 756c 6174 6564   fully populated
+00002f10: 2045 5845 4355 5445 5f45 5850 4c41 494e   EXECUTE_EXPLAIN
+00002f20: 2072 6571 7565 7374 2070 726f 746f 6275   request protobu
+00002f30: 6622 2222 0a20 2020 2020 2020 2072 6571  f""".        req
+00002f40: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
+00002f50: 2829 0a20 2020 2020 2020 2072 6571 2e74  ().        req.t
+00002f60: 7970 6520 3d20 7072 6f74 6f2e 5265 7175  ype = proto.Requ
+00002f70: 6573 742e 5265 7175 6573 7454 7970 652e  est.RequestType.
+00002f80: 5661 6c75 6528 2245 5845 4355 5445 5f45  Value("EXECUTE_E
+00002f90: 5850 4c41 494e 2229 0a20 2020 2020 2020  XPLAIN").       
+00002fa0: 2072 6571 2e65 7865 6375 7465 5f65 7870   req.execute_exp
+00002fb0: 6c61 696e 2e66 6f72 6d61 7420 3d20 7072  lain.format = pr
+00002fc0: 6f74 6f2e 4578 706c 6169 6e46 6f72 6d61  oto.ExplainForma
+00002fd0: 742e 4a53 4f4e 0a20 2020 2020 2020 2073  t.JSON.        s
+00002fe0: 706c 6974 7465 6420 3d20 6f70 6572 6174  plitted = operat
+00002ff0: 696f 6e2e 7370 6c69 7428 6d61 7873 706c  ion.split(maxspl
+00003000: 6974 3d31 290a 2020 2020 2020 2020 6966  it=1).        if
+00003010: 206c 656e 2873 706c 6974 7465 6429 203d   len(splitted) =
+00003020: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
+00003030: 2072 6571 2e65 7865 6375 7465 5f65 7870   req.execute_exp
+00003040: 6c61 696e 2e73 716c 203d 2073 706c 6974  lain.sql = split
+00003050: 7465 645b 315d 0a20 2020 2020 2020 2072  ted[1].        r
+00003060: 6574 7572 6e20 7265 710a 0a20 2020 2064  eturn req..    d
+00003070: 6566 2072 6573 706f 6e73 6528 7365 6c66  ef response(self
+00003080: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
+00003090: 6e65 7261 7465 7320 6120 6675 6c6c 7920  nerates a fully 
+000030a0: 706f 7075 6c61 7465 6420 4558 4543 5554  populated EXECUT
+000030b0: 455f 4558 504c 4149 4e20 7265 7370 6f6e  E_EXPLAIN respon
+000030c0: 7365 2070 726f 746f 6275 6622 2222 0a20  se protobuf""". 
+000030d0: 2020 2020 2020 2072 6574 7572 6e20 7072         return pr
+000030e0: 6f74 6f2e 4578 706c 6169 6e52 6573 706f  oto.ExplainRespo
+000030f0: 6e73 6553 7472 696e 6750 6c61 6e28 290a  nseStringPlan().
+00003100: 0a0a 636c 6173 7320 5f45 7865 6375 7465  ..class _Execute
+00003110: 4578 706f 7274 4661 6374 6f72 7928 5f4f  ExportFactory(_O
+00003120: 6369 656e 7452 6571 7565 7374 4661 6374  cientRequestFact
+00003130: 6f72 7929 3a0a 2020 2020 6465 6620 7265  ory):.    def re
+00003140: 7175 6573 7428 7365 6c66 2c20 6f70 6572  quest(self, oper
+00003150: 6174 696f 6e3a 2073 7472 293a 0a20 2020  ation: str):.   
+00003160: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
+00003170: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
+00003180: 7465 6420 4558 4543 5554 455f 4558 504f  ted EXECUTE_EXPO
+00003190: 5254 2072 6571 7565 7374 2070 726f 746f  RT request proto
+000031a0: 6275 6622 2222 0a20 2020 2020 2020 2072  buf""".        r
+000031b0: 6571 203d 2070 726f 746f 2e52 6571 7565  eq = proto.Reque
+000031c0: 7374 2829 0a20 2020 2020 2020 2072 6571  st().        req
+000031d0: 2e74 7970 6520 3d20 7072 6f74 6f2e 5265  .type = proto.Re
+000031e0: 7175 6573 742e 5265 7175 6573 7454 7970  quest.RequestTyp
+000031f0: 652e 5661 6c75 6528 2245 5845 4355 5445  e.Value("EXECUTE
+00003200: 5f45 5850 4f52 5422 290a 2020 2020 2020  _EXPORT").      
+00003210: 2020 7265 712e 6578 6563 7574 655f 6578    req.execute_ex
+00003220: 706f 7274 2e73 716c 203d 206f 7065 7261  port.sql = opera
+00003230: 7469 6f6e 0a20 2020 2020 2020 2072 6574  tion.        ret
+00003240: 7572 6e20 7265 710a 0a20 2020 2064 6566  urn req..    def
+00003250: 2072 6573 706f 6e73 6528 7365 6c66 293a   response(self):
+00003260: 0a20 2020 2020 2020 2022 2222 4765 6e65  .        """Gene
+00003270: 7261 7465 7320 6120 6675 6c6c 7920 706f  rates a fully po
+00003280: 7075 6c61 7465 6420 4558 4543 5554 455f  pulated EXECUTE_
+00003290: 4558 504f 5254 2072 6573 706f 6e73 6520  EXPORT response 
+000032a0: 7072 6f74 6f62 7566 2222 220a 2020 2020  protobuf""".    
+000032b0: 2020 2020 7265 7475 726e 2070 726f 746f      return proto
+000032c0: 2e45 7865 6375 7465 4578 706f 7274 5265  .ExecuteExportRe
+000032d0: 7370 6f6e 7365 2829 0a0a 0a63 6c61 7373  sponse()...class
+000032e0: 205f 4578 706c 6169 6e50 6970 656c 696e   _ExplainPipelin
+000032f0: 6546 6163 746f 7279 285f 4f63 6965 6e74  eFactory(_Ocient
+00003300: 5265 7175 6573 7446 6163 746f 7279 293a  RequestFactory):
+00003310: 0a20 2020 2064 6566 2072 6571 7565 7374  .    def request
+00003320: 2873 656c 662c 206f 7065 7261 7469 6f6e  (self, operation
+00003330: 3a20 7374 7229 3a0a 2020 2020 2020 2020  : str):.        
+00003340: 2222 2247 656e 6572 6174 6573 2061 2066  """Generates a f
+00003350: 756c 6c79 2070 6f70 756c 6174 6564 2045  ully populated E
+00003360: 5850 4c41 494e 5f50 4950 454c 494e 4520  XPLAIN_PIPELINE 
+00003370: 7265 7175 6573 7420 7072 6f74 6f62 7566  request protobuf
+00003380: 2222 220a 2020 2020 2020 2020 7265 7120  """.        req 
+00003390: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
+000033a0: 290a 2020 2020 2020 2020 7265 712e 7479  ).        req.ty
+000033b0: 7065 203d 2070 726f 746f 2e52 6571 7565  pe = proto.Reque
+000033c0: 7374 2e52 6571 7565 7374 5479 7065 2e56  st.RequestType.V
+000033d0: 616c 7565 2822 4558 504c 4149 4e5f 5049  alue("EXPLAIN_PI
+000033e0: 5045 4c49 4e45 2229 0a20 2020 2020 2020  PELINE").       
+000033f0: 2072 6571 2e65 7870 6c61 696e 5f70 6970   req.explain_pip
+00003400: 656c 696e 652e 7371 6c20 3d20 6f70 6572  eline.sql = oper
+00003410: 6174 696f 6e0a 2020 2020 2020 2020 7265  ation.        re
+00003420: 7475 726e 2072 6571 0a0a 2020 2020 6465  turn req..    de
+00003430: 6620 7265 7370 6f6e 7365 2873 656c 6629  f response(self)
+00003440: 3a0a 2020 2020 2020 2020 2222 2247 656e  :.        """Gen
+00003450: 6572 6174 6573 2061 2066 756c 6c79 2070  erates a fully p
+00003460: 6f70 756c 6174 6564 2045 5850 4c41 494e  opulated EXPLAIN
+00003470: 5f50 4950 454c 494e 4520 7265 7370 6f6e  _PIPELINE respon
+00003480: 7365 2070 726f 746f 6275 6622 2222 0a20  se protobuf""". 
+00003490: 2020 2020 2020 2072 6574 7572 6e20 7072         return pr
+000034a0: 6f74 6f2e 4578 706c 6169 6e50 6970 656c  oto.ExplainPipel
+000034b0: 696e 6552 6573 706f 6e73 6528 290a 0a0a  ineResponse()...
+000034c0: 636c 6173 7320 5f43 6865 636b 4461 7461  class _CheckData
+000034d0: 4661 6374 6f72 7928 5f4f 6369 656e 7452  Factory(_OcientR
+000034e0: 6571 7565 7374 4661 6374 6f72 7929 3a0a  equestFactory):.
+000034f0: 2020 2020 6465 6620 7265 7175 6573 7428      def request(
+00003500: 7365 6c66 2c20 6f70 6572 6174 696f 6e3a  self, operation:
+00003510: 2073 7472 293a 0a20 2020 2020 2020 2022   str):.        "
+00003520: 2222 4765 6e65 7261 7465 7320 6120 6675  ""Generates a fu
+00003530: 6c6c 7920 706f 7075 6c61 7465 6420 4348  lly populated CH
+00003540: 4543 4b5f 4441 5441 2072 6571 7565 7374  ECK_DATA request
+00003550: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
+00003560: 2020 2020 2072 6571 203d 2070 726f 746f       req = proto
+00003570: 2e52 6571 7565 7374 2829 0a20 2020 2020  .Request().     
+00003580: 2020 2072 6571 2e74 7970 6520 3d20 7072     req.type = pr
+00003590: 6f74 6f2e 5265 7175 6573 742e 5265 7175  oto.Request.Requ
+000035a0: 6573 7454 7970 652e 5661 6c75 6528 2243  estType.Value("C
+000035b0: 4845 434b 5f44 4154 4122 290a 2020 2020  HECK_DATA").    
+000035c0: 2020 2020 7265 712e 6368 6563 6b5f 6461      req.check_da
+000035d0: 7461 2e73 716c 203d 206f 7065 7261 7469  ta.sql = operati
+000035e0: 6f6e 0a20 2020 2020 2020 2072 6574 7572  on.        retur
+000035f0: 6e20 7265 710a 0a20 2020 2064 6566 2072  n req..    def r
+00003600: 6573 706f 6e73 6528 7365 6c66 293a 0a20  esponse(self):. 
+00003610: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
+00003620: 7465 7320 6120 6675 6c6c 7920 706f 7075  tes a fully popu
+00003630: 6c61 7465 6420 4348 4543 4b5f 4441 5441  lated CHECK_DATA
+00003640: 2072 6573 706f 6e73 6520 7072 6f74 6f62   response protob
+00003650: 7566 2222 220a 2020 2020 2020 2020 7265  uf""".        re
+00003660: 7475 726e 2070 726f 746f 2e43 6865 636b  turn proto.Check
+00003670: 4461 7461 5265 7370 6f6e 7365 2829 0a0a  DataResponse()..
+00003680: 0a63 6c61 7373 205f 466f 7263 6545 7874  .class _ForceExt
+00003690: 6572 6e61 6c46 6163 746f 7279 285f 4f63  ernalFactory(_Oc
+000036a0: 6965 6e74 5265 7175 6573 7446 6163 746f  ientRequestFacto
+000036b0: 7279 293a 0a20 2020 2064 6566 2072 6571  ry):.    def req
+000036c0: 7565 7374 2873 656c 662c 206f 7065 7261  uest(self, opera
+000036d0: 7469 6f6e 3a20 7374 7229 3a0a 2020 2020  tion: str):.    
+000036e0: 2020 2020 2222 2247 656e 6572 6174 6573      """Generates
+000036f0: 2061 2066 756c 6c79 2070 6f70 756c 6174   a fully populat
+00003700: 6564 2046 4f52 4345 5f45 5854 4552 4e41  ed FORCE_EXTERNA
+00003710: 4c20 7265 7175 6573 7420 7072 6f74 6f62  L request protob
+00003720: 7566 2222 220a 2020 2020 2020 2020 7265  uf""".        re
+00003730: 7120 3d20 7072 6f74 6f2e 5265 7175 6573  q = proto.Reques
+00003740: 7428 290a 2020 2020 2020 2020 7265 712e  t().        req.
+00003750: 7479 7065 203d 2070 726f 746f 2e52 6571  type = proto.Req
+00003760: 7565 7374 2e52 6571 7565 7374 5479 7065  uest.RequestType
+00003770: 2e56 616c 7565 2822 5345 545f 5041 5241  .Value("SET_PARA
+00003780: 4d45 5445 5222 290a 2020 2020 2020 2020  METER").        
+00003790: 7370 203d 2072 6571 2e73 6574 5f70 6172  sp = req.set_par
+000037a0: 616d 6574 6572 0a20 2020 2020 2020 2069  ameter.        i
+000037b0: 6620 6f70 6572 6174 696f 6e2e 656e 6473  f operation.ends
+000037c0: 7769 7468 2822 6f6e 2229 3a0a 2020 2020  with("on"):.    
+000037d0: 2020 2020 2020 2020 7370 2e66 6f72 6365          sp.force
+000037e0: 5f65 7874 6572 6e61 6c2e 6973 5f6f 6e20  _external.is_on 
+000037f0: 3d20 5472 7565 0a20 2020 2020 2020 2065  = True.        e
+00003800: 6c69 6620 6f70 6572 6174 696f 6e2e 656e  lif operation.en
+00003810: 6473 7769 7468 2822 6f66 6622 293a 0a20  dswith("off"):. 
+00003820: 2020 2020 2020 2020 2020 2073 702e 666f             sp.fo
+00003830: 7263 655f 6578 7465 726e 616c 2e69 735f  rce_external.is_
+00003840: 6f6e 203d 2046 616c 7365 0a20 2020 2020  on = False.     
+00003850: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00003860: 2020 2020 2072 6169 7365 2053 796e 7461       raise Synta
+00003870: 7845 7272 6f72 2827 466f 726d 6174 206d  xError('Format m
+00003880: 7573 7420 6265 2022 464f 5243 4520 4558  ust be "FORCE EX
+00003890: 5445 524e 414c 2028 6f6e 7c6f 6666 2922  TERNAL (on|off)"
+000038a0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+000038b0: 6e20 7265 710a 0a20 2020 2064 6566 2072  n req..    def r
+000038c0: 6573 706f 6e73 6528 7365 6c66 293a 0a20  esponse(self):. 
+000038d0: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
+000038e0: 7465 7320 6120 6675 6c6c 7920 706f 7075  tes a fully popu
+000038f0: 6c61 7465 6420 464f 5243 455f 4558 5445  lated FORCE_EXTE
+00003900: 524e 414c 2072 6573 706f 6e73 6520 7072  RNAL response pr
+00003910: 6f74 6f62 7566 2222 220a 2020 2020 2020  otobuf""".      
+00003920: 2020 7265 7475 726e 2070 726f 746f 2e43    return proto.C
+00003930: 6f6e 6669 726d 6174 696f 6e52 6573 706f  onfirmationRespo
+00003940: 6e73 6528 290a 0a0a 636c 6173 7320 5f53  nse()...class _S
+00003950: 6574 5363 6865 6d61 4661 6374 6f72 7928  etSchemaFactory(
+00003960: 5f4f 6369 656e 7452 6571 7565 7374 4661  _OcientRequestFa
+00003970: 6374 6f72 7929 3a0a 2020 2020 6465 6620  ctory):.    def 
+00003980: 7265 7175 6573 7428 7365 6c66 2c20 7363  request(self, sc
+00003990: 6865 6d61 3a20 7374 7229 3a0a 2020 2020  hema: str):.    
+000039a0: 2020 2020 2222 2247 656e 6572 6174 6573      """Generates
+000039b0: 2061 2066 756c 6c79 2070 6f70 756c 6174   a fully populat
+000039c0: 6564 2053 4554 2053 4348 454d 4120 7265  ed SET SCHEMA re
+000039d0: 7175 6573 7420 7072 6f74 6f62 7566 2222  quest protobuf""
+000039e0: 220a 2020 2020 2020 2020 7265 7120 3d20  ".        req = 
+000039f0: 7072 6f74 6f2e 5265 7175 6573 7428 290a  proto.Request().
+00003a00: 2020 2020 2020 2020 7265 712e 7479 7065          req.type
+00003a10: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
+00003a20: 2e52 6571 7565 7374 5479 7065 2e56 616c  .RequestType.Val
+00003a30: 7565 2822 5345 545f 5343 4845 4d41 2229  ue("SET_SCHEMA")
+00003a40: 0a20 2020 2020 2020 2072 6571 2e73 6574  .        req.set
+00003a50: 5f73 6368 656d 612e 7363 6865 6d61 203d  _schema.schema =
+00003a60: 2073 6368 656d 610a 2020 2020 2020 2020   schema.        
+00003a70: 7265 7475 726e 2072 6571 0a0a 2020 2020  return req..    
+00003a80: 6465 6620 7265 7370 6f6e 7365 2873 656c  def response(sel
+00003a90: 6629 3a0a 2020 2020 2020 2020 2222 2247  f):.        """G
+00003aa0: 656e 6572 6174 6573 2053 4554 5f53 4348  enerates SET_SCH
+00003ab0: 454d 4120 7265 7370 6f6e 7365 2070 726f  EMA response pro
+00003ac0: 746f 6275 6622 2222 0a20 2020 2020 2020  tobuf""".       
+00003ad0: 2072 6574 7572 6e20 7072 6f74 6f2e 436f   return proto.Co
+00003ae0: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
+00003af0: 7365 2829 0a0a 0a63 6c61 7373 205f 4765  se()...class _Ge
+00003b00: 7453 6368 656d 6146 6163 746f 7279 285f  tSchemaFactory(_
+00003b10: 4f63 6965 6e74 5265 7175 6573 7446 6163  OcientRequestFac
+00003b20: 746f 7279 293a 0a20 2020 2064 6566 2072  tory):.    def r
+00003b30: 6571 7565 7374 2873 656c 6629 3a0a 2020  equest(self):.  
+00003b40: 2020 2020 2020 2222 2247 656e 6572 6174        """Generat
+00003b50: 6573 2061 2066 756c 6c79 2070 6f70 756c  es a fully popul
+00003b60: 6174 6564 2047 4554 2053 4348 454d 4120  ated GET SCHEMA 
+00003b70: 7265 7175 6573 7420 7072 6f74 6f62 7566  request protobuf
+00003b80: 2222 220a 2020 2020 2020 2020 7265 7120  """.        req 
+00003b90: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
+00003ba0: 290a 2020 2020 2020 2020 7265 712e 7479  ).        req.ty
+00003bb0: 7065 203d 2070 726f 746f 2e52 6571 7565  pe = proto.Reque
+00003bc0: 7374 2e52 6571 7565 7374 5479 7065 2e56  st.RequestType.V
+00003bd0: 616c 7565 2822 4745 545f 5343 4845 4d41  alue("GET_SCHEMA
+00003be0: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+00003bf0: 6e20 7265 710a 0a20 2020 2064 6566 2072  n req..    def r
+00003c00: 6573 706f 6e73 6528 7365 6c66 293a 0a20  esponse(self):. 
+00003c10: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
+00003c20: 7465 7320 5345 545f 5343 4845 4d41 2072  tes SET_SCHEMA r
+00003c30: 6573 706f 6e73 6520 7072 6f74 6f62 7566  esponse protobuf
+00003c40: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00003c50: 726e 2070 726f 746f 2e47 6574 5363 6865  rn proto.GetSche
+00003c60: 6d61 5265 7370 6f6e 7365 2829 0a0a 0a63  maResponse()...c
+00003c70: 6c61 7373 205f 436c 6561 7243 6163 6865  lass _ClearCache
+00003c80: 4661 6374 6f72 7928 5f4f 6369 656e 7452  Factory(_OcientR
+00003c90: 6571 7565 7374 4661 6374 6f72 7929 3a0a  equestFactory):.
+00003ca0: 2020 2020 6465 6620 7265 7175 6573 7428      def request(
+00003cb0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00003cc0: 2222 4765 6e65 7261 7465 7320 6120 6675  ""Generates a fu
+00003cd0: 6c6c 7920 706f 7075 6c61 7465 6420 434c  lly populated CL
+00003ce0: 4541 5220 4341 4348 4520 7265 7175 6573  EAR CACHE reques
+00003cf0: 7420 7072 6f74 6f62 7566 2222 220a 2020  t protobuf""".  
+00003d00: 2020 2020 2020 7265 7120 3d20 7072 6f74        req = prot
+00003d10: 6f2e 5265 7175 6573 7428 290a 2020 2020  o.Request().    
+00003d20: 2020 2020 7265 712e 7479 7065 203d 2070      req.type = p
+00003d30: 726f 746f 2e52 6571 7565 7374 2e52 6571  roto.Request.Req
+00003d40: 7565 7374 5479 7065 2e56 616c 7565 2822  uestType.Value("
+00003d50: 434c 4541 525f 4341 4348 4522 290a 2020  CLEAR_CACHE").  
+00003d60: 2020 2020 2020 7265 712e 636c 6561 725f        req.clear_
+00003d70: 6361 6368 652e 616c 6c5f 6e6f 6465 7320  cache.all_nodes 
+00003d80: 3d20 5472 7565 0a20 2020 2020 2020 2072  = True.        r
+00003d90: 6574 7572 6e20 7265 710a 0a20 2020 2064  eturn req..    d
+00003da0: 6566 2072 6573 706f 6e73 6528 7365 6c66  ef response(self
+00003db0: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
+00003dc0: 6e65 7261 7465 7320 5345 545f 5343 4845  nerates SET_SCHE
+00003dd0: 4d41 2072 6573 706f 6e73 6520 7072 6f74  MA response prot
+00003de0: 6f62 7566 2222 220a 2020 2020 2020 2020  obuf""".        
+00003df0: 7265 7475 726e 2070 726f 746f 2e43 6f6e  return proto.Con
+00003e00: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
+00003e10: 6528 290a 0a0a 636c 6173 7320 5f53 6574  e()...class _Set
+00003e20: 5061 7261 6d65 7465 7246 6163 746f 7279  ParameterFactory
+00003e30: 285f 4f63 6965 6e74 5265 7175 6573 7446  (_OcientRequestF
+00003e40: 6163 746f 7279 293a 0a20 2020 2064 6566  actory):.    def
+00003e50: 2072 6571 7565 7374 2873 656c 662c 206f   request(self, o
+00003e60: 703a 2073 7472 2c20 7661 6c3a 2069 6e74  p: str, val: int
+00003e70: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
+00003e80: 6e65 7261 7465 7320 6120 6675 6c6c 7920  nerates a fully 
+00003e90: 706f 7075 6c61 7465 6420 5345 5420 5041  populated SET PA
+00003ea0: 5241 4d45 5445 5220 7265 7175 6573 7420  RAMETER request 
+00003eb0: 7072 6f74 6f62 7566 2222 220a 2020 2020  protobuf""".    
+00003ec0: 2020 2020 7265 7120 3d20 7072 6f74 6f2e      req = proto.
+00003ed0: 5265 7175 6573 7428 290a 2020 2020 2020  Request().      
+00003ee0: 2020 7265 712e 7479 7065 203d 2070 726f    req.type = pro
+00003ef0: 746f 2e52 6571 7565 7374 2e52 6571 7565  to.Request.Reque
+00003f00: 7374 5479 7065 2e56 616c 7565 2822 5345  stType.Value("SE
+00003f10: 545f 5041 5241 4d45 5445 5222 290a 0a20  T_PARAMETER").. 
+00003f20: 2020 2020 2020 2073 7020 3d20 7265 712e         sp = req.
+00003f30: 7365 745f 7061 7261 6d65 7465 720a 0a20  set_parameter.. 
+00003f40: 2020 2020 2020 2069 6620 6f70 203d 3d20         if op == 
+00003f50: 224d 4158 524f 5753 223a 0a20 2020 2020  "MAXROWS":.     
+00003f60: 2020 2020 2020 2073 702e 726f 775f 6c69         sp.row_li
+00003f70: 6d69 742e 726f 774c 696d 6974 203d 2076  mit.rowLimit = v
+00003f80: 616c 0a20 2020 2020 2020 2065 6c69 6620  al.        elif 
+00003f90: 6f70 203d 3d20 224d 4158 5449 4d45 223a  op == "MAXTIME":
+00003fa0: 0a20 2020 2020 2020 2020 2020 2073 702e  .            sp.
+00003fb0: 7469 6d65 5f6c 696d 6974 2e74 696d 654c  time_limit.timeL
+00003fc0: 696d 6974 203d 2076 616c 0a20 2020 2020  imit = val.     
+00003fd0: 2020 2065 6c69 6620 6f70 203d 3d20 224d     elif op == "M
+00003fe0: 4158 5445 4d50 4449 534b 223a 0a20 2020  AXTEMPDISK":.   
+00003ff0: 2020 2020 2020 2020 2073 702e 7465 6d70           sp.temp
+00004000: 5f64 6973 6b5f 6c69 6d69 742e 7465 6d70  _disk_limit.temp
+00004010: 4469 736b 4c69 6d69 7420 3d20 7661 6c0a  DiskLimit = val.
+00004020: 2020 2020 2020 2020 656c 6966 206f 7020          elif op 
+00004030: 3d3d 2022 5052 494f 5249 5459 223a 0a20  == "PRIORITY":. 
+00004040: 2020 2020 2020 2020 2020 2073 702e 7072             sp.pr
+00004050: 696f 7269 7479 2e70 7269 6f72 6974 7920  iority.priority 
+00004060: 3d20 7661 6c0a 2020 2020 2020 2020 656c  = val.        el
+00004070: 6966 206f 7020 3d3d 2022 5041 5241 4c4c  if op == "PARALL
+00004080: 454c 4953 4d22 3a0a 2020 2020 2020 2020  ELISM":.        
+00004090: 2020 2020 7370 2e63 6f6e 6375 7272 656e      sp.concurren
+000040a0: 6379 2e63 6f6e 6375 7272 656e 6379 203d  cy.concurrency =
+000040b0: 2076 616c 0a20 2020 2020 2020 2065 6c69   val.        eli
+000040c0: 6620 6f70 203d 3d20 2250 5249 4f52 4954  f op == "PRIORIT
+000040d0: 595f 4144 4a55 5354 4d45 4e54 5f46 4143  Y_ADJUSTMENT_FAC
+000040e0: 544f 5222 3a0a 2020 2020 2020 2020 2020  TOR":.          
+000040f0: 2020 7370 2e70 7269 6f72 6974 795f 6164    sp.priority_ad
+00004100: 6a75 7374 5f66 6163 746f 722e 7072 696f  just_factor.prio
+00004110: 7269 7479 5f61 646a 7573 745f 6661 6374  rity_adjust_fact
+00004120: 6f72 203d 2076 616c 0a20 2020 2020 2020  or = val.       
+00004130: 2065 6c69 6620 6f70 203d 3d20 2250 5249   elif op == "PRI
+00004140: 4f52 4954 595f 4144 4a55 5354 4d45 4e54  ORITY_ADJUSTMENT
+00004150: 5f54 494d 4522 3a0a 2020 2020 2020 2020  _TIME":.        
+00004160: 2020 2020 7370 2e70 7269 6f72 6974 795f      sp.priority_
+00004170: 6164 6a75 7374 5f74 696d 652e 7072 696f  adjust_time.prio
+00004180: 7269 7479 5f61 646a 7573 745f 7469 6d65  rity_adjust_time
+00004190: 203d 2076 616c 0a20 2020 2020 2020 2065   = val.        e
+000041a0: 6c69 6620 6f70 203d 3d20 224d 494e 5f50  lif op == "MIN_P
+000041b0: 5249 4f52 4954 5922 3a0a 2020 2020 2020  RIORITY":.      
+000041c0: 2020 2020 2020 7370 2e6d 696e 5f70 7269        sp.min_pri
+000041d0: 6f72 6974 792e 6d69 6e5f 7072 696f 7269  ority.min_priori
+000041e0: 7479 203d 2076 616c 0a20 2020 2020 2020  ty = val.       
+000041f0: 2065 6c69 6620 6f70 203d 3d20 224d 4158   elif op == "MAX
+00004200: 5f50 5249 4f52 4954 5922 3a0a 2020 2020  _PRIORITY":.    
+00004210: 2020 2020 2020 2020 7370 2e6d 6178 5f70          sp.max_p
+00004220: 7269 6f72 6974 792e 6d61 785f 7072 696f  riority.max_prio
+00004230: 7269 7479 203d 2076 616c 0a20 2020 2020  rity = val.     
+00004240: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00004250: 2020 2020 2072 6169 7365 2050 726f 6772       raise Progr
+00004260: 616d 6d69 6e67 4572 726f 7228 7265 6173  ammingError(reas
+00004270: 6f6e 3d66 2253 796e 7461 7820 6572 726f  on=f"Syntax erro
+00004280: 722e 2049 6e76 616c 6964 2053 4554 207b  r. Invalid SET {
+00004290: 6f70 7d22 290a 0a20 2020 2020 2020 2072  op}")..        r
+000042a0: 6574 7572 6e20 7265 710a 0a20 2020 2064  eturn req..    d
+000042b0: 6566 2072 6573 706f 6e73 6528 7365 6c66  ef response(self
+000042c0: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
+000042d0: 6e65 7261 7465 7320 6120 5345 545f 5041  nerates a SET_PA
+000042e0: 5241 4d45 5445 5220 7265 7370 6f6e 7365  RAMETER response
+000042f0: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
+00004300: 2020 2020 2072 6574 7572 6e20 7072 6f74       return prot
+00004310: 6f2e 436f 6e66 6972 6d61 7469 6f6e 5265  o.ConfirmationRe
+00004320: 7370 6f6e 7365 2829 0a0a 0a63 6c61 7373  sponse()...class
+00004330: 205f 4361 6e63 656c 5175 6572 7946 6163   _CancelQueryFac
+00004340: 746f 7279 285f 4f63 6965 6e74 5265 7175  tory(_OcientRequ
+00004350: 6573 7446 6163 746f 7279 293a 0a20 2020  estFactory):.   
+00004360: 2064 6566 2072 6571 7565 7374 2873 656c   def request(sel
+00004370: 662c 2069 643a 2073 7472 293a 0a20 2020  f, id: str):.   
+00004380: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
+00004390: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
+000043a0: 7465 6420 4341 4e43 454c 2051 5545 5259  ted CANCEL QUERY
+000043b0: 2072 6571 7565 7374 2070 726f 746f 6275   request protobu
+000043c0: 6622 2222 0a20 2020 2020 2020 2072 6571  f""".        req
+000043d0: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
+000043e0: 2829 0a20 2020 2020 2020 2072 6571 2e74  ().        req.t
+000043f0: 7970 6520 3d20 7072 6f74 6f2e 5265 7175  ype = proto.Requ
+00004400: 6573 742e 5265 7175 6573 7454 7970 652e  est.RequestType.
+00004410: 5661 6c75 6528 2243 414e 4345 4c5f 5155  Value("CANCEL_QU
+00004420: 4552 5922 290a 2020 2020 2020 2020 7265  ERY").        re
+00004430: 712e 6361 6e63 656c 5f71 7565 7279 2e73  q.cancel_query.s
+00004440: 716c 203d 2069 640a 2020 2020 2020 2020  ql = id.        
+00004450: 7265 7475 726e 2072 6571 0a0a 2020 2020  return req..    
+00004460: 6465 6620 7265 7370 6f6e 7365 2873 656c  def response(sel
+00004470: 6629 3a0a 2020 2020 2020 2020 2222 2247  f):.        """G
+00004480: 656e 6572 6174 6573 2061 2043 414e 4345  enerates a CANCE
+00004490: 4c5f 5155 4552 5920 7265 7370 6f6e 7365  L_QUERY response
+000044a0: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
+000044b0: 2020 2020 2072 6574 7572 6e20 7072 6f74       return prot
+000044c0: 6f2e 4361 6e63 656c 5175 6572 7952 6573  o.CancelQueryRes
+000044d0: 706f 6e73 6528 290a 0a0a 636c 6173 7320  ponse()...class 
+000044e0: 5f4b 696c 6c51 7565 7279 4661 6374 6f72  _KillQueryFactor
+000044f0: 7928 5f4f 6369 656e 7452 6571 7565 7374  y(_OcientRequest
+00004500: 4661 6374 6f72 7929 3a0a 2020 2020 6465  Factory):.    de
+00004510: 6620 7265 7175 6573 7428 7365 6c66 2c20  f request(self, 
+00004520: 6964 3a20 7374 7229 3a0a 2020 2020 2020  id: str):.      
+00004530: 2020 2222 2247 656e 6572 6174 6573 2061    """Generates a
+00004540: 2066 756c 6c79 2070 6f70 756c 6174 6564   fully populated
+00004550: 204b 494c 4c20 5155 4552 5920 7265 7175   KILL QUERY requ
+00004560: 6573 7420 7072 6f74 6f62 7566 2222 220a  est protobuf""".
+00004570: 2020 2020 2020 2020 7265 7120 3d20 7072          req = pr
+00004580: 6f74 6f2e 5265 7175 6573 7428 290a 2020  oto.Request().  
+00004590: 2020 2020 2020 7265 712e 7479 7065 203d        req.type =
+000045a0: 2070 726f 746f 2e52 6571 7565 7374 2e52   proto.Request.R
+000045b0: 6571 7565 7374 5479 7065 2e56 616c 7565  equestType.Value
+000045c0: 2822 4b49 4c4c 5f51 5545 5259 2229 0a20  ("KILL_QUERY"). 
+000045d0: 2020 2020 2020 2072 6571 2e6b 696c 6c5f         req.kill_
+000045e0: 7175 6572 792e 7371 6c20 3d20 6964 0a20  query.sql = id. 
+000045f0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00004600: 710a 0a20 2020 2064 6566 2072 6573 706f  q..    def respo
+00004610: 6e73 6528 7365 6c66 293a 0a20 2020 2020  nse(self):.     
+00004620: 2020 2022 2222 4765 6e65 7261 7465 7320     """Generates 
+00004630: 6120 4b49 4c4c 5f51 5545 5259 2072 6573  a KILL_QUERY res
+00004640: 706f 6e73 6520 7072 6f74 6f62 7566 2222  ponse protobuf""
+00004650: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00004660: 2070 726f 746f 2e4b 696c 6c51 7565 7279   proto.KillQuery
+00004670: 5265 7370 6f6e 7365 2829 0a0a 0a63 6c61  Response()...cla
+00004680: 7373 205f 4765 7453 7973 7465 6d4d 6574  ss _GetSystemMet
+00004690: 6164 6174 6146 6163 746f 7279 285f 4f63  adataFactory(_Oc
+000046a0: 6965 6e74 5265 7175 6573 7446 6163 746f  ientRequestFacto
+000046b0: 7279 293a 0a20 2020 2064 6566 2072 6571  ry):.    def req
+000046c0: 7565 7374 2873 656c 662c 206f 702c 2073  uest(self, op, s
+000046d0: 6368 656d 612c 2074 6162 6c65 2c20 636f  chema, table, co
+000046e0: 6c75 6d6e 2c20 7669 6577 293a 0a20 2020  lumn, view):.   
+000046f0: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
+00004700: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
+00004710: 7465 6420 4745 545f 5359 5354 454d 5f4d  ted GET_SYSTEM_M
+00004720: 4554 4144 4154 4120 7265 7175 6573 7420  ETADATA request 
+00004730: 7072 6f74 6f62 7566 2222 220a 2020 2020  protobuf""".    
+00004740: 2020 2020 7265 7120 3d20 7072 6f74 6f2e      req = proto.
+00004750: 5265 7175 6573 7428 290a 2020 2020 2020  Request().      
+00004760: 2020 7265 712e 7479 7065 203d 2070 726f    req.type = pro
+00004770: 746f 2e52 6571 7565 7374 2e52 6571 7565  to.Request.Reque
+00004780: 7374 5479 7065 2e56 616c 7565 2822 4645  stType.Value("FE
+00004790: 5443 485f 5359 5354 454d 5f4d 4554 4144  TCH_SYSTEM_METAD
+000047a0: 4154 4122 290a 2020 2020 2020 2020 7265  ATA").        re
+000047b0: 712e 6665 7463 685f 7379 7374 656d 5f6d  q.fetch_system_m
+000047c0: 6574 6164 6174 612e 6361 6c6c 203d 206f  etadata.call = o
+000047d0: 700a 0a20 2020 2020 2020 2069 6620 7363  p..        if sc
+000047e0: 6865 6d61 2069 7320 6e6f 7420 4e6f 6e65  hema is not None
+000047f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00004800: 712e 6665 7463 685f 7379 7374 656d 5f6d  q.fetch_system_m
+00004810: 6574 6164 6174 612e 7363 6865 6d61 203d  etadata.schema =
+00004820: 2073 6368 656d 610a 2020 2020 2020 2020   schema.        
+00004830: 6966 2074 6162 6c65 2069 7320 6e6f 7420  if table is not 
+00004840: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00004850: 2020 7265 712e 6665 7463 685f 7379 7374    req.fetch_syst
+00004860: 656d 5f6d 6574 6164 6174 612e 7461 626c  em_metadata.tabl
+00004870: 6520 3d20 7461 626c 650a 2020 2020 2020  e = table.      
+00004880: 2020 6966 2063 6f6c 756d 6e20 6973 206e    if column is n
+00004890: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000048a0: 2020 2020 2072 6571 2e66 6574 6368 5f73       req.fetch_s
+000048b0: 7973 7465 6d5f 6d65 7461 6461 7461 2e63  ystem_metadata.c
+000048c0: 6f6c 756d 6e20 3d20 636f 6c75 6d6e 0a20  olumn = column. 
+000048d0: 2020 2020 2020 2069 6620 7669 6577 2069         if view i
+000048e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000048f0: 2020 2020 2020 2020 7265 712e 6665 7463          req.fetc
+00004900: 685f 7379 7374 656d 5f6d 6574 6164 6174  h_system_metadat
+00004910: 612e 7669 6577 203d 2076 6965 770a 0a20  a.view = view.. 
+00004920: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00004930: 710a 0a20 2020 2064 6566 2072 6573 706f  q..    def respo
+00004940: 6e73 6528 7365 6c66 293a 0a20 2020 2020  nse(self):.     
+00004950: 2020 2022 2222 4765 6e65 7261 7465 7320     """Generates 
+00004960: 6120 6675 6c6c 7920 706f 7075 6c61 7465  a fully populate
+00004970: 6420 4348 4543 4b5f 4441 5441 2072 6573  d CHECK_DATA res
+00004980: 706f 6e73 6520 7072 6f74 6f62 7566 2222  ponse protobuf""
+00004990: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+000049a0: 2070 726f 746f 2e46 6574 6368 5379 7374   proto.FetchSyst
+000049b0: 656d 4d65 7461 6461 7461 5265 7370 6f6e  emMetadataRespon
+000049c0: 7365 2829 0a0a 0a22 2222 4d61 7070 696e  se()..."""Mappin
+000049d0: 6720 6672 6f6d 2071 7565 7279 2074 7970  g from query typ
+000049e0: 6520 746f 2069 7473 2072 6571 7565 7374  e to its request
+000049f0: 2066 6163 746f 7279 2222 220a 5f4f 4349   factory"""._OCI
+00004a00: 454e 545f 5245 5155 4553 545f 4641 4354  ENT_REQUEST_FACT
+00004a10: 4f52 4945 5320 3d20 7b0a 2020 2020 2253  ORIES = {.    "S
+00004a20: 454c 4543 5422 3a20 5f45 7865 6375 7465  ELECT": _Execute
+00004a30: 5175 6572 7946 6163 746f 7279 2829 2c0a  QueryFactory(),.
+00004a40: 2020 2020 2257 4954 4822 3a20 5f45 7865      "WITH": _Exe
+00004a50: 6375 7465 5175 6572 7946 6163 746f 7279  cuteQueryFactory
+00004a60: 2829 2c0a 2020 2020 2245 5850 4c41 494e  (),.    "EXPLAIN
+00004a70: 2050 4950 454c 494e 4522 3a20 5f45 7870   PIPELINE": _Exp
+00004a80: 6c61 696e 5069 7065 6c69 6e65 4661 6374  lainPipelineFact
+00004a90: 6f72 7928 292c 0a20 2020 2022 4558 504c  ory(),.    "EXPL
+00004aa0: 4149 4e22 3a20 5f45 7865 6375 7465 4578  AIN": _ExecuteEx
+00004ab0: 706c 6169 6e46 6163 746f 7279 2829 2c0a  plainFactory(),.
+00004ac0: 2020 2020 2245 5850 4f52 5422 3a20 5f45      "EXPORT": _E
+00004ad0: 7865 6375 7465 4578 706f 7274 4661 6374  xecuteExportFact
+00004ae0: 6f72 7928 292c 0a20 2020 2022 4348 4543  ory(),.    "CHEC
+00004af0: 4b22 3a20 5f43 6865 636b 4461 7461 4661  K": _CheckDataFa
+00004b00: 6374 6f72 7928 292c 0a20 2020 2022 464f  ctory(),.    "FO
+00004b10: 5243 4522 3a20 5f46 6f72 6365 4578 7465  RCE": _ForceExte
+00004b20: 726e 616c 4661 6374 6f72 7928 292c 0a20  rnalFactory(),. 
+00004b30: 2020 2022 5345 5420 5343 4845 4d41 223a     "SET SCHEMA":
+00004b40: 205f 5365 7453 6368 656d 6146 6163 746f   _SetSchemaFacto
+00004b50: 7279 2829 2c0a 2020 2020 2247 4554 2053  ry(),.    "GET S
+00004b60: 4348 454d 4122 3a20 5f47 6574 5363 6865  CHEMA": _GetSche
+00004b70: 6d61 4661 6374 6f72 7928 292c 0a20 2020  maFactory(),.   
+00004b80: 2022 434c 4541 5220 4341 4348 4522 3a20   "CLEAR CACHE": 
+00004b90: 5f43 6c65 6172 4361 6368 6546 6163 746f  _ClearCacheFacto
+00004ba0: 7279 2829 2c0a 2020 2020 2253 4554 223a  ry(),.    "SET":
+00004bb0: 205f 5365 7450 6172 616d 6574 6572 4661   _SetParameterFa
+00004bc0: 6374 6f72 7928 292c 0a20 2020 2022 4341  ctory(),.    "CA
+00004bd0: 4e43 454c 223a 205f 4361 6e63 656c 5175  NCEL": _CancelQu
+00004be0: 6572 7946 6163 746f 7279 2829 2c0a 2020  eryFactory(),.  
+00004bf0: 2020 224b 494c 4c22 3a20 5f4b 696c 6c51    "KILL": _KillQ
+00004c00: 7565 7279 4661 6374 6f72 7928 292c 0a20  ueryFactory(),. 
+00004c10: 2020 2022 4745 5420 5359 5354 454d 204d     "GET SYSTEM M
+00004c20: 4554 4144 4154 4122 3a20 5f47 6574 5379  ETADATA": _GetSy
+00004c30: 7374 656d 4d65 7461 6461 7461 4661 6374  stemMetadataFact
+00004c40: 6f72 7928 292c 0a7d 0a0a 0a64 6566 205f  ory(),.}...def _
+00004c50: 636f 6e76 6572 745f 6578 6365 7074 696f  convert_exceptio
+00004c60: 6e28 6d73 6729 3a0a 2020 2020 2222 2249  n(msg):.    """I
+00004c70: 6e74 6572 6e61 6c20 726f 7574 696e 6520  nternal routine 
+00004c80: 746f 2063 6f6e 7665 7274 2074 6865 2067  to convert the g
+00004c90: 6f6f 676c 6520 7072 6f74 6f62 7566 2043  oogle protobuf C
+00004ca0: 6f6e 6669 726d 6174 696f 6e52 6573 706f  onfirmationRespo
+00004cb0: 6e73 650a 2020 2020 746f 2061 6e20 6578  nse.    to an ex
+00004cc0: 6365 7074 696f 6e0a 2020 2020 2222 220a  ception.    """.
+00004cd0: 2020 2020 6966 206d 7367 2e76 656e 646f      if msg.vendo
+00004ce0: 725f 636f 6465 203c 2030 3a0a 2020 2020  r_code < 0:.    
+00004cf0: 2020 2020 7265 7475 726e 2045 7272 6f72      return Error
+00004d00: 2873 716c 5f73 7461 7465 3d6d 7367 2e73  (sql_state=msg.s
+00004d10: 716c 5f73 7461 7465 2c20 7265 6173 6f6e  ql_state, reason
+00004d20: 3d6d 7367 2e72 6561 736f 6e2c 2076 656e  =msg.reason, ven
+00004d30: 646f 725f 636f 6465 3d6d 7367 2e76 656e  dor_code=msg.ven
+00004d40: 646f 725f 636f 6465 290a 0a20 2020 2072  dor_code)..    r
+00004d50: 6574 7572 6e20 5761 726e 696e 6728 7371  eturn Warning(sq
+00004d60: 6c5f 7374 6174 653d 6d73 672e 7371 6c5f  l_state=msg.sql_
+00004d70: 7374 6174 652c 2072 6561 736f 6e3d 6d73  state, reason=ms
+00004d80: 672e 7265 6173 6f6e 2c20 7665 6e64 6f72  g.reason, vendor
+00004d90: 5f63 6f64 653d 6d73 672e 7665 6e64 6f72  _code=msg.vendor
+00004da0: 5f63 6f64 6529 0a0a 0a64 6566 205f 7365  _code)...def _se
+00004db0: 6e64 5f6d 7367 2863 6f6e 6e2c 2070 726f  nd_msg(conn, pro
+00004dc0: 746f 6275 665f 6d73 6729 3a0a 2020 2020  tobuf_msg):.    
+00004dd0: 2222 2249 6e74 6572 6e61 6c20 726f 7574  """Internal rout
+00004de0: 696e 6520 746f 2073 656e 6420 6120 7072  ine to send a pr
+00004df0: 6f74 6f62 7566 206d 6573 7361 6765 206f  otobuf message o
+00004e00: 6e20 6120 636f 6e6e 6563 7469 6f6e 2222  n a connection""
+00004e10: 220a 2020 2020 6966 206e 6f74 2063 6f6e  ".    if not con
+00004e20: 6e2e 736f 636b 3a0a 2020 2020 2020 2020  n.sock:.        
+00004e30: 7261 6973 6520 5072 6f67 7261 6d6d 696e  raise Programmin
+00004e40: 6745 7272 6f72 2822 436f 6e6e 6563 7469  gError("Connecti
+00004e50: 6f6e 206e 6f74 2061 7661 696c 6162 6c65  on not available
+00004e60: 2229 0a0a 2020 2020 6c6f 6767 6572 2e64  ")..    logger.d
+00004e70: 6562 7567 2866 2253 656e 6469 6e67 206d  ebug(f"Sending m
+00004e80: 6573 7361 6765 206f 6e20 736f 636b 6574  essage on socket
+00004e90: 207b 636f 6e6e 2e73 6f63 6b7d 3a20 7b70   {conn.sock}: {p
+00004ea0: 726f 746f 6275 665f 6d73 677d 2229 0a0a  rotobuf_msg}")..
+00004eb0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00004ec0: 2063 6f6e 6e2e 736f 636b 2e73 656e 6461   conn.sock.senda
+00004ed0: 6c6c 2873 7472 7563 742e 7061 636b 2822  ll(struct.pack("
+00004ee0: 2169 222c 2070 726f 746f 6275 665f 6d73  !i", protobuf_ms
+00004ef0: 672e 4279 7465 5369 7a65 2829 2920 2b20  g.ByteSize()) + 
+00004f00: 7072 6f74 6f62 7566 5f6d 7367 2e53 6572  protobuf_msg.Ser
+00004f10: 6961 6c69 7a65 546f 5374 7269 6e67 2829  ializeToString()
+00004f20: 290a 2020 2020 6578 6365 7074 2049 4f45  ).    except IOE
+00004f30: 7272 6f72 3a0a 2020 2020 2020 2020 7261  rror:.        ra
+00004f40: 6973 6520 494f 4572 726f 7228 224e 6574  ise IOError("Net
+00004f50: 776f 726b 2073 656e 6420 6572 726f 7222  work send error"
+00004f60: 290a 0a0a 6465 6620 5f72 6563 765f 616c  )...def _recv_al
+00004f70: 6c28 636f 6e6e 2c20 7369 7a65 293a 0a20  l(conn, size):. 
+00004f80: 2020 2022 2222 496e 7465 726e 616c 2072     """Internal r
+00004f90: 6f75 7469 6e65 2074 6f20 7265 6365 6976  outine to receiv
+00004fa0: 6520 6073 697a 6560 2062 7974 6573 206f  e `size` bytes o
+00004fb0: 6620 6461 7461 2066 726f 6d20 6120 636f  f data from a co
+00004fc0: 6e6e 6563 7469 6f6e 2222 220a 2020 2020  nnection""".    
+00004fd0: 6966 206e 6f74 2063 6f6e 6e2e 736f 636b  if not conn.sock
+00004fe0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+00004ff0: 4572 726f 7228 2243 6f6e 6e65 6374 696f  Error("Connectio
+00005000: 6e20 6e6f 7420 6176 6169 6c61 626c 6522  n not available"
+00005010: 290a 0a20 2020 2077 6869 6c65 206c 656e  )..    while len
+00005020: 2863 6f6e 6e2e 5f62 7566 6665 7229 203c  (conn._buffer) <
+00005030: 2073 697a 653a 0a20 2020 2020 2020 2072   size:.        r
+00005040: 6563 6569 7665 6420 3d20 636f 6e6e 2e73  eceived = conn.s
+00005050: 6f63 6b2e 7265 6376 2831 3637 3737 3231  ock.recv(1677721
+00005060: 3629 2020 2320 3136 4d42 2062 7566 6665  6)  # 16MB buffe
+00005070: 720a 2020 2020 2020 2020 6966 206e 6f74  r.        if not
+00005080: 2072 6563 6569 7665 643a 0a20 2020 2020   received:.     
+00005090: 2020 2020 2020 2072 6169 7365 2049 4f45         raise IOE
+000050a0: 7272 6f72 2822 4e65 7477 6f72 6b20 7265  rror("Network re
+000050b0: 6365 6976 6520 6572 726f 7222 290a 2020  ceive error").  
+000050c0: 2020 2020 2020 636f 6e6e 2e5f 6275 6666        conn._buff
+000050d0: 6572 202b 3d20 7265 6365 6976 6564 0a0a  er += received..
+000050e0: 2020 2020 7265 7420 3d20 636f 6e6e 2e5f      ret = conn._
+000050f0: 6275 6666 6572 5b3a 7369 7a65 5d0a 2020  buffer[:size].  
+00005100: 2020 636f 6e6e 2e5f 6275 6666 6572 203d    conn._buffer =
+00005110: 2063 6f6e 6e2e 5f62 7566 6665 725b 7369   conn._buffer[si
+00005120: 7a65 3a5d 0a0a 2020 2020 7265 7475 726e  ze:]..    return
+00005130: 2072 6574 0a0a 0a64 6566 205f 7265 6376   ret...def _recv
+00005140: 5f6d 7367 2863 6f6e 6e2c 2070 726f 746f  _msg(conn, proto
+00005150: 6275 665f 6d73 6729 3a0a 2020 2020 2222  buf_msg):.    ""
+00005160: 2249 6e74 6572 6e61 6c20 726f 7574 696e  "Internal routin
+00005170: 6520 746f 2072 6563 6569 7665 2061 2070  e to receive a p
+00005180: 726f 746f 6275 6620 6d65 7373 6167 6520  rotobuf message 
+00005190: 6f6e 2061 2063 6f6e 6e65 6374 696f 6e22  on a connection"
+000051a0: 2222 0a20 2020 2068 6472 203d 205f 7265  "".    hdr = _re
+000051b0: 6376 5f61 6c6c 2863 6f6e 6e2c 2034 290a  cv_all(conn, 4).
+000051c0: 2020 2020 6d73 6773 697a 6520 3d20 5f75      msgsize = _u
+000051d0: 6e70 6163 6b5f 696e 7428 6864 7229 5b30  npack_int(hdr)[0
+000051e0: 5d0a 0a20 2020 206d 7367 203d 205f 7265  ]..    msg = _re
+000051f0: 6376 5f61 6c6c 2863 6f6e 6e2c 206d 7367  cv_all(conn, msg
+00005200: 7369 7a65 290a 0a20 2020 2070 726f 746f  size)..    proto
+00005210: 6275 665f 6d73 672e 5061 7273 6546 726f  buf_msg.ParseFro
+00005220: 6d53 7472 696e 6728 6d73 6729 0a0a 2020  mString(msg)..  
+00005230: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
+00005240: 2252 6563 6569 7665 6420 6d65 7373 6167  "Received messag
+00005250: 6520 6f6e 2063 6f6e 6e65 6374 696f 6e20  e on connection 
+00005260: 7b63 6f6e 6e2e 736f 636b 7d3a 207b 7072  {conn.sock}: {pr
+00005270: 6f74 6f62 7566 5f6d 7367 7d22 290a 0a20  otobuf_msg}").. 
+00005280: 2020 2072 6574 7572 6e20 7072 6f74 6f62     return protob
+00005290: 7566 5f6d 7367 0a0a 0a64 6566 2044 6174  uf_msg...def Dat
+000052a0: 6528 7965 6172 2c20 6d6f 6e74 682c 2064  e(year, month, d
+000052b0: 6179 293a 2020 2320 7079 6c69 6e74 3a20  ay):  # pylint: 
+000052c0: 6469 7361 626c 653d 696e 7661 6c69 642d  disable=invalid-
+000052d0: 6e61 6d65 0a20 2020 2022 2222 5479 7065  name.    """Type
+000052e0: 2063 6f6e 7374 7275 6374 6f72 2072 6571   constructor req
+000052f0: 7569 7265 6420 696e 2050 4550 2032 3439  uired in PEP 249
+00005300: 2074 6f20 636f 6e73 7472 7563 7420 610a   to construct a.
+00005310: 2020 2020 4461 7465 206f 626a 6563 7420      Date object 
+00005320: 6672 6f6d 2079 6561 722c 206d 6f6e 7468  from year, month
+00005330: 2c20 6461 790a 2020 2020 2222 220a 2020  , day.    """.  
+00005340: 2020 7265 7475 726e 2064 6174 6574 696d    return datetim
+00005350: 652e 6461 7465 7469 6d65 2879 6561 722c  e.datetime(year,
+00005360: 206d 6f6e 7468 2c20 6461 7929 0a0a 0a64   month, day)...d
+00005370: 6566 2054 696d 6528 686f 7572 2c20 6d69  ef Time(hour, mi
+00005380: 6e75 7465 2c20 7365 636f 6e64 293a 2020  nute, second):  
+00005390: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+000053a0: 653d 696e 7661 6c69 642d 6e61 6d65 0a20  e=invalid-name. 
+000053b0: 2020 2022 2222 5479 7065 2063 6f6e 7374     """Type const
+000053c0: 7275 6374 6f72 2072 6571 7569 7265 6420  ructor required 
+000053d0: 696e 2050 4550 2032 3439 2074 6f20 636f  in PEP 249 to co
+000053e0: 6e73 7472 7563 7420 610a 2020 2020 5469  nstruct a.    Ti
+000053f0: 6d65 206f 626a 6563 7420 6672 6f6d 2068  me object from h
+00005400: 6f75 722c 206d 696e 7574 652c 2073 6563  our, minute, sec
+00005410: 6f6e 640a 2020 2020 2222 220a 2020 2020  ond.    """.    
+00005420: 7265 7475 726e 2064 6174 6574 696d 652e  return datetime.
+00005430: 7469 6d65 2868 6f75 722c 206d 696e 7574  time(hour, minut
+00005440: 652c 2073 6563 6f6e 6429 0a0a 0a64 6566  e, second)...def
+00005450: 2054 696d 6573 7461 6d70 2879 6561 722c   Timestamp(year,
+00005460: 206d 6f6e 7468 2c20 6461 792c 2068 6f75   month, day, hou
+00005470: 722c 206d 696e 7574 652c 2073 6563 6f6e  r, minute, secon
+00005480: 6429 3a20 2023 2070 796c 696e 743a 2064  d):  # pylint: d
+00005490: 6973 6162 6c65 3d69 6e76 616c 6964 2d6e  isable=invalid-n
+000054a0: 616d 652c 746f 6f2d 6d61 6e79 2d61 7267  ame,too-many-arg
+000054b0: 756d 656e 7473 0a20 2020 2022 2222 5479  uments.    """Ty
+000054c0: 7065 2063 6f6e 7374 7275 6374 6f72 2072  pe constructor r
+000054d0: 6571 7569 7265 6420 696e 2050 4550 2032  equired in PEP 2
+000054e0: 3439 2074 6f20 636f 6e73 7472 7563 740a  49 to construct.
+000054f0: 2020 2020 6120 5469 6d65 7374 616d 7020      a Timestamp 
+00005500: 6f62 6a65 6374 2066 726f 6d20 7965 6172  object from year
+00005510: 2c20 6d6f 6e74 682c 2064 6179 2c20 686f  , month, day, ho
+00005520: 7572 2c20 6d69 6e75 7465 2c20 7365 636f  ur, minute, seco
+00005530: 6e64 0a20 2020 2022 2222 0a20 2020 2072  nd.    """.    r
+00005540: 6574 7572 6e20 6461 7465 7469 6d65 2e64  eturn datetime.d
+00005550: 6174 6574 696d 6528 7965 6172 2c20 6d6f  atetime(year, mo
+00005560: 6e74 682c 2064 6179 2c20 686f 7572 2c20  nth, day, hour, 
+00005570: 6d69 6e75 7465 2c20 7365 636f 6e64 292e  minute, second).
+00005580: 7469 6d65 7374 616d 7028 290a 0a0a 6465  timestamp()...de
+00005590: 6620 4461 7465 4672 6f6d 5469 636b 7328  f DateFromTicks(
+000055a0: 7469 636b 7329 3a20 2023 2070 796c 696e  ticks):  # pylin
+000055b0: 743a 2064 6973 6162 6c65 3d69 6e76 616c  t: disable=inval
+000055c0: 6964 2d6e 616d 650a 2020 2020 2222 2254  id-name.    """T
+000055d0: 7970 6520 636f 6e73 7472 7563 746f 7220  ype constructor 
+000055e0: 7265 7175 6972 6564 2069 6e20 5045 5020  required in PEP 
+000055f0: 3234 3920 746f 2063 6f6e 7374 7275 6374  249 to construct
+00005600: 0a20 2020 2061 2044 6174 6520 6f62 6a65  .    a Date obje
+00005610: 6374 2066 726f 6d20 6120 7469 6d65 7374  ct from a timest
+00005620: 616d 7020 6f66 2073 6563 6f6e 6473 2073  amp of seconds s
+00005630: 696e 6365 2065 706f 6368 0a20 2020 2022  ince epoch.    "
+00005640: 2222 0a20 2020 2072 6574 7572 6e20 6461  "".    return da
+00005650: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
+00005660: 7574 6366 726f 6d74 696d 6573 7461 6d70  utcfromtimestamp
+00005670: 2874 6963 6b73 290a 0a0a 6465 6620 5469  (ticks)...def Ti
+00005680: 6d65 4672 6f6d 5469 636b 7328 7469 636b  meFromTicks(tick
+00005690: 7329 3a20 2023 2070 796c 696e 743a 2064  s):  # pylint: d
+000056a0: 6973 6162 6c65 3d69 6e76 616c 6964 2d6e  isable=invalid-n
+000056b0: 616d 650a 2020 2020 2222 2254 7970 6520  ame.    """Type 
+000056c0: 636f 6e73 7472 7563 746f 7220 7265 7175  constructor requ
+000056d0: 6972 6564 2069 6e20 5045 5020 3234 3920  ired in PEP 249 
+000056e0: 746f 2063 6f6e 7374 7275 6374 0a20 2020  to construct.   
+000056f0: 2061 2054 696d 6520 6f62 6a65 6374 2066   a Time object f
+00005700: 726f 6d20 6120 7469 6d65 7374 616d 7020  rom a timestamp 
+00005710: 6f66 2073 6563 6f6e 6473 2073 696e 6365  of seconds since
+00005720: 2065 706f 6368 0a20 2020 2022 2222 0a20   epoch.    """. 
+00005730: 2020 2064 6174 655f 7469 6d65 203d 2064     date_time = d
+00005740: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
+00005750: 2e75 7463 6672 6f6d 7469 6d65 7374 616d  .utcfromtimestam
+00005760: 7028 7469 636b 7329 0a20 2020 2072 6574  p(ticks).    ret
+00005770: 7572 6e20 6461 7465 7469 6d65 2e74 696d  urn datetime.tim
+00005780: 6528 6461 7465 5f74 696d 652e 686f 7572  e(date_time.hour
+00005790: 2c20 6461 7465 5f74 696d 652e 6d69 6e75  , date_time.minu
+000057a0: 7465 2c20 6461 7465 5f74 696d 652e 7365  te, date_time.se
+000057b0: 636f 6e64 290a 0a0a 6465 6620 5469 6d65  cond)...def Time
+000057c0: 7374 616d 7046 726f 6d54 6963 6b73 2874  stampFromTicks(t
+000057d0: 6963 6b73 293a 2020 2320 7079 6c69 6e74  icks):  # pylint
+000057e0: 3a20 6469 7361 626c 653d 696e 7661 6c69  : disable=invali
+000057f0: 642d 6e61 6d65 0a20 2020 2022 2222 5479  d-name.    """Ty
+00005800: 7065 2063 6f6e 7374 7275 6374 6f72 2072  pe constructor r
+00005810: 6571 7569 7265 6420 696e 2050 4550 2032  equired in PEP 2
+00005820: 3439 2074 6f20 636f 6e73 7472 7563 740a  49 to construct.
+00005830: 2020 2020 6120 5469 6d65 7374 616d 7020      a Timestamp 
+00005840: 6f62 6a65 6374 2066 726f 6d20 6120 7469  object from a ti
+00005850: 6d65 7374 616d 7020 6f66 2073 6563 6f6e  mestamp of secon
+00005860: 6473 2073 696e 6365 2065 706f 6368 0a20  ds since epoch. 
+00005870: 2020 2022 2222 0a20 2020 2072 6574 7572     """.    retur
+00005880: 6e20 7469 636b 730a 0a0a 6465 6620 5f68  n ticks...def _h
+00005890: 6173 685f 6b65 7928 7368 6172 6564 5f6b  ash_key(shared_k
+000058a0: 6579 2c20 7361 6c74 293a 0a20 2020 2022  ey, salt):.    "
+000058b0: 2222 496e 7465 726e 616c 206b 6579 2068  ""Internal key h
+000058c0: 6173 6820 6675 6e63 7469 6f6e 2222 220a  ash function""".
+000058d0: 2020 2020 2320 4e6f 2069 6465 6120 7768      # No idea wh
+000058e0: 6572 6520 7468 6973 2061 6c67 6f72 6974  ere this algorit
+000058f0: 686d 2063 616d 6520 6672 6f6d 2c20 6275  hm came from, bu
+00005900: 7420 646f 2061 2068 6f6d 6520 6772 6f77  t do a home grow
+00005910: 6e20 6b65 790a 2020 2020 2320 6465 7269  n key.    # deri
+00005920: 7661 7469 6f6e 2066 756e 6374 696f 6e0a  vation function.
+00005930: 2020 2020 6275 6666 6572 203d 2073 7472      buffer = str
+00005940: 7563 742e 7061 636b 2822 2169 222c 206c  uct.pack("!i", l
+00005950: 656e 2873 6861 7265 645f 6b65 7929 290a  en(shared_key)).
+00005960: 2020 2020 6275 6666 6572 203d 2062 7566      buffer = buf
+00005970: 6665 7220 2b20 7361 6c74 0a20 2020 2062  fer + salt.    b
+00005980: 7566 6665 7220 3d20 6275 6666 6572 202b  uffer = buffer +
+00005990: 2073 6861 7265 645f 6b65 790a 2020 2020   shared_key.    
+000059a0: 6861 7368 6572 203d 2068 6173 6865 732e  hasher = hashes.
+000059b0: 4861 7368 2868 6173 6865 732e 5348 4132  Hash(hashes.SHA2
+000059c0: 3536 2829 2c20 6261 636b 656e 643d 6465  56(), backend=de
+000059d0: 6661 756c 745f 6261 636b 656e 6428 2929  fault_backend())
+000059e0: 0a20 2020 2068 6173 6865 722e 7570 6461  .    hasher.upda
+000059f0: 7465 2862 7566 6665 7229 0a20 2020 2072  te(buffer).    r
+00005a00: 6574 7572 6e20 6861 7368 6572 2e66 696e  eturn hasher.fin
+00005a10: 616c 697a 6528 290a 0a0a 2320 5365 7373  alize()...# Sess
+00005a20: 696f 6e73 2063 6f64 650a 0a23 2055 7365  ions code..# Use
+00005a30: 6420 666f 7220 7265 7072 6573 656e 7469  d for representi
+00005a40: 6e67 2061 2073 6573 7369 6f6e 2063 7265  ng a session cre
+00005a50: 6174 6564 2077 6974 6820 6120 7365 6375  ated with a secu
+00005a60: 7269 7479 2074 6f6b 656e 2073 6967 6e20  rity token sign 
+00005a70: 696e 0a0a 0a63 6c61 7373 2053 6563 7572  in...class Secur
+00005a80: 6974 7954 6f6b 656e 3a0a 2020 2020 6465  ityToken:.    de
+00005a90: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00005aa0: 2074 6f6b 656e 4461 7461 3a20 7374 722c   tokenData: str,
+00005ab0: 2074 6f6b 656e 5369 676e 6174 7572 653a   tokenSignature:
+00005ac0: 2073 7472 2c20 6973 7375 6572 4669 6e67   str, issuerFing
+00005ad0: 6572 7072 696e 743a 2073 7472 293a 0a20  erprint: str):. 
+00005ae0: 2020 2020 2020 2073 656c 662e 746f 6b65         self.toke
+00005af0: 6e44 6174 6120 3d20 746f 6b65 6e44 6174  nData = tokenDat
+00005b00: 610a 2020 2020 2020 2020 7365 6c66 2e74  a.        self.t
+00005b10: 6f6b 656e 5369 676e 6174 7572 6520 3d20  okenSignature = 
+00005b20: 746f 6b65 6e53 6967 6e61 7475 7265 0a20  tokenSignature. 
+00005b30: 2020 2020 2020 2073 656c 662e 6973 7375         self.issu
+00005b40: 6572 4669 6e67 6572 7072 696e 7420 3d20  erFingerprint = 
+00005b50: 6973 7375 6572 4669 6e67 6572 7072 696e  issuerFingerprin
+00005b60: 740a 0a0a 2320 5573 6564 2066 6f72 2072  t...# Used for r
+00005b70: 6570 7265 7365 6e74 696e 6720 6120 7365  epresenting a se
+00005b80: 7373 696f 6e20 6372 6561 7465 6420 7769  ssion created wi
+00005b90: 7468 2061 2075 7365 7220 616e 6420 7061  th a user and pa
+00005ba0: 7373 776f 7264 2073 6967 6e20 696e 2e0a  ssword sign in..
+00005bb0: 0a0a 636c 6173 7320 5573 6572 416e 6450  ..class UserAndP
+00005bc0: 6173 7377 6f72 643a 0a20 2020 2064 6566  assword:.    def
+00005bd0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00005be0: 7573 6572 3a20 7374 722c 2070 6173 7377  user: str, passw
+00005bf0: 6f72 643a 2073 7472 293a 0a20 2020 2020  ord: str):.     
+00005c00: 2020 2073 656c 662e 7573 6572 203d 2075     self.user = u
+00005c10: 7365 720a 2020 2020 2020 2020 7365 6c66  ser.        self
+00005c20: 2e70 6173 7377 6f72 6420 3d20 7061 7373  .password = pass
+00005c30: 776f 7264 0a0a 0a63 6c61 7373 2053 6573  word...class Ses
+00005c40: 7369 6f6e 3a0a 2020 2020 6465 6620 5f5f  sion:.    def __
+00005c50: 696e 6974 5f5f 2873 656c 662c 2073 6563  init__(self, sec
+00005c60: 7572 6974 7954 6f6b 656e 3d4e 6f6e 652c  urityToken=None,
+00005c70: 2075 7365 7241 6e64 5061 7373 776f 7264   userAndPassword
+00005c80: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00005c90: 2320 4f6e 6c79 206f 6e65 206f 6620 7468  # Only one of th
+00005ca0: 6573 6520 7368 6f75 6c64 2062 6520 696e  ese should be in
+00005cb0: 7374 616e 7469 6174 6564 2e20 5468 6520  stantiated. The 
+00005cc0: 6f74 6865 7220 4d55 5354 2062 6520 6e6f  other MUST be no
+00005cd0: 6e65 2e0a 2020 2020 2020 2020 7365 6c66  ne..        self
+00005ce0: 2e73 6563 7572 6974 7954 6f6b 656e 203d  .securityToken =
+00005cf0: 2073 6563 7572 6974 7954 6f6b 656e 0a20   securityToken. 
+00005d00: 2020 2020 2020 2073 656c 662e 7573 6572         self.user
+00005d10: 416e 6450 6173 7377 6f72 6420 3d20 7573  AndPassword = us
+00005d20: 6572 416e 6450 6173 7377 6f72 640a 0a0a  erAndPassword...
+00005d30: 636c 6173 7320 436f 6e6e 6563 7469 6f6e  class Connection
+00005d40: 3a0a 2020 2020 2222 2241 2063 6f6e 6e65  :.    """A conne
+00005d50: 6374 696f 6e20 746f 2074 6865 204f 6369  ction to the Oci
+00005d60: 656e 7420 6461 7461 6261 7365 2e20 4e6f  ent database. No
+00005d70: 726d 616c 6c79 2063 6f6e 7374 7275 6374  rmally construct
+00005d80: 6564 2062 790a 2020 2020 6361 6c6c 696e  ed by.    callin
+00005d90: 6720 7468 6520 6d6f 6475 6c65 2060 636f  g the module `co
+00005da0: 6e6e 6563 7428 2960 2063 616c 6c2c 2062  nnect()` call, b
+00005db0: 7574 2063 616e 2062 6520 636f 6e73 7472  ut can be constr
+00005dc0: 7563 7465 640a 2020 2020 6469 7265 6374  ucted.    direct
+00005dd0: 6c79 0a20 2020 2022 2222 0a0a 2020 2020  ly.    """..    
+00005de0: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+00005df0: 653d 746f 6f2d 6d61 6e79 2d69 6e73 7461  e=too-many-insta
+00005e00: 6e63 652d 6174 7472 6962 7574 6573 0a20  nce-attributes. 
+00005e10: 2020 2054 4c53 5f4e 4f4e 4520 3d20 3120     TLS_NONE = 1 
+00005e20: 2023 203a 203a 6d65 7461 2070 7269 7661   # : :meta priva
+00005e30: 7465 3a0a 2020 2020 544c 535f 554e 5645  te:.    TLS_UNVE
+00005e40: 5249 4649 4544 203d 2032 2020 2320 3a20  RIFIED = 2  # : 
+00005e50: 3a6d 6574 6120 7072 6976 6174 653a 0a20  :meta private:. 
+00005e60: 2020 2054 4c53 5f4f 4e20 3d20 3320 2023     TLS_ON = 3  #
+00005e70: 203a 203a 6d65 7461 2070 7269 7661 7465   : :meta private
+00005e80: 3a0a 0a20 2020 2048 414e 4453 4841 4b45  :..    HANDSHAKE
+00005e90: 5f43 4243 203d 2031 0a20 2020 2048 414e  _CBC = 1.    HAN
+00005ea0: 4453 4841 4b45 5f47 434d 203d 2032 0a20  DSHAKE_GCM = 2. 
+00005eb0: 2020 2048 414e 4453 4841 4b45 5f53 534f     HANDSHAKE_SSO
+00005ec0: 203d 2033 0a0a 2020 2020 4445 4641 554c   = 3..    DEFAUL
+00005ed0: 545f 484f 5354 203d 2022 6c6f 6361 6c68  T_HOST = "localh
+00005ee0: 6f73 7422 0a20 2020 2044 4546 4155 4c54  ost".    DEFAULT
+00005ef0: 5f50 4f52 5420 3d20 3430 3530 0a20 2020  _PORT = 4050.   
+00005f00: 2044 4546 4155 4c54 5f44 4154 4142 4153   DEFAULT_DATABAS
+00005f10: 4520 3d20 2273 7973 7465 6d22 0a0a 2020  E = "system"..  
+00005f20: 2020 686f 7374 7320 3d20 5b5d 0a20 2020    hosts = [].   
+00005f30: 2070 6f72 7420 3d20 4e6f 6e65 0a20 2020   port = None.   
+00005f40: 2064 6174 6162 6173 6520 3d20 4e6f 6e65   database = None
+00005f50: 0a20 2020 2074 6c73 203d 204e 6f6e 650a  .    tls = None.
+00005f60: 2020 2020 666f 7263 6520 3d20 4e6f 6e65      force = None
+00005f70: 0a20 2020 2068 616e 6473 6861 6b65 203d  .    handshake =
+00005f80: 204e 6f6e 650a 2020 2020 7573 6572 203d   None.    user =
+00005f90: 204e 6f6e 650a 2020 2020 7061 7373 776f   None.    passwo
+00005fa0: 7264 203d 204e 6f6e 650a 2020 2020 7365  rd = None.    se
+00005fb0: 636f 6e64 6172 795f 696e 7465 7266 6163  condary_interfac
+00005fc0: 6573 203d 204e 6f6e 650a 2020 2020 7365  es = None.    se
+00005fd0: 636f 6e64 6172 795f 696e 6465 7820 3d20  condary_index = 
+00005fe0: 2d31 0a20 2020 2073 6f63 6b20 3d20 4e6f  -1.    sock = No
+00005ff0: 6e65 0a20 2020 2073 6573 7369 6f6e 5f69  ne.    session_i
+00006000: 6420 3d20 7374 7228 7575 6964 2e75 7569  d = str(uuid.uui
+00006010: 6431 2829 290a 0a20 2020 2073 6573 7369  d1())..    sessi
+00006020: 6f6e 203d 204e 6f6e 650a 2020 2020 7365  on = None.    se
+00006030: 7276 6572 5365 7373 696f 6e49 6420 3d20  rverSessionId = 
+00006040: 4e6f 6e65 0a0a 2020 2020 2320 5768 6574  None..    # Whet
+00006050: 6865 7220 7468 6520 6e65 7874 2065 7865  her the next exe
+00006060: 6375 7465 2071 7565 7279 2072 756e 206f  cute query run o
+00006070: 6e20 7468 6973 2063 6f6e 6e65 6374 696f  n this connectio
+00006080: 6e20 7769 6c6c 2062 6520 7265 6469 7265  n will be redire
+00006090: 6374 6564 2e20 446f 6573 206e 6f74 6869  cted. Does nothi
+000060a0: 6e67 2069 6620 666f 7263 6520 6973 2073  ng if force is s
+000060b0: 6574 2074 6f20 7472 7565 0a20 2020 2066  et to true.    f
+000060c0: 6f72 6365 5f6e 6578 745f 7265 6469 7265  orce_next_redire
+000060d0: 6374 203d 2046 616c 7365 0a0a 2020 2020  ct = False..    
+000060e0: 2320 5365 7373 696f 6e73 2063 6f64 6520  # Sessions code 
+000060f0: 656e 640a 0a20 2020 2023 2074 6865 2050  end..    # the P
+00006100: 4550 2032 3439 2073 7461 6e64 6172 6420  EP 249 standard 
+00006110: 7265 636f 6d6d 656e 6473 206d 616b 696e  recommends makin
+00006120: 6720 7468 6520 6d6f 6475 6c65 206c 6576  g the module lev
+00006130: 656c 2065 7863 6570 7469 6f6e 730a 2020  el exceptions.  
+00006140: 2020 2320 616c 736f 2061 7474 7269 6275    # also attribu
+00006150: 7465 7320 6f6e 2074 6865 2043 6f6e 6e65  tes on the Conne
+00006160: 6374 696f 6e20 636c 6173 730a 2020 2020  ction class.    
+00006170: 4572 726f 7220 3d20 4572 726f 720a 2020  Error = Error.  
+00006180: 2020 5761 726e 696e 6720 3d20 5761 726e    Warning = Warn
+00006190: 696e 670a 2020 2020 496e 7465 7266 6163  ing.    Interfac
+000061a0: 6545 7272 6f72 203d 2049 6e74 6572 6661  eError = Interfa
+000061b0: 6365 4572 726f 720a 2020 2020 4461 7461  ceError.    Data
+000061c0: 6261 7365 4572 726f 7220 3d20 4461 7461  baseError = Data
+000061d0: 6261 7365 4572 726f 720a 2020 2020 496e  baseError.    In
+000061e0: 7465 726e 616c 4572 726f 7220 3d20 496e  ternalError = In
+000061f0: 7465 726e 616c 4572 726f 720a 2020 2020  ternalError.    
+00006200: 4f70 6572 6174 696f 6e61 6c45 7272 6f72  OperationalError
+00006210: 203d 204f 7065 7261 7469 6f6e 616c 4572   = OperationalEr
+00006220: 726f 720a 2020 2020 5072 6f67 7261 6d6d  ror.    Programm
+00006230: 696e 6745 7272 6f72 203d 2050 726f 6772  ingError = Progr
+00006240: 616d 6d69 6e67 4572 726f 720a 2020 2020  ammingError.    
+00006250: 496e 7465 6772 6974 7945 7272 6f72 203d  IntegrityError =
+00006260: 2049 6e74 6567 7269 7479 4572 726f 720a   IntegrityError.
+00006270: 2020 2020 4461 7461 4572 726f 7220 3d20      DataError = 
+00006280: 4461 7461 4572 726f 720a 2020 2020 4e6f  DataError.    No
+00006290: 7453 7570 706f 7274 6564 4572 726f 7220  tSupportedError 
+000062a0: 3d20 4e6f 7453 7570 706f 7274 6564 4572  = NotSupportedEr
+000062b0: 726f 720a 0a20 2020 2064 6566 205f 7373  ror..    def _ss
+000062c0: 6c69 7a65 5f63 6f6e 6e65 6374 696f 6e28  lize_connection(
+000062d0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+000062e0: 2222 0a20 2020 2020 2020 2049 6620 5353  "".        If SS
+000062f0: 4c20 6973 2073 7065 6369 6669 6564 2c20  L is specified, 
+00006300: 7772 6170 2074 6865 2073 6f63 6b65 7420  wrap the socket 
+00006310: 696e 2061 6e20 5353 4c20 636f 6e6e 6563  in an SSL connec
+00006320: 7469 6f6e 0a20 2020 2020 2020 2022 2222  tion.        """
+00006330: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00006340: 2e74 6c73 2021 3d20 7365 6c66 2e54 4c53  .tls != self.TLS
+00006350: 5f4e 4f4e 453a 0a20 2020 2020 2020 2020  _NONE:.         
+00006360: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00006370: 2243 7265 6174 696e 6720 544c 5320 636f  "Creating TLS co
+00006380: 6e6e 6563 7469 6f6e 2229 0a20 2020 2020  nnection").     
+00006390: 2020 2020 2020 2063 6f6e 7465 7874 203d         context =
+000063a0: 2073 736c 2e63 7265 6174 655f 6465 6661   ssl.create_defa
+000063b0: 756c 745f 636f 6e74 6578 7428 290a 2020  ult_context().  
+000063c0: 2020 2020 2020 2020 2020 636f 6e74 6578            contex
+000063d0: 742e 6368 6563 6b5f 686f 7374 6e61 6d65  t.check_hostname
+000063e0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+000063f0: 2020 2020 2069 6620 7365 6c66 2e74 6c73       if self.tls
+00006400: 2021 3d20 7365 6c66 2e54 4c53 5f4f 4e3a   != self.TLS_ON:
+00006410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006420: 2063 6f6e 7465 7874 2e76 6572 6966 795f   context.verify_
+00006430: 6d6f 6465 203d 2073 736c 2e43 4552 545f  mode = ssl.CERT_
+00006440: 4e4f 4e45 0a20 2020 2020 2020 2020 2020  NONE.           
+00006450: 2073 656c 662e 736f 636b 203d 2063 6f6e   self.sock = con
+00006460: 7465 7874 2e77 7261 705f 736f 636b 6574  text.wrap_socket
+00006470: 2873 656c 662e 736f 636b 290a 0a20 2020  (self.sock)..   
+00006480: 2023 204e 6f74 6520 7468 6174 2074 6865   # Note that the
+00006490: 7265 2061 7265 2061 2063 6f75 706c 6520  re are a couple 
+000064a0: 6f66 2070 6c61 6365 7320 696e 2074 6865  of places in the
+000064b0: 2063 6f64 6520 7768 6572 6520 7765 2072   code where we r
+000064c0: 6563 6f6e 7374 7275 6374 2074 6865 2043  econstruct the C
+000064d0: 6f6e 6e65 6374 696f 6e2e 2020 4966 2079  onnection.  If y
+000064e0: 6f75 2061 6464 2061 2070 6172 616d 6574  ou add a paramet
+000064f0: 6572 2068 6572 652c 206d 616b 6520 7375  er here, make su
+00006500: 7265 2074 6f20 7570 6461 7465 2074 686f  re to update tho
+00006510: 7365 0a20 2020 2023 2070 6c61 6365 730a  se.    # places.
+00006520: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00006530: 2873 656c 662c 2064 736e 3d4e 6f6e 652c  (self, dsn=None,
+00006540: 2075 7365 723d 4e6f 6e65 2c20 7061 7373   user=None, pass
+00006550: 776f 7264 3d4e 6f6e 652c 2068 6f73 743d  word=None, host=
+00006560: 4e6f 6e65 2c20 6461 7461 6261 7365 3d4e  None, database=N
+00006570: 6f6e 652c 2074 6c73 3d4e 6f6e 652c 2068  one, tls=None, h
+00006580: 616e 6473 6861 6b65 3d4e 6f6e 652c 2066  andshake=None, f
+00006590: 6f72 6365 3d4e 6f6e 652c 2063 6f6e 6669  orce=None, confi
+000065a0: 6766 696c 653d 4e6f 6e65 2c20 7365 7373  gfile=None, sess
+000065b0: 696f 6e3d 4e6f 6e65 293a 0a20 2020 2020  ion=None):.     
+000065c0: 2020 2023 2070 796c 696e 743a 2064 6973     # pylint: dis
+000065d0: 6162 6c65 3d74 6f6f 2d6d 616e 792d 6172  able=too-many-ar
+000065e0: 6775 6d65 6e74 732c 6e6f 2d6d 656d 6265  guments,no-membe
+000065f0: 720a 2020 2020 2020 2020 2222 2243 6f6e  r.        """Con
+00006600: 6e65 6374 696f 6e20 7061 7261 6d65 7465  nection paramete
+00006610: 7273 2063 616e 2062 6520 7370 6563 6966  rs can be specif
+00006620: 6965 6420 6173 2070 6172 7420 6f66 2074  ied as part of t
+00006630: 6865 2064 736e 2c0a 2020 2020 2020 2020  he dsn,.        
+00006640: 7573 696e 6720 6b65 7977 6f72 6420 6172  using keyword ar
+00006650: 6775 6d65 6e74 7320 6f72 2062 6f74 682e  guments or both.
+00006660: 2020 4966 2062 6f74 6820 6172 6520 7370    If both are sp
+00006670: 6563 6966 6965 642c 2074 6865 206b 6579  ecified, the key
+00006680: 776f 7264 0a20 2020 2020 2020 2070 6172  word.        par
+00006690: 616d 6574 6572 206f 7665 7272 6964 6573  ameter overrides
+000066a0: 2074 6865 2076 616c 7565 2069 6e20 7468   the value in th
+000066b0: 6520 6473 6e2e 0a0a 2020 2020 2020 2020  e dsn...        
+000066c0: 5468 6520 4f63 6965 6e74 2044 534e 2069  The Ocient DSN i
+000066d0: 7320 6f66 2074 6865 2066 6f72 6d61 743a  s of the format:
+000066e0: 0a20 2020 2020 2020 2060 6f63 6965 6e74  .        `ocient
+000066f0: 3a2f 2f75 7365 723a 7061 7373 776f 7264  ://user:password
+00006700: 405b 686f 7374 5d5b 3a70 6f72 745d 5b2f  @[host][:port][/
+00006710: 6461 7461 6261 7365 5d5b 3f70 6172 616d  database][?param
+00006720: 313d 7661 6c75 6531 262e 2e2e 5d60 0a0a  1=value1&...]`..
+00006730: 2020 2020 2020 2020 6075 7365 7260 2061          `user` a
+00006740: 6e64 2060 7061 7373 776f 7264 6020 6d75  nd `password` mu
+00006750: 7374 2062 6520 7375 7070 6c69 6564 2e20  st be supplied. 
+00006760: 2060 686f 7374 6020 6465 6661 756c 7473   `host` defaults
+00006770: 2074 6f20 6c6f 6361 6c68 6f73 742c 0a20   to localhost,. 
+00006780: 2020 2020 2020 2070 6f72 7420 6465 6661         port defa
+00006790: 756c 7473 2074 6f20 3430 3530 2c20 6461  ults to 4050, da
+000067a0: 7461 6261 7365 2064 6566 6175 6c74 7320  tabase defaults 
+000067b0: 746f 2060 7379 7374 656d 6020 616e 6420  to `system` and 
+000067c0: 6074 6c73 6020 6465 6661 756c 7473 0a20  `tls` defaults. 
+000067d0: 2020 2020 2020 2074 6f20 606f 6666 602e         to `off`.
+000067e0: 0a0a 2020 2020 2020 2020 4d75 6c74 6970  ..        Multip
+000067f0: 6c65 2068 6f73 7473 206d 6179 2062 6520  le hosts may be 
+00006800: 7370 6563 6966 6965 642c 2073 6570 6172  specified, separ
+00006810: 6174 6564 2062 7920 6120 636f 6d6d 612c  ated by a comma,
+00006820: 2069 6e20 7768 6963 6820 6361 7365 2074   in which case t
+00006830: 6865 0a20 2020 2020 2020 2068 6f73 7473  he.        hosts
+00006840: 2077 696c 6c20 6265 2074 7269 6564 2069   will be tried i
+00006850: 6e20 6f72 6465 7220 2054 6875 7320 616e  n order  Thus an
+00006860: 2065 7861 6d70 6c65 2044 534e 206d 6967   example DSN mig
+00006870: 6874 2062 650a 2020 2020 2020 2020 606f  ht be.        `o
+00006880: 6369 656e 743a 2f2f 736f 6d65 6f6e 653a  cient://someone:
+00006890: 736f 6d65 7061 7373 776f 7264 4068 6f73  somepassword@hos
+000068a0: 7431 2c68 6f73 7432 3a34 3035 312f 6d79  t1,host2:4051/my
+000068b0: 6462 600a 0a20 2020 2020 2020 2063 6f6e  db`..        con
+000068c0: 6669 6766 696c 6520 6973 2074 6865 206e  figfile is the n
+000068d0: 616d 6520 6f66 2061 2063 6f6e 6669 6775  ame of a configu
+000068e0: 7261 7469 6f6e 2066 696c 6520 696e 2049  ration file in I
+000068f0: 4e49 2066 6f72 6d61 742c 2077 6865 7265  NI format, where
+00006900: 2065 6163 680a 2020 2020 2020 2020 7365   each.        se
+00006910: 6374 696f 6e20 6973 2065 6974 6865 7220  ction is either 
+00006920: 6465 6661 756c 742c 206f 7220 6120 7061  default, or a pa
+00006930: 7474 6572 6e20 7468 6174 206d 6174 6368  ttern that match
+00006940: 6573 2074 6865 2068 6f73 7420 616e 6420  es the host and 
+00006950: 6f70 7469 6f6e 616c 6c79 0a20 2020 2020  optionally.     
+00006960: 2020 2064 6174 6162 6173 652e 2073 6563     database. sec
+00006970: 7469 6f6e 7320 6172 6520 6d61 7463 6865  tions are matche
+00006980: 6420 696e 206f 7264 6572 2c20 736f 206d  d in order, so m
+00006990: 6f72 6520 7370 6563 6966 6963 2073 6563  ore specific sec
+000069a0: 7469 6f6e 7320 7368 6f75 6c64 0a20 2020  tions should.   
+000069b0: 2020 2020 2070 7265 6365 6465 206c 6573       precede les
+000069c0: 7320 7370 6563 6966 6963 2073 6563 7469  s specific secti
+000069d0: 6f6e 733a 3a0a 0a20 2020 2020 2020 2020  ons::..         
+000069e0: 2020 205b 4445 4641 554c 545d 0a20 2020     [DEFAULT].   
+000069f0: 2020 2020 2020 2020 2074 6c73 203d 2075           tls = u
+00006a00: 6e76 6572 6966 6965 640a 0a20 2020 2020  nverified..     
+00006a10: 2020 2020 2020 2023 2054 6869 7320 7769         # This wi
+00006a20: 6c6c 206d 6174 6368 2074 6865 2073 7065  ll match the spe
+00006a30: 6369 6669 6320 686f 7374 2061 6e64 2064  cific host and d
+00006a40: 6174 6162 6173 650a 2020 2020 2020 2020  atabase.        
+00006a50: 2020 2020 5b66 6f6f 2e6f 6369 656e 742e      [foo.ocient.
+00006a60: 636f 6d2f 736f 6d65 6462 5d0a 2020 2020  com/somedb].    
+00006a70: 2020 2020 2020 2020 7573 6572 203d 2070          user = p
+00006a80: 616e 7468 6572 0a20 2020 2020 2020 2020  anther.         
+00006a90: 2020 2070 6173 7377 6f72 6420 3d20 7069     password = pi
+00006aa0: 6e6b 0a0a 2020 2020 2020 2020 2020 2020  nk..            
+00006ab0: 2320 5468 6973 2077 696c 6c20 6d61 7463  # This will matc
+00006ac0: 6820 7468 6520 7370 6563 6966 6963 2068  h the specific h
+00006ad0: 6f73 740a 2020 2020 2020 2020 2020 2020  ost.            
+00006ae0: 5b66 6f6f 2e6f 6369 656e 742e 636f 6d5d  [foo.ocient.com]
+00006af0: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+00006b00: 7220 3d20 7061 6e74 6865 720a 2020 2020  r = panther.    
+00006b10: 2020 2020 2020 2020 7061 7373 776f 7264          password
+00006b20: 203d 2070 696e 6b0a 0a20 2020 2020 2020   = pink..       
+00006b30: 2020 2020 2023 2054 6869 7320 7769 6c6c       # This will
+00006b40: 206d 6174 6368 2061 6e79 2068 6f73 7420   match any host 
+00006b50: 696e 2074 6865 206f 6369 656e 742e 636f  in the ocient.co
+00006b60: 6d20 646f 6d61 696e 0a20 2020 2020 2020  m domain.       
+00006b70: 2020 2020 205b 2a2e 6f63 6965 6e74 2e63       [*.ocient.c
+00006b80: 6f6d 5d0a 2020 2020 2020 2020 2020 2020  om].            
+00006b90: 7573 6572 203d 2074 6f6d 0a20 2020 2020  user = tom.     
+00006ba0: 2020 2020 2020 2070 6173 7377 6f72 6420         password 
+00006bb0: 3d20 6a65 7272 790a 2020 2020 2020 2020  = jerry.        
+00006bc0: 2020 2020 6461 7461 6261 7365 203d 206d      database = m
+00006bd0: 6963 650a 0a20 2020 2020 2020 2020 2020  ice..           
+00006be0: 2023 2054 6869 7320 7769 6c6c 206d 6174   # This will mat
+00006bf0: 6368 2061 6e79 2068 6f73 7420 696e 2074  ch any host in t
+00006c00: 6865 206f 6369 656e 742e 636f 6d20 646f  he ocient.com do
+00006c10: 6d61 696e 0a20 2020 2020 2020 2020 2020  main.           
+00006c20: 205b 2a2e 6f63 6965 6e74 2e63 6f6d 5d0a   [*.ocient.com].
+00006c30: 2020 2020 2020 2020 2020 2020 7573 6572              user
+00006c40: 203d 2074 6f6d 0a20 2020 2020 2020 2020   = tom.         
+00006c50: 2020 2070 6173 7377 6f72 6420 3d20 6a65     password = je
+00006c60: 7272 790a 0a20 2020 2020 2020 2043 7572  rry..        Cur
+00006c70: 7265 6e74 6c79 2073 7570 706f 7274 6564  rently supported
+00006c80: 2070 6172 616d 6574 6572 7320 6172 653a   parameters are:
+00006c90: 0a0a 2020 2020 2020 2020 2d20 746c 733a  ..        - tls:
+00006ca0: 2057 6869 6368 2063 616e 2068 6176 6520   Which can have 
+00006cb0: 7468 6520 7661 6c75 6573 2022 6f66 6622  the values "off"
+00006cc0: 2c20 2275 6e76 6572 6966 6965 6422 2c20  , "unverified", 
+00006cd0: 6f72 2022 6f6e 2220 696e 2074 6865 2064  or "on" in the d
+00006ce0: 736e 2c0a 2020 2020 2020 2020 2020 2020  sn,.            
+00006cf0: 6f72 2043 6f6e 6e65 6374 696f 6e2e 544c  or Connection.TL
+00006d00: 535f 4e4f 4e45 2c20 436f 6e6e 6563 7469  S_NONE, Connecti
+00006d10: 6f6e 2e54 4c53 5f55 4e56 4552 4946 4945  on.TLS_UNVERIFIE
+00006d20: 442c 206f 720a 2020 2020 2020 2020 2020  D, or.          
+00006d30: 2020 436f 6e6e 6563 7469 6f6e 2e54 4c53    Connection.TLS
+00006d40: 5f4f 4e20 6173 2061 206b 6579 776f 7264  _ON as a keyword
+00006d50: 2070 6172 616d 6574 6572 2e0a 2020 2020   parameter..    
+00006d60: 2020 2020 2d20 666f 7263 653a 2054 7275      - force: Tru
+00006d70: 6520 6f72 2046 616c 7365 2c20 7768 6574  e or False, whet
+00006d80: 6865 7220 746f 2066 6f72 6365 2074 6865  her to force the
+00006d90: 2063 6f6e 6e65 6374 696f 6e20 746f 2072   connection to r
+00006da0: 656d 6169 6e20 6f6e 2074 6869 730a 2020  emain on this.  
+00006db0: 2020 2020 2020 2020 2020 7365 7276 6572            server
+00006dc0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00006dd0: 2020 2020 2023 2070 796c 696e 743a 2064       # pylint: d
+00006de0: 6973 6162 6c65 3d6e 6f2d 6d65 6d62 6572  isable=no-member
+00006df0: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
+00006e00: 6172 7365 5f61 7267 7328 6473 6e2c 2075  arse_args(dsn, u
+00006e10: 7365 722c 2070 6173 7377 6f72 642c 2068  ser, password, h
+00006e20: 6f73 742c 2064 6174 6162 6173 652c 2074  ost, database, t
+00006e30: 6c73 2c20 6861 6e64 7368 616b 652c 2066  ls, handshake, f
+00006e40: 6f72 6365 2c20 636f 6e66 6967 6669 6c65  orce, configfile
+00006e50: 290a 0a20 2020 2020 2020 2073 6176 6564  )..        saved
+00006e60: 5f65 7863 203d 204e 6f6e 650a 2020 2020  _exc = None.    
+00006e70: 2020 2020 666f 7220 6f6e 655f 686f 7374      for one_host
+00006e80: 2069 6e20 7365 6c66 2e68 6f73 7473 3a0a   in self.hosts:.
+00006e90: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00006ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006eb0: 206c 6f67 6765 722e 696e 666f 2866 2254   logger.info(f"T
+00006ec0: 7279 696e 6720 746f 2063 6f6e 6e65 6374  rying to connect
+00006ed0: 2074 6f20 7b6f 6e65 5f68 6f73 747d 3a7b   to {one_host}:{
+00006ee0: 7365 6c66 2e70 6f72 747d 2229 0a20 2020  self.port}").   
+00006ef0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006f00: 662e 736f 636b 203d 2073 6f63 6b65 742e  f.sock = socket.
+00006f10: 6372 6561 7465 5f63 6f6e 6e65 6374 696f  create_connectio
+00006f20: 6e28 286f 6e65 5f68 6f73 742c 2073 656c  n((one_host, sel
+00006f30: 662e 706f 7274 2929 0a20 2020 2020 2020  f.port)).       
+00006f40: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00006f50: 696e 666f 2866 2243 6f6e 6e65 6374 6564  info(f"Connected
+00006f60: 2074 6f20 7b6f 6e65 5f68 6f73 747d 3a7b   to {one_host}:{
+00006f70: 7365 6c66 2e70 6f72 747d 206f 6e20 736f  self.port} on so
+00006f80: 636b 6574 207b 7365 6c66 2e73 6f63 6b7d  cket {self.sock}
+00006f90: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00006fa0: 2020 2073 6176 6564 5f65 7863 203d 204e     saved_exc = N
+00006fb0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00006fc0: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+00006fd0: 2020 2020 2020 6578 6365 7074 2043 6f6e        except Con
+00006fe0: 6e65 6374 696f 6e45 7272 6f72 2061 7320  nectionError as 
+00006ff0: 6578 633a 0a20 2020 2020 2020 2020 2020  exc:.           
+00007000: 2020 2020 2073 6176 6564 5f65 7863 203d       saved_exc =
+00007010: 2065 7863 0a20 2020 2020 2020 2020 2020   exc.           
+00007020: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00007030: 6e20 6173 2065 7863 3a0a 2020 2020 2020  n as exc:.      
+00007040: 2020 2020 2020 2020 2020 7361 7665 645f            saved_
+00007050: 6578 6320 3d20 6578 630a 0a20 2020 2020  exc = exc..     
+00007060: 2020 2069 6620 7361 7665 645f 6578 6320     if saved_exc 
+00007070: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00007080: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+00007090: 7272 6f72 2866 2255 6e61 626c 6520 746f  rror(f"Unable to
+000070a0: 2063 6f6e 6e65 6374 2074 6f20 7b27 2c27   connect to {','
+000070b0: 2e6a 6f69 6e28 7365 6c66 2e68 6f73 7473  .join(self.hosts
+000070c0: 297d 3a7b 7365 6c66 2e70 6f72 747d 3a20  )}:{self.port}: 
+000070d0: 7b73 7472 2873 6176 6564 5f65 7863 297d  {str(saved_exc)}
+000070e0: 2229 2066 726f 6d20 7361 7665 645f 6578  ") from saved_ex
+000070f0: 630a 0a20 2020 2020 2020 2073 656c 662e  c..        self.
+00007100: 5f73 736c 697a 655f 636f 6e6e 6563 7469  _sslize_connecti
+00007110: 6f6e 2829 0a0a 2020 2020 2020 2020 7365  on()..        se
+00007120: 6c66 2e5f 6275 6666 6572 203d 2062 2222  lf._buffer = b""
+00007130: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00007140: 7373 696f 6e20 3d20 7365 7373 696f 6e0a  ssion = session.
+00007150: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00007160: 6861 6e64 7368 616b 6520 3d3d 2073 656c  handshake == sel
+00007170: 662e 4841 4e44 5348 414b 455f 5353 4f3a  f.HANDSHAKE_SSO:
+00007180: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00007190: 7365 6c66 2e75 7365 722e 6c6f 7765 7228  self.user.lower(
+000071a0: 2920 213d 2022 2220 6f72 2073 656c 662e  ) != "" or self.
+000071b0: 7061 7373 776f 7264 2e6c 6f77 6572 2829  password.lower()
+000071c0: 2021 3d20 2222 3a0a 2020 2020 2020 2020   != "":.        
+000071d0: 2020 2020 2020 2020 2320 4966 2065 6974          # If eit
+000071e0: 6865 7220 6172 6520 6e6f 6e2d 656d 7074  her are non-empt
+000071f0: 792c 2075 7365 2074 6865 2043 4243 5f47  y, use the CBC_G
+00007200: 434d 2e0a 2020 2020 2020 2020 2020 2020  CM..            
+00007210: 2020 2020 7365 6c66 2e5f 636c 6965 6e74      self._client
+00007220: 5f68 616e 6473 6861 6b65 5f43 4243 5f47  _handshake_CBC_G
+00007230: 434d 2869 735f 6578 706c 6963 6974 5f73  CM(is_explicit_s
+00007240: 736f 3d54 7275 652c 2066 6f72 6365 3d73  so=True, force=s
+00007250: 656c 662e 666f 7263 6529 0a20 2020 2020  elf.force).     
+00007260: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00007270: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00007280: 7365 6c66 2e73 6573 7369 6f6e 2069 7320  self.session is 
+00007290: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000072a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000072b0: 6c66 2e5f 636c 6965 6e74 5f68 616e 6473  lf._client_hands
+000072c0: 6861 6b65 5f73 6563 7572 6974 795f 746f  hake_security_to
+000072d0: 6b65 6e28 290a 2020 2020 2020 2020 2020  ken().          
+000072e0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007300: 7365 6c66 2e5f 636c 6965 6e74 5f68 616e  self._client_han
+00007310: 6473 6861 6b65 5f53 534f 2829 0a20 2020  dshake_SSO().   
+00007320: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00007330: 2020 2020 2020 2073 656c 662e 5f63 6c69         self._cli
+00007340: 656e 745f 6861 6e64 7368 616b 655f 4342  ent_handshake_CB
+00007350: 435f 4743 4d28 6973 5f65 7870 6c69 6369  C_GCM(is_explici
+00007360: 745f 7373 6f3d 4661 6c73 652c 2066 6f72  t_sso=False, for
+00007370: 6365 3d73 656c 662e 666f 7263 6529 0a0a  ce=self.force)..
+00007380: 2020 2020 6465 6620 5f69 6e69 7469 616c      def _initial
+00007390: 697a 655f 636c 6965 6e74 5f63 6f6e 6e65  ize_client_conne
+000073a0: 6374 696f 6e28 7365 6c66 2c20 636c 6965  ction(self, clie
+000073b0: 6e74 5f63 6f6e 6e65 6374 696f 6e5f 6d65  nt_connection_me
+000073c0: 7373 6167 6529 3a0a 2020 2020 2020 2020  ssage):.        
+000073d0: 2222 2249 6e69 7469 616c 697a 6573 2066  """Initializes f
+000073e0: 6965 6c64 7320 7573 6564 2069 6e20 696e  ields used in in
+000073f0: 6974 6961 6c20 636c 6965 6e74 2068 616e  itial client han
+00007400: 6473 6861 6b65 2072 6571 7565 7374 732e  dshake requests.
+00007410: 0a20 2020 2020 2020 2031 2e20 6461 7461  .        1. data
+00007420: 6261 7365 0a20 2020 2020 2020 2032 2e20  base.        2. 
+00007430: 636c 6965 6e74 6964 2028 7079 6f63 6965  clientid (pyocie
+00007440: 6e74 290a 2020 2020 2020 2020 332e 2070  nt).        3. p
+00007450: 726f 746f 636f 6c20 7665 7273 696f 6e0a  rotocol version.
+00007460: 2020 2020 2020 2020 342e 2076 6572 7369          4. versi
+00007470: 6f6e 5f6d 616a 6f72 0a20 2020 2020 2020  on_major.       
+00007480: 2035 2e20 7665 7273 696f 6e5f 6d69 6e6f   5. version_mino
+00007490: 720a 2020 2020 2020 2020 362e 2073 6573  r.        6. ses
+000074a0: 7369 6f6e 2069 640a 0a20 2020 2020 2020  sion id..       
+000074b0: 204e 6f74 652c 206e 6f74 2061 6c6c 2066   Note, not all f
+000074c0: 6965 6c64 7320 6172 6520 696e 6974 6961  ields are initia
+000074d0: 6c69 7a65 642e 2053 6f6d 6520 6669 656c  lized. Some fiel
+000074e0: 6473 2061 7265 2073 7065 6369 616c 2074  ds are special t
+000074f0: 6f20 6365 7274 6169 6e20 636c 6965 6e74  o certain client
+00007500: 2068 616e 6473 6861 6b65 732e 0a20 2020   handshakes..   
+00007510: 2020 2020 2046 6f72 2065 7861 6d70 6c65       For example
+00007520: 2c20 7468 6520 5353 4f20 6861 6e64 7368  , the SSO handsh
+00007530: 616b 6520 7769 7468 2074 6f6b 656e 2064  ake with token d
+00007540: 6f65 7320 6e6f 7420 7461 6b65 2075 7365  oes not take use
+00007550: 7220 616e 6420 696e 7374 6561 6420 7461  r and instead ta
+00007560: 6b65 7320 6120 7365 6375 7269 7479 2074  kes a security t
+00007570: 6f6b 656e 2e0a 0a20 2020 2020 2020 2041  oken...        A
+00007580: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00007590: 2063 6c69 656e 745f 636f 6e6e 6563 7469   client_connecti
+000075a0: 6f6e 5f6d 6573 7361 6765 2028 5b70 726f  on_message ([pro
+000075b0: 746f 206d 6573 7361 6765 5d29 3a20 7468  to message]): th
+000075c0: 6520 636c 6965 6e74 2068 616e 6473 6861  e client handsha
+000075d0: 6b65 2072 6571 7565 7374 2074 6f20 696e  ke request to in
+000075e0: 6974 6961 6c69 7a65 0a20 2020 2020 2020  itialize.       
+000075f0: 2022 2222 0a20 2020 2020 2020 2063 6c69   """.        cli
+00007600: 656e 745f 636f 6e6e 6563 7469 6f6e 5f6d  ent_connection_m
+00007610: 6573 7361 6765 2e64 6174 6162 6173 6520  essage.database 
+00007620: 3d20 7365 6c66 2e64 6174 6162 6173 650a  = self.database.
+00007630: 2020 2020 2020 2020 636c 6965 6e74 5f63          client_c
+00007640: 6f6e 6e65 6374 696f 6e5f 6d65 7373 6167  onnection_messag
+00007650: 652e 636c 6965 6e74 6964 203d 2044 5249  e.clientid = DRI
+00007660: 5645 525f 4944 0a20 2020 2020 2020 2063  VER_ID.        c
+00007670: 6c69 656e 745f 636f 6e6e 6563 7469 6f6e  lient_connection
+00007680: 5f6d 6573 7361 6765 2e76 6572 7369 6f6e  _message.version
+00007690: 203d 2050 524f 544f 434f 4c5f 5645 5253   = PROTOCOL_VERS
+000076a0: 494f 4e0a 2020 2020 2020 2020 636c 6965  ION.        clie
+000076b0: 6e74 5f63 6f6e 6e65 6374 696f 6e5f 6d65  nt_connection_me
+000076c0: 7373 6167 652e 6d61 6a6f 7243 6c69 656e  ssage.majorClien
+000076d0: 7456 6572 7369 6f6e 203d 2076 6572 7369  tVersion = versi
+000076e0: 6f6e 5f6d 616a 6f72 0a20 2020 2020 2020  on_major.       
+000076f0: 2063 6c69 656e 745f 636f 6e6e 6563 7469   client_connecti
+00007700: 6f6e 5f6d 6573 7361 6765 2e6d 696e 6f72  on_message.minor
+00007710: 436c 6965 6e74 5665 7273 696f 6e20 3d20  ClientVersion = 
+00007720: 7665 7273 696f 6e5f 6d69 6e6f 720a 2020  version_minor.  
+00007730: 2020 2020 2020 636c 6965 6e74 5f63 6f6e        client_con
+00007740: 6e65 6374 696f 6e5f 6d65 7373 6167 652e  nection_message.
+00007750: 7365 7373 696f 6e49 4420 3d20 7365 6c66  sessionID = self
+00007760: 2e73 6573 7369 6f6e 5f69 640a 0a20 2020  .session_id..   
+00007770: 2064 6566 205f 636c 6965 6e74 5f68 616e   def _client_han
+00007780: 6473 6861 6b65 5f43 4243 5f47 434d 2873  dshake_CBC_GCM(s
+00007790: 656c 662c 2069 735f 6578 706c 6963 6974  elf, is_explicit
+000077a0: 5f73 736f 3d46 616c 7365 2c20 666f 7263  _sso=False, forc
+000077b0: 653d 4661 6c73 6529 3a0a 2020 2020 2020  e=False):.      
+000077c0: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
+000077d0: 2020 2020 2020 2020 2020 2323 2323 2323            ######
+000077e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000077f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00007800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007810: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007820: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007830: 2323 230a 2020 2020 2020 2020 2020 2020  ###.            
-00007840: 6966 2073 656c 662e 6861 6e64 7368 616b  if self.handshak
-00007850: 6520 3d3d 2073 656c 662e 4841 4e44 5348  e == self.HANDSH
-00007860: 414b 455f 4342 433a 0a20 2020 2020 2020  AKE_CBC:.       
-00007870: 2020 2020 2020 2020 2023 2043 4243 0a20           # CBC. 
-00007880: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00007890: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
-000078a0: 656c 662c 2070 726f 746f 2e43 6c69 656e  elf, proto.Clien
-000078b0: 7443 6f6e 6e65 6374 696f 6e32 5265 7370  tConnection2Resp
-000078c0: 6f6e 7365 2829 290a 2020 2020 2020 2020  onse()).        
-000078d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000078e0: 2020 2020 2020 2020 2020 2320 4743 4d20            # GCM 
-000078f0: 6f72 2065 7870 6c69 6369 7420 5353 4f0a  or explicit SSO.
-00007900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007910: 7273 7020 3d20 5f72 6563 765f 6d73 6728  rsp = _recv_msg(
-00007920: 7365 6c66 2c20 7072 6f74 6f2e 436c 6965  self, proto.Clie
-00007930: 6e74 436f 6e6e 6563 7469 6f6e 4743 4d32  ntConnectionGCM2
-00007940: 5265 7370 6f6e 7365 2829 290a 0a20 2020  Response())..   
-00007950: 2020 2020 2020 2020 2069 6620 7273 702e           if rsp.
-00007960: 7265 7370 6f6e 7365 2e74 7970 6520 3d3d  response.type ==
-00007970: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
-00007980: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
-00007990: 4f4e 5345 5f57 4152 4e3a 0a20 2020 2020  ONSE_WARN:.     
-000079a0: 2020 2020 2020 2020 2020 2077 6172 6e28             warn(
-000079b0: 7273 702e 7265 7370 6f6e 7365 2e72 6561  rsp.response.rea
-000079c0: 736f 6e29 0a20 2020 2020 2020 2020 2020  son).           
-000079d0: 2065 6c69 6620 7273 702e 7265 7370 6f6e   elif rsp.respon
-000079e0: 7365 2e74 7970 6520 3d3d 2070 726f 746f  se.type == proto
-000079f0: 2e43 6f6e 6669 726d 6174 696f 6e52 6573  .ConfirmationRes
-00007a00: 706f 6e73 652e 5245 5350 4f4e 5345 5f4f  ponse.RESPONSE_O
-00007a10: 4b3a 0a20 2020 2020 2020 2020 2020 2020  K:.             
-00007a20: 2020 2023 2053 6176 6520 7468 6520 7365     # Save the se
-00007a30: 7276 6572 2073 6573 7369 6f6e 2069 640a  rver session id.
-00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a50: 7365 6c66 2e73 6572 7665 7253 6573 7369  self.serverSessi
-00007a60: 6f6e 4964 203d 2072 7370 2e73 6572 7665  onId = rsp.serve
-00007a70: 7253 6573 7369 6f6e 4964 0a20 2020 2020  rSessionId.     
-00007a80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007a90: 7365 7373 696f 6e20 3d20 5365 7373 696f  session = Sessio
-00007aa0: 6e28 7573 6572 416e 6450 6173 7377 6f72  n(userAndPasswor
-00007ab0: 643d 5573 6572 416e 6450 6173 7377 6f72  d=UserAndPasswor
-00007ac0: 6428 7365 6c66 2e75 7365 722c 2073 656c  d(self.user, sel
-00007ad0: 662e 7061 7373 776f 7264 2929 0a20 2020  f.password)).   
-00007ae0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00007af0: 6765 722e 696e 666f 2866 2243 6f6e 6e65  ger.info(f"Conne
-00007b00: 6374 6564 2074 6f20 7365 7276 6572 2073  cted to server s
-00007b10: 6573 7369 6f6e 2049 643a 207b 7365 6c66  ession Id: {self
-00007b20: 2e73 6572 7665 7253 6573 7369 6f6e 4964  .serverSessionId
-00007b30: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00007b40: 2020 2020 2320 5361 7665 2073 6563 6f6e      # Save secon
-00007b50: 6461 7279 2069 6e74 6572 6661 6365 732e  dary interfaces.
-00007b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b70: 2073 656c 662e 5f73 6176 655f 7365 636f   self._save_seco
-00007b80: 6e64 6172 795f 696e 7465 7266 6163 6573  ndary_interfaces
-00007b90: 2872 7370 2e73 6563 6f6e 6461 7279 290a  (rsp.secondary).
-00007ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007bb0: 2023 2052 6564 6972 6563 7420 7468 6520   # Redirect the 
-00007bc0: 636f 6e6e 6563 7469 6f6e 0a20 2020 2020  connection.     
-00007bd0: 2020 2020 2020 2020 2020 2069 6620 7273             if rs
-00007be0: 702e 7265 6469 7265 6374 3a0a 2020 2020  p.redirect:.    
-00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c00: 7365 6c66 2e73 6f63 6b2e 636c 6f73 6528  self.sock.close(
-00007c10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00007c20: 2020 2020 2020 6d61 7070 6564 5f68 6f73        mapped_hos
-00007c30: 742c 206d 6170 7065 645f 706f 7274 203d  t, mapped_port =
-00007c40: 2073 656c 662e 7265 736f 6c76 655f 6e65   self.resolve_ne
-00007c50: 775f 656e 6470 6f69 6e74 2872 7370 2e72  w_endpoint(rsp.r
-00007c60: 6564 6972 6563 7448 6f73 742c 2072 7370  edirectHost, rsp
-00007c70: 2e72 6564 6972 6563 7450 6f72 7429 0a20  .redirectPort). 
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00007ca0: 6622 5265 6469 7265 6374 696e 6720 636f  f"Redirecting co
-00007cb0: 6e6e 6563 7469 6f6e 2074 6f20 7b72 7370  nnection to {rsp
-00007cc0: 2e72 6564 6972 6563 7448 6f73 747d 3a7b  .redirectHost}:{
-00007cd0: 7273 702e 7265 6469 7265 6374 506f 7274  rsp.redirectPort
-00007ce0: 7d2c 2077 6869 6368 206d 6170 7320 746f  }, which maps to
-00007cf0: 207b 6d61 7070 6564 5f68 6f73 747d 3a7b   {mapped_host}:{
-00007d00: 6d61 7070 6564 5f70 6f72 747d 2229 0a20  mapped_port}"). 
-00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d20: 2020 2073 656c 662e 736f 636b 203d 2073     self.sock = s
-00007d30: 6f63 6b65 742e 6372 6561 7465 5f63 6f6e  ocket.create_con
-00007d40: 6e65 6374 696f 6e28 286d 6170 7065 645f  nection((mapped_
-00007d50: 686f 7374 2c20 6d61 7070 6564 5f70 6f72  host, mapped_por
-00007d60: 7429 290a 2020 2020 2020 2020 2020 2020  t)).            
-00007d70: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00007d80: 6e66 6f28 6622 436f 6e6e 6563 7465 6420  nfo(f"Connected 
-00007d90: 746f 207b 6d61 7070 6564 5f68 6f73 747d  to {mapped_host}
-00007da0: 3a7b 6d61 7070 6564 5f70 6f72 747d 206f  :{mapped_port} o
-00007db0: 6e20 736f 636b 6574 207b 7365 6c66 2e73  n socket {self.s
-00007dc0: 6f63 6b7d 2229 0a20 2020 2020 2020 2020  ock}").         
-00007dd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007de0: 5f73 736c 697a 655f 636f 6e6e 6563 7469  _sslize_connecti
-00007df0: 6f6e 2829 0a0a 2020 2020 2020 2020 2020  on()..          
-00007e00: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00007e10: 2073 656c 662e 5f63 6c69 656e 745f 6861   self._client_ha
-00007e20: 6e64 7368 616b 655f 4342 435f 4743 4d28  ndshake_CBC_GCM(
-00007e30: 6973 5f65 7870 6c69 6369 745f 7373 6f2c  is_explicit_sso,
-00007e40: 2054 7275 6529 0a0a 2020 2020 2020 2020   True)..        
-00007e50: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
-00007e60: 2020 2020 2020 2020 2020 2023 2074 6865             # the
-00007e70: 7265 2069 7320 736f 6d65 7468 696e 6720  re is something 
-00007e80: 6272 6f6b 656e 2069 6e20 6f75 7220 6861  broken in our ha
-00007e90: 6e64 7368 616b 652e 2e2e 7265 7472 790a  ndshake...retry.
-00007ea0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00007eb0: 7370 2e72 6573 706f 6e73 652e 7665 6e64  sp.response.vend
-00007ec0: 6f72 5f63 6f64 6520 3d3d 202d 3230 323a  or_code == -202:
-00007ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007ee0: 206c 6f67 6765 722e 6465 6275 6728 2248   logger.debug("H
-00007ef0: 616e 6473 6861 6b65 2065 7272 6f72 2e2e  andshake error..
-00007f00: 2e72 6574 7279 696e 6722 290a 2020 2020  .retrying").    
-00007f10: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00007f20: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
-00007f30: 2020 7261 6973 6520 5f63 6f6e 7665 7274    raise _convert
-00007f40: 5f65 7863 6570 7469 6f6e 2872 7370 2e72  _exception(rsp.r
-00007f50: 6573 706f 6e73 6529 0a0a 2020 2020 6465  esponse)..    de
-00007f60: 6620 5f63 6c69 656e 745f 6861 6e64 7368  f _client_handsh
-00007f70: 616b 655f 5353 4f28 7365 6c66 293a 0a20  ake_SSO(self):. 
-00007f80: 2020 2020 2020 2022 2222 496e 7465 726e         """Intern
-00007f90: 616c 2072 6f75 7469 6e65 2066 6f72 2073  al routine for s
-00007fa0: 696e 676c 6520 7369 676e 206f 6e20 6861  ingle sign on ha
-00007fb0: 6e64 7368 616b 6520 2853 534f 292e 0a20  ndshake (SSO).. 
-00007fc0: 2020 2020 2020 2031 2e20 4472 6976 6572         1. Driver
-00007fd0: 2072 6571 7565 7374 7320 746f 2073 6967   requests to sig
-00007fe0: 6e20 6f6e 2076 6961 2053 534f 2e0a 2020  n on via SSO..  
-00007ff0: 2020 2020 2020 322e 2053 6572 7665 7220        2. Server 
-00008000: 7365 6e64 7320 6261 636b 2061 6e20 6175  sends back an au
-00008010: 7468 7468 656e 7469 6361 7469 6f6e 2055  ththentication U
-00008020: 524c 2e0a 2020 2020 2020 2020 332e 2044  RL..        3. D
-00008030: 7269 7665 7220 6c61 756e 6368 6573 2055  river launches U
-00008040: 524c 2069 6e20 6465 6661 756c 7420 6272  RL in default br
-00008050: 6f77 7365 7220 286f 7220 7072 696e 7473  owser (or prints
-00008060: 2074 6865 2075 726c 2074 6f20 7374 6420   the url to std 
-00008070: 6f75 7420 6966 206e 6f74 2070 6f73 7369  out if not possi
-00008080: 626c 6529 0a20 2020 2020 2020 2034 2e20  ble).        4. 
-00008090: 5573 6572 2061 7574 6865 6e74 6963 6174  User authenticat
-000080a0: 6573 2069 6e20 6272 6f77 7365 722e 0a20  es in browser.. 
-000080b0: 2020 2020 2020 2035 2e20 4472 6976 6572         5. Driver
-000080c0: 2063 6f6e 7469 6e75 6f75 736c 7920 706f   continuously po
-000080d0: 6c6c 7320 7468 6520 6461 7461 6261 7365  lls the database
-000080e0: 2075 6e74 696c 206c 6f67 696e 2063 6f6d   until login com
-000080f0: 706c 6574 6573 2e0a 2020 2020 2020 2020  pletes..        
-00008100: 362e 2055 706f 6e20 636f 6d70 6c65 7465  6. Upon complete
-00008110: 7469 6f6e 2c20 7365 7276 6572 2073 656e  tion, server sen
-00008120: 6473 2062 6163 6b20 6120 7365 6375 7269  ds back a securi
-00008130: 7479 2074 6f6b 656e 2077 6974 6820 7768  ty token with wh
-00008140: 6963 6820 7468 6520 6472 6976 6572 2063  ich the driver c
-00008150: 616e 2063 6f6e 6e65 6374 2e20 2855 7365  an connect. (Use
-00008160: 6420 666f 7220 7265 6469 7265 6374 696e  d for redirectin
-00008170: 6720 2f20 7265 636f 6e6e 6563 7469 6e67  g / reconnecting
-00008180: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
-00008190: 2020 2020 2020 6672 6f6d 2077 6562 6272        from webbr
-000081a0: 6f77 7365 7220 696d 706f 7274 206f 7065  owser import ope
-000081b0: 6e5f 6e65 770a 0a20 2020 2020 2020 2072  n_new..        r
-000081c0: 6571 203d 2070 726f 746f 2e52 6571 7565  eq = proto.Reque
-000081d0: 7374 2829 0a20 2020 2020 2020 2072 6571  st().        req
-000081e0: 2e74 7970 6520 3d20 7265 712e 434c 4945  .type = req.CLIE
-000081f0: 4e54 5f43 4f4e 4e45 4354 494f 4e5f 5353  NT_CONNECTION_SS
-00008200: 4f0a 2020 2020 2020 2020 636c 6965 6e74  O.        client
-00008210: 5f63 6f6e 6e65 6374 696f 6e20 3d20 7265  _connection = re
-00008220: 712e 636c 6965 6e74 5f63 6f6e 6e65 6374  q.client_connect
-00008230: 696f 6e5f 7373 6f0a 0a20 2020 2020 2020  ion_sso..       
-00008240: 2073 656c 662e 5f69 6e69 7469 616c 697a   self._initializ
-00008250: 655f 636c 6965 6e74 5f63 6f6e 6e65 6374  e_client_connect
-00008260: 696f 6e28 636c 6965 6e74 5f63 6f6e 6e65  ion(client_conne
-00008270: 6374 696f 6e29 0a20 2020 2020 2020 2023  ction).        #
-00008280: 2053 656e 6420 6d65 7373 6167 650a 2020   Send message.  
-00008290: 2020 2020 2020 5f73 656e 645f 6d73 6728        _send_msg(
-000082a0: 7365 6c66 2c20 7265 7129 0a20 2020 2020  self, req).     
-000082b0: 2020 2023 2052 6563 6569 7665 2072 6573     # Receive res
-000082c0: 706f 6e73 650a 2020 2020 2020 2020 7273  ponse.        rs
-000082d0: 7020 3d20 5f72 6563 765f 6d73 6728 7365  p = _recv_msg(se
-000082e0: 6c66 2c20 7072 6f74 6f2e 436c 6965 6e74  lf, proto.Client
-000082f0: 436f 6e6e 6563 7469 6f6e 5353 4f52 6573  ConnectionSSORes
-00008300: 706f 6e73 6528 2929 0a0a 2020 2020 2020  ponse())..      
-00008310: 2020 6966 2072 7370 2e72 6573 706f 6e73    if rsp.respons
-00008320: 652e 7479 7065 203d 3d20 7072 6f74 6f2e  e.type == proto.
-00008330: 436f 6e66 6972 6d61 7469 6f6e 5265 7370  ConfirmationResp
-00008340: 6f6e 7365 2e52 4553 504f 4e53 455f 5741  onse.RESPONSE_WA
-00008350: 524e 3a0a 2020 2020 2020 2020 2020 2020  RN:.            
-00008360: 7761 726e 2872 7370 2e72 6573 706f 6e73  warn(rsp.respons
-00008370: 652e 7265 6173 6f6e 290a 2020 2020 2020  e.reason).      
-00008380: 2020 656c 6966 206e 6f74 2072 7370 2e72    elif not rsp.r
-00008390: 6573 706f 6e73 652e 7479 7065 203d 3d20  esponse.type == 
-000083a0: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
-000083b0: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
-000083c0: 4e53 455f 4f4b 3a0a 2020 2020 2020 2020  NSE_OK:.        
-000083d0: 2020 2020 7261 6973 6520 5f63 6f6e 7665      raise _conve
-000083e0: 7274 5f65 7863 6570 7469 6f6e 2872 7370  rt_exception(rsp
-000083f0: 2e72 6573 706f 6e73 6529 0a0a 2020 2020  .response)..    
-00008400: 2020 2020 2320 4f70 656e 2062 726f 7773      # Open brows
-00008410: 6572 2066 6f72 2075 7365 7220 746f 2061  er for user to a
-00008420: 7574 6865 6e74 6963 6174 652e 0a20 2020  uthenticate..   
-00008430: 2020 2020 2069 6620 6e6f 7420 6f70 656e       if not open
-00008440: 5f6e 6577 2872 7370 2e61 7574 6855 726c  _new(rsp.authUrl
-00008450: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
-00008460: 6f67 6765 722e 696e 666f 2822 5b70 796f  ogger.info("[pyo
-00008470: 6369 656e 745d 2043 6f75 6c64 206e 6f74  cient] Could not
-00008480: 206f 7065 6e20 6465 6661 756c 7420 6272   open default br
-00008490: 6f77 7365 7220 7769 7468 2077 6562 6272  owser with webbr
-000084a0: 6f77 7365 7220 6c69 6272 6172 792e 2050  owser library. P
-000084b0: 6c65 6173 6520 6175 7468 656e 7469 6361  lease authentica
-000084c0: 7465 2061 743a 2022 202b 2072 7370 2e61  te at: " + rsp.a
-000084d0: 7574 6855 726c 290a 2020 2020 2020 2020  uthUrl).        
-000084e0: 2020 2020 7072 696e 7428 225b 7079 6f63      print("[pyoc
-000084f0: 6965 6e74 5d20 436f 756c 6420 6e6f 7420  ient] Could not 
-00008500: 6f70 656e 2064 6566 6175 6c74 2062 726f  open default bro
-00008510: 7773 6572 2077 6974 6820 7765 6262 726f  wser with webbro
-00008520: 7773 6572 206c 6962 7261 7279 2e20 506c  wser library. Pl
-00008530: 6561 7365 2061 7574 6865 6e74 6963 6174  ease authenticat
-00008540: 6520 6174 3a20 222c 2072 7370 2e61 7574  e at: ", rsp.aut
-00008550: 6855 726c 290a 0a20 2020 2020 2020 2023  hUrl)..        #
-00008560: 2050 6f6c 6c20 7468 6520 6461 7461 6261   Poll the databa
-00008570: 7365 0a20 2020 2020 2020 2073 656c 662e  se.        self.
-00008580: 5f70 6f6c 6c5f 6461 7461 6261 7365 2872  _poll_database(r
-00008590: 7370 2e72 6571 7565 7374 4964 290a 0a20  sp.requestId).. 
-000085a0: 2020 2064 6566 205f 706f 6c6c 5f64 6174     def _poll_dat
-000085b0: 6162 6173 6528 7365 6c66 2c20 7265 7175  abase(self, requ
-000085c0: 6573 7449 6429 3a0a 2020 2020 2020 2020  estId):.        
-000085d0: 2222 2250 6f6c 6c73 2074 6865 2064 6174  """Polls the dat
-000085e0: 6162 6173 6520 756e 7469 6c20 7765 2065  abase until we e
-000085f0: 6974 6865 7220 7265 6365 6976 6520 616e  ither receive an
-00008600: 2065 7272 6f72 206f 7220 6120 7375 6363   error or a succ
-00008610: 6573 7366 756c 206c 6f67 696e 206d 6573  essful login mes
-00008620: 7361 6765 2e0a 0a20 2020 2020 2020 2041  sage...        A
-00008630: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00008640: 2072 6571 7565 7374 4964 2028 5374 7269   requestId (Stri
-00008650: 6e67 293a 2074 6865 2072 6571 7565 7374  ng): the request
-00008660: 2049 4420 6173 736f 6369 6174 6564 2077   ID associated w
-00008670: 6974 6820 7468 6973 206c 6f67 696e 2061  ith this login a
-00008680: 7474 656d 7074 2e0a 2020 2020 2020 2020  ttempt..        
-00008690: 2222 220a 0a20 2020 2020 2020 2072 6571  """..        req
-000086a0: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
-000086b0: 2829 0a20 2020 2020 2020 2072 6571 2e74  ().        req.t
-000086c0: 7970 6520 3d20 7265 712e 434c 4945 4e54  ype = req.CLIENT
-000086d0: 5f43 4f4e 4e45 4354 494f 4e5f 5353 4f32  _CONNECTION_SSO2
-000086e0: 0a20 2020 2020 2020 2072 6571 2e63 6c69  .        req.cli
-000086f0: 656e 745f 636f 6e6e 6563 7469 6f6e 5f73  ent_connection_s
-00008700: 736f 322e 666f 7263 6520 3d20 7365 6c66  so2.force = self
-00008710: 2e66 6f72 6365 0a20 2020 2020 2020 2072  .force.        r
-00008720: 6571 2e63 6c69 656e 745f 636f 6e6e 6563  eq.client_connec
-00008730: 7469 6f6e 5f73 736f 322e 7265 7175 6573  tion_sso2.reques
-00008740: 7449 6420 3d20 7265 7175 6573 7449 640a  tId = requestId.
-00008750: 0a20 2020 2020 2020 206b 6565 7050 6f6c  .        keepPol
-00008760: 6c69 6e67 203d 2054 7275 650a 2020 2020  ling = True.    
-00008770: 2020 2020 7761 6974 466f 7220 3d20 300a      waitFor = 0.
-00008780: 2020 2020 2020 2020 7768 696c 6520 6b65          while ke
-00008790: 6570 506f 6c6c 696e 673a 0a20 2020 2020  epPolling:.     
-000087a0: 2020 2020 2020 2073 6c65 6570 2877 6169         sleep(wai
-000087b0: 7446 6f72 290a 2020 2020 2020 2020 2020  tFor).          
-000087c0: 2020 2320 506f 6c6c 0a20 2020 2020 2020    # Poll.       
-000087d0: 2020 2020 205f 7365 6e64 5f6d 7367 2873       _send_msg(s
-000087e0: 656c 662c 2072 6571 290a 0a20 2020 2020  elf, req)..     
-000087f0: 2020 2020 2020 2023 2052 6563 6569 7665         # Receive
-00008800: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
-00008810: 2020 2020 2020 7273 7020 3d20 5f72 6563        rsp = _rec
-00008820: 765f 6d73 6728 7365 6c66 2c20 7072 6f74  v_msg(self, prot
-00008830: 6f2e 436c 6965 6e74 436f 6e6e 6563 7469  o.ClientConnecti
-00008840: 6f6e 5353 4f32 5265 7370 6f6e 7365 2829  onSSO2Response()
-00008850: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00008860: 6620 7273 702e 7265 7370 6f6e 7365 2e74  f rsp.response.t
-00008870: 7970 6520 3d3d 2070 726f 746f 2e43 6f6e  ype == proto.Con
-00008880: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
-00008890: 652e 5245 5350 4f4e 5345 5f57 4152 4e3a  e.RESPONSE_WARN:
-000088a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000088b0: 2077 6172 6e28 7273 702e 7265 7370 6f6e   warn(rsp.respon
-000088c0: 7365 2e72 6561 736f 6e29 0a20 2020 2020  se.reason).     
-000088d0: 2020 2020 2020 2065 6c69 6620 6e6f 7420         elif not 
-000088e0: 7273 702e 7265 7370 6f6e 7365 2e74 7970  rsp.response.typ
-000088f0: 6520 3d3d 2070 726f 746f 2e43 6f6e 6669  e == proto.Confi
-00008900: 726d 6174 696f 6e52 6573 706f 6e73 652e  rmationResponse.
-00008910: 5245 5350 4f4e 5345 5f4f 4b3a 0a20 2020  RESPONSE_OK:.   
-00008920: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00008930: 7365 205f 636f 6e76 6572 745f 6578 6365  se _convert_exce
-00008940: 7074 696f 6e28 7273 702e 7265 7370 6f6e  ption(rsp.respon
-00008950: 7365 290a 0a20 2020 2020 2020 2020 2020  se)..           
-00008960: 2069 6620 7273 702e 4861 7346 6965 6c64   if rsp.HasField
-00008970: 2822 706f 6c6c 696e 6749 6e74 6572 7661  ("pollingInterva
-00008980: 6c53 6563 6f6e 6473 2229 3a0a 2020 2020  lSeconds"):.    
-00008990: 2020 2020 2020 2020 2020 2020 2320 436f              # Co
-000089a0: 6e74 696e 7565 2070 6f6c 6c69 6e67 0a20  ntinue polling. 
-000089b0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-000089c0: 6169 7446 6f72 203d 2072 7370 2e70 6f6c  aitFor = rsp.pol
-000089d0: 6c69 6e67 496e 7465 7276 616c 5365 636f  lingIntervalSeco
-000089e0: 6e64 730a 2020 2020 2020 2020 2020 2020  nds.            
-000089f0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-00008a00: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00008a10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00008a20: 2053 7563 6365 7373 0a20 2020 2020 2020   Success.       
-00008a30: 2020 2020 2020 2020 2077 6169 7446 6f72           waitFor
-00008a40: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
-00008a50: 2020 2020 206b 6565 7050 6f6c 6c69 6e67       keepPolling
-00008a60: 203d 2046 616c 7365 0a0a 2020 2020 2020   = False..      
-00008a70: 2020 7365 6c66 2e73 6572 7665 7253 6573    self.serverSes
-00008a80: 7369 6f6e 4964 203d 2072 7370 2e73 6573  sionId = rsp.ses
-00008a90: 7369 6f6e 496e 666f 2e73 6572 7665 7253  sionInfo.serverS
-00008aa0: 6573 7369 6f6e 4964 0a20 2020 2020 2020  essionId.       
-00008ab0: 206c 6f67 6765 722e 6465 6275 6728 6622   logger.debug(f"
-00008ac0: 436f 6e6e 6563 7465 6420 746f 2073 6572  Connected to ser
-00008ad0: 7665 7220 7365 7373 696f 6e20 4964 3a20  ver session Id: 
-00008ae0: 7b73 656c 662e 7365 7276 6572 5365 7373  {self.serverSess
-00008af0: 696f 6e49 647d 2229 0a20 2020 2020 2020  ionId}").       
-00008b00: 2072 6563 6569 7665 645f 746f 6b65 6e20   received_token 
-00008b10: 3d20 7273 702e 7365 7373 696f 6e49 6e66  = rsp.sessionInf
-00008b20: 6f2e 7365 6375 7269 7479 546f 6b65 6e0a  o.securityToken.
-00008b30: 2020 2020 2020 2020 7365 6c66 2e73 6573          self.ses
-00008b40: 7369 6f6e 203d 2053 6573 7369 6f6e 2873  sion = Session(s
-00008b50: 6563 7572 6974 7954 6f6b 656e 3d53 6563  ecurityToken=Sec
-00008b60: 7572 6974 7954 6f6b 656e 2872 6563 6569  urityToken(recei
-00008b70: 7665 645f 746f 6b65 6e2e 6461 7461 2c20  ved_token.data, 
-00008b80: 7265 6365 6976 6564 5f74 6f6b 656e 2e73  received_token.s
-00008b90: 6967 6e61 7475 7265 2c20 7265 6365 6976  ignature, receiv
-00008ba0: 6564 5f74 6f6b 656e 2e69 7373 7565 7246  ed_token.issuerF
-00008bb0: 696e 6765 7270 7269 6e74 2929 0a0a 2020  ingerprint))..  
-00008bc0: 2020 2020 2020 2320 5361 7665 2073 6563        # Save sec
-00008bd0: 6f6e 6461 7279 2069 6e74 6572 6661 6365  ondary interface
-00008be0: 732e 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-00008bf0: 5f73 6176 655f 7365 636f 6e64 6172 795f  _save_secondary_
-00008c00: 696e 7465 7266 6163 6573 2872 7370 2e73  interfaces(rsp.s
-00008c10: 6563 6f6e 6461 7279 290a 0a20 2020 2020  econdary)..     
-00008c20: 2020 2023 2052 6564 6972 6563 7420 7468     # Redirect th
-00008c30: 6520 636f 6e6e 6563 7469 6f6e 0a20 2020  e connection.   
-00008c40: 2020 2020 2069 6620 7273 702e 7265 6469       if rsp.redi
-00008c50: 7265 6374 3a0a 2020 2020 2020 2020 2020  rect:.          
-00008c60: 2020 7365 6c66 2e73 6f63 6b2e 636c 6f73    self.sock.clos
-00008c70: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00008c80: 6d61 7070 6564 5f68 6f73 742c 206d 6170  mapped_host, map
-00008c90: 7065 645f 706f 7274 203d 2073 656c 662e  ped_port = self.
-00008ca0: 7265 736f 6c76 655f 6e65 775f 656e 6470  resolve_new_endp
-00008cb0: 6f69 6e74 2872 7370 2e72 6564 6972 6563  oint(rsp.redirec
-00008cc0: 7448 6f73 742c 2072 7370 2e72 6564 6972  tHost, rsp.redir
-00008cd0: 6563 7450 6f72 7429 0a20 2020 2020 2020  ectPort).       
-00008ce0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00008cf0: 6728 6622 5265 6469 7265 6374 696e 6720  g(f"Redirecting 
-00008d00: 636f 6e6e 6563 7469 6f6e 2074 6f20 7b72  connection to {r
-00008d10: 7370 2e72 6564 6972 6563 7448 6f73 747d  sp.redirectHost}
-00008d20: 3a7b 7273 702e 7265 6469 7265 6374 506f  :{rsp.redirectPo
-00008d30: 7274 7d2c 2077 6869 6368 206d 6170 7320  rt}, which maps 
-00008d40: 746f 207b 6d61 7070 6564 5f68 6f73 747d  to {mapped_host}
-00008d50: 3a7b 6d61 7070 6564 5f70 6f72 747d 2229  :{mapped_port}")
-00008d60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008d70: 662e 736f 636b 203d 2073 6f63 6b65 742e  f.sock = socket.
-00008d80: 6372 6561 7465 5f63 6f6e 6e65 6374 696f  create_connectio
-00008d90: 6e28 286d 6170 7065 645f 686f 7374 2c20  n((mapped_host, 
-00008da0: 6d61 7070 6564 5f70 6f72 7429 290a 2020  mapped_port)).  
-00008db0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00008dc0: 2e69 6e66 6f28 6622 436f 6e6e 6563 7465  .info(f"Connecte
-00008dd0: 6420 746f 207b 6d61 7070 6564 5f68 6f73  d to {mapped_hos
-00008de0: 747d 3a7b 6d61 7070 6564 5f70 6f72 747d  t}:{mapped_port}
-00008df0: 206f 6e20 736f 636b 6574 207b 7365 6c66   on socket {self
-00008e00: 2e73 6f63 6b7d 2229 0a20 2020 2020 2020  .sock}").       
-00008e10: 2020 2020 2073 656c 662e 5f73 736c 697a       self._ssliz
-00008e20: 655f 636f 6e6e 6563 7469 6f6e 2829 0a0a  e_connection()..
-00008e30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00008e40: 726e 2073 656c 662e 5f63 6c69 656e 745f  rn self._client_
-00008e50: 6861 6e64 7368 616b 655f 7365 6375 7269  handshake_securi
-00008e60: 7479 5f74 6f6b 656e 2854 7275 6529 0a0a  ty_token(True)..
-00008e70: 2020 2020 6465 6620 5f63 6c69 656e 745f      def _client_
-00008e80: 6861 6e64 7368 616b 655f 7365 6375 7269  handshake_securi
-00008e90: 7479 5f74 6f6b 656e 2873 656c 662c 2066  ty_token(self, f
-00008ea0: 6f72 6365 3d46 616c 7365 293a 0a20 2020  orce=False):.   
-00008eb0: 2020 2020 2022 2222 4f6e 6365 2061 2063       """Once a c
-00008ec0: 6f6e 6e65 6374 696f 6e20 6163 7175 6972  onnection acquir
-00008ed0: 6573 2061 2073 6563 7572 6974 7920 746f  es a security to
-00008ee0: 6b65 6e2c 2069 7420 6361 6e20 7573 6520  ken, it can use 
-00008ef0: 7468 6174 2074 6f20 6c6f 6720 696e 2e20  that to log in. 
-00008f00: 5468 6973 2068 616e 6473 6861 6b65 206f  This handshake o
-00008f10: 6e6c 790a 2020 2020 2020 2020 7365 6e64  nly.        send
-00008f20: 7320 3120 6d65 7373 6167 6520 7768 6572  s 1 message wher
-00008f30: 6561 7320 7468 6520 6f74 6865 7220 6861  eas the other ha
-00008f40: 6e64 7368 616b 6573 2073 656e 6420 322e  ndshakes send 2.
-00008f50: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00008f60: 2020 2020 2077 6869 6c65 2054 7275 653a       while True:
-00008f70: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-00008f80: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
-00008f90: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
-00008fa0: 6571 2e74 7970 6520 3d20 7265 712e 434c  eq.type = req.CL
-00008fb0: 4945 4e54 5f43 4f4e 4e45 4354 494f 4e5f  IENT_CONNECTION_
-00008fc0: 5345 4355 5249 5459 5f54 4f4b 454e 0a20  SECURITY_TOKEN. 
-00008fd0: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
-00008fe0: 745f 636f 6e6e 6563 7469 6f6e 203d 2072  t_connection = r
-00008ff0: 6571 2e63 6c69 656e 745f 636f 6e6e 6563  eq.client_connec
-00009000: 7469 6f6e 5f73 6563 7572 6974 795f 746f  tion_security_to
-00009010: 6b65 6e0a 0a20 2020 2020 2020 2020 2020  ken..           
-00009020: 2073 656c 662e 5f69 6e69 7469 616c 697a   self._initializ
-00009030: 655f 636c 6965 6e74 5f63 6f6e 6e65 6374  e_client_connect
-00009040: 696f 6e28 636c 6965 6e74 5f63 6f6e 6e65  ion(client_conne
-00009050: 6374 696f 6e29 0a20 2020 2020 2020 2020  ction).         
-00009060: 2020 2023 2041 7474 6163 6820 7468 6520     # Attach the 
-00009070: 7365 6375 7269 7479 2074 6f6b 656e 2075  security token u
-00009080: 7365 6420 746f 206c 6f67 2069 6e0a 2020  sed to log in.  
-00009090: 2020 2020 2020 2020 2020 636c 6965 6e74            client
-000090a0: 5f63 6f6e 6e65 6374 696f 6e2e 7365 6375  _connection.secu
-000090b0: 7269 7479 546f 6b65 6e20 3d20 7365 6c66  rityToken = self
-000090c0: 2e73 6573 7369 6f6e 2e73 6563 7572 6974  .session.securit
-000090d0: 7954 6f6b 656e 2e74 6f6b 656e 4461 7461  yToken.tokenData
-000090e0: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-000090f0: 656e 745f 636f 6e6e 6563 7469 6f6e 2e74  ent_connection.t
-00009100: 6f6b 656e 5369 676e 6174 7572 6520 3d20  okenSignature = 
-00009110: 7365 6c66 2e73 6573 7369 6f6e 2e73 6563  self.session.sec
-00009120: 7572 6974 7954 6f6b 656e 2e74 6f6b 656e  urityToken.token
-00009130: 5369 676e 6174 7572 650a 2020 2020 2020  Signature.      
-00009140: 2020 2020 2020 636c 6965 6e74 5f63 6f6e        client_con
-00009150: 6e65 6374 696f 6e2e 6973 7375 6572 4669  nection.issuerFi
-00009160: 6e67 6572 7072 696e 7420 3d20 7365 6c66  ngerprint = self
-00009170: 2e73 6573 7369 6f6e 2e73 6563 7572 6974  .session.securit
-00009180: 7954 6f6b 656e 2e69 7373 7565 7246 696e  yToken.issuerFin
-00009190: 6765 7270 7269 6e74 0a20 2020 2020 2020  gerprint.       
-000091a0: 2020 2020 2063 6c69 656e 745f 636f 6e6e       client_conn
-000091b0: 6563 7469 6f6e 2e66 6f72 6365 203d 2066  ection.force = f
-000091c0: 6f72 6365 0a0a 2020 2020 2020 2020 2020  orce..          
-000091d0: 2020 5f73 656e 645f 6d73 6728 7365 6c66    _send_msg(self
-000091e0: 2c20 7265 7129 0a0a 2020 2020 2020 2020  , req)..        
-000091f0: 2020 2020 7273 7020 3d20 5f72 6563 765f      rsp = _recv_
-00009200: 6d73 6728 7365 6c66 2c20 7072 6f74 6f2e  msg(self, proto.
-00009210: 436c 6965 6e74 436f 6e6e 6563 7469 6f6e  ClientConnection
-00009220: 5365 6375 7269 7479 546f 6b65 6e52 6573  SecurityTokenRes
-00009230: 706f 6e73 6528 2929 0a0a 2020 2020 2020  ponse())..      
-00009240: 2020 2020 2020 6966 2072 7370 2e72 6573        if rsp.res
-00009250: 706f 6e73 652e 7479 7065 203d 3d20 7072  ponse.type == pr
-00009260: 6f74 6f2e 436f 6e66 6972 6d61 7469 6f6e  oto.Confirmation
-00009270: 5265 7370 6f6e 7365 2e52 4553 504f 4e53  Response.RESPONS
-00009280: 455f 5741 524e 3a0a 2020 2020 2020 2020  E_WARN:.        
-00009290: 2020 2020 2020 2020 7761 726e 2872 7370          warn(rsp
-000092a0: 2e72 6573 706f 6e73 652e 7265 6173 6f6e  .response.reason
-000092b0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000092c0: 6966 2072 7370 2e72 6573 706f 6e73 652e  if rsp.response.
-000092d0: 7479 7065 203d 3d20 7072 6f74 6f2e 436f  type == proto.Co
-000092e0: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
-000092f0: 7365 2e52 4553 504f 4e53 455f 4f4b 3a0a  se.RESPONSE_OK:.
-00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009310: 2320 5361 7665 2073 6563 6f6e 6461 7279  # Save secondary
-00009320: 2069 6e74 6572 6661 6365 732e 0a20 2020   interfaces..   
-00009330: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00009340: 662e 5f73 6176 655f 7365 636f 6e64 6172  f._save_secondar
-00009350: 795f 696e 7465 7266 6163 6573 2872 7370  y_interfaces(rsp
-00009360: 2e73 6563 6f6e 6461 7279 290a 2020 2020  .secondary).    
-00009370: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
-00009380: 6469 7265 6374 2074 6865 2063 6f6e 6e65  direct the conne
-00009390: 6374 696f 6e20 6966 2072 6571 7565 7374  ction if request
-000093a0: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
-000093b0: 2020 2069 6620 7273 702e 7265 6469 7265     if rsp.redire
-000093c0: 6374 3a0a 2020 2020 2020 2020 2020 2020  ct:.            
-000093d0: 2020 2020 2020 2020 7365 6c66 2e73 6f63          self.soc
-000093e0: 6b2e 636c 6f73 6528 290a 2020 2020 2020  k.close().      
-000093f0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00009400: 7070 6564 5f68 6f73 742c 206d 6170 7065  pped_host, mappe
-00009410: 645f 706f 7274 203d 2073 656c 662e 7265  d_port = self.re
-00009420: 736f 6c76 655f 6e65 775f 656e 6470 6f69  solve_new_endpoi
-00009430: 6e74 2872 7370 2e72 6564 6972 6563 7448  nt(rsp.redirectH
-00009440: 6f73 742c 2072 7370 2e72 6564 6972 6563  ost, rsp.redirec
-00009450: 7450 6f72 7429 0a20 2020 2020 2020 2020  tPort).         
-00009460: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00009470: 722e 6465 6275 6728 6622 5265 6469 7265  r.debug(f"Redire
-00009480: 6374 696e 6720 636f 6e6e 6563 7469 6f6e  cting connection
-00009490: 2074 6f20 7b72 7370 2e72 6564 6972 6563   to {rsp.redirec
-000094a0: 7448 6f73 747d 3a7b 7273 702e 7265 6469  tHost}:{rsp.redi
-000094b0: 7265 6374 506f 7274 7d2c 2077 6869 6368  rectPort}, which
-000094c0: 206d 6170 7320 746f 207b 6d61 7070 6564   maps to {mapped
-000094d0: 5f68 6f73 747d 3a7b 6d61 7070 6564 5f70  _host}:{mapped_p
-000094e0: 6f72 747d 2229 0a20 2020 2020 2020 2020  ort}").         
-000094f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009500: 736f 636b 203d 2073 6f63 6b65 742e 6372  sock = socket.cr
-00009510: 6561 7465 5f63 6f6e 6e65 6374 696f 6e28  eate_connection(
-00009520: 286d 6170 7065 645f 686f 7374 2c20 6d61  (mapped_host, ma
-00009530: 7070 6564 5f70 6f72 7429 290a 2020 2020  pped_port)).    
-00009540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009550: 6c6f 6767 6572 2e69 6e66 6f28 6622 436f  logger.info(f"Co
-00009560: 6e6e 6563 7465 6420 746f 207b 6d61 7070  nnected to {mapp
-00009570: 6564 5f68 6f73 747d 3a7b 6d61 7070 6564  ed_host}:{mapped
-00009580: 5f70 6f72 747d 206f 6e20 736f 636b 6574  _port} on socket
-00009590: 207b 7365 6c66 2e73 6f63 6b7d 2229 0a20   {self.sock}"). 
-000095a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095b0: 2020 2073 656c 662e 5f73 736c 697a 655f     self._sslize_
-000095c0: 636f 6e6e 6563 7469 6f6e 2829 0a0a 2020  connection()..  
-000095d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095e0: 2020 7265 7475 726e 2073 656c 662e 5f63    return self._c
-000095f0: 6c69 656e 745f 6861 6e64 7368 616b 655f  lient_handshake_
-00009600: 7365 6375 7269 7479 5f74 6f6b 656e 2854  security_token(T
-00009610: 7275 6529 0a0a 2020 2020 2020 2020 2020  rue)..          
-00009620: 2020 2020 2020 2320 4361 7074 7572 6520        # Capture 
-00009630: 7468 6520 7365 7373 696f 6e20 6964 0a20  the session id. 
-00009640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00009650: 656c 662e 7365 7276 6572 5365 7373 696f  elf.serverSessio
-00009660: 6e49 6420 3d20 7273 702e 7365 7276 6572  nId = rsp.server
-00009670: 5365 7373 696f 6e49 640a 2020 2020 2020  SessionId.      
-00009680: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00009690: 2e64 6562 7567 2866 2243 6f6e 6e65 6374  .debug(f"Connect
-000096a0: 6564 2074 6f20 7365 7276 6572 2073 6573  ed to server ses
-000096b0: 7369 6f6e 2049 643a 207b 7365 6c66 2e73  sion Id: {self.s
-000096c0: 6572 7665 7253 6573 7369 6f6e 4964 7d22  erverSessionId}"
-000096d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000096e0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-000096f0: 2020 2020 2320 7468 6572 6520 6973 2073      # there is s
-00009700: 6f6d 6574 6869 6e67 2062 726f 6b65 6e20  omething broken 
-00009710: 696e 206f 7572 2068 616e 6473 6861 6b65  in our handshake
-00009720: 2e2e 2e72 6574 7279 0a20 2020 2020 2020  ...retry.       
-00009730: 2020 2020 2069 6620 7273 702e 7265 7370       if rsp.resp
-00009740: 6f6e 7365 2e76 656e 646f 725f 636f 6465  onse.vendor_code
-00009750: 203d 3d20 2d32 3032 3a0a 2020 2020 2020   == -202:.      
-00009760: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00009770: 2e64 6562 7567 2822 4861 6e64 7368 616b  .debug("Handshak
-00009780: 6520 6572 726f 722e 2e2e 7265 7472 7969  e error...retryi
-00009790: 6e67 2229 0a20 2020 2020 2020 2020 2020  ng").           
-000097a0: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-000097b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000097c0: 205f 636f 6e76 6572 745f 6578 6365 7074   _convert_except
-000097d0: 696f 6e28 7273 702e 7265 7370 6f6e 7365  ion(rsp.response
-000097e0: 290a 0a20 2020 2064 6566 205f 7361 7665  )..    def _save
-000097f0: 5f73 6563 6f6e 6461 7279 5f69 6e74 6572  _secondary_inter
-00009800: 6661 6365 7328 7365 6c66 2c20 6e65 775f  faces(self, new_
-00009810: 7365 636f 6e64 6172 795f 696e 7465 7266  secondary_interf
-00009820: 6163 6573 293a 0a20 2020 2020 2020 2022  aces):.        "
-00009830: 2222 4166 7465 7220 7365 636f 6e64 6172  ""After secondar
-00009840: 7920 696e 7465 7266 6163 6573 2061 7265  y interfaces are
-00009850: 2073 656e 7420 6672 6f6d 2074 6865 2073   sent from the s
-00009860: 6572 7665 722c 2077 6520 6e65 6564 2074  erver, we need t
-00009870: 6f0a 2020 2020 2020 2020 7361 7665 2074  o.        save t
-00009880: 6865 6d20 616e 6420 7573 6520 7468 656d  hem and use them
-00009890: 2066 6f72 2072 6564 6972 6563 7469 6e67   for redirecting
-000098a0: 2e20 5468 6973 2069 7320 696d 706f 7274  . This is import
-000098b0: 616e 7420 6966 2077 650a 2020 2020 2020  ant if we.      
-000098c0: 2020 6765 7420 7265 6469 7265 6374 6564    get redirected
-000098d0: 2074 6f20 6d61 7070 6564 2073 716c 2065   to mapped sql e
-000098e0: 6e64 706f 696e 7473 2e0a 0a20 2020 2020  ndpoints...     
-000098f0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00009900: 2020 2020 2073 6563 6f6e 6461 7279 5f69       secondary_i
-00009910: 6e74 6572 6661 6365 7320 285b 636c 6173  nterfaces ([clas
-00009920: 7320 2767 6f6f 676c 652e 7072 6f74 6f62  s 'google.protob
-00009930: 7566 2e70 7965 7874 2e5f 6d65 7373 6167  uf.pyext._messag
-00009940: 652e 5265 7065 6174 6564 436f 6d70 6f73  e.RepeatedCompos
-00009950: 6974 6543 6f6e 7461 696e 6572 275d 293a  iteContainer']):
-00009960: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-00009970: 2073 6563 6f6e 6461 7279 2069 6e74 6572   secondary inter
-00009980: 6661 6365 732c 2077 6869 6368 2069 7320  faces, which is 
-00009990: 7265 616c 6c79 2061 206c 6973 7420 6f66  really a list of
-000099a0: 206c 6973 7420 6f66 2073 7472 696e 6773   list of strings
-000099b0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000099c0: 2020 2020 2020 7365 6c66 2e73 6563 6f6e        self.secon
-000099d0: 6461 7279 5f69 6e74 6572 6661 6365 7320  dary_interfaces 
-000099e0: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
-000099f0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00009a00: 6e65 775f 7365 636f 6e64 6172 795f 696e  new_secondary_in
-00009a10: 7465 7266 6163 6573 2929 3a0a 2020 2020  terfaces)):.    
-00009a20: 2020 2020 2020 2020 7365 6c66 2e73 6563          self.sec
-00009a30: 6f6e 6461 7279 5f69 6e74 6572 6661 6365  ondary_interface
-00009a40: 732e 6170 7065 6e64 285b 5d29 0a20 2020  s.append([]).   
-00009a50: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-00009a60: 6e20 7261 6e67 6528 6c65 6e28 6e65 775f  n range(len(new_
-00009a70: 7365 636f 6e64 6172 795f 696e 7465 7266  secondary_interf
-00009a80: 6163 6573 5b69 5d2e 6164 6472 6573 7329  aces[i].address)
-00009a90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00009aa0: 2020 2069 6e74 6572 6661 6365 203d 206e     interface = n
-00009ab0: 6577 5f73 6563 6f6e 6461 7279 5f69 6e74  ew_secondary_int
-00009ac0: 6572 6661 6365 735b 695d 2e61 6464 7265  erfaces[i].addre
-00009ad0: 7373 5b6a 5d0a 2020 2020 2020 2020 2020  ss[j].          
-00009ae0: 2020 2020 2020 2869 6e74 6572 6661 6365        (interface
-00009af0: 5f69 702c 2069 6e74 6572 6661 6365 5f70  _ip, interface_p
-00009b00: 6f72 7429 203d 2069 6e74 6572 6661 6365  ort) = interface
-00009b10: 2e73 706c 6974 2822 3a22 290a 2020 2020  .split(":").    
-00009b20: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
-00009b30: 7475 726e 206f 6620 6765 7468 6f73 7462  turn of gethostb
-00009b40: 796e 616d 655f 6578 2069 7320 2868 6f73  yname_ex is (hos
-00009b50: 746e 616d 652c 2061 6c69 6173 206f 6620  tname, alias of 
-00009b60: 686f 7374 206e 616d 652c 206f 7468 6572  host name, other
-00009b70: 2069 7020 6164 6472 6573 7365 7320 6f66   ip addresses of
-00009b80: 2068 6f73 7420 6e61 6d65 290a 2020 2020   host name).    
-00009b90: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-00009ba0: 725f 6970 7320 3d20 736f 636b 6574 2e67  r_ips = socket.g
-00009bb0: 6574 686f 7374 6279 6e61 6d65 5f65 7828  ethostbyname_ex(
-00009bc0: 696e 7465 7266 6163 655f 6970 295b 325d  interface_ip)[2]
-00009bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009be0: 2066 6f72 206f 7468 6572 5f69 7020 696e   for other_ip in
-00009bf0: 206f 7468 6572 5f69 7073 3a0a 2020 2020   other_ips:.    
-00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c10: 7365 6c66 2e73 6563 6f6e 6461 7279 5f69  self.secondary_i
-00009c20: 6e74 6572 6661 6365 735b 695d 2e61 7070  nterfaces[i].app
-00009c30: 656e 6428 286f 7468 6572 5f69 702c 2069  end((other_ip, i
-00009c40: 6e74 2869 6e74 6572 6661 6365 5f70 6f72  nt(interface_por
-00009c50: 7429 2929 0a0a 2020 2020 2020 2020 686f  t)))..        ho
-00009c60: 7374 7320 3d20 5b5d 0a20 2020 2020 2020  sts = [].       
-00009c70: 2066 6f72 206f 6e65 5f68 6f73 7420 696e   for one_host in
-00009c80: 2073 656c 662e 686f 7374 733a 0a20 2020   self.hosts:.   
-00009c90: 2020 2020 2020 2020 2068 6f73 7473 203d           hosts =
-00009ca0: 2068 6f73 7473 202b 205b 2868 6f73 742c   hosts + [(host,
-00009cb0: 2073 656c 662e 706f 7274 2920 666f 7220   self.port) for 
-00009cc0: 686f 7374 2069 6e20 736f 636b 6574 2e67  host in socket.g
-00009cd0: 6574 686f 7374 6279 6e61 6d65 5f65 7828  ethostbyname_ex(
-00009ce0: 6f6e 655f 686f 7374 295b 325d 5d0a 2020  one_host)[2]].  
-00009cf0: 2020 2020 2020 666f 7220 6f75 7465 725f        for outer_
-00009d00: 6c69 7374 2069 6e20 7365 6c66 2e73 6563  list in self.sec
-00009d10: 6f6e 6461 7279 5f69 6e74 6572 6661 6365  ondary_interface
-00009d20: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-00009d30: 6f72 2069 6e64 6578 2069 6e20 7261 6e67  or index in rang
-00009d40: 6528 6c65 6e28 6f75 7465 725f 6c69 7374  e(len(outer_list
-00009d50: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00009d60: 2020 2020 6966 206f 7574 6572 5f6c 6973      if outer_lis
-00009d70: 745b 696e 6465 785d 2069 6e20 686f 7374  t[index] in host
-00009d80: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00009d90: 2020 2020 2020 2073 656c 662e 7365 636f         self.seco
-00009da0: 6e64 6172 795f 696e 6465 7820 3d20 696e  ndary_index = in
-00009db0: 6465 780a 2020 2020 2020 2020 2020 2020  dex.            
-00009dc0: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
-00009dd0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00009de0: 6275 6728 6622 5361 7669 6e67 2073 6563  bug(f"Saving sec
-00009df0: 6f6e 6461 7279 2069 6e74 6572 6661 6365  ondary interface
-00009e00: 733a 2069 6e64 6578 207b 7365 6c66 2e73  s: index {self.s
-00009e10: 6563 6f6e 6461 7279 5f69 6e64 6578 7d20  econdary_index} 
-00009e20: 696e 7465 7266 6163 6573 3a20 7b73 656c  interfaces: {sel
-00009e30: 662e 7365 636f 6e64 6172 795f 696e 7465  f.secondary_inte
-00009e40: 7266 6163 6573 7d22 290a 0a20 2020 2064  rfaces}")..    d
-00009e50: 6566 205f 656e 6372 7970 7469 6f6e 5f72  ef _encryption_r
-00009e60: 6f75 7469 6e65 2873 656c 662c 2069 6e69  outine(self, ini
-00009e70: 7469 616c 697a 6174 696f 6e5f 7665 6374  tialization_vect
-00009e80: 6f72 2c20 7065 6572 5f6b 6579 293a 0a20  or, peer_key):. 
-00009e90: 2020 2020 2020 2022 2222 496e 7465 726e         """Intern
-00009ea0: 616c 2072 6f75 7469 6e65 2074 6f20 646f  al routine to do
-00009eb0: 2074 6865 2065 6e63 7279 7074 696f 6e20   the encryption 
-00009ec0: 6861 6e64 7368 616b 6520 6f66 0a20 2020  handshake of.   
-00009ed0: 2020 2020 2074 6865 2070 6173 7377 6f72       the passwor
-00009ee0: 640a 2020 2020 2020 2020 4342 4320 6973  d.        CBC is
-00009ef0: 2074 6865 2070 7265 7669 6f75 7320 666f   the previous fo
-00009f00: 726d 206f 6620 656e 6372 7970 7469 6f6e  rm of encryption
-00009f10: 2e20 5765 206e 6f77 2075 7365 2047 434d  . We now use GCM
-00009f20: 2062 7920 6465 6661 756c 742e 0a20 2020   by default..   
-00009f30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00009f40: 2023 2043 7265 6174 6520 6f75 7220 6b65   # Create our ke
-00009f50: 7973 2075 7369 6e67 2074 6865 2070 6172  ys using the par
-00009f60: 616d 6574 6572 7320 6672 6f6d 2074 6865  ameters from the
-00009f70: 2070 6565 7220 6b65 790a 2020 2020 2020   peer key.      
-00009f80: 2020 7061 7261 6d73 203d 2070 6565 725f    params = peer_
-00009f90: 6b65 792e 7061 7261 6d65 7465 7273 2829  key.parameters()
-00009fa0: 0a20 2020 2020 2020 2070 7269 7661 7465  .        private
-00009fb0: 5f6b 6579 203d 2070 6172 616d 732e 6765  _key = params.ge
-00009fc0: 6e65 7261 7465 5f70 7269 7661 7465 5f6b  nerate_private_k
-00009fd0: 6579 2829 0a0a 2020 2020 2020 2020 2320  ey()..        # 
-00009fe0: 4372 6561 7465 2061 2073 6861 7265 6420  Create a shared 
-00009ff0: 6b65 790a 2020 2020 2020 2020 7368 6172  key.        shar
-0000a000: 6564 5f6b 6579 203d 2070 7269 7661 7465  ed_key = private
-0000a010: 5f6b 6579 2e65 7863 6861 6e67 6528 7065  _key.exchange(pe
-0000a020: 6572 5f6b 6579 290a 0a20 2020 2020 2020  er_key)..       
-0000a030: 206b 6579 203d 205f 6861 7368 5f6b 6579   key = _hash_key
-0000a040: 2873 6861 7265 645f 6b65 792c 2062 225c  (shared_key, b"\
-0000a050: 3022 290a 2020 2020 2020 2020 6d61 635f  0").        mac_
-0000a060: 6b65 7920 3d20 5f68 6173 685f 6b65 7928  key = _hash_key(
-0000a070: 7368 6172 6564 5f6b 6579 2c20 6222 5c31  shared_key, b"\1
-0000a080: 2229 0a0a 2020 2020 2020 2020 6966 2073  ")..        if s
-0000a090: 656c 662e 6861 6e64 7368 616b 6520 3d3d  elf.handshake ==
-0000a0a0: 2073 656c 662e 4841 4e44 5348 414b 455f   self.HANDSHAKE_
-0000a0b0: 4342 433a 0a20 2020 2020 2020 2020 2020  CBC:.           
-0000a0c0: 2023 2050 6164 2074 6865 2070 6c61 696e   # Pad the plain
-0000a0d0: 7465 7874 2070 6173 7377 6f72 6420 6f75  text password ou
-0000a0e0: 7420 7573 696e 6720 504b 4353 370a 2020  t using PKCS7.  
-0000a0f0: 2020 2020 2020 2020 2020 7061 6464 6572            padder
-0000a100: 203d 2070 6164 6469 6e67 2e50 4b43 5337   = padding.PKCS7
-0000a110: 2831 3238 292e 7061 6464 6572 2829 0a20  (128).padder(). 
-0000a120: 2020 2020 2020 2020 2020 2070 6164 6465             padde
-0000a130: 645f 6461 7461 203d 2070 6164 6465 722e  d_data = padder.
-0000a140: 7570 6461 7465 2873 656c 662e 7061 7373  update(self.pass
-0000a150: 776f 7264 2e65 6e63 6f64 6528 656e 636f  word.encode(enco
-0000a160: 6469 6e67 3d22 5554 462d 3822 2c20 6572  ding="UTF-8", er
-0000a170: 726f 7273 3d22 7374 7269 6374 2229 290a  rors="strict")).
-0000a180: 2020 2020 2020 2020 2020 2020 7061 6464              padd
-0000a190: 6564 5f64 6174 6120 2b3d 2070 6164 6465  ed_data += padde
-0000a1a0: 722e 6669 6e61 6c69 7a65 2829 0a0a 2020  r.finalize()..  
-0000a1b0: 2020 2020 2020 2020 2020 2320 456e 6372            # Encr
-0000a1c0: 7970 7420 7468 6520 7061 6464 6564 2070  ypt the padded p
-0000a1d0: 6c61 696e 7465 7874 2070 6173 7377 6f72  laintext passwor
-0000a1e0: 6420 7573 696e 6720 4145 5320 4342 4320  d using AES CBC 
-0000a1f0: 616e 6420 7468 6520 6b65 790a 2020 2020  and the key.    
-0000a200: 2020 2020 2020 2020 2320 7765 2067 6f74          # we got
-0000a210: 2066 726f 6d20 6f75 7220 4b44 460a 2020   from our KDF.  
-0000a220: 2020 2020 2020 2020 2020 656e 6372 7970            encryp
-0000a230: 746f 7220 3d20 4369 7068 6572 2861 6c67  tor = Cipher(alg
-0000a240: 6f72 6974 686d 732e 4145 5328 6b65 7929  orithms.AES(key)
-0000a250: 2c20 6d6f 6465 732e 4342 4328 696e 6974  , modes.CBC(init
-0000a260: 6961 6c69 7a61 7469 6f6e 5f76 6563 746f  ialization_vecto
-0000a270: 7229 2c20 6261 636b 656e 643d 6465 6661  r), backend=defa
-0000a280: 756c 745f 6261 636b 656e 6428 2929 2e65  ult_backend()).e
-0000a290: 6e63 7279 7074 6f72 2829 0a20 2020 2020  ncryptor().     
-0000a2a0: 2020 2020 2020 206d 696e 5f63 6970 6865         min_ciphe
-0000a2b0: 725f 6279 7465 7320 3d20 6c65 6e28 7061  r_bytes = len(pa
-0000a2c0: 6464 6564 5f64 6174 6129 202b 2034 3039  dded_data) + 409
-0000a2d0: 360a 2020 2020 2020 2020 2020 2020 6369  6.            ci
-0000a2e0: 7068 6572 203d 2062 7974 6561 7272 6179  pher = bytearray
-0000a2f0: 286d 696e 5f63 6970 6865 725f 6279 7465  (min_cipher_byte
-0000a300: 7329 0a20 2020 2020 2020 2020 2020 206c  s).            l
-0000a310: 656e 5f65 6e63 7279 7074 6564 203d 2065  en_encrypted = e
-0000a320: 6e63 7279 7074 6f72 2e75 7064 6174 655f  ncryptor.update_
-0000a330: 696e 746f 2870 6164 6465 645f 6461 7461  into(padded_data
-0000a340: 2c20 6369 7068 6572 290a 2020 2020 2020  , cipher).      
-0000a350: 2020 2020 2020 6369 7068 6572 203d 2062        cipher = b
-0000a360: 7974 6573 2863 6970 6865 725b 3a6c 656e  ytes(cipher[:len
-0000a370: 5f65 6e63 7279 7074 6564 5d29 202b 2065  _encrypted]) + e
-0000a380: 6e63 7279 7074 6f72 2e66 696e 616c 697a  ncryptor.finaliz
-0000a390: 6528 290a 2020 2020 2020 2020 656c 7365  e().        else
-0000a3a0: 3a0a 2020 2020 2020 2020 2020 2020 656e  :.            en
-0000a3b0: 6372 7970 746f 7220 3d20 4369 7068 6572  cryptor = Cipher
-0000a3c0: 2861 6c67 6f72 6974 686d 732e 4145 5328  (algorithms.AES(
-0000a3d0: 6b65 7929 2c20 6d6f 6465 732e 4743 4d28  key), modes.GCM(
-0000a3e0: 696e 6974 6961 6c69 7a61 7469 6f6e 5f76  initialization_v
-0000a3f0: 6563 746f 7229 2c20 6261 636b 656e 643d  ector), backend=
-0000a400: 6465 6661 756c 745f 6261 636b 656e 6428  default_backend(
-0000a410: 2929 2e65 6e63 7279 7074 6f72 2829 0a20  )).encryptor(). 
-0000a420: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
-0000a430: 646f 206e 6f74 2075 7365 2041 4144 0a20  do not use AAD. 
-0000a440: 2020 2020 2020 2020 2020 2063 6970 6865             ciphe
-0000a450: 7220 3d20 656e 6372 7970 746f 722e 7570  r = encryptor.up
-0000a460: 6461 7465 2873 656c 662e 7061 7373 776f  date(self.passwo
-0000a470: 7264 2e65 6e63 6f64 6528 656e 636f 6469  rd.encode(encodi
-0000a480: 6e67 3d22 5554 462d 3822 2c20 6572 726f  ng="UTF-8", erro
-0000a490: 7273 3d22 7374 7269 6374 2229 2920 2b20  rs="strict")) + 
-0000a4a0: 656e 6372 7970 746f 722e 6669 6e61 6c69  encryptor.finali
-0000a4b0: 7a65 2829 0a20 2020 2020 2020 2020 2020  ze().           
-0000a4c0: 2023 2053 6572 7665 7220 7369 6465 2065   # Server side e
-0000a4d0: 7870 6563 7473 2074 6861 7420 7468 6520  xpects that the 
-0000a4e0: 7461 6720 6973 2061 7420 7468 6520 656e  tag is at the en
-0000a4f0: 6420 6f66 2074 6865 2063 6970 6865 7220  d of the cipher 
-0000a500: 7465 7874 2e0a 2020 2020 2020 2020 2020  text..          
-0000a510: 2020 6369 7068 6572 202b 3d20 656e 6372    cipher += encr
-0000a520: 7970 746f 722e 7461 670a 0a20 2020 2020  yptor.tag..     
-0000a530: 2020 2023 204e 6f77 2063 7265 6174 6520     # Now create 
-0000a540: 616e 2048 4d41 4320 7573 696e 6720 7468  an HMAC using th
-0000a550: 6520 6f74 6865 7220 4b44 4620 6465 7269  e other KDF deri
-0000a560: 7665 6420 6b65 7920 616e 6420 7468 650a  ved key and the.
-0000a570: 2020 2020 2020 2020 2320 656e 6372 7970          # encryp
-0000a580: 7465 6420 7061 7373 776f 7264 0a20 2020  ted password.   
-0000a590: 2020 2020 2068 6173 6865 7220 3d20 686d       hasher = hm
-0000a5a0: 6163 2e48 4d41 4328 6d61 635f 6b65 792c  ac.HMAC(mac_key,
-0000a5b0: 2068 6173 6865 732e 5348 4132 3536 2829   hashes.SHA256()
-0000a5c0: 2c20 6261 636b 656e 643d 6465 6661 756c  , backend=defaul
-0000a5d0: 745f 6261 636b 656e 6428 2929 0a20 2020  t_backend()).   
-0000a5e0: 2020 2020 2068 6173 6865 722e 7570 6461       hasher.upda
-0000a5f0: 7465 2863 6970 6865 7229 0a20 2020 2020  te(cipher).     
-0000a600: 2020 2067 656e 6572 6174 6564 5f68 6d61     generated_hma
-0000a610: 6320 3d20 6861 7368 6572 2e66 696e 616c  c = hasher.final
-0000a620: 697a 6528 290a 0a20 2020 2020 2020 2072  ize()..        r
-0000a630: 6574 7572 6e20 2863 6970 6865 722c 2067  eturn (cipher, g
-0000a640: 656e 6572 6174 6564 5f68 6d61 632c 2070  enerated_hmac, p
-0000a650: 7269 7661 7465 5f6b 6579 2e70 7562 6c69  rivate_key.publi
-0000a660: 635f 6b65 7928 2929 0a0a 2020 2020 6465  c_key())..    de
-0000a670: 6620 5f70 6172 7365 5f61 7267 7328 7365  f _parse_args(se
-0000a680: 6c66 2c20 6473 6e2c 2075 7365 722c 2070  lf, dsn, user, p
-0000a690: 6173 7377 6f72 642c 2068 6f73 742c 2064  assword, host, d
-0000a6a0: 6174 6162 6173 652c 2074 6c73 2c20 6861  atabase, tls, ha
-0000a6b0: 6e64 7368 616b 652c 2066 6f72 6365 2c20  ndshake, force, 
-0000a6c0: 636f 6e66 6967 6669 6c65 293a 2020 2320  configfile):  # 
-0000a6d0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
-0000a6e0: 746f 6f2d 6d61 6e79 2d61 7267 756d 656e  too-many-argumen
-0000a6f0: 7473 0a20 2020 2020 2020 2022 2222 496e  ts.        """In
-0000a700: 7465 726e 616c 2072 6f75 7469 6e65 2074  ternal routine t
-0000a710: 6f20 7265 736f 6c76 6520 6675 6e63 7469  o resolve functi
-0000a720: 6f6e 2061 7267 756d 656e 7473 2c20 636f  on arguments, co
-0000a730: 6e66 6967 2066 696c 652c 2061 6e64 2064  nfig file, and d
-0000a740: 736e 2222 220a 2020 2020 2020 2020 2320  sn""".        # 
-0000a750: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
-0000a760: 6e6f 2d6d 656d 6265 722c 746f 6f2d 6d61  no-member,too-ma
-0000a770: 6e79 2d62 7261 6e63 6865 732c 746f 6f2d  ny-branches,too-
-0000a780: 6d61 6e79 2d73 7461 7465 6d65 6e74 730a  many-statements.
-0000a790: 2020 2020 2020 2020 2320 4669 7273 742c          # First,
-0000a7a0: 2070 6172 7365 2074 6865 2044 534e 2069   parse the DSN i
-0000a7b0: 6620 6974 2065 7869 7374 730a 2020 2020  f it exists.    
-0000a7c0: 2020 2020 6966 2064 736e 2069 7320 6e6f      if dsn is no
-0000a7d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000a7e0: 2020 2020 7061 7273 6564 203d 2064 736e      parsed = dsn
-0000a7f0: 7061 7273 652e 7061 7273 6528 6473 6e29  parse.parse(dsn)
-0000a800: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000a810: 2070 6172 7365 642e 7363 6865 6d65 2061   parsed.scheme a
-0000a820: 6e64 2070 6172 7365 642e 7363 6865 6d65  nd parsed.scheme
-0000a830: 2e6c 6f77 6572 2829 2021 3d20 226f 6369  .lower() != "oci
-0000a840: 656e 7422 3a0a 2020 2020 2020 2020 2020  ent":.          
-0000a850: 2020 2020 2020 7261 6973 6520 4d61 6c66        raise Malf
-0000a860: 6f72 6d65 6455 524c 2866 2249 6e76 616c  ormedURL(f"Inval
-0000a870: 6964 2044 534e 2073 6368 656d 653a 207b  id DSN scheme: {
-0000a880: 7061 7273 6564 2e73 6368 656d 657d 2229  parsed.scheme}")
-0000a890: 0a0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-0000a8a0: 7220 6174 7472 2069 6e20 5b22 6461 7461  r attr in ["data
-0000a8b0: 6261 7365 222c 2022 7573 6572 222c 2022  base", "user", "
-0000a8c0: 7061 7373 776f 7264 222c 2022 706f 7274  password", "port
-0000a8d0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0000a8e0: 2020 2020 7365 7461 7474 7228 7365 6c66      setattr(self
-0000a8f0: 2c20 6174 7472 2c20 6765 7461 7474 7228  , attr, getattr(
-0000a900: 7061 7273 6564 2c20 6174 7472 2929 0a0a  parsed, attr))..
-0000a910: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-0000a920: 6172 7365 642e 686f 7374 3a0a 2020 2020  arsed.host:.    
-0000a930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a940: 2e68 6f73 7473 203d 2070 6172 7365 642e  .hosts = parsed.
-0000a950: 686f 7374 2e73 706c 6974 2822 2c22 290a  host.split(",").
-0000a960: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000a970: 7365 6c66 2e64 6174 6162 6173 6520 6973  self.database is
-0000a980: 206e 6f74 204e 6f6e 6520 616e 6420 6c65   not None and le
-0000a990: 6e28 7365 6c66 2e64 6174 6162 6173 6529  n(self.database)
-0000a9a0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0000a9b0: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-0000a9c0: 6261 7365 203d 204e 6f6e 650a 2020 2020  base = None.    
-0000a9d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000a9e0: 6461 7461 6261 7365 2069 7320 6e6f 7420  database is not 
-0000a9f0: 4e6f 6e65 2061 6e64 2073 656c 662e 6461  None and self.da
-0000aa00: 7461 6261 7365 5b30 5d20 3d3d 2022 2f22  tabase[0] == "/"
-0000aa10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000aa20: 2020 7365 6c66 2e64 6174 6162 6173 6520    self.database 
-0000aa30: 3d20 7365 6c66 2e64 6174 6162 6173 655b  = self.database[
-0000aa40: 313a 5d0a 0a20 2020 2020 2020 2020 2020  1:]..           
-0000aa50: 2069 6620 2274 6c73 2220 696e 2070 6172   if "tls" in par
-0000aa60: 7365 642e 7175 6572 793a 0a20 2020 2020  sed.query:.     
-0000aa70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000aa80: 746c 7320 3d20 7061 7273 6564 2e71 7565  tls = parsed.que
-0000aa90: 7279 5b22 746c 7322 5d0a 0a20 2020 2020  ry["tls"]..     
-0000aaa0: 2020 2020 2020 2069 6620 2266 6f72 6365         if "force
-0000aab0: 2220 696e 2070 6172 7365 642e 7175 6572  " in parsed.quer
-0000aac0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000aad0: 2020 2073 686f 756c 6446 6f72 6365 203d     shouldForce =
-0000aae0: 2070 6172 7365 642e 7175 6572 795b 2266   parsed.query["f
-0000aaf0: 6f72 6365 225d 0a20 2020 2020 2020 2020  orce"].         
-0000ab00: 2020 2020 2020 2069 6620 7368 6f75 6c64         if should
-0000ab10: 466f 7263 652e 7570 7065 7228 2920 3d3d  Force.upper() ==
-0000ab20: 2022 5452 5545 223a 0a20 2020 2020 2020   "TRUE":.       
-0000ab30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ab40: 662e 666f 7263 6520 3d20 5472 7565 0a20  f.force = True. 
-0000ab50: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000ab60: 6c69 6620 7368 6f75 6c64 466f 7263 652e  lif shouldForce.
-0000ab70: 7570 7065 7228 2920 3d3d 2022 4641 4c53  upper() == "FALS
-0000ab80: 4522 3a0a 2020 2020 2020 2020 2020 2020  E":.            
-0000ab90: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
-0000aba0: 6365 203d 2046 616c 7365 0a20 2020 2020  ce = False.     
-0000abb0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000abc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000abd0: 2020 2020 2072 6169 7365 204d 616c 666f       raise Malfo
-0000abe0: 726d 6564 5552 4c28 6622 496e 7661 6c69  rmedURL(f"Invali
-0000abf0: 6420 666f 7263 6520 7374 7269 6e67 3a20  d force string: 
-0000ac00: 7b73 686f 756c 6446 6f72 6365 7d22 290a  {shouldForce}").
-0000ac10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000ac20: 666f 7263 6520 6973 206e 6f74 204e 6f6e  force is not Non
-0000ac30: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000ac40: 2020 2073 656c 662e 666f 7263 6520 3d20     self.force = 
-0000ac50: 666f 7263 650a 0a20 2020 2020 2020 2020  force..         
-0000ac60: 2020 2069 6620 2268 616e 6473 6861 6b65     if "handshake
-0000ac70: 2220 696e 2070 6172 7365 642e 7175 6572  " in parsed.quer
-0000ac80: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000ac90: 2020 2068 616e 6473 6861 6b65 203d 2070     handshake = p
-0000aca0: 6172 7365 642e 7175 6572 795b 2268 616e  arsed.query["han
-0000acb0: 6473 6861 6b65 225d 2e6c 6f77 6572 2829  dshake"].lower()
-0000acc0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000acd0: 2073 656c 662e 7573 6572 2069 7320 4e6f   self.user is No
-0000ace0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000acf0: 2020 2020 7365 6c66 2e75 7365 7220 3d20      self.user = 
-0000ad00: 2222 0a0a 2020 2020 2020 2020 2020 2020  ""..            
-0000ad10: 6966 2073 656c 662e 7061 7373 776f 7264  if self.password
-0000ad20: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000ad30: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000ad40: 6173 7377 6f72 6420 3d20 2222 0a0a 2020  assword = ""..  
-0000ad50: 2020 2020 2020 2320 4e6f 7720 6f76 6572        # Now over
-0000ad60: 7269 6465 2074 6865 2044 534e 2076 616c  ride the DSN val
-0000ad70: 7565 7320 7769 7468 2061 6e79 2076 616c  ues with any val
-0000ad80: 7565 7320 7061 7373 6564 2069 6e20 6173  ues passed in as
-0000ad90: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
-0000ada0: 2020 2020 6966 2075 7365 7220 6973 206e      if user is n
-0000adb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000adc0: 2020 2020 2073 656c 662e 7573 6572 203d       self.user =
-0000add0: 2075 7365 720a 0a20 2020 2020 2020 2069   user..        i
-0000ade0: 6620 7061 7373 776f 7264 2069 7320 6e6f  f password is no
-0000adf0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000ae00: 2020 2020 7365 6c66 2e70 6173 7377 6f72      self.passwor
-0000ae10: 6420 3d20 7061 7373 776f 7264 0a0a 2020  d = password..  
-0000ae20: 2020 2020 2020 6966 2068 6f73 743a 0a20        if host:. 
-0000ae30: 2020 2020 2020 2020 2020 2023 2048 616e             # Han
-0000ae40: 646c 6520 686f 7374 3a70 6f72 740a 2020  dle host:port.  
-0000ae50: 2020 2020 2020 2020 2020 7061 7274 7320            parts 
-0000ae60: 3d20 686f 7374 2e73 706c 6974 2822 3a22  = host.split(":"
-0000ae70: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000ae80: 206c 656e 2870 6172 7473 2920 3d3d 2031   len(parts) == 1
-0000ae90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000aea0: 2020 7365 6c66 2e68 6f73 7473 203d 2070    self.hosts = p
-0000aeb0: 6172 7473 5b30 5d2e 7370 6c69 7428 222c  arts[0].split(",
-0000aec0: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
-0000aed0: 6c69 6620 6c65 6e28 7061 7274 7329 203d  lif len(parts) =
-0000aee0: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
-0000aef0: 2020 2020 2073 656c 662e 686f 7374 7320       self.hosts 
-0000af00: 3d20 7061 7274 735b 305d 2e73 706c 6974  = parts[0].split
-0000af10: 2822 2c22 290a 2020 2020 2020 2020 2020  (",").          
-0000af20: 2020 2020 2020 7365 6c66 2e70 6f72 7420        self.port 
-0000af30: 3d20 696e 7428 7061 7274 735b 315d 290a  = int(parts[1]).
-0000af40: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000af50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000af60: 2020 7261 6973 6520 4d61 6c66 6f72 6d65    raise Malforme
-0000af70: 6455 524c 2866 2249 6e76 616c 6964 2068  dURL(f"Invalid h
-0000af80: 6f73 7420 7661 6c75 653a 207b 686f 7374  ost value: {host
-0000af90: 7d22 290a 0a20 2020 2020 2020 2069 6620  }")..        if 
-0000afa0: 6461 7461 6261 7365 3a0a 2020 2020 2020  database:.      
-0000afb0: 2020 2020 2020 7365 6c66 2e64 6174 6162        self.datab
-0000afc0: 6173 6520 3d20 6461 7461 6261 7365 0a0a  ase = database..
-0000afd0: 2020 2020 2020 2020 6966 2074 6c73 2069          if tls i
-0000afe0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000aff0: 2020 2020 2020 2020 7365 6c66 2e74 6c73          self.tls
-0000b000: 203d 2074 6c73 0a0a 2020 2020 2020 2020   = tls..        
-0000b010: 6966 2068 616e 6473 6861 6b65 2069 7320  if handshake is 
-0000b020: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000b030: 2020 2020 2020 7365 6c66 2e68 616e 6473        self.hands
-0000b040: 6861 6b65 203d 2068 616e 6473 6861 6b65  hake = handshake
-0000b050: 0a0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
-0000b060: 7468 6520 6465 6661 756c 7420 686f 7374  the default host
-0000b070: 206e 6f77 2c20 7369 6e63 6520 7765 2075   now, since we u
-0000b080: 7365 2074 6861 7420 6173 2061 206b 6579  se that as a key
-0000b090: 2069 6e74 6f20 7468 650a 2020 2020 2020   into the.      
-0000b0a0: 2020 2320 636f 6e66 6967 2066 696c 650a    # config file.
-0000b0b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000b0c0: 686f 7374 7320 6973 204e 6f6e 653a 0a20  hosts is None:. 
-0000b0d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b0e0: 686f 7374 7320 3d20 5b73 656c 662e 4445  hosts = [self.DE
-0000b0f0: 4641 554c 545f 484f 5354 5d0a 0a20 2020  FAULT_HOST]..   
-0000b100: 2020 2020 2023 204e 6f77 2062 7569 6c64       # Now build
-0000b110: 2061 2063 6f6e 6669 6770 6172 7365 7220   a configparser 
-0000b120: 7769 7468 2064 6566 6175 6c74 2076 616c  with default val
-0000b130: 7565 730a 2020 2020 2020 2020 636f 6e66  ues.        conf
-0000b140: 6967 203d 2063 6f6e 6669 6770 6172 7365  ig = configparse
-0000b150: 722e 436f 6e66 6967 5061 7273 6572 280a  r.ConfigParser(.
-0000b160: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-0000b170: 756c 7473 3d7b 2270 6f72 7422 3a20 7374  ults={"port": st
-0000b180: 7228 7365 6c66 2e44 4546 4155 4c54 5f50  r(self.DEFAULT_P
-0000b190: 4f52 5429 2c20 2264 6174 6162 6173 6522  ORT), "database"
-0000b1a0: 3a20 7365 6c66 2e44 4546 4155 4c54 5f44  : self.DEFAULT_D
-0000b1b0: 4154 4142 4153 452c 2022 746c 7322 3a20  ATABASE, "tls": 
-0000b1c0: 2275 6e76 6572 6966 6965 6422 2c20 2266  "unverified", "f
-0000b1d0: 6f72 6365 223a 2022 6661 6c73 6522 2c20  orce": "false", 
-0000b1e0: 2268 616e 6473 6861 6b65 223a 2022 227d  "handshake": ""}
-0000b1f0: 2c20 696e 7465 7270 6f6c 6174 696f 6e3d  , interpolation=
-0000b200: 4e6f 6e65 0a20 2020 2020 2020 2029 0a20  None.        ). 
-0000b210: 2020 2020 2020 2063 6f6e 6669 6776 616c         configval
-0000b220: 7320 3d20 4e6f 6e65 0a0a 2020 2020 2020  s = None..      
-0000b230: 2020 2320 4966 2077 6520 6861 7665 2061    # If we have a
-0000b240: 2063 6f6e 6669 6720 6669 6c65 2074 7279   config file try
-0000b250: 206c 6f61 6469 6e67 2074 6861 740a 2020   loading that.  
-0000b260: 2020 2020 2020 6966 2063 6f6e 6669 6766        if configf
-0000b270: 696c 6520 6973 206e 6f74 204e 6f6e 653a  ile is not None:
-0000b280: 0a0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-0000b290: 6e66 6967 2e72 6561 6428 636f 6e66 6967  nfig.read(config
-0000b2a0: 6669 6c65 290a 0a20 2020 2020 2020 2020  file)..         
-0000b2b0: 2020 2023 2057 6f72 6b20 6f75 7420 7468     # Work out th
-0000b2c0: 6520 686f 7374 2f64 6174 6162 6173 6520  e host/database 
-0000b2d0: 6966 2077 6520 6b6e 6f77 2069 740a 2020  if we know it.  
-0000b2e0: 2020 2020 2020 2020 2020 686f 7374 5f64            host_d
-0000b2f0: 6220 3d20 222c 222e 6a6f 696e 2873 656c  b = ",".join(sel
-0000b300: 662e 686f 7374 7329 0a20 2020 2020 2020  f.hosts).       
-0000b310: 2020 2020 2069 6620 7365 6c66 2e64 6174       if self.dat
-0000b320: 6162 6173 6520 6973 206e 6f74 204e 6f6e  abase is not Non
-0000b330: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000b340: 2020 2068 6f73 745f 6462 203d 2068 6f73     host_db = hos
-0000b350: 745f 6462 202b 2022 2f22 202b 2073 656c  t_db + "/" + sel
-0000b360: 662e 6461 7461 6261 7365 0a0a 2020 2020  f.database..    
-0000b370: 2020 2020 2020 2020 2320 5472 7920 616e          # Try an
-0000b380: 6420 6d61 7463 6820 6561 6368 2073 6563  d match each sec
-0000b390: 7469 6f6e 2069 6e20 7468 6520 494e 4920  tion in the INI 
-0000b3a0: 6669 6c65 2077 6974 6820 7468 6520 686f  file with the ho
-0000b3b0: 7374 2f64 6174 6162 6173 650a 2020 2020  st/database.    
-0000b3c0: 2020 2020 2020 2020 666f 7220 7320 696e          for s in
-0000b3d0: 2063 6f6e 6669 672e 7365 6374 696f 6e73   config.sections
-0000b3e0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000b3f0: 2020 2020 6966 2072 652e 6d61 7463 6828      if re.match(
-0000b400: 732c 2068 6f73 745f 6462 293a 0a20 2020  s, host_db):.   
-0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b420: 2063 6f6e 6669 6776 616c 7320 3d20 636f   configvals = co
-0000b430: 6e66 6967 5b73 5d0a 2020 2020 2020 2020  nfig[s].        
-0000b440: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-0000b450: 6b0a 0a20 2020 2020 2020 2023 2069 6620  k..        # if 
-0000b460: 7765 2064 6964 6e27 7420 6669 6e64 2061  we didn't find a
-0000b470: 206d 6174 6368 696e 6720 686f 7374 2028   matching host (
-0000b480: 6f72 2074 6865 7265 2069 7320 6e6f 2066  or there is no f
-0000b490: 696c 6529 2e20 7573 6520 7468 6520 6465  ile). use the de
-0000b4a0: 6661 756c 7473 0a20 2020 2020 2020 2069  faults.        i
-0000b4b0: 6620 636f 6e66 6967 7661 6c73 2069 7320  f configvals is 
-0000b4c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000b4d0: 2020 636f 6e66 6967 7661 6c73 203d 2063    configvals = c
-0000b4e0: 6f6e 6669 675b 2244 4546 4155 4c54 225d  onfig["DEFAULT"]
-0000b4f0: 0a20 2020 2020 2020 2023 2046 6f72 6365  .        # Force
-0000b500: 2069 7320 6e6f 7420 706c 6163 6573 2068   is not places h
-0000b510: 6572 6520 736f 2069 7420 6361 6e20 6765  ere so it can ge
-0000b520: 7420 7061 7273 6564 2062 656c 6f77 2e0a  t parsed below..
-0000b530: 2020 2020 2020 2020 666f 7220 6174 7472          for attr
-0000b540: 2069 6e20 5b22 706f 7274 222c 2022 6461   in ["port", "da
-0000b550: 7461 6261 7365 222c 2022 746c 7322 2c20  tabase", "tls", 
-0000b560: 2268 616e 6473 6861 6b65 225d 3a0a 2020  "handshake"]:.  
-0000b570: 2020 2020 2020 2020 2020 6966 2067 6574            if get
-0000b580: 6174 7472 2873 656c 662c 2061 7474 7229  attr(self, attr)
-0000b590: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000b5a0: 2020 2020 2020 2020 2020 7365 7461 7474            setatt
-0000b5b0: 7228 7365 6c66 2c20 6174 7472 2c20 636f  r(self, attr, co
-0000b5c0: 6e66 6967 7661 6c73 5b61 7474 725d 290a  nfigvals[attr]).
-0000b5d0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000b5e0: 7365 6c66 2e75 7365 723a 0a20 2020 2020  self.user:.     
-0000b5f0: 2020 2020 2020 2073 656c 662e 7573 6572         self.user
-0000b600: 203d 2063 6f6e 6669 6776 616c 732e 6765   = configvals.ge
-0000b610: 7428 2275 7365 7222 2c20 2222 290a 0a20  t("user", "").. 
-0000b620: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0000b630: 6c66 2e70 6173 7377 6f72 643a 0a20 2020  lf.password:.   
-0000b640: 2020 2020 2020 2020 2073 656c 662e 7061           self.pa
-0000b650: 7373 776f 7264 203d 2063 6f6e 6669 6776  ssword = configv
-0000b660: 616c 732e 6765 7428 2270 6173 7377 6f72  als.get("passwor
-0000b670: 6422 2c20 2222 290a 0a20 2020 2020 2020  d", "")..       
-0000b680: 2069 6620 7365 6c66 2e66 6f72 6365 2069   if self.force i
-0000b690: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000b6a0: 2020 2020 7365 6c66 2e66 6f72 6365 203d      self.force =
-0000b6b0: 2063 6f6e 6669 6776 616c 732e 6765 7462   configvals.getb
-0000b6c0: 6f6f 6c65 616e 2822 666f 7263 6522 290a  oolean("force").
-0000b6d0: 0a20 2020 2020 2020 2023 2041 6e64 2066  .        # And f
-0000b6e0: 696e 616c 6c79 2074 6964 7920 7570 2073  inally tidy up s
-0000b6f0: 6f6d 6520 7468 696e 6773 0a20 2020 2020  ome things.     
-0000b700: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0000b710: 2873 656c 662e 706f 7274 2c20 7374 7229  (self.port, str)
-0000b720: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000b730: 6c66 2e70 6f72 7420 3d20 696e 7428 7365  lf.port = int(se
-0000b740: 6c66 2e70 6f72 7429 0a0a 2020 2020 2020  lf.port)..      
-0000b750: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000b760: 7365 6c66 2e74 6c73 2c20 7374 7229 3a0a  self.tls, str):.
-0000b770: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000b780: 656c 662e 746c 732e 6c6f 7765 7228 2920  elf.tls.lower() 
-0000b790: 3d3d 2022 6f66 6622 3a0a 2020 2020 2020  == "off":.      
-0000b7a0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0000b7b0: 6c73 203d 2073 656c 662e 544c 535f 4e4f  ls = self.TLS_NO
-0000b7c0: 4e45 0a20 2020 2020 2020 2020 2020 2065  NE.            e
-0000b7d0: 6c69 6620 7365 6c66 2e74 6c73 2e6c 6f77  lif self.tls.low
-0000b7e0: 6572 2829 203d 3d20 2275 6e76 6572 6966  er() == "unverif
-0000b7f0: 6965 6422 3a0a 2020 2020 2020 2020 2020  ied":.          
-0000b800: 2020 2020 2020 7365 6c66 2e74 6c73 203d        self.tls =
-0000b810: 2073 656c 662e 544c 535f 554e 5645 5249   self.TLS_UNVERI
-0000b820: 4649 4544 0a20 2020 2020 2020 2020 2020  FIED.           
-0000b830: 2065 6c69 6620 7365 6c66 2e74 6c73 2e6c   elif self.tls.l
-0000b840: 6f77 6572 2829 203d 3d20 226f 6e22 3a0a  ower() == "on":.
-0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 7365 6c66 2e74 6c73 203d 2073 656c 662e  self.tls = self.
-0000b870: 544c 535f 4f4e 0a20 2020 2020 2020 2020  TLS_ON.         
-0000b880: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000b890: 2020 2020 2020 2020 2072 6169 7365 204d           raise M
-0000b8a0: 616c 666f 726d 6564 5552 4c28 6622 496e  alformedURL(f"In
-0000b8b0: 7661 6c69 6420 746c 7320 7661 6c75 653a  valid tls value:
-0000b8c0: 207b 7365 6c66 2e74 6c73 7d22 290a 2020   {self.tls}").  
-0000b8d0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-0000b8e0: 7461 6e63 6528 7365 6c66 2e74 6c73 2c20  tance(self.tls, 
-0000b8f0: 6c69 7374 293a 0a20 2020 2020 2020 2020  list):.         
-0000b900: 2020 2072 6169 7365 204d 616c 666f 726d     raise Malform
-0000b910: 6564 5552 4c28 6622 4d75 6c74 6970 6c65  edURL(f"Multiple
-0000b920: 2054 4c53 2076 616c 7565 7320 6465 7465   TLS values dete
-0000b930: 6374 6564 3a20 7b73 656c 662e 746c 737d  cted: {self.tls}
-0000b940: 2229 0a0a 2020 2020 2020 2020 6966 2069  ")..        if i
-0000b950: 7369 6e73 7461 6e63 6528 7365 6c66 2e68  sinstance(self.h
-0000b960: 616e 6473 6861 6b65 2c20 7374 7229 3a0a  andshake, str):.
-0000b970: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000b980: 656c 662e 6861 6e64 7368 616b 652e 6c6f  elf.handshake.lo
-0000b990: 7765 7228 2920 3d3d 2022 6362 6322 3a0a  wer() == "cbc":.
-0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9b0: 7365 6c66 2e68 616e 6473 6861 6b65 203d  self.handshake =
-0000b9c0: 2073 656c 662e 4841 4e44 5348 414b 455f   self.HANDSHAKE_
-0000b9d0: 4342 430a 2020 2020 2020 2020 2020 2020  CBC.            
-0000b9e0: 656c 6966 2073 656c 662e 6861 6e64 7368  elif self.handsh
-0000b9f0: 616b 652e 6c6f 7765 7228 2920 3d3d 2022  ake.lower() == "
-0000ba00: 7373 6f22 3a0a 2020 2020 2020 2020 2020  sso":.          
-0000ba10: 2020 2020 2020 7365 6c66 2e68 616e 6473        self.hands
-0000ba20: 6861 6b65 203d 2073 656c 662e 4841 4e44  hake = self.HAND
-0000ba30: 5348 414b 455f 5353 4f0a 2020 2020 2020  SHAKE_SSO.      
-0000ba40: 2020 2020 2020 2320 4966 2074 6865 7920        # If they 
-0000ba50: 6469 646e 2774 2073 7065 6369 6679 2068  didn't specify h
-0000ba60: 616e 6473 6861 6b65 2c20 6974 2077 696c  andshake, it wil
-0000ba70: 6c20 6265 2062 6c61 6e6b 2061 6e64 2074  l be blank and t
-0000ba80: 6875 7320 7368 6f75 6c64 2062 6520 4743  hus should be GC
-0000ba90: 4d2e 0a20 2020 2020 2020 2020 2020 2065  M..            e
-0000baa0: 6c69 6620 7365 6c66 2e68 616e 6473 6861  lif self.handsha
-0000bab0: 6b65 2e6c 6f77 6572 2829 203d 3d20 2267  ke.lower() == "g
-0000bac0: 636d 2220 6f72 2073 656c 662e 6861 6e64  cm" or self.hand
-0000bad0: 7368 616b 652e 6c6f 7765 7228 2920 3d3d  shake.lower() ==
-0000bae0: 2022 223a 0a20 2020 2020 2020 2020 2020   "":.           
-0000baf0: 2020 2020 2073 656c 662e 6861 6e64 7368       self.handsh
-0000bb00: 616b 6520 3d20 7365 6c66 2e48 414e 4453  ake = self.HANDS
-0000bb10: 4841 4b45 5f47 434d 0a20 2020 2020 2020  HAKE_GCM.       
-0000bb20: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000bb30: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000bb40: 2873 656c 662e 6861 6e64 7368 616b 6529  (self.handshake)
+00007810: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
+00007820: 2020 2020 2020 2020 2023 2053 656e 6420           # Send 
+00007830: 7468 6520 434c 4945 4e54 5f43 4f4e 4e45  the CLIENT_CONNE
+00007840: 4354 494f 4e20 7265 7175 6573 740a 2020  CTION request.  
+00007850: 2020 2020 2020 2020 2020 2323 2323 2323            ######
+00007860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007870: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007880: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007890: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
+000078a0: 2020 2020 2020 2020 2072 6571 203d 2070           req = p
+000078b0: 726f 746f 2e52 6571 7565 7374 2829 0a20  roto.Request(). 
+000078c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000078d0: 6c66 2e68 616e 6473 6861 6b65 203d 3d20  lf.handshake == 
+000078e0: 7365 6c66 2e48 414e 4453 4841 4b45 5f43  self.HANDSHAKE_C
+000078f0: 4243 3a0a 2020 2020 2020 2020 2020 2020  BC:.            
+00007900: 2020 2020 7265 712e 7479 7065 203d 2072      req.type = r
+00007910: 6571 2e43 4c49 454e 545f 434f 4e4e 4543  eq.CLIENT_CONNEC
+00007920: 5449 4f4e 0a20 2020 2020 2020 2020 2020  TION.           
+00007930: 2020 2020 2063 6c69 656e 745f 636f 6e6e       client_conn
+00007940: 6563 7469 6f6e 203d 2072 6571 2e63 6c69  ection = req.cli
+00007950: 656e 745f 636f 6e6e 6563 7469 6f6e 0a20  ent_connection. 
+00007960: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00007970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007980: 2023 2053 686f 756c 6420 6265 2047 434d   # Should be GCM
+00007990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000079a0: 2072 6571 2e74 7970 6520 3d20 7265 712e   req.type = req.
+000079b0: 434c 4945 4e54 5f43 4f4e 4e45 4354 494f  CLIENT_CONNECTIO
+000079c0: 4e5f 4743 4d0a 2020 2020 2020 2020 2020  N_GCM.          
+000079d0: 2020 2020 2020 636c 6965 6e74 5f63 6f6e        client_con
+000079e0: 6e65 6374 696f 6e20 3d20 7265 712e 636c  nection = req.cl
+000079f0: 6965 6e74 5f63 6f6e 6e65 6374 696f 6e5f  ient_connection_
+00007a00: 6763 6d0a 2020 2020 2020 2020 2020 2020  gcm.            
+00007a10: 2020 2020 636c 6965 6e74 5f63 6f6e 6e65      client_conne
+00007a20: 6374 696f 6e2e 6578 706c 6963 6974 5353  ction.explicitSS
+00007a30: 4f20 3d20 6973 5f65 7870 6c69 6369 745f  O = is_explicit_
+00007a40: 7373 6f0a 2020 2020 2020 2020 2020 2020  sso.            
+00007a50: 636c 6965 6e74 5f63 6f6e 6e65 6374 696f  client_connectio
+00007a60: 6e2e 7573 6572 6964 203d 2073 656c 662e  n.userid = self.
+00007a70: 7573 6572 0a20 2020 2020 2020 2020 2020  user.           
+00007a80: 2073 656c 662e 5f69 6e69 7469 616c 697a   self._initializ
+00007a90: 655f 636c 6965 6e74 5f63 6f6e 6e65 6374  e_client_connect
+00007aa0: 696f 6e28 636c 6965 6e74 5f63 6f6e 6e65  ion(client_conne
+00007ab0: 6374 696f 6e29 0a0a 2020 2020 2020 2020  ction)..        
+00007ac0: 2020 2020 5f73 656e 645f 6d73 6728 7365      _send_msg(se
+00007ad0: 6c66 2c20 7265 7129 0a0a 2020 2020 2020  lf, req)..      
+00007ae0: 2020 2020 2020 2323 2323 2323 2323 2323        ##########
+00007af0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007b00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007b10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007b20: 2323 2323 2323 2323 0a20 2020 2020 2020  ########.       
+00007b30: 2020 2020 2023 2047 6574 2074 6865 2043       # Get the C
+00007b40: 4c49 454e 545f 434f 4e4e 4543 5449 4f4e  LIENT_CONNECTION
+00007b50: 2072 6573 706f 6e73 6520 616e 6420 7072   response and pr
+00007b60: 6f63 6573 7320 6974 0a20 2020 2020 2020  ocess it.       
+00007b70: 2020 2020 2023 2323 2323 2323 2323 2323       ###########
+00007b80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007b90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007ba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007bb0: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
+00007bc0: 2020 2020 6966 2073 656c 662e 6861 6e64      if self.hand
+00007bd0: 7368 616b 6520 3d3d 2073 656c 662e 4841  shake == self.HA
+00007be0: 4e44 5348 414b 455f 4342 433a 0a20 2020  NDSHAKE_CBC:.   
+00007bf0: 2020 2020 2020 2020 2020 2020 2023 2043               # C
+00007c00: 4243 0a20 2020 2020 2020 2020 2020 2020  BC.             
+00007c10: 2020 2072 7370 203d 205f 7265 6376 5f6d     rsp = _recv_m
+00007c20: 7367 2873 656c 662c 2070 726f 746f 2e43  sg(self, proto.C
+00007c30: 6c69 656e 7443 6f6e 6e65 6374 696f 6e52  lientConnectionR
+00007c40: 6573 706f 6e73 6528 2929 0a20 2020 2020  esponse()).     
+00007c50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00007c60: 2020 2020 2020 2020 2020 2020 2023 2047               # G
+00007c70: 434d 206f 7220 6578 706c 6963 6974 2053  CM or explicit S
+00007c80: 534f 0a20 2020 2020 2020 2020 2020 2020  SO.             
+00007c90: 2020 2072 7370 203d 205f 7265 6376 5f6d     rsp = _recv_m
+00007ca0: 7367 2873 656c 662c 2070 726f 746f 2e43  sg(self, proto.C
+00007cb0: 6c69 656e 7443 6f6e 6e65 6374 696f 6e47  lientConnectionG
+00007cc0: 434d 5265 7370 6f6e 7365 2829 290a 0a20  CMResponse()).. 
+00007cd0: 2020 2020 2020 2020 2020 2069 6620 7273             if rs
+00007ce0: 702e 7265 7370 6f6e 7365 2e74 7970 6520  p.response.type 
+00007cf0: 3d3d 2070 726f 746f 2e43 6f6e 6669 726d  == proto.Confirm
+00007d00: 6174 696f 6e52 6573 706f 6e73 652e 5245  ationResponse.RE
+00007d10: 5350 4f4e 5345 5f57 4152 4e3a 0a20 2020  SPONSE_WARN:.   
+00007d20: 2020 2020 2020 2020 2020 2020 2077 6172               war
+00007d30: 6e28 7273 702e 7265 7370 6f6e 7365 2e72  n(rsp.response.r
+00007d40: 6561 736f 6e29 0a20 2020 2020 2020 2020  eason).         
+00007d50: 2020 2065 6c69 6620 6e6f 7420 7273 702e     elif not rsp.
+00007d60: 7265 7370 6f6e 7365 2e74 7970 6520 3d3d  response.type ==
+00007d70: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
+00007d80: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
+00007d90: 4f4e 5345 5f4f 4b3a 0a20 2020 2020 2020  ONSE_OK:.       
+00007da0: 2020 2020 2020 2020 2072 6169 7365 205f           raise _
+00007db0: 636f 6e76 6572 745f 6578 6365 7074 696f  convert_exceptio
+00007dc0: 6e28 7273 702e 7265 7370 6f6e 7365 290a  n(rsp.response).
+00007dd0: 0a20 2020 2020 2020 2020 2020 2070 6565  .            pee
+00007de0: 725f 6b65 7920 3d20 6c6f 6164 5f70 656d  r_key = load_pem
+00007df0: 5f70 7562 6c69 635f 6b65 7928 7273 702e  _public_key(rsp.
+00007e00: 7075 624b 6579 2e65 6e63 6f64 6528 656e  pubKey.encode(en
+00007e10: 636f 6469 6e67 3d22 5554 462d 3822 2c20  coding="UTF-8", 
+00007e20: 6572 726f 7273 3d22 7374 7269 6374 2229  errors="strict")
+00007e30: 2c20 6261 636b 656e 643d 6465 6661 756c  , backend=defaul
+00007e40: 745f 6261 636b 656e 6428 2929 0a20 2020  t_backend()).   
+00007e50: 2020 2020 2020 2020 2028 6369 7068 6572           (cipher
+00007e60: 2c20 6765 6e65 7261 7465 645f 686d 6163  , generated_hmac
+00007e70: 2c20 7075 626c 6963 5f6b 6579 2920 3d20  , public_key) = 
+00007e80: 7365 6c66 2e5f 656e 6372 7970 7469 6f6e  self._encryption
+00007e90: 5f72 6f75 7469 6e65 2872 7370 2e69 762c  _routine(rsp.iv,
+00007ea0: 2070 6565 725f 6b65 7929 0a0a 2020 2020   peer_key)..    
+00007eb0: 2020 2020 2020 2020 2323 2323 2323 2323          ########
+00007ec0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007ed0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007ef0: 2323 2323 2323 2323 2323 0a20 2020 2020  ##########.     
+00007f00: 2020 2020 2020 2023 2053 656e 6420 7468         # Send th
+00007f10: 6520 434c 4945 4e54 5f43 4f4e 4e45 4354  e CLIENT_CONNECT
+00007f20: 494f 4e32 2072 6571 7565 7374 0a20 2020  ION2 request.   
+00007f30: 2020 2020 2020 2020 2023 2323 2323 2323           #######
+00007f40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007f50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007f60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007f70: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
+00007f80: 2020 2020 2020 2020 7265 7120 3d20 7072          req = pr
+00007f90: 6f74 6f2e 5265 7175 6573 7428 290a 2020  oto.Request().  
+00007fa0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00007fb0: 662e 6861 6e64 7368 616b 6520 3d3d 2073  f.handshake == s
+00007fc0: 656c 662e 4841 4e44 5348 414b 455f 4342  elf.HANDSHAKE_CB
+00007fd0: 433a 0a20 2020 2020 2020 2020 2020 2020  C:.             
+00007fe0: 2020 2072 6571 2e74 7970 6520 3d20 7265     req.type = re
+00007ff0: 712e 434c 4945 4e54 5f43 4f4e 4e45 4354  q.CLIENT_CONNECT
+00008000: 494f 4e32 0a20 2020 2020 2020 2020 2020  ION2.           
+00008010: 2020 2020 2072 6571 2e63 6c69 656e 745f       req.client_
+00008020: 636f 6e6e 6563 7469 6f6e 322e 6369 7068  connection2.ciph
+00008030: 6572 203d 2063 6970 6865 720a 2020 2020  er = cipher.    
+00008040: 2020 2020 2020 2020 2020 2020 7265 712e              req.
+00008050: 636c 6965 6e74 5f63 6f6e 6e65 6374 696f  client_connectio
+00008060: 6e32 2e66 6f72 6365 203d 2066 6f72 6365  n2.force = force
+00008070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008080: 2072 6571 2e63 6c69 656e 745f 636f 6e6e   req.client_conn
+00008090: 6563 7469 6f6e 322e 686d 6163 203d 2067  ection2.hmac = g
+000080a0: 656e 6572 6174 6564 5f68 6d61 630a 2020  enerated_hmac.  
+000080b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000080c0: 712e 636c 6965 6e74 5f63 6f6e 6e65 6374  q.client_connect
+000080d0: 696f 6e32 2e70 7562 4b65 7920 3d20 7075  ion2.pubKey = pu
+000080e0: 626c 6963 5f6b 6579 2e70 7562 6c69 635f  blic_key.public_
+000080f0: 6279 7465 7328 656e 636f 6469 6e67 3d73  bytes(encoding=s
+00008100: 6572 6961 6c69 7a61 7469 6f6e 2e45 6e63  erialization.Enc
+00008110: 6f64 696e 672e 5045 4d2c 2066 6f72 6d61  oding.PEM, forma
+00008120: 743d 7365 7269 616c 697a 6174 696f 6e2e  t=serialization.
+00008130: 5075 626c 6963 466f 726d 6174 2e53 7562  PublicFormat.Sub
+00008140: 6a65 6374 5075 626c 6963 4b65 7949 6e66  jectPublicKeyInf
+00008150: 6f29 0a20 2020 2020 2020 2020 2020 2065  o).            e
+00008160: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00008170: 2020 2020 2072 6571 2e74 7970 6520 3d20       req.type = 
+00008180: 7265 712e 434c 4945 4e54 5f43 4f4e 4e45  req.CLIENT_CONNE
+00008190: 4354 494f 4e5f 4743 4d32 0a20 2020 2020  CTION_GCM2.     
+000081a0: 2020 2020 2020 2020 2020 2072 6571 2e63             req.c
+000081b0: 6c69 656e 745f 636f 6e6e 6563 7469 6f6e  lient_connection
+000081c0: 5f67 636d 322e 6369 7068 6572 203d 2063  _gcm2.cipher = c
+000081d0: 6970 6865 720a 2020 2020 2020 2020 2020  ipher.          
+000081e0: 2020 2020 2020 7265 712e 636c 6965 6e74        req.client
+000081f0: 5f63 6f6e 6e65 6374 696f 6e5f 6763 6d32  _connection_gcm2
+00008200: 2e66 6f72 6365 203d 2066 6f72 6365 0a20  .force = force. 
+00008210: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00008220: 6571 2e63 6c69 656e 745f 636f 6e6e 6563  eq.client_connec
+00008230: 7469 6f6e 5f67 636d 322e 686d 6163 203d  tion_gcm2.hmac =
+00008240: 2067 656e 6572 6174 6564 5f68 6d61 630a   generated_hmac.
+00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008260: 7265 712e 636c 6965 6e74 5f63 6f6e 6e65  req.client_conne
+00008270: 6374 696f 6e5f 6763 6d32 2e65 7870 6c69  ction_gcm2.expli
+00008280: 6369 7453 534f 203d 2069 735f 6578 706c  citSSO = is_expl
+00008290: 6963 6974 5f73 736f 0a20 2020 2020 2020  icit_sso.       
+000082a0: 2020 2020 2020 2020 2072 6571 2e63 6c69           req.cli
+000082b0: 656e 745f 636f 6e6e 6563 7469 6f6e 5f67  ent_connection_g
+000082c0: 636d 322e 7075 624b 6579 203d 2070 7562  cm2.pubKey = pub
+000082d0: 6c69 635f 6b65 792e 7075 626c 6963 5f62  lic_key.public_b
+000082e0: 7974 6573 2865 6e63 6f64 696e 673d 7365  ytes(encoding=se
+000082f0: 7269 616c 697a 6174 696f 6e2e 456e 636f  rialization.Enco
+00008300: 6469 6e67 2e50 454d 2c20 666f 726d 6174  ding.PEM, format
+00008310: 3d73 6572 6961 6c69 7a61 7469 6f6e 2e50  =serialization.P
+00008320: 7562 6c69 6346 6f72 6d61 742e 5375 626a  ublicFormat.Subj
+00008330: 6563 7450 7562 6c69 634b 6579 496e 666f  ectPublicKeyInfo
+00008340: 290a 0a20 2020 2020 2020 2020 2020 205f  )..            _
+00008350: 7365 6e64 5f6d 7367 2873 656c 662c 2072  send_msg(self, r
+00008360: 6571 290a 0a20 2020 2020 2020 2020 2020  eq)..           
+00008370: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00008380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000083a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000083b0: 2323 230a 2020 2020 2020 2020 2020 2020  ###.            
+000083c0: 2320 4765 7420 7468 6520 434c 4945 4e54  # Get the CLIENT
+000083d0: 5f43 4f4e 4e45 4354 494f 4e20 7265 7370  _CONNECTION resp
+000083e0: 6f6e 7365 2061 6e64 2070 726f 6365 7373  onse and process
+000083f0: 2069 740a 2020 2020 2020 2020 2020 2020   it.            
+00008400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008420: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008430: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008440: 2323 0a20 2020 2020 2020 2020 2020 2069  ##.            i
+00008450: 6620 7365 6c66 2e68 616e 6473 6861 6b65  f self.handshake
+00008460: 203d 3d20 7365 6c66 2e48 414e 4453 4841   == self.HANDSHA
+00008470: 4b45 5f43 4243 3a0a 2020 2020 2020 2020  KE_CBC:.        
+00008480: 2020 2020 2020 2020 2320 4342 430a 2020          # CBC.  
+00008490: 2020 2020 2020 2020 2020 2020 2020 7273                rs
+000084a0: 7020 3d20 5f72 6563 765f 6d73 6728 7365  p = _recv_msg(se
+000084b0: 6c66 2c20 7072 6f74 6f2e 436c 6965 6e74  lf, proto.Client
+000084c0: 436f 6e6e 6563 7469 6f6e 3252 6573 706f  Connection2Respo
+000084d0: 6e73 6528 2929 0a20 2020 2020 2020 2020  nse()).         
+000084e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000084f0: 2020 2020 2020 2020 2023 2047 434d 206f           # GCM o
+00008500: 7220 6578 706c 6963 6974 2053 534f 0a20  r explicit SSO. 
+00008510: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00008520: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
+00008530: 656c 662c 2070 726f 746f 2e43 6c69 656e  elf, proto.Clien
+00008540: 7443 6f6e 6e65 6374 696f 6e47 434d 3252  tConnectionGCM2R
+00008550: 6573 706f 6e73 6528 2929 0a0a 2020 2020  esponse())..    
+00008560: 2020 2020 2020 2020 6966 2072 7370 2e72          if rsp.r
+00008570: 6573 706f 6e73 652e 7479 7065 203d 3d20  esponse.type == 
+00008580: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
+00008590: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
+000085a0: 4e53 455f 5741 524e 3a0a 2020 2020 2020  NSE_WARN:.      
+000085b0: 2020 2020 2020 2020 2020 7761 726e 2872            warn(r
+000085c0: 7370 2e72 6573 706f 6e73 652e 7265 6173  sp.response.reas
+000085d0: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
+000085e0: 656c 6966 2072 7370 2e72 6573 706f 6e73  elif rsp.respons
+000085f0: 652e 7479 7065 203d 3d20 7072 6f74 6f2e  e.type == proto.
+00008600: 436f 6e66 6972 6d61 7469 6f6e 5265 7370  ConfirmationResp
+00008610: 6f6e 7365 2e52 4553 504f 4e53 455f 4f4b  onse.RESPONSE_OK
+00008620: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00008630: 2020 2320 5361 7665 2074 6865 2073 6572    # Save the ser
+00008640: 7665 7220 7365 7373 696f 6e20 6964 0a20  ver session id. 
+00008650: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008660: 656c 662e 7365 7276 6572 5365 7373 696f  elf.serverSessio
+00008670: 6e49 6420 3d20 7273 702e 7365 7276 6572  nId = rsp.server
+00008680: 5365 7373 696f 6e49 640a 2020 2020 2020  SessionId.      
+00008690: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000086a0: 6573 7369 6f6e 203d 2053 6573 7369 6f6e  ession = Session
+000086b0: 2875 7365 7241 6e64 5061 7373 776f 7264  (userAndPassword
+000086c0: 3d55 7365 7241 6e64 5061 7373 776f 7264  =UserAndPassword
+000086d0: 2873 656c 662e 7573 6572 2c20 7365 6c66  (self.user, self
+000086e0: 2e70 6173 7377 6f72 6429 290a 2020 2020  .password)).    
+000086f0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00008700: 6572 2e69 6e66 6f28 6622 436f 6e6e 6563  er.info(f"Connec
+00008710: 7465 6420 746f 2073 6572 7665 7220 7365  ted to server se
+00008720: 7373 696f 6e20 4964 3a20 7b73 656c 662e  ssion Id: {self.
+00008730: 7365 7276 6572 5365 7373 696f 6e49 647d  serverSessionId}
+00008740: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00008750: 2020 2023 2053 6176 6520 7365 636f 6e64     # Save second
+00008760: 6172 7920 696e 7465 7266 6163 6573 2e0a  ary interfaces..
+00008770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008780: 7365 6c66 2e5f 7361 7665 5f73 6563 6f6e  self._save_secon
+00008790: 6461 7279 5f69 6e74 6572 6661 6365 7328  dary_interfaces(
+000087a0: 7273 702e 7365 636f 6e64 6172 7929 0a0a  rsp.secondary)..
+000087b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087c0: 2320 5265 6469 7265 6374 2074 6865 2063  # Redirect the c
+000087d0: 6f6e 6e65 6374 696f 6e0a 2020 2020 2020  onnection.      
+000087e0: 2020 2020 2020 2020 2020 6966 2072 7370            if rsp
+000087f0: 2e72 6564 6972 6563 743a 0a20 2020 2020  .redirect:.     
+00008800: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008810: 656c 662e 736f 636b 2e63 6c6f 7365 2829  elf.sock.close()
+00008820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008830: 2020 2020 206d 6170 7065 645f 686f 7374       mapped_host
+00008840: 2c20 6d61 7070 6564 5f70 6f72 7420 3d20  , mapped_port = 
+00008850: 7365 6c66 2e72 6573 6f6c 7665 5f6e 6577  self.resolve_new
+00008860: 5f65 6e64 706f 696e 7428 7273 702e 7265  _endpoint(rsp.re
+00008870: 6469 7265 6374 486f 7374 2c20 7273 702e  directHost, rsp.
+00008880: 7265 6469 7265 6374 506f 7274 290a 2020  redirectPort).  
+00008890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088a0: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
+000088b0: 2252 6564 6972 6563 7469 6e67 2063 6f6e  "Redirecting con
+000088c0: 6e65 6374 696f 6e20 746f 207b 7273 702e  nection to {rsp.
+000088d0: 7265 6469 7265 6374 486f 7374 7d3a 7b72  redirectHost}:{r
+000088e0: 7370 2e72 6564 6972 6563 7450 6f72 747d  sp.redirectPort}
+000088f0: 2c20 7768 6963 6820 6d61 7073 2074 6f20  , which maps to 
+00008900: 7b6d 6170 7065 645f 686f 7374 7d3a 7b6d  {mapped_host}:{m
+00008910: 6170 7065 645f 706f 7274 7d22 290a 2020  apped_port}").  
+00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008930: 2020 7365 6c66 2e73 6f63 6b20 3d20 736f    self.sock = so
+00008940: 636b 6574 2e63 7265 6174 655f 636f 6e6e  cket.create_conn
+00008950: 6563 7469 6f6e 2828 6d61 7070 6564 5f68  ection((mapped_h
+00008960: 6f73 742c 206d 6170 7065 645f 706f 7274  ost, mapped_port
+00008970: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00008980: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00008990: 666f 2866 2243 6f6e 6e65 6374 6564 2074  fo(f"Connected t
+000089a0: 6f20 7b6d 6170 7065 645f 686f 7374 7d3a  o {mapped_host}:
+000089b0: 7b6d 6170 7065 645f 706f 7274 7d20 6f6e  {mapped_port} on
+000089c0: 2073 6f63 6b65 7420 7b73 656c 662e 736f   socket {self.so
+000089d0: 636b 7d22 290a 2020 2020 2020 2020 2020  ck}").          
+000089e0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000089f0: 7373 6c69 7a65 5f63 6f6e 6e65 6374 696f  sslize_connectio
+00008a00: 6e28 290a 0a20 2020 2020 2020 2020 2020  n()..           
+00008a10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008a20: 7365 6c66 2e5f 636c 6965 6e74 5f68 616e  self._client_han
+00008a30: 6473 6861 6b65 5f43 4243 5f47 434d 2869  dshake_CBC_GCM(i
+00008a40: 735f 6578 706c 6963 6974 5f73 736f 2c20  s_explicit_sso, 
+00008a50: 5472 7565 290a 0a20 2020 2020 2020 2020  True)..         
+00008a60: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
+00008a70: 2020 2020 2020 2020 2020 2320 7468 6572            # ther
+00008a80: 6520 6973 2073 6f6d 6574 6869 6e67 2062  e is something b
+00008a90: 726f 6b65 6e20 696e 206f 7572 2068 616e  roken in our han
+00008aa0: 6473 6861 6b65 2e2e 2e72 6574 7279 0a20  dshake...retry. 
+00008ab0: 2020 2020 2020 2020 2020 2069 6620 7273             if rs
+00008ac0: 702e 7265 7370 6f6e 7365 2e76 656e 646f  p.response.vendo
+00008ad0: 725f 636f 6465 203d 3d20 2d32 3032 3a0a  r_code == -202:.
+00008ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008af0: 6c6f 6767 6572 2e64 6562 7567 2822 4861  logger.debug("Ha
+00008b00: 6e64 7368 616b 6520 6572 726f 722e 2e2e  ndshake error...
+00008b10: 7265 7472 7969 6e67 2229 0a20 2020 2020  retrying").     
+00008b20: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00008b30: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
+00008b40: 2072 6169 7365 205f 636f 6e76 6572 745f   raise _convert_
+00008b50: 6578 6365 7074 696f 6e28 7273 702e 7265  exception(rsp.re
+00008b60: 7370 6f6e 7365 290a 0a20 2020 2064 6566  sponse)..    def
+00008b70: 205f 636c 6965 6e74 5f68 616e 6473 6861   _client_handsha
+00008b80: 6b65 5f53 534f 2873 656c 6629 3a0a 2020  ke_SSO(self):.  
+00008b90: 2020 2020 2020 2222 2249 6e74 6572 6e61        """Interna
+00008ba0: 6c20 726f 7574 696e 6520 666f 7220 7369  l routine for si
+00008bb0: 6e67 6c65 2073 6967 6e20 6f6e 2068 616e  ngle sign on han
+00008bc0: 6473 6861 6b65 2028 5353 4f29 2e0a 2020  dshake (SSO)..  
+00008bd0: 2020 2020 2020 312e 2044 7269 7665 7220        1. Driver 
+00008be0: 7265 7175 6573 7473 2074 6f20 7369 676e  requests to sign
+00008bf0: 206f 6e20 7669 6120 5353 4f2e 0a20 2020   on via SSO..   
+00008c00: 2020 2020 2032 2e20 5365 7276 6572 2073       2. Server s
+00008c10: 656e 6473 2062 6163 6b20 616e 2061 7574  ends back an aut
+00008c20: 6874 6865 6e74 6963 6174 696f 6e20 5552  hthentication UR
+00008c30: 4c2e 0a20 2020 2020 2020 2033 2e20 4472  L..        3. Dr
+00008c40: 6976 6572 206c 6175 6e63 6865 7320 5552  iver launches UR
+00008c50: 4c20 696e 2064 6566 6175 6c74 2062 726f  L in default bro
+00008c60: 7773 6572 2028 6f72 2070 7269 6e74 7320  wser (or prints 
+00008c70: 7468 6520 7572 6c20 746f 2073 7464 206f  the url to std o
+00008c80: 7574 2069 6620 6e6f 7420 706f 7373 6962  ut if not possib
+00008c90: 6c65 290a 2020 2020 2020 2020 342e 2055  le).        4. U
+00008ca0: 7365 7220 6175 7468 656e 7469 6361 7465  ser authenticate
+00008cb0: 7320 696e 2062 726f 7773 6572 2e0a 2020  s in browser..  
+00008cc0: 2020 2020 2020 352e 2044 7269 7665 7220        5. Driver 
+00008cd0: 636f 6e74 696e 756f 7573 6c79 2070 6f6c  continuously pol
+00008ce0: 6c73 2074 6865 2064 6174 6162 6173 6520  ls the database 
+00008cf0: 756e 7469 6c20 6c6f 6769 6e20 636f 6d70  until login comp
+00008d00: 6c65 7465 732e 0a20 2020 2020 2020 2036  letes..        6
+00008d10: 2e20 5570 6f6e 2063 6f6d 706c 6574 6574  . Upon completet
+00008d20: 696f 6e2c 2073 6572 7665 7220 7365 6e64  ion, server send
+00008d30: 7320 6261 636b 2061 2073 6563 7572 6974  s back a securit
+00008d40: 7920 746f 6b65 6e20 7769 7468 2077 6869  y token with whi
+00008d50: 6368 2074 6865 2064 7269 7665 7220 6361  ch the driver ca
+00008d60: 6e20 636f 6e6e 6563 742e 2028 5573 6564  n connect. (Used
+00008d70: 2066 6f72 2072 6564 6972 6563 7469 6e67   for redirecting
+00008d80: 202f 2072 6563 6f6e 6e65 6374 696e 6729   / reconnecting)
+00008d90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00008da0: 2020 2020 2066 726f 6d20 7765 6262 726f       from webbro
+00008db0: 7773 6572 2069 6d70 6f72 7420 6f70 656e  wser import open
+00008dc0: 5f6e 6577 0a0a 2020 2020 2020 2020 7265  _new..        re
+00008dd0: 7120 3d20 7072 6f74 6f2e 5265 7175 6573  q = proto.Reques
+00008de0: 7428 290a 2020 2020 2020 2020 7265 712e  t().        req.
+00008df0: 7479 7065 203d 2072 6571 2e43 4c49 454e  type = req.CLIEN
+00008e00: 545f 434f 4e4e 4543 5449 4f4e 5f53 534f  T_CONNECTION_SSO
+00008e10: 0a20 2020 2020 2020 2063 6c69 656e 745f  .        client_
+00008e20: 636f 6e6e 6563 7469 6f6e 203d 2072 6571  connection = req
+00008e30: 2e63 6c69 656e 745f 636f 6e6e 6563 7469  .client_connecti
+00008e40: 6f6e 5f73 736f 0a0a 2020 2020 2020 2020  on_sso..        
+00008e50: 7365 6c66 2e5f 696e 6974 6961 6c69 7a65  self._initialize
+00008e60: 5f63 6c69 656e 745f 636f 6e6e 6563 7469  _client_connecti
+00008e70: 6f6e 2863 6c69 656e 745f 636f 6e6e 6563  on(client_connec
+00008e80: 7469 6f6e 290a 2020 2020 2020 2020 2320  tion).        # 
+00008e90: 5365 6e64 206d 6573 7361 6765 0a20 2020  Send message.   
+00008ea0: 2020 2020 205f 7365 6e64 5f6d 7367 2873       _send_msg(s
+00008eb0: 656c 662c 2072 6571 290a 2020 2020 2020  elf, req).      
+00008ec0: 2020 2320 5265 6365 6976 6520 7265 7370    # Receive resp
+00008ed0: 6f6e 7365 0a20 2020 2020 2020 2072 7370  onse.        rsp
+00008ee0: 203d 205f 7265 6376 5f6d 7367 2873 656c   = _recv_msg(sel
+00008ef0: 662c 2070 726f 746f 2e43 6c69 656e 7443  f, proto.ClientC
+00008f00: 6f6e 6e65 6374 696f 6e53 534f 5265 7370  onnectionSSOResp
+00008f10: 6f6e 7365 2829 290a 0a20 2020 2020 2020  onse())..       
+00008f20: 2069 6620 7273 702e 7265 7370 6f6e 7365   if rsp.response
+00008f30: 2e74 7970 6520 3d3d 2070 726f 746f 2e43  .type == proto.C
+00008f40: 6f6e 6669 726d 6174 696f 6e52 6573 706f  onfirmationRespo
+00008f50: 6e73 652e 5245 5350 4f4e 5345 5f57 4152  nse.RESPONSE_WAR
+00008f60: 4e3a 0a20 2020 2020 2020 2020 2020 2077  N:.            w
+00008f70: 6172 6e28 7273 702e 7265 7370 6f6e 7365  arn(rsp.response
+00008f80: 2e72 6561 736f 6e29 0a20 2020 2020 2020  .reason).       
+00008f90: 2065 6c69 6620 6e6f 7420 7273 702e 7265   elif not rsp.re
+00008fa0: 7370 6f6e 7365 2e74 7970 6520 3d3d 2070  sponse.type == p
+00008fb0: 726f 746f 2e43 6f6e 6669 726d 6174 696f  roto.Confirmatio
+00008fc0: 6e52 6573 706f 6e73 652e 5245 5350 4f4e  nResponse.RESPON
+00008fd0: 5345 5f4f 4b3a 0a20 2020 2020 2020 2020  SE_OK:.         
+00008fe0: 2020 2072 6169 7365 205f 636f 6e76 6572     raise _conver
+00008ff0: 745f 6578 6365 7074 696f 6e28 7273 702e  t_exception(rsp.
+00009000: 7265 7370 6f6e 7365 290a 0a20 2020 2020  response)..     
+00009010: 2020 2023 204f 7065 6e20 6272 6f77 7365     # Open browse
+00009020: 7220 666f 7220 7573 6572 2074 6f20 6175  r for user to au
+00009030: 7468 656e 7469 6361 7465 2e0a 2020 2020  thenticate..    
+00009040: 2020 2020 6966 206e 6f74 206f 7065 6e5f      if not open_
+00009050: 6e65 7728 7273 702e 6175 7468 5572 6c29  new(rsp.authUrl)
+00009060: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00009070: 6767 6572 2e69 6e66 6f28 225b 7079 6f63  gger.info("[pyoc
+00009080: 6965 6e74 5d20 436f 756c 6420 6e6f 7420  ient] Could not 
+00009090: 6f70 656e 2064 6566 6175 6c74 2062 726f  open default bro
+000090a0: 7773 6572 2077 6974 6820 7765 6262 726f  wser with webbro
+000090b0: 7773 6572 206c 6962 7261 7279 2e20 506c  wser library. Pl
+000090c0: 6561 7365 2061 7574 6865 6e74 6963 6174  ease authenticat
+000090d0: 6520 6174 3a20 2220 2b20 7273 702e 6175  e at: " + rsp.au
+000090e0: 7468 5572 6c29 0a20 2020 2020 2020 2020  thUrl).         
+000090f0: 2020 2070 7269 6e74 2822 5b70 796f 6369     print("[pyoci
+00009100: 656e 745d 2043 6f75 6c64 206e 6f74 206f  ent] Could not o
+00009110: 7065 6e20 6465 6661 756c 7420 6272 6f77  pen default brow
+00009120: 7365 7220 7769 7468 2077 6562 6272 6f77  ser with webbrow
+00009130: 7365 7220 6c69 6272 6172 792e 2050 6c65  ser library. Ple
+00009140: 6173 6520 6175 7468 656e 7469 6361 7465  ase authenticate
+00009150: 2061 743a 2022 2c20 7273 702e 6175 7468   at: ", rsp.auth
+00009160: 5572 6c29 0a0a 2020 2020 2020 2020 2320  Url)..        # 
+00009170: 506f 6c6c 2074 6865 2064 6174 6162 6173  Poll the databas
+00009180: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+00009190: 706f 6c6c 5f64 6174 6162 6173 6528 7273  poll_database(rs
+000091a0: 702e 7265 7175 6573 7449 6429 0a0a 2020  p.requestId)..  
+000091b0: 2020 6465 6620 5f70 6f6c 6c5f 6461 7461    def _poll_data
+000091c0: 6261 7365 2873 656c 662c 2072 6571 7565  base(self, reque
+000091d0: 7374 4964 293a 0a20 2020 2020 2020 2022  stId):.        "
+000091e0: 2222 506f 6c6c 7320 7468 6520 6461 7461  ""Polls the data
+000091f0: 6261 7365 2075 6e74 696c 2077 6520 6569  base until we ei
+00009200: 7468 6572 2072 6563 6569 7665 2061 6e20  ther receive an 
+00009210: 6572 726f 7220 6f72 2061 2073 7563 6365  error or a succe
+00009220: 7373 6675 6c20 6c6f 6769 6e20 6d65 7373  ssful login mess
+00009230: 6167 652e 0a0a 2020 2020 2020 2020 4172  age...        Ar
+00009240: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00009250: 7265 7175 6573 7449 6420 2853 7472 696e  requestId (Strin
+00009260: 6729 3a20 7468 6520 7265 7175 6573 7420  g): the request 
+00009270: 4944 2061 7373 6f63 6961 7465 6420 7769  ID associated wi
+00009280: 7468 2074 6869 7320 6c6f 6769 6e20 6174  th this login at
+00009290: 7465 6d70 742e 0a20 2020 2020 2020 2022  tempt..        "
+000092a0: 2222 0a0a 2020 2020 2020 2020 7265 7120  ""..        req 
+000092b0: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
+000092c0: 290a 2020 2020 2020 2020 7265 712e 7479  ).        req.ty
+000092d0: 7065 203d 2072 6571 2e43 4c49 454e 545f  pe = req.CLIENT_
+000092e0: 434f 4e4e 4543 5449 4f4e 5f53 534f 320a  CONNECTION_SSO2.
+000092f0: 2020 2020 2020 2020 7265 712e 636c 6965          req.clie
+00009300: 6e74 5f63 6f6e 6e65 6374 696f 6e5f 7373  nt_connection_ss
+00009310: 6f32 2e66 6f72 6365 203d 2073 656c 662e  o2.force = self.
+00009320: 666f 7263 650a 2020 2020 2020 2020 7265  force.        re
+00009330: 712e 636c 6965 6e74 5f63 6f6e 6e65 6374  q.client_connect
+00009340: 696f 6e5f 7373 6f32 2e72 6571 7565 7374  ion_sso2.request
+00009350: 4964 203d 2072 6571 7565 7374 4964 0a0a  Id = requestId..
+00009360: 2020 2020 2020 2020 6b65 6570 506f 6c6c          keepPoll
+00009370: 696e 6720 3d20 5472 7565 0a20 2020 2020  ing = True.     
+00009380: 2020 2077 6169 7446 6f72 203d 2030 0a20     waitFor = 0. 
+00009390: 2020 2020 2020 2077 6869 6c65 206b 6565         while kee
+000093a0: 7050 6f6c 6c69 6e67 3a0a 2020 2020 2020  pPolling:.      
+000093b0: 2020 2020 2020 736c 6565 7028 7761 6974        sleep(wait
+000093c0: 466f 7229 0a20 2020 2020 2020 2020 2020  For).           
+000093d0: 2023 2050 6f6c 6c0a 2020 2020 2020 2020   # Poll.        
+000093e0: 2020 2020 5f73 656e 645f 6d73 6728 7365      _send_msg(se
+000093f0: 6c66 2c20 7265 7129 0a0a 2020 2020 2020  lf, req)..      
+00009400: 2020 2020 2020 2320 5265 6365 6976 6520        # Receive 
+00009410: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
+00009420: 2020 2020 2072 7370 203d 205f 7265 6376       rsp = _recv
+00009430: 5f6d 7367 2873 656c 662c 2070 726f 746f  _msg(self, proto
+00009440: 2e43 6c69 656e 7443 6f6e 6e65 6374 696f  .ClientConnectio
+00009450: 6e53 534f 3252 6573 706f 6e73 6528 2929  nSSO2Response())
+00009460: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00009470: 2072 7370 2e72 6573 706f 6e73 652e 7479   rsp.response.ty
+00009480: 7065 203d 3d20 7072 6f74 6f2e 436f 6e66  pe == proto.Conf
+00009490: 6972 6d61 7469 6f6e 5265 7370 6f6e 7365  irmationResponse
+000094a0: 2e52 4553 504f 4e53 455f 5741 524e 3a0a  .RESPONSE_WARN:.
+000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094c0: 7761 726e 2872 7370 2e72 6573 706f 6e73  warn(rsp.respons
+000094d0: 652e 7265 6173 6f6e 290a 2020 2020 2020  e.reason).      
+000094e0: 2020 2020 2020 656c 6966 206e 6f74 2072        elif not r
+000094f0: 7370 2e72 6573 706f 6e73 652e 7479 7065  sp.response.type
+00009500: 203d 3d20 7072 6f74 6f2e 436f 6e66 6972   == proto.Confir
+00009510: 6d61 7469 6f6e 5265 7370 6f6e 7365 2e52  mationResponse.R
+00009520: 4553 504f 4e53 455f 4f4b 3a0a 2020 2020  ESPONSE_OK:.    
+00009530: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00009540: 6520 5f63 6f6e 7665 7274 5f65 7863 6570  e _convert_excep
+00009550: 7469 6f6e 2872 7370 2e72 6573 706f 6e73  tion(rsp.respons
+00009560: 6529 0a0a 2020 2020 2020 2020 2020 2020  e)..            
+00009570: 6966 2072 7370 2e48 6173 4669 656c 6428  if rsp.HasField(
+00009580: 2270 6f6c 6c69 6e67 496e 7465 7276 616c  "pollingInterval
+00009590: 5365 636f 6e64 7322 293a 0a20 2020 2020  Seconds"):.     
+000095a0: 2020 2020 2020 2020 2020 2023 2043 6f6e             # Con
+000095b0: 7469 6e75 6520 706f 6c6c 696e 670a 2020  tinue polling.  
+000095c0: 2020 2020 2020 2020 2020 2020 2020 7761                wa
+000095d0: 6974 466f 7220 3d20 7273 702e 706f 6c6c  itFor = rsp.poll
+000095e0: 696e 6749 6e74 6572 7661 6c53 6563 6f6e  ingIntervalSecon
+000095f0: 6473 0a20 2020 2020 2020 2020 2020 2020  ds.             
+00009600: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+00009610: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00009620: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00009630: 5375 6363 6573 730a 2020 2020 2020 2020  Success.        
+00009640: 2020 2020 2020 2020 7761 6974 466f 7220          waitFor 
+00009650: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
+00009660: 2020 2020 6b65 6570 506f 6c6c 696e 6720      keepPolling 
+00009670: 3d20 4661 6c73 650a 0a20 2020 2020 2020  = False..       
+00009680: 2073 656c 662e 7365 7276 6572 5365 7373   self.serverSess
+00009690: 696f 6e49 6420 3d20 7273 702e 7365 7373  ionId = rsp.sess
+000096a0: 696f 6e49 6e66 6f2e 7365 7276 6572 5365  ionInfo.serverSe
+000096b0: 7373 696f 6e49 640a 2020 2020 2020 2020  ssionId.        
+000096c0: 6c6f 6767 6572 2e64 6562 7567 2866 2243  logger.debug(f"C
+000096d0: 6f6e 6e65 6374 6564 2074 6f20 7365 7276  onnected to serv
+000096e0: 6572 2073 6573 7369 6f6e 2049 643a 207b  er session Id: {
+000096f0: 7365 6c66 2e73 6572 7665 7253 6573 7369  self.serverSessi
+00009700: 6f6e 4964 7d22 290a 2020 2020 2020 2020  onId}").        
+00009710: 7265 6365 6976 6564 5f74 6f6b 656e 203d  received_token =
+00009720: 2072 7370 2e73 6573 7369 6f6e 496e 666f   rsp.sessionInfo
+00009730: 2e73 6563 7572 6974 7954 6f6b 656e 0a20  .securityToken. 
+00009740: 2020 2020 2020 2073 656c 662e 7365 7373         self.sess
+00009750: 696f 6e20 3d20 5365 7373 696f 6e28 7365  ion = Session(se
+00009760: 6375 7269 7479 546f 6b65 6e3d 5365 6375  curityToken=Secu
+00009770: 7269 7479 546f 6b65 6e28 7265 6365 6976  rityToken(receiv
+00009780: 6564 5f74 6f6b 656e 2e64 6174 612c 2072  ed_token.data, r
+00009790: 6563 6569 7665 645f 746f 6b65 6e2e 7369  eceived_token.si
+000097a0: 676e 6174 7572 652c 2072 6563 6569 7665  gnature, receive
+000097b0: 645f 746f 6b65 6e2e 6973 7375 6572 4669  d_token.issuerFi
+000097c0: 6e67 6572 7072 696e 7429 290a 0a20 2020  ngerprint))..   
+000097d0: 2020 2020 2023 2053 6176 6520 7365 636f       # Save seco
+000097e0: 6e64 6172 7920 696e 7465 7266 6163 6573  ndary interfaces
+000097f0: 2e0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00009800: 7361 7665 5f73 6563 6f6e 6461 7279 5f69  save_secondary_i
+00009810: 6e74 6572 6661 6365 7328 7273 702e 7365  nterfaces(rsp.se
+00009820: 636f 6e64 6172 7929 0a0a 2020 2020 2020  condary)..      
+00009830: 2020 2320 5265 6469 7265 6374 2074 6865    # Redirect the
+00009840: 2063 6f6e 6e65 6374 696f 6e0a 2020 2020   connection.    
+00009850: 2020 2020 6966 2072 7370 2e72 6564 6972      if rsp.redir
+00009860: 6563 743a 0a20 2020 2020 2020 2020 2020  ect:.           
+00009870: 2073 656c 662e 736f 636b 2e63 6c6f 7365   self.sock.close
+00009880: 2829 0a20 2020 2020 2020 2020 2020 206d  ().            m
+00009890: 6170 7065 645f 686f 7374 2c20 6d61 7070  apped_host, mapp
+000098a0: 6564 5f70 6f72 7420 3d20 7365 6c66 2e72  ed_port = self.r
+000098b0: 6573 6f6c 7665 5f6e 6577 5f65 6e64 706f  esolve_new_endpo
+000098c0: 696e 7428 7273 702e 7265 6469 7265 6374  int(rsp.redirect
+000098d0: 486f 7374 2c20 7273 702e 7265 6469 7265  Host, rsp.redire
+000098e0: 6374 506f 7274 290a 2020 2020 2020 2020  ctPort).        
+000098f0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00009900: 2866 2252 6564 6972 6563 7469 6e67 2063  (f"Redirecting c
+00009910: 6f6e 6e65 6374 696f 6e20 746f 207b 7273  onnection to {rs
+00009920: 702e 7265 6469 7265 6374 486f 7374 7d3a  p.redirectHost}:
+00009930: 7b72 7370 2e72 6564 6972 6563 7450 6f72  {rsp.redirectPor
+00009940: 747d 2c20 7768 6963 6820 6d61 7073 2074  t}, which maps t
+00009950: 6f20 7b6d 6170 7065 645f 686f 7374 7d3a  o {mapped_host}:
+00009960: 7b6d 6170 7065 645f 706f 7274 7d22 290a  {mapped_port}").
+00009970: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009980: 2e73 6f63 6b20 3d20 736f 636b 6574 2e63  .sock = socket.c
+00009990: 7265 6174 655f 636f 6e6e 6563 7469 6f6e  reate_connection
+000099a0: 2828 6d61 7070 6564 5f68 6f73 742c 206d  ((mapped_host, m
+000099b0: 6170 7065 645f 706f 7274 2929 0a20 2020  apped_port)).   
+000099c0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+000099d0: 696e 666f 2866 2243 6f6e 6e65 6374 6564  info(f"Connected
+000099e0: 2074 6f20 7b6d 6170 7065 645f 686f 7374   to {mapped_host
+000099f0: 7d3a 7b6d 6170 7065 645f 706f 7274 7d20  }:{mapped_port} 
+00009a00: 6f6e 2073 6f63 6b65 7420 7b73 656c 662e  on socket {self.
+00009a10: 736f 636b 7d22 290a 2020 2020 2020 2020  sock}").        
+00009a20: 2020 2020 7365 6c66 2e5f 7373 6c69 7a65      self._sslize
+00009a30: 5f63 6f6e 6e65 6374 696f 6e28 290a 0a20  _connection().. 
+00009a40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009a50: 6e20 7365 6c66 2e5f 636c 6965 6e74 5f68  n self._client_h
+00009a60: 616e 6473 6861 6b65 5f73 6563 7572 6974  andshake_securit
+00009a70: 795f 746f 6b65 6e28 5472 7565 290a 0a20  y_token(True).. 
+00009a80: 2020 2064 6566 205f 636c 6965 6e74 5f68     def _client_h
+00009a90: 616e 6473 6861 6b65 5f73 6563 7572 6974  andshake_securit
+00009aa0: 795f 746f 6b65 6e28 7365 6c66 2c20 666f  y_token(self, fo
+00009ab0: 7263 653d 4661 6c73 6529 3a0a 2020 2020  rce=False):.    
+00009ac0: 2020 2020 2222 224f 6e63 6520 6120 636f      """Once a co
+00009ad0: 6e6e 6563 7469 6f6e 2061 6371 7569 7265  nnection acquire
+00009ae0: 7320 6120 7365 6375 7269 7479 2074 6f6b  s a security tok
+00009af0: 656e 2c20 6974 2063 616e 2075 7365 2074  en, it can use t
+00009b00: 6861 7420 746f 206c 6f67 2069 6e2e 2054  hat to log in. T
+00009b10: 6869 7320 6861 6e64 7368 616b 6520 6f6e  his handshake on
+00009b20: 6c79 0a20 2020 2020 2020 2073 656e 6473  ly.        sends
+00009b30: 2031 206d 6573 7361 6765 2077 6865 7265   1 message where
+00009b40: 6173 2074 6865 206f 7468 6572 2068 616e  as the other han
+00009b50: 6473 6861 6b65 7320 7365 6e64 2032 2e0a  dshakes send 2..
+00009b60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00009b70: 2020 2020 7768 696c 6520 5472 7565 3a0a      while True:.
+00009b80: 2020 2020 2020 2020 2020 2020 7265 7120              req 
+00009b90: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
+00009ba0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00009bb0: 712e 7479 7065 203d 2072 6571 2e43 4c49  q.type = req.CLI
+00009bc0: 454e 545f 434f 4e4e 4543 5449 4f4e 5f53  ENT_CONNECTION_S
+00009bd0: 4543 5552 4954 595f 544f 4b45 4e0a 2020  ECURITY_TOKEN.  
+00009be0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+00009bf0: 5f63 6f6e 6e65 6374 696f 6e20 3d20 7265  _connection = re
+00009c00: 712e 636c 6965 6e74 5f63 6f6e 6e65 6374  q.client_connect
+00009c10: 696f 6e5f 7365 6375 7269 7479 5f74 6f6b  ion_security_tok
+00009c20: 656e 0a0a 2020 2020 2020 2020 2020 2020  en..            
+00009c30: 7365 6c66 2e5f 696e 6974 6961 6c69 7a65  self._initialize
+00009c40: 5f63 6c69 656e 745f 636f 6e6e 6563 7469  _client_connecti
+00009c50: 6f6e 2863 6c69 656e 745f 636f 6e6e 6563  on(client_connec
+00009c60: 7469 6f6e 290a 2020 2020 2020 2020 2020  tion).          
+00009c70: 2020 2320 4174 7461 6368 2074 6865 2073    # Attach the s
+00009c80: 6563 7572 6974 7920 746f 6b65 6e20 7573  ecurity token us
+00009c90: 6564 2074 6f20 6c6f 6720 696e 0a20 2020  ed to log in.   
+00009ca0: 2020 2020 2020 2020 2063 6c69 656e 745f           client_
+00009cb0: 636f 6e6e 6563 7469 6f6e 2e73 6563 7572  connection.secur
+00009cc0: 6974 7954 6f6b 656e 203d 2073 656c 662e  ityToken = self.
+00009cd0: 7365 7373 696f 6e2e 7365 6375 7269 7479  session.security
+00009ce0: 546f 6b65 6e2e 746f 6b65 6e44 6174 610a  Token.tokenData.
+00009cf0: 2020 2020 2020 2020 2020 2020 636c 6965              clie
+00009d00: 6e74 5f63 6f6e 6e65 6374 696f 6e2e 746f  nt_connection.to
+00009d10: 6b65 6e53 6967 6e61 7475 7265 203d 2073  kenSignature = s
+00009d20: 656c 662e 7365 7373 696f 6e2e 7365 6375  elf.session.secu
+00009d30: 7269 7479 546f 6b65 6e2e 746f 6b65 6e53  rityToken.tokenS
+00009d40: 6967 6e61 7475 7265 0a20 2020 2020 2020  ignature.       
+00009d50: 2020 2020 2063 6c69 656e 745f 636f 6e6e       client_conn
+00009d60: 6563 7469 6f6e 2e69 7373 7565 7246 696e  ection.issuerFin
+00009d70: 6765 7270 7269 6e74 203d 2073 656c 662e  gerprint = self.
+00009d80: 7365 7373 696f 6e2e 7365 6375 7269 7479  session.security
+00009d90: 546f 6b65 6e2e 6973 7375 6572 4669 6e67  Token.issuerFing
+00009da0: 6572 7072 696e 740a 2020 2020 2020 2020  erprint.        
+00009db0: 2020 2020 636c 6965 6e74 5f63 6f6e 6e65      client_conne
+00009dc0: 6374 696f 6e2e 666f 7263 6520 3d20 666f  ction.force = fo
+00009dd0: 7263 650a 0a20 2020 2020 2020 2020 2020  rce..           
+00009de0: 205f 7365 6e64 5f6d 7367 2873 656c 662c   _send_msg(self,
+00009df0: 2072 6571 290a 0a20 2020 2020 2020 2020   req)..         
+00009e00: 2020 2072 7370 203d 205f 7265 6376 5f6d     rsp = _recv_m
+00009e10: 7367 2873 656c 662c 2070 726f 746f 2e43  sg(self, proto.C
+00009e20: 6c69 656e 7443 6f6e 6e65 6374 696f 6e53  lientConnectionS
+00009e30: 6563 7572 6974 7954 6f6b 656e 5265 7370  ecurityTokenResp
+00009e40: 6f6e 7365 2829 290a 0a20 2020 2020 2020  onse())..       
+00009e50: 2020 2020 2069 6620 7273 702e 7265 7370       if rsp.resp
+00009e60: 6f6e 7365 2e74 7970 6520 3d3d 2070 726f  onse.type == pro
+00009e70: 746f 2e43 6f6e 6669 726d 6174 696f 6e52  to.ConfirmationR
+00009e80: 6573 706f 6e73 652e 5245 5350 4f4e 5345  esponse.RESPONSE
+00009e90: 5f57 4152 4e3a 0a20 2020 2020 2020 2020  _WARN:.         
+00009ea0: 2020 2020 2020 2077 6172 6e28 7273 702e         warn(rsp.
+00009eb0: 7265 7370 6f6e 7365 2e72 6561 736f 6e29  response.reason)
+00009ec0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00009ed0: 6620 7273 702e 7265 7370 6f6e 7365 2e74  f rsp.response.t
+00009ee0: 7970 6520 3d3d 2070 726f 746f 2e43 6f6e  ype == proto.Con
+00009ef0: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
+00009f00: 652e 5245 5350 4f4e 5345 5f4f 4b3a 0a20  e.RESPONSE_OK:. 
+00009f10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00009f20: 2053 6176 6520 7365 636f 6e64 6172 7920   Save secondary 
+00009f30: 696e 7465 7266 6163 6573 2e0a 2020 2020  interfaces..    
+00009f40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009f50: 2e5f 7361 7665 5f73 6563 6f6e 6461 7279  ._save_secondary
+00009f60: 5f69 6e74 6572 6661 6365 7328 7273 702e  _interfaces(rsp.
+00009f70: 7365 636f 6e64 6172 7929 0a20 2020 2020  secondary).     
+00009f80: 2020 2020 2020 2020 2020 2023 2052 6564             # Red
+00009f90: 6972 6563 7420 7468 6520 636f 6e6e 6563  irect the connec
+00009fa0: 7469 6f6e 2069 6620 7265 7175 6573 7465  tion if requeste
+00009fb0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00009fc0: 2020 6966 2072 7370 2e72 6564 6972 6563    if rsp.redirec
+00009fd0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00009fe0: 2020 2020 2020 2073 656c 662e 736f 636b         self.sock
+00009ff0: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+0000a000: 2020 2020 2020 2020 2020 2020 206d 6170               map
+0000a010: 7065 645f 686f 7374 2c20 6d61 7070 6564  ped_host, mapped
+0000a020: 5f70 6f72 7420 3d20 7365 6c66 2e72 6573  _port = self.res
+0000a030: 6f6c 7665 5f6e 6577 5f65 6e64 706f 696e  olve_new_endpoin
+0000a040: 7428 7273 702e 7265 6469 7265 6374 486f  t(rsp.redirectHo
+0000a050: 7374 2c20 7273 702e 7265 6469 7265 6374  st, rsp.redirect
+0000a060: 506f 7274 290a 2020 2020 2020 2020 2020  Port).          
+0000a070: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000a080: 2e64 6562 7567 2866 2252 6564 6972 6563  .debug(f"Redirec
+0000a090: 7469 6e67 2063 6f6e 6e65 6374 696f 6e20  ting connection 
+0000a0a0: 746f 207b 7273 702e 7265 6469 7265 6374  to {rsp.redirect
+0000a0b0: 486f 7374 7d3a 7b72 7370 2e72 6564 6972  Host}:{rsp.redir
+0000a0c0: 6563 7450 6f72 747d 2c20 7768 6963 6820  ectPort}, which 
+0000a0d0: 6d61 7073 2074 6f20 7b6d 6170 7065 645f  maps to {mapped_
+0000a0e0: 686f 7374 7d3a 7b6d 6170 7065 645f 706f  host}:{mapped_po
+0000a0f0: 7274 7d22 290a 2020 2020 2020 2020 2020  rt}").          
+0000a100: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000a110: 6f63 6b20 3d20 736f 636b 6574 2e63 7265  ock = socket.cre
+0000a120: 6174 655f 636f 6e6e 6563 7469 6f6e 2828  ate_connection((
+0000a130: 6d61 7070 6564 5f68 6f73 742c 206d 6170  mapped_host, map
+0000a140: 7065 645f 706f 7274 2929 0a20 2020 2020  ped_port)).     
+0000a150: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000a160: 6f67 6765 722e 696e 666f 2866 2243 6f6e  ogger.info(f"Con
+0000a170: 6e65 6374 6564 2074 6f20 7b6d 6170 7065  nected to {mappe
+0000a180: 645f 686f 7374 7d3a 7b6d 6170 7065 645f  d_host}:{mapped_
+0000a190: 706f 7274 7d20 6f6e 2073 6f63 6b65 7420  port} on socket 
+0000a1a0: 7b73 656c 662e 736f 636b 7d22 290a 2020  {self.sock}").  
+0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1c0: 2020 7365 6c66 2e5f 7373 6c69 7a65 5f63    self._sslize_c
+0000a1d0: 6f6e 6e65 6374 696f 6e28 290a 0a20 2020  onnection()..   
+0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1f0: 2072 6574 7572 6e20 7365 6c66 2e5f 636c   return self._cl
+0000a200: 6965 6e74 5f68 616e 6473 6861 6b65 5f73  ient_handshake_s
+0000a210: 6563 7572 6974 795f 746f 6b65 6e28 5472  ecurity_token(Tr
+0000a220: 7565 290a 0a20 2020 2020 2020 2020 2020  ue)..           
+0000a230: 2020 2020 2023 2043 6170 7475 7265 2074       # Capture t
+0000a240: 6865 2073 6573 7369 6f6e 2069 640a 2020  he session id.  
+0000a250: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a260: 6c66 2e73 6572 7665 7253 6573 7369 6f6e  lf.serverSession
+0000a270: 4964 203d 2072 7370 2e73 6572 7665 7253  Id = rsp.serverS
+0000a280: 6573 7369 6f6e 4964 0a20 2020 2020 2020  essionId.       
+0000a290: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000a2a0: 6465 6275 6728 6622 436f 6e6e 6563 7465  debug(f"Connecte
+0000a2b0: 6420 746f 2073 6572 7665 7220 7365 7373  d to server sess
+0000a2c0: 696f 6e20 4964 3a20 7b73 656c 662e 7365  ion Id: {self.se
+0000a2d0: 7276 6572 5365 7373 696f 6e49 647d 2229  rverSessionId}")
+0000a2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a2f0: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
+0000a300: 2020 2023 2074 6865 7265 2069 7320 736f     # there is so
+0000a310: 6d65 7468 696e 6720 6272 6f6b 656e 2069  mething broken i
+0000a320: 6e20 6f75 7220 6861 6e64 7368 616b 652e  n our handshake.
+0000a330: 2e2e 7265 7472 790a 2020 2020 2020 2020  ..retry.        
+0000a340: 2020 2020 6966 2072 7370 2e72 6573 706f      if rsp.respo
+0000a350: 6e73 652e 7665 6e64 6f72 5f63 6f64 6520  nse.vendor_code 
+0000a360: 3d3d 202d 3230 323a 0a20 2020 2020 2020  == -202:.       
+0000a370: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000a380: 6465 6275 6728 2248 616e 6473 6861 6b65  debug("Handshake
+0000a390: 2065 7272 6f72 2e2e 2e72 6574 7279 696e   error...retryin
+0000a3a0: 6722 290a 2020 2020 2020 2020 2020 2020  g").            
+0000a3b0: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
+0000a3c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000a3d0: 5f63 6f6e 7665 7274 5f65 7863 6570 7469  _convert_excepti
+0000a3e0: 6f6e 2872 7370 2e72 6573 706f 6e73 6529  on(rsp.response)
+0000a3f0: 0a0a 2020 2020 6465 6620 5f73 6176 655f  ..    def _save_
+0000a400: 7365 636f 6e64 6172 795f 696e 7465 7266  secondary_interf
+0000a410: 6163 6573 2873 656c 662c 206e 6577 5f73  aces(self, new_s
+0000a420: 6563 6f6e 6461 7279 5f69 6e74 6572 6661  econdary_interfa
+0000a430: 6365 7329 3a0a 2020 2020 2020 2020 2222  ces):.        ""
+0000a440: 2241 6674 6572 2073 6563 6f6e 6461 7279  "After secondary
+0000a450: 2069 6e74 6572 6661 6365 7320 6172 6520   interfaces are 
+0000a460: 7365 6e74 2066 726f 6d20 7468 6520 7365  sent from the se
+0000a470: 7276 6572 2c20 7765 206e 6565 6420 746f  rver, we need to
+0000a480: 0a20 2020 2020 2020 2073 6176 6520 7468  .        save th
+0000a490: 656d 2061 6e64 2075 7365 2074 6865 6d20  em and use them 
+0000a4a0: 666f 7220 7265 6469 7265 6374 696e 672e  for redirecting.
+0000a4b0: 2054 6869 7320 6973 2069 6d70 6f72 7461   This is importa
+0000a4c0: 6e74 2069 6620 7765 0a20 2020 2020 2020  nt if we.       
+0000a4d0: 2067 6574 2072 6564 6972 6563 7465 6420   get redirected 
+0000a4e0: 746f 206d 6170 7065 6420 7371 6c20 656e  to mapped sql en
+0000a4f0: 6470 6f69 6e74 732e 0a0a 2020 2020 2020  dpoints...      
+0000a500: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000a510: 2020 2020 7365 636f 6e64 6172 795f 696e      secondary_in
+0000a520: 7465 7266 6163 6573 2028 5b63 6c61 7373  terfaces ([class
+0000a530: 2027 676f 6f67 6c65 2e70 726f 746f 6275   'google.protobu
+0000a540: 662e 7079 6578 742e 5f6d 6573 7361 6765  f.pyext._message
+0000a550: 2e52 6570 6561 7465 6443 6f6d 706f 7369  .RepeatedComposi
+0000a560: 7465 436f 6e74 6169 6e65 7227 5d29 3a0a  teContainer']):.
+0000a570: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+0000a580: 7365 636f 6e64 6172 7920 696e 7465 7266  secondary interf
+0000a590: 6163 6573 2c20 7768 6963 6820 6973 2072  aces, which is r
+0000a5a0: 6561 6c6c 7920 6120 6c69 7374 206f 6620  eally a list of 
+0000a5b0: 6c69 7374 206f 6620 7374 7269 6e67 732e  list of strings.
+0000a5c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000a5d0: 2020 2020 2073 656c 662e 7365 636f 6e64       self.second
+0000a5e0: 6172 795f 696e 7465 7266 6163 6573 203d  ary_interfaces =
+0000a5f0: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
+0000a600: 6920 696e 2072 616e 6765 286c 656e 286e  i in range(len(n
+0000a610: 6577 5f73 6563 6f6e 6461 7279 5f69 6e74  ew_secondary_int
+0000a620: 6572 6661 6365 7329 293a 0a20 2020 2020  erfaces)):.     
+0000a630: 2020 2020 2020 2073 656c 662e 7365 636f         self.seco
+0000a640: 6e64 6172 795f 696e 7465 7266 6163 6573  ndary_interfaces
+0000a650: 2e61 7070 656e 6428 5b5d 290a 2020 2020  .append([]).    
+0000a660: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
+0000a670: 2072 616e 6765 286c 656e 286e 6577 5f73   range(len(new_s
+0000a680: 6563 6f6e 6461 7279 5f69 6e74 6572 6661  econdary_interfa
+0000a690: 6365 735b 695d 2e61 6464 7265 7373 2929  ces[i].address))
+0000a6a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a6b0: 2020 696e 7465 7266 6163 6520 3d20 6e65    interface = ne
+0000a6c0: 775f 7365 636f 6e64 6172 795f 696e 7465  w_secondary_inte
+0000a6d0: 7266 6163 6573 5b69 5d2e 6164 6472 6573  rfaces[i].addres
+0000a6e0: 735b 6a5d 0a20 2020 2020 2020 2020 2020  s[j].           
+0000a6f0: 2020 2020 2028 696e 7465 7266 6163 655f       (interface_
+0000a700: 6970 2c20 696e 7465 7266 6163 655f 706f  ip, interface_po
+0000a710: 7274 2920 3d20 696e 7465 7266 6163 652e  rt) = interface.
+0000a720: 7370 6c69 7428 223a 2229 0a20 2020 2020  split(":").     
+0000a730: 2020 2020 2020 2020 2020 2023 2052 6574             # Ret
+0000a740: 7572 6e20 6f66 2067 6574 686f 7374 6279  urn of gethostby
+0000a750: 6e61 6d65 5f65 7820 6973 2028 686f 7374  name_ex is (host
+0000a760: 6e61 6d65 2c20 616c 6961 7320 6f66 2068  name, alias of h
+0000a770: 6f73 7420 6e61 6d65 2c20 6f74 6865 7220  ost name, other 
+0000a780: 6970 2061 6464 7265 7373 6573 206f 6620  ip addresses of 
+0000a790: 686f 7374 206e 616d 6529 0a20 2020 2020  host name).     
+0000a7a0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7c0: 2020 2020 6f74 6865 725f 6970 7320 3d20      other_ips = 
+0000a7d0: 736f 636b 6574 2e67 6574 686f 7374 6279  socket.gethostby
+0000a7e0: 6e61 6d65 5f65 7828 696e 7465 7266 6163  name_ex(interfac
+0000a7f0: 655f 6970 295b 325d 0a20 2020 2020 2020  e_ip)[2].       
+0000a800: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000a810: 206f 7468 6572 5f69 7020 696e 206f 7468   other_ip in oth
+0000a820: 6572 5f69 7073 3a0a 2020 2020 2020 2020  er_ips:.        
+0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a840: 7365 6c66 2e73 6563 6f6e 6461 7279 5f69  self.secondary_i
+0000a850: 6e74 6572 6661 6365 735b 695d 2e61 7070  nterfaces[i].app
+0000a860: 656e 6428 286f 7468 6572 5f69 702c 2069  end((other_ip, i
+0000a870: 6e74 2869 6e74 6572 6661 6365 5f70 6f72  nt(interface_por
+0000a880: 7429 2929 0a20 2020 2020 2020 2020 2020  t))).           
+0000a890: 2020 2020 2065 7863 6570 7420 736f 636b       except sock
+0000a8a0: 6574 2e67 6169 6572 726f 723a 0a20 2020  et.gaierror:.   
+0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8c0: 2070 6173 730a 0a20 2020 2020 2020 2068   pass..        h
+0000a8d0: 6f73 7473 203d 205b 5d0a 2020 2020 2020  osts = [].      
+0000a8e0: 2020 666f 7220 6f6e 655f 686f 7374 2069    for one_host i
+0000a8f0: 6e20 7365 6c66 2e68 6f73 7473 3a0a 2020  n self.hosts:.  
+0000a900: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+0000a910: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0000a920: 6f73 7473 203d 2068 6f73 7473 202b 205b  osts = hosts + [
+0000a930: 2868 6f73 742c 2073 656c 662e 706f 7274  (host, self.port
+0000a940: 2920 666f 7220 686f 7374 2069 6e20 736f  ) for host in so
+0000a950: 636b 6574 2e67 6574 686f 7374 6279 6e61  cket.gethostbyna
+0000a960: 6d65 5f65 7828 6f6e 655f 686f 7374 295b  me_ex(one_host)[
+0000a970: 325d 5d0a 2020 2020 2020 2020 2020 2020  2]].            
+0000a980: 6578 6365 7074 2073 6f63 6b65 742e 6761  except socket.ga
+0000a990: 6965 7272 6f72 3a0a 2020 2020 2020 2020  ierror:.        
+0000a9a0: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+0000a9b0: 2020 2020 2066 6f72 206f 7574 6572 5f6c       for outer_l
+0000a9c0: 6973 7420 696e 2073 656c 662e 7365 636f  ist in self.seco
+0000a9d0: 6e64 6172 795f 696e 7465 7266 6163 6573  ndary_interfaces
+0000a9e0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+0000a9f0: 7220 696e 6465 7820 696e 2072 616e 6765  r index in range
+0000aa00: 286c 656e 286f 7574 6572 5f6c 6973 7429  (len(outer_list)
+0000aa10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000aa20: 2020 2069 6620 6f75 7465 725f 6c69 7374     if outer_list
+0000aa30: 5b69 6e64 6578 5d20 696e 2068 6f73 7473  [index] in hosts
+0000aa40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000aa50: 2020 2020 2020 7365 6c66 2e73 6563 6f6e        self.secon
+0000aa60: 6461 7279 5f69 6e64 6578 203d 2069 6e64  dary_index = ind
+0000aa70: 6578 0a20 2020 2020 2020 2020 2020 2020  ex.             
+0000aa80: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
+0000aa90: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000aaa0: 7567 2866 2253 6176 696e 6720 7365 636f  ug(f"Saving seco
+0000aab0: 6e64 6172 7920 696e 7465 7266 6163 6573  ndary interfaces
+0000aac0: 3a20 696e 6465 7820 7b73 656c 662e 7365  : index {self.se
+0000aad0: 636f 6e64 6172 795f 696e 6465 787d 2069  condary_index} i
+0000aae0: 6e74 6572 6661 6365 733a 207b 7365 6c66  nterfaces: {self
+0000aaf0: 2e73 6563 6f6e 6461 7279 5f69 6e74 6572  .secondary_inter
+0000ab00: 6661 6365 737d 2229 0a0a 2020 2020 6465  faces}")..    de
+0000ab10: 6620 5f65 6e63 7279 7074 696f 6e5f 726f  f _encryption_ro
+0000ab20: 7574 696e 6528 7365 6c66 2c20 696e 6974  utine(self, init
+0000ab30: 6961 6c69 7a61 7469 6f6e 5f76 6563 746f  ialization_vecto
+0000ab40: 722c 2070 6565 725f 6b65 7929 3a0a 2020  r, peer_key):.  
+0000ab50: 2020 2020 2020 2222 2249 6e74 6572 6e61        """Interna
+0000ab60: 6c20 726f 7574 696e 6520 746f 2064 6f20  l routine to do 
+0000ab70: 7468 6520 656e 6372 7970 7469 6f6e 2068  the encryption h
+0000ab80: 616e 6473 6861 6b65 206f 660a 2020 2020  andshake of.    
+0000ab90: 2020 2020 7468 6520 7061 7373 776f 7264      the password
+0000aba0: 0a20 2020 2020 2020 2043 4243 2069 7320  .        CBC is 
+0000abb0: 7468 6520 7072 6576 696f 7573 2066 6f72  the previous for
+0000abc0: 6d20 6f66 2065 6e63 7279 7074 696f 6e2e  m of encryption.
+0000abd0: 2057 6520 6e6f 7720 7573 6520 4743 4d20   We now use GCM 
+0000abe0: 6279 2064 6566 6175 6c74 2e0a 2020 2020  by default..    
+0000abf0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000ac00: 2320 4372 6561 7465 206f 7572 206b 6579  # Create our key
+0000ac10: 7320 7573 696e 6720 7468 6520 7061 7261  s using the para
+0000ac20: 6d65 7465 7273 2066 726f 6d20 7468 6520  meters from the 
+0000ac30: 7065 6572 206b 6579 0a20 2020 2020 2020  peer key.       
+0000ac40: 2070 6172 616d 7320 3d20 7065 6572 5f6b   params = peer_k
+0000ac50: 6579 2e70 6172 616d 6574 6572 7328 290a  ey.parameters().
+0000ac60: 2020 2020 2020 2020 7072 6976 6174 655f          private_
+0000ac70: 6b65 7920 3d20 7061 7261 6d73 2e67 656e  key = params.gen
+0000ac80: 6572 6174 655f 7072 6976 6174 655f 6b65  erate_private_ke
+0000ac90: 7928 290a 0a20 2020 2020 2020 2023 2043  y()..        # C
+0000aca0: 7265 6174 6520 6120 7368 6172 6564 206b  reate a shared k
+0000acb0: 6579 0a20 2020 2020 2020 2073 6861 7265  ey.        share
+0000acc0: 645f 6b65 7920 3d20 7072 6976 6174 655f  d_key = private_
+0000acd0: 6b65 792e 6578 6368 616e 6765 2870 6565  key.exchange(pee
+0000ace0: 725f 6b65 7929 0a0a 2020 2020 2020 2020  r_key)..        
+0000acf0: 6b65 7920 3d20 5f68 6173 685f 6b65 7928  key = _hash_key(
+0000ad00: 7368 6172 6564 5f6b 6579 2c20 6222 5c30  shared_key, b"\0
+0000ad10: 2229 0a20 2020 2020 2020 206d 6163 5f6b  ").        mac_k
+0000ad20: 6579 203d 205f 6861 7368 5f6b 6579 2873  ey = _hash_key(s
+0000ad30: 6861 7265 645f 6b65 792c 2062 225c 3122  hared_key, b"\1"
+0000ad40: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+0000ad50: 6c66 2e68 616e 6473 6861 6b65 203d 3d20  lf.handshake == 
+0000ad60: 7365 6c66 2e48 414e 4453 4841 4b45 5f43  self.HANDSHAKE_C
+0000ad70: 4243 3a0a 2020 2020 2020 2020 2020 2020  BC:.            
+0000ad80: 2320 5061 6420 7468 6520 706c 6169 6e74  # Pad the plaint
+0000ad90: 6578 7420 7061 7373 776f 7264 206f 7574  ext password out
+0000ada0: 2075 7369 6e67 2050 4b43 5337 0a20 2020   using PKCS7.   
+0000adb0: 2020 2020 2020 2020 2070 6164 6465 7220           padder 
+0000adc0: 3d20 7061 6464 696e 672e 504b 4353 3728  = padding.PKCS7(
+0000add0: 3132 3829 2e70 6164 6465 7228 290a 2020  128).padder().  
+0000ade0: 2020 2020 2020 2020 2020 7061 6464 6564            padded
+0000adf0: 5f64 6174 6120 3d20 7061 6464 6572 2e75  _data = padder.u
+0000ae00: 7064 6174 6528 7365 6c66 2e70 6173 7377  pdate(self.passw
+0000ae10: 6f72 642e 656e 636f 6465 2865 6e63 6f64  ord.encode(encod
+0000ae20: 696e 673d 2255 5446 2d38 222c 2065 7272  ing="UTF-8", err
+0000ae30: 6f72 733d 2273 7472 6963 7422 2929 0a20  ors="strict")). 
+0000ae40: 2020 2020 2020 2020 2020 2070 6164 6465             padde
+0000ae50: 645f 6461 7461 202b 3d20 7061 6464 6572  d_data += padder
+0000ae60: 2e66 696e 616c 697a 6528 290a 0a20 2020  .finalize()..   
+0000ae70: 2020 2020 2020 2020 2023 2045 6e63 7279           # Encry
+0000ae80: 7074 2074 6865 2070 6164 6465 6420 706c  pt the padded pl
+0000ae90: 6169 6e74 6578 7420 7061 7373 776f 7264  aintext password
+0000aea0: 2075 7369 6e67 2041 4553 2043 4243 2061   using AES CBC a
+0000aeb0: 6e64 2074 6865 206b 6579 0a20 2020 2020  nd the key.     
+0000aec0: 2020 2020 2020 2023 2077 6520 676f 7420         # we got 
+0000aed0: 6672 6f6d 206f 7572 204b 4446 0a20 2020  from our KDF.   
+0000aee0: 2020 2020 2020 2020 2065 6e63 7279 7074           encrypt
+0000aef0: 6f72 203d 2043 6970 6865 7228 616c 676f  or = Cipher(algo
+0000af00: 7269 7468 6d73 2e41 4553 286b 6579 292c  rithms.AES(key),
+0000af10: 206d 6f64 6573 2e43 4243 2869 6e69 7469   modes.CBC(initi
+0000af20: 616c 697a 6174 696f 6e5f 7665 6374 6f72  alization_vector
+0000af30: 292c 2062 6163 6b65 6e64 3d64 6566 6175  ), backend=defau
+0000af40: 6c74 5f62 6163 6b65 6e64 2829 292e 656e  lt_backend()).en
+0000af50: 6372 7970 746f 7228 290a 2020 2020 2020  cryptor().      
+0000af60: 2020 2020 2020 6d69 6e5f 6369 7068 6572        min_cipher
+0000af70: 5f62 7974 6573 203d 206c 656e 2870 6164  _bytes = len(pad
+0000af80: 6465 645f 6461 7461 2920 2b20 3430 3936  ded_data) + 4096
+0000af90: 0a20 2020 2020 2020 2020 2020 2063 6970  .            cip
+0000afa0: 6865 7220 3d20 6279 7465 6172 7261 7928  her = bytearray(
+0000afb0: 6d69 6e5f 6369 7068 6572 5f62 7974 6573  min_cipher_bytes
+0000afc0: 290a 2020 2020 2020 2020 2020 2020 6c65  ).            le
+0000afd0: 6e5f 656e 6372 7970 7465 6420 3d20 656e  n_encrypted = en
+0000afe0: 6372 7970 746f 722e 7570 6461 7465 5f69  cryptor.update_i
+0000aff0: 6e74 6f28 7061 6464 6564 5f64 6174 612c  nto(padded_data,
+0000b000: 2063 6970 6865 7229 0a20 2020 2020 2020   cipher).       
+0000b010: 2020 2020 2063 6970 6865 7220 3d20 6279       cipher = by
+0000b020: 7465 7328 6369 7068 6572 5b3a 6c65 6e5f  tes(cipher[:len_
+0000b030: 656e 6372 7970 7465 645d 2920 2b20 656e  encrypted]) + en
+0000b040: 6372 7970 746f 722e 6669 6e61 6c69 7a65  cryptor.finalize
+0000b050: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
+0000b060: 0a20 2020 2020 2020 2020 2020 2065 6e63  .            enc
+0000b070: 7279 7074 6f72 203d 2043 6970 6865 7228  ryptor = Cipher(
+0000b080: 616c 676f 7269 7468 6d73 2e41 4553 286b  algorithms.AES(k
+0000b090: 6579 292c 206d 6f64 6573 2e47 434d 2869  ey), modes.GCM(i
+0000b0a0: 6e69 7469 616c 697a 6174 696f 6e5f 7665  nitialization_ve
+0000b0b0: 6374 6f72 292c 2062 6163 6b65 6e64 3d64  ctor), backend=d
+0000b0c0: 6566 6175 6c74 5f62 6163 6b65 6e64 2829  efault_backend()
+0000b0d0: 292e 656e 6372 7970 746f 7228 290a 2020  ).encryptor().  
+0000b0e0: 2020 2020 2020 2020 2020 2320 5765 2064            # We d
+0000b0f0: 6f20 6e6f 7420 7573 6520 4141 440a 2020  o not use AAD.  
+0000b100: 2020 2020 2020 2020 2020 6369 7068 6572            cipher
+0000b110: 203d 2065 6e63 7279 7074 6f72 2e75 7064   = encryptor.upd
+0000b120: 6174 6528 7365 6c66 2e70 6173 7377 6f72  ate(self.passwor
+0000b130: 642e 656e 636f 6465 2865 6e63 6f64 696e  d.encode(encodin
+0000b140: 673d 2255 5446 2d38 222c 2065 7272 6f72  g="UTF-8", error
+0000b150: 733d 2273 7472 6963 7422 2929 202b 2065  s="strict")) + e
+0000b160: 6e63 7279 7074 6f72 2e66 696e 616c 697a  ncryptor.finaliz
+0000b170: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+0000b180: 2320 5365 7276 6572 2073 6964 6520 6578  # Server side ex
+0000b190: 7065 6374 7320 7468 6174 2074 6865 2074  pects that the t
+0000b1a0: 6167 2069 7320 6174 2074 6865 2065 6e64  ag is at the end
+0000b1b0: 206f 6620 7468 6520 6369 7068 6572 2074   of the cipher t
+0000b1c0: 6578 742e 0a20 2020 2020 2020 2020 2020  ext..           
+0000b1d0: 2063 6970 6865 7220 2b3d 2065 6e63 7279   cipher += encry
+0000b1e0: 7074 6f72 2e74 6167 0a0a 2020 2020 2020  ptor.tag..      
+0000b1f0: 2020 2320 4e6f 7720 6372 6561 7465 2061    # Now create a
+0000b200: 6e20 484d 4143 2075 7369 6e67 2074 6865  n HMAC using the
+0000b210: 206f 7468 6572 204b 4446 2064 6572 6976   other KDF deriv
+0000b220: 6564 206b 6579 2061 6e64 2074 6865 0a20  ed key and the. 
+0000b230: 2020 2020 2020 2023 2065 6e63 7279 7074         # encrypt
+0000b240: 6564 2070 6173 7377 6f72 640a 2020 2020  ed password.    
+0000b250: 2020 2020 6861 7368 6572 203d 2068 6d61      hasher = hma
+0000b260: 632e 484d 4143 286d 6163 5f6b 6579 2c20  c.HMAC(mac_key, 
+0000b270: 6861 7368 6573 2e53 4841 3235 3628 292c  hashes.SHA256(),
+0000b280: 2062 6163 6b65 6e64 3d64 6566 6175 6c74   backend=default
+0000b290: 5f62 6163 6b65 6e64 2829 290a 2020 2020  _backend()).    
+0000b2a0: 2020 2020 6861 7368 6572 2e75 7064 6174      hasher.updat
+0000b2b0: 6528 6369 7068 6572 290a 2020 2020 2020  e(cipher).      
+0000b2c0: 2020 6765 6e65 7261 7465 645f 686d 6163    generated_hmac
+0000b2d0: 203d 2068 6173 6865 722e 6669 6e61 6c69   = hasher.finali
+0000b2e0: 7a65 2829 0a0a 2020 2020 2020 2020 7265  ze()..        re
+0000b2f0: 7475 726e 2028 6369 7068 6572 2c20 6765  turn (cipher, ge
+0000b300: 6e65 7261 7465 645f 686d 6163 2c20 7072  nerated_hmac, pr
+0000b310: 6976 6174 655f 6b65 792e 7075 626c 6963  ivate_key.public
+0000b320: 5f6b 6579 2829 290a 0a20 2020 2064 6566  _key())..    def
+0000b330: 205f 7061 7273 655f 6172 6773 2873 656c   _parse_args(sel
+0000b340: 662c 2064 736e 2c20 7573 6572 2c20 7061  f, dsn, user, pa
+0000b350: 7373 776f 7264 2c20 686f 7374 2c20 6461  ssword, host, da
+0000b360: 7461 6261 7365 2c20 746c 732c 2068 616e  tabase, tls, han
+0000b370: 6473 6861 6b65 2c20 666f 7263 652c 2063  dshake, force, c
+0000b380: 6f6e 6669 6766 696c 6529 3a20 2023 2070  onfigfile):  # p
+0000b390: 796c 696e 743a 2064 6973 6162 6c65 3d74  ylint: disable=t
+0000b3a0: 6f6f 2d6d 616e 792d 6172 6775 6d65 6e74  oo-many-argument
+0000b3b0: 730a 2020 2020 2020 2020 2222 2249 6e74  s.        """Int
+0000b3c0: 6572 6e61 6c20 726f 7574 696e 6520 746f  ernal routine to
+0000b3d0: 2072 6573 6f6c 7665 2066 756e 6374 696f   resolve functio
+0000b3e0: 6e20 6172 6775 6d65 6e74 732c 2063 6f6e  n arguments, con
+0000b3f0: 6669 6720 6669 6c65 2c20 616e 6420 6473  fig file, and ds
+0000b400: 6e22 2222 0a20 2020 2020 2020 2023 2070  n""".        # p
+0000b410: 796c 696e 743a 2064 6973 6162 6c65 3d6e  ylint: disable=n
+0000b420: 6f2d 6d65 6d62 6572 2c74 6f6f 2d6d 616e  o-member,too-man
+0000b430: 792d 6272 616e 6368 6573 2c74 6f6f 2d6d  y-branches,too-m
+0000b440: 616e 792d 7374 6174 656d 656e 7473 0a20  any-statements. 
+0000b450: 2020 2020 2020 2023 2046 6972 7374 2c20         # First, 
+0000b460: 7061 7273 6520 7468 6520 4453 4e20 6966  parse the DSN if
+0000b470: 2069 7420 6578 6973 7473 0a20 2020 2020   it exists.     
+0000b480: 2020 2069 6620 6473 6e20 6973 206e 6f74     if dsn is not
+0000b490: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000b4a0: 2020 2070 6172 7365 6420 3d20 6473 6e70     parsed = dsnp
+0000b4b0: 6172 7365 2e70 6172 7365 2864 736e 290a  arse.parse(dsn).
+0000b4c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000b4d0: 7061 7273 6564 2e73 6368 656d 6520 616e  parsed.scheme an
+0000b4e0: 6420 7061 7273 6564 2e73 6368 656d 652e  d parsed.scheme.
+0000b4f0: 6c6f 7765 7228 2920 213d 2022 6f63 6965  lower() != "ocie
+0000b500: 6e74 223a 0a20 2020 2020 2020 2020 2020  nt":.           
+0000b510: 2020 2020 2072 6169 7365 204d 616c 666f       raise Malfo
+0000b520: 726d 6564 5552 4c28 6622 496e 7661 6c69  rmedURL(f"Invali
+0000b530: 6420 4453 4e20 7363 6865 6d65 3a20 7b70  d DSN scheme: {p
+0000b540: 6172 7365 642e 7363 6865 6d65 7d22 290a  arsed.scheme}").
+0000b550: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000b560: 2061 7474 7220 696e 205b 2264 6174 6162   attr in ["datab
+0000b570: 6173 6522 2c20 2275 7365 7222 2c20 2270  ase", "user", "p
+0000b580: 6173 7377 6f72 6422 2c20 2270 6f72 7422  assword", "port"
+0000b590: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0000b5a0: 2020 2073 6574 6174 7472 2873 656c 662c     setattr(self,
+0000b5b0: 2061 7474 722c 2067 6574 6174 7472 2870   attr, getattr(p
+0000b5c0: 6172 7365 642c 2061 7474 7229 290a 0a20  arsed, attr)).. 
+0000b5d0: 2020 2020 2020 2020 2020 2069 6620 7061             if pa
+0000b5e0: 7273 6564 2e68 6f73 743a 0a20 2020 2020  rsed.host:.     
+0000b5f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b600: 686f 7374 7320 3d20 7061 7273 6564 2e68  hosts = parsed.h
+0000b610: 6f73 742e 7370 6c69 7428 222c 2229 0a0a  ost.split(",")..
+0000b620: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000b630: 656c 662e 6461 7461 6261 7365 2069 7320  elf.database is 
+0000b640: 6e6f 7420 4e6f 6e65 2061 6e64 206c 656e  not None and len
+0000b650: 2873 656c 662e 6461 7461 6261 7365 2920  (self.database) 
+0000b660: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+0000b670: 2020 2020 2020 7365 6c66 2e64 6174 6162        self.datab
+0000b680: 6173 6520 3d20 4e6f 6e65 0a20 2020 2020  ase = None.     
+0000b690: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+0000b6a0: 6174 6162 6173 6520 6973 206e 6f74 204e  atabase is not N
+0000b6b0: 6f6e 6520 616e 6420 7365 6c66 2e64 6174  one and self.dat
+0000b6c0: 6162 6173 655b 305d 203d 3d20 222f 223a  abase[0] == "/":
+0000b6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b6e0: 2073 656c 662e 6461 7461 6261 7365 203d   self.database =
+0000b6f0: 2073 656c 662e 6461 7461 6261 7365 5b31   self.database[1
+0000b700: 3a5d 0a0a 2020 2020 2020 2020 2020 2020  :]..            
+0000b710: 6966 2022 746c 7322 2069 6e20 7061 7273  if "tls" in pars
+0000b720: 6564 2e71 7565 7279 3a0a 2020 2020 2020  ed.query:.      
+0000b730: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000b740: 6c73 203d 2070 6172 7365 642e 7175 6572  ls = parsed.quer
+0000b750: 795b 2274 6c73 225d 0a0a 2020 2020 2020  y["tls"]..      
+0000b760: 2020 2020 2020 6966 2022 666f 7263 6522        if "force"
+0000b770: 2069 6e20 7061 7273 6564 2e71 7565 7279   in parsed.query
+0000b780: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b790: 2020 7368 6f75 6c64 466f 7263 6520 3d20    shouldForce = 
+0000b7a0: 7061 7273 6564 2e71 7565 7279 5b22 666f  parsed.query["fo
+0000b7b0: 7263 6522 5d0a 2020 2020 2020 2020 2020  rce"].          
+0000b7c0: 2020 2020 2020 6966 2073 686f 756c 6446        if shouldF
+0000b7d0: 6f72 6365 2e75 7070 6572 2829 203d 3d20  orce.upper() == 
+0000b7e0: 2254 5255 4522 3a0a 2020 2020 2020 2020  "TRUE":.        
+0000b7f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b800: 2e66 6f72 6365 203d 2054 7275 650a 2020  .force = True.  
+0000b810: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000b820: 6966 2073 686f 756c 6446 6f72 6365 2e75  if shouldForce.u
+0000b830: 7070 6572 2829 203d 3d20 2246 414c 5345  pper() == "FALSE
+0000b840: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000b850: 2020 2020 2020 2073 656c 662e 666f 7263         self.forc
+0000b860: 6520 3d20 4661 6c73 650a 2020 2020 2020  e = False.      
+0000b870: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b890: 2020 2020 7261 6973 6520 4d61 6c66 6f72      raise Malfor
+0000b8a0: 6d65 6455 524c 2866 2249 6e76 616c 6964  medURL(f"Invalid
+0000b8b0: 2066 6f72 6365 2073 7472 696e 673a 207b   force string: {
+0000b8c0: 7368 6f75 6c64 466f 7263 657d 2229 0a0a  shouldForce}")..
+0000b8d0: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+0000b8e0: 6f72 6365 2069 7320 6e6f 7420 4e6f 6e65  orce is not None
+0000b8f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b900: 2020 7365 6c66 2e66 6f72 6365 203d 2066    self.force = f
+0000b910: 6f72 6365 0a0a 2020 2020 2020 2020 2020  orce..          
+0000b920: 2020 6966 2022 6861 6e64 7368 616b 6522    if "handshake"
+0000b930: 2069 6e20 7061 7273 6564 2e71 7565 7279   in parsed.query
+0000b940: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b950: 2020 6861 6e64 7368 616b 6520 3d20 7061    handshake = pa
+0000b960: 7273 6564 2e71 7565 7279 5b22 6861 6e64  rsed.query["hand
+0000b970: 7368 616b 6522 5d2e 6c6f 7765 7228 290a  shake"].lower().
+0000b980: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000b990: 7365 6c66 2e75 7365 7220 6973 204e 6f6e  self.user is Non
+0000b9a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000b9b0: 2020 2073 656c 662e 7573 6572 203d 2022     self.user = "
+0000b9c0: 220a 0a20 2020 2020 2020 2020 2020 2069  "..            i
+0000b9d0: 6620 7365 6c66 2e70 6173 7377 6f72 6420  f self.password 
+0000b9e0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000b9f0: 2020 2020 2020 2020 2073 656c 662e 7061           self.pa
+0000ba00: 7373 776f 7264 203d 2022 220a 0a20 2020  ssword = ""..   
+0000ba10: 2020 2020 2023 204e 6f77 206f 7665 7272       # Now overr
+0000ba20: 6964 6520 7468 6520 4453 4e20 7661 6c75  ide the DSN valu
+0000ba30: 6573 2077 6974 6820 616e 7920 7661 6c75  es with any valu
+0000ba40: 6573 2070 6173 7365 6420 696e 2061 7320  es passed in as 
+0000ba50: 7061 7261 6d65 7465 7273 0a20 2020 2020  parameters.     
+0000ba60: 2020 2069 6620 7573 6572 2069 7320 6e6f     if user is no
+0000ba70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000ba80: 2020 2020 7365 6c66 2e75 7365 7220 3d20      self.user = 
+0000ba90: 7573 6572 0a0a 2020 2020 2020 2020 6966  user..        if
+0000baa0: 2070 6173 7377 6f72 6420 6973 206e 6f74   password is not
+0000bab0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000bac0: 2020 2073 656c 662e 7061 7373 776f 7264     self.password
+0000bad0: 203d 2070 6173 7377 6f72 640a 0a20 2020   = password..   
+0000bae0: 2020 2020 2069 6620 686f 7374 3a0a 2020       if host:.  
+0000baf0: 2020 2020 2020 2020 2020 2320 4861 6e64            # Hand
+0000bb00: 6c65 2068 6f73 743a 706f 7274 0a20 2020  le host:port.   
+0000bb10: 2020 2020 2020 2020 2070 6172 7473 203d           parts =
+0000bb20: 2068 6f73 742e 7370 6c69 7428 223a 2229   host.split(":")
+0000bb30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000bb40: 6c65 6e28 7061 7274 7329 203d 3d20 313a  len(parts) == 1:
 0000bb50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bb60: 2072 6169 7365 204d 616c 666f 726d 6564   raise Malformed
-0000bb70: 5552 4c28 6622 496e 7661 6c69 6420 6861  URL(f"Invalid ha
-0000bb80: 6e64 7368 616b 6520 7661 6c75 653a 207b  ndshake value: {
-0000bb90: 7365 6c66 2e68 616e 6473 6861 6b65 7d22  self.handshake}"
-0000bba0: 290a 0a20 2020 2020 2020 2023 2044 6f6e  )..        # Don
-0000bbb0: 2774 2061 7373 6572 7420 6120 7573 6572  't assert a user
-0000bbc0: 2070 6172 616d 6574 6572 2068 6173 2062   parameter has b
-0000bbd0: 6565 6e20 7365 742e 2041 6e20 656d 7074  een set. An empt
-0000bbe0: 790a 2020 2020 2020 2020 2320 7374 7269  y.        # stri
-0000bbf0: 6e67 2066 6f72 2074 6869 7320 6669 656c  ng for this fiel
-0000bc00: 6420 6973 2075 7365 6420 666f 7220 6175  d is used for au
-0000bc10: 7468 656e 7469 6361 7469 6e67 2053 534f  thenticating SSO
-0000bc20: 2075 7365 7273 0a0a 2020 2020 2020 2020   users..        
-0000bc30: 2320 446f 6e27 7420 6173 7365 7274 2061  # Don't assert a
-0000bc40: 2070 6173 7377 6f72 6420 7061 7261 6d65   password parame
-0000bc50: 7465 7220 6861 7320 6265 656e 2073 6574  ter has been set
-0000bc60: 2e20 4174 2065 6d70 7479 0a20 2020 2020  . At empty.     
-0000bc70: 2020 2023 2075 7365 7220 616e 6420 7061     # user and pa
-0000bc80: 7373 776f 7264 2069 7320 666f 7220 6175  ssword is for au
-0000bc90: 7468 656e 7469 6361 7469 6f6e 2066 6c6f  thentication flo
-0000bca0: 7720 7769 7468 2053 534f 2e0a 0a20 2020  w with SSO...   
-0000bcb0: 2064 6566 2063 6c6f 7365 2873 656c 6629   def close(self)
-0000bcc0: 3a0a 2020 2020 2020 2020 2222 2243 6c6f  :.        """Clo
-0000bcd0: 7365 2074 6865 2063 6f6e 6e65 6374 696f  se the connectio
-0000bce0: 6e2e 2053 7562 7365 7175 656e 7420 7175  n. Subsequent qu
-0000bcf0: 6572 6965 7320 6f6e 2074 6869 7320 636f  eries on this co
-0000bd00: 6e6e 6563 7469 6f6e 0a20 2020 2020 2020  nnection.       
-0000bd10: 2077 696c 6c20 6661 696c 0a20 2020 2020   will fail.     
-0000bd20: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-0000bd30: 6620 6e6f 7420 7365 6c66 2e73 6f63 6b3a  f not self.sock:
-0000bd40: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000bd50: 7365 2045 7272 6f72 2822 4e6f 2063 6f6e  se Error("No con
-0000bd60: 6e65 6374 696f 6e22 290a 0a20 2020 2020  nection")..     
-0000bd70: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000bd80: 6622 436c 6f73 696e 6720 636f 6e6e 6563  f"Closing connec
-0000bd90: 7469 6f6e 206f 6e20 736f 636b 6574 207b  tion on socket {
-0000bda0: 7365 6c66 2e73 6f63 6b7d 2229 0a20 2020  self.sock}").   
-0000bdb0: 2020 2020 2023 2044 6f20 7468 6973 206c       # Do this l
-0000bdc0: 6974 746c 6520 6461 6e63 6520 736f 2074  ittle dance so t
-0000bdd0: 6861 7420 6576 656e 2069 6620 7468 6520  hat even if the 
-0000bde0: 636c 6f73 6528 2920 6361 6c6c 0a20 2020  close() call.   
-0000bdf0: 2020 2020 2023 2062 6c6f 7773 2075 702c       # blows up,
-0000be00: 2077 6520 6861 7665 2061 6c72 6561 6479   we have already
-0000be10: 2073 6574 2073 656c 662e 736f 636b 2074   set self.sock t
-0000be20: 6f20 4e6f 6e65 0a20 2020 2020 2020 2073  o None.        s
-0000be30: 6f63 6b20 3d20 7365 6c66 2e73 6f63 6b0a  ock = self.sock.
-0000be40: 2020 2020 2020 2020 7365 6c66 2e73 6f63          self.soc
-0000be50: 6b20 3d20 4e6f 6e65 0a20 2020 2020 2020  k = None.       
-0000be60: 2073 6f63 6b2e 636c 6f73 6528 290a 0a20   sock.close().. 
-0000be70: 2020 2064 6566 2063 6f6d 6d69 7428 7365     def commit(se
-0000be80: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000be90: 436f 6d6d 6974 2061 2074 7261 6e73 6163  Commit a transac
-0000bea0: 7469 6f6e 2e20 4375 7272 656e 746c 7920  tion. Currently 
-0000beb0: 6967 6e6f 7265 6422 2222 0a0a 2020 2020  ignored"""..    
-0000bec0: 6465 6620 6375 7273 6f72 2873 656c 6629  def cursor(self)
-0000bed0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
-0000bee0: 7572 6e20 6120 6e65 7720 6375 7273 6f72  urn a new cursor
-0000bef0: 2066 6f72 2074 6869 7320 636f 6e6e 6563   for this connec
-0000bf00: 7469 6f6e 2222 220a 2020 2020 2020 2020  tion""".        
-0000bf10: 6966 206e 6f74 2073 656c 662e 736f 636b  if not self.sock
-0000bf20: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000bf30: 6973 6520 4572 726f 7228 224e 6f20 636f  ise Error("No co
-0000bf40: 6e6e 6563 7469 6f6e 2229 0a20 2020 2020  nnection").     
-0000bf50: 2020 2072 6574 7572 6e20 4375 7273 6f72     return Cursor
-0000bf60: 2873 656c 6629 0a0a 2020 2020 6465 6620  (self)..    def 
-0000bf70: 5f5f 6465 6c5f 5f28 7365 6c66 293a 0a20  __del__(self):. 
-0000bf80: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0000bf90: 6f63 6b20 6973 206e 6f74 204e 6f6e 653a  ock is not None:
-0000bfa0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000bfb0: 662e 636c 6f73 6528 290a 0a20 2020 2064  f.close()..    d
-0000bfc0: 6566 2072 6573 6f6c 7665 5f6e 6577 5f65  ef resolve_new_e
-0000bfd0: 6e64 706f 696e 7428 7365 6c66 2c20 6e65  ndpoint(self, ne
-0000bfe0: 775f 686f 7374 2c20 6e65 775f 706f 7274  w_host, new_port
-0000bff0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000c000: 2020 2020 2020 2048 616e 646c 6573 206d         Handles m
-0000c010: 6170 7069 6e67 2074 6f20 6120 7365 636f  apping to a seco
-0000c020: 6e64 6172 7920 696e 7465 7266 6163 6520  ndary interface 
-0000c030: 6261 7365 6420 6f6e 2074 6865 2073 6563  based on the sec
-0000c040: 6f6e 6461 7279 2069 6e74 6572 6661 6365  ondary interface
-0000c050: 206d 6170 7069 6e67 2073 6176 6564 206f   mapping saved o
-0000c060: 6e20 7468 6973 2063 6f6e 6e65 6374 696f  n this connectio
-0000c070: 6e2e 0a0a 2020 2020 2020 2020 4172 6773  n...        Args
-0000c080: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
-0000c090: 775f 686f 7374 5b73 7472 696e 675d 3a20  w_host[string]: 
-0000c0a0: 7468 6520 6e65 7720 686f 7374 2074 6f20  the new host to 
-0000c0b0: 6265 2072 656d 6170 7065 640a 2020 2020  be remapped.    
-0000c0c0: 2020 2020 2020 2020 6e65 775f 706f 7274          new_port
-0000c0d0: 5b69 6e74 5d3a 2074 6865 206e 6577 2070  [int]: the new p
-0000c0e0: 6f72 7420 746f 2062 6520 7265 6d61 7070  ort to be remapp
-0000c0f0: 6564 0a0a 2020 2020 2020 2020 5265 7475  ed..        Retu
-0000c100: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000c110: 205b 7475 706c 6528 7374 7269 6e67 2c20   [tuple(string, 
-0000c120: 696e 7429 5d3a 2054 6865 2061 6374 7561  int)]: The actua
-0000c130: 6c20 656e 6470 6f69 6e74 2074 6f20 636f  l endpoint to co
-0000c140: 6e6e 6563 7420 746f 2069 6e20 7468 6520  nnect to in the 
-0000c150: 666f 726d 6174 3a20 2868 6f73 742c 2070  format: (host, p
-0000c160: 6f72 7429 2e0a 2020 2020 2020 2020 2222  ort)..        ""
-0000c170: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000c180: 2e64 6562 7567 2866 2252 6573 6f6c 7669  .debug(f"Resolvi
-0000c190: 6e67 206e 6577 2065 6e64 706f 696e 7420  ng new endpoint 
-0000c1a0: 7b6e 6577 5f68 6f73 747d 3a7b 6e65 775f  {new_host}:{new_
-0000c1b0: 706f 7274 7d20 7769 7468 2073 6563 6f6e  port} with secon
-0000c1c0: 6461 7279 5f69 6e64 6578 207b 7365 6c66  dary_index {self
-0000c1d0: 2e73 6563 6f6e 6461 7279 5f69 6e64 6578  .secondary_index
-0000c1e0: 7d20 616e 6420 7365 636f 6e64 6172 795f  } and secondary_
-0000c1f0: 696e 7465 7266 6163 6520 7b73 656c 662e  interface {self.
-0000c200: 7365 636f 6e64 6172 795f 696e 7465 7266  secondary_interf
-0000c210: 6163 6573 7d22 290a 0a20 2020 2020 2020  aces}")..       
-0000c220: 206e 6577 5f65 6e64 706f 696e 7420 3d20   new_endpoint = 
-0000c230: 286e 6577 5f68 6f73 742c 206e 6577 5f70  (new_host, new_p
-0000c240: 6f72 7429 0a20 2020 2020 2020 2065 6e64  ort).        end
-0000c250: 706f 696e 745f 746f 5f63 6f6e 6e65 6374  point_to_connect
-0000c260: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000c270: 6966 2073 656c 662e 7365 636f 6e64 6172  if self.secondar
-0000c280: 795f 696e 6465 7820 213d 202d 313a 0a20  y_index != -1:. 
-0000c290: 2020 2020 2020 2020 2020 206f 7574 6572             outer
-0000c2a0: 5f69 6e64 6578 203d 2030 0a20 2020 2020  _index = 0.     
-0000c2b0: 2020 2020 2020 2066 6f72 206f 7574 6572         for outer
-0000c2c0: 5f6c 6973 7420 696e 2073 656c 662e 7365  _list in self.se
-0000c2d0: 636f 6e64 6172 795f 696e 7465 7266 6163  condary_interfac
-0000c2e0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-0000c2f0: 2020 2020 6966 206f 7574 6572 5f6c 6973      if outer_lis
-0000c300: 745b 305d 203d 3d20 6e65 775f 656e 6470  t[0] == new_endp
-0000c310: 6f69 6e74 3a0a 2020 2020 2020 2020 2020  oint:.          
-0000c320: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c340: 6f75 7465 725f 696e 6465 7820 2b3d 2031  outer_index += 1
-0000c350: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c360: 6f75 7465 725f 696e 6465 7820 3c20 6c65  outer_index < le
-0000c370: 6e28 7365 6c66 2e73 6563 6f6e 6461 7279  n(self.secondary
-0000c380: 5f69 6e74 6572 6661 6365 7329 3a0a 2020  _interfaces):.  
-0000c390: 2020 2020 2020 2020 2020 2020 2020 656e                en
-0000c3a0: 6470 6f69 6e74 5f74 6f5f 636f 6e6e 6563  dpoint_to_connec
-0000c3b0: 7420 3d20 7365 6c66 2e73 6563 6f6e 6461  t = self.seconda
-0000c3c0: 7279 5f69 6e74 6572 6661 6365 735b 6f75  ry_interfaces[ou
-0000c3d0: 7465 725f 696e 6465 785d 5b73 656c 662e  ter_index][self.
-0000c3e0: 7365 636f 6e64 6172 795f 696e 6465 785d  secondary_index]
-0000c3f0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000c400: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000c410: 2020 2065 6e64 706f 696e 745f 746f 5f63     endpoint_to_c
-0000c420: 6f6e 6e65 6374 203d 206e 6577 5f65 6e64  onnect = new_end
-0000c430: 706f 696e 740a 0a20 2020 2020 2020 2065  point..        e
-0000c440: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000c450: 2065 6e64 706f 696e 745f 746f 5f63 6f6e   endpoint_to_con
-0000c460: 6e65 6374 203d 206e 6577 5f65 6e64 706f  nect = new_endpo
-0000c470: 696e 740a 0a20 2020 2020 2020 206c 6f67  int..        log
-0000c480: 6765 722e 6465 6275 6728 6622 5265 736f  ger.debug(f"Reso
-0000c490: 6c76 6564 206e 6577 2065 6e64 706f 696e  lved new endpoin
-0000c4a0: 7420 7b6e 6577 5f68 6f73 747d 3a7b 6e65  t {new_host}:{ne
-0000c4b0: 775f 706f 7274 7d20 746f 207b 656e 6470  w_port} to {endp
-0000c4c0: 6f69 6e74 5f74 6f5f 636f 6e6e 6563 747d  oint_to_connect}
-0000c4d0: 2229 0a0a 2020 2020 2020 2020 7265 7475  ")..        retu
-0000c4e0: 726e 2065 6e64 706f 696e 745f 746f 5f63  rn endpoint_to_c
-0000c4f0: 6f6e 6e65 6374 0a0a 2020 2020 6465 6620  onnect..    def 
-0000c500: 7265 6469 7265 6374 2873 656c 662c 206e  redirect(self, n
-0000c510: 6577 5f68 6f73 742c 206e 6577 5f70 6f72  ew_host, new_por
-0000c520: 7429 3a0a 2020 2020 2020 2020 2222 220a  t):.        """.
-0000c530: 2020 2020 2020 2020 5265 6469 7265 6374          Redirect
-0000c540: 7320 746f 2074 6865 2070 726f 7065 7220  s to the proper 
-0000c550: 7365 636f 6e64 6172 7920 696e 7465 7266  secondary interf
-0000c560: 6163 6520 6769 7665 6e20 6120 6e65 7720  ace given a new 
-0000c570: 656e 6470 6f69 6e74 2e0a 0a20 2020 2020  endpoint...     
-0000c580: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000c590: 2020 2020 206e 6577 5f68 6f73 745b 7374       new_host[st
-0000c5a0: 7269 6e67 5d3a 2074 6865 206e 6577 2068  ring]: the new h
-0000c5b0: 6f73 7420 746f 2062 6520 7265 6d61 7070  ost to be remapp
-0000c5c0: 6564 0a20 2020 2020 2020 2020 2020 206e  ed.            n
-0000c5d0: 6577 5f70 6f72 745b 696e 745d 3a20 7468  ew_port[int]: th
-0000c5e0: 6520 6e65 7720 706f 7274 2074 6f20 6265  e new port to be
-0000c5f0: 2072 656d 6170 7065 640a 0a20 2020 2020   remapped..     
-0000c600: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0000c610: 2020 2020 2020 2020 5b43 6f6e 6e65 6374          [Connect
-0000c620: 696f 6e5d 3a20 4120 6e65 7720 636f 6e6e  ion]: A new conn
-0000c630: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
-0000c640: 2222 220a 2020 2020 2020 2020 7265 6d61  """.        rema
-0000c650: 7070 6564 5f68 6f73 742c 2072 656d 6170  pped_host, remap
-0000c660: 7065 645f 706f 7274 203d 2073 656c 662e  ped_port = self.
-0000c670: 7265 736f 6c76 655f 6e65 775f 656e 6470  resolve_new_endp
-0000c680: 6f69 6e74 286e 6577 5f68 6f73 742c 206e  oint(new_host, n
-0000c690: 6577 5f70 6f72 7429 0a20 2020 2020 2020  ew_port).       
-0000c6a0: 206e 6577 5f65 6e64 706f 696e 7420 3d20   new_endpoint = 
-0000c6b0: 6622 7b72 656d 6170 7065 645f 686f 7374  f"{remapped_host
-0000c6c0: 7d3a 7b72 656d 6170 7065 645f 706f 7274  }:{remapped_port
-0000c6d0: 7d22 0a20 2020 2020 2020 206c 6f67 6765  }".        logge
-0000c6e0: 722e 6465 6275 6728 6622 5265 6469 7265  r.debug(f"Redire
-0000c6f0: 6374 696e 6720 636f 6e6e 6563 7469 6f6e  cting connection
-0000c700: 2074 6f20 7b6e 6577 5f68 6f73 747d 3a7b   to {new_host}:{
-0000c710: 6e65 775f 706f 7274 7d2c 2077 6869 6368  new_port}, which
-0000c720: 206d 6170 7320 746f 207b 7265 6d61 7070   maps to {remapp
-0000c730: 6564 5f68 6f73 747d 3a7b 7265 6d61 7070  ed_host}:{remapp
-0000c740: 6564 5f70 6f72 747d 2229 0a0a 2020 2020  ed_port}")..    
-0000c750: 2020 2020 7265 7475 726e 2043 6f6e 6e65      return Conne
-0000c760: 6374 696f 6e28 0a20 2020 2020 2020 2020  ction(.         
-0000c770: 2020 2075 7365 723d 7365 6c66 2e75 7365     user=self.use
-0000c780: 722c 2070 6173 7377 6f72 643d 7365 6c66  r, password=self
-0000c790: 2e70 6173 7377 6f72 642c 2068 6f73 743d  .password, host=
-0000c7a0: 6e65 775f 656e 6470 6f69 6e74 2c20 6461  new_endpoint, da
-0000c7b0: 7461 6261 7365 3d73 656c 662e 6461 7461  tabase=self.data
-0000c7c0: 6261 7365 2c20 746c 733d 7365 6c66 2e74  base, tls=self.t
-0000c7d0: 6c73 2c20 6861 6e64 7368 616b 653d 7365  ls, handshake=se
-0000c7e0: 6c66 2e68 616e 6473 6861 6b65 2c20 666f  lf.handshake, fo
-0000c7f0: 7263 653d 7365 6c66 2e66 6f72 6365 2c20  rce=self.force, 
-0000c800: 7365 7373 696f 6e3d 7365 6c66 2e73 6573  session=self.ses
-0000c810: 7369 6f6e 0a20 2020 2020 2020 2029 0a0a  sion.        )..
-0000c820: 2020 2020 6465 6620 7265 6672 6573 6828      def refresh(
-0000c830: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000c840: 2222 0a20 2020 2020 2020 2055 7365 6420  "".        Used 
-0000c850: 746f 2072 6566 7265 7368 2074 6865 2073  to refresh the s
-0000c860: 6573 7369 6f6e 2061 7373 6f63 6961 7465  ession associate
-0000c870: 6420 7769 7468 2074 6869 7320 636f 6e6e  d with this conn
-0000c880: 6563 7469 6f6e 2e20 5468 6520 7365 7276  ection. The serv
-0000c890: 6572 2077 696c 6c0a 2020 2020 2020 2020  er will.        
-0000c8a0: 7265 7475 726e 2061 206e 6577 2073 6572  return a new ser
-0000c8b0: 7665 7220 7365 7373 696f 6e20 6964 2061  ver session id a
-0000c8c0: 6e64 2073 6563 7572 6974 7920 746f 6b65  nd security toke
-0000c8d0: 6e2e 0a20 2020 2020 2020 2022 2222 0a20  n..        """. 
-0000c8e0: 2020 2020 2020 2072 6571 203d 2070 726f         req = pro
-0000c8f0: 746f 2e52 6571 7565 7374 2829 0a20 2020  to.Request().   
-0000c900: 2020 2020 2072 6571 2e74 7970 6520 3d20       req.type = 
-0000c910: 7265 712e 434c 4945 4e54 5f43 4f4e 4e45  req.CLIENT_CONNE
-0000c920: 4354 494f 4e5f 5245 4652 4553 485f 5345  CTION_REFRESH_SE
-0000c930: 5353 494f 4e0a 2020 2020 2020 2020 636c  SSION.        cl
-0000c940: 6965 6e74 5f63 6f6e 6e65 6374 696f 6e20  ient_connection 
-0000c950: 3d20 7265 712e 636c 6965 6e74 5f63 6f6e  = req.client_con
-0000c960: 6e65 6374 696f 6e5f 7265 6672 6573 685f  nection_refresh_
-0000c970: 7365 7373 696f 6e0a 0a20 2020 2020 2020  session..       
-0000c980: 2023 2053 656e 6420 6d65 7373 6167 650a   # Send message.
-0000c990: 2020 2020 2020 2020 5f73 656e 645f 6d73          _send_ms
-0000c9a0: 6728 7365 6c66 2c20 7265 7129 0a20 2020  g(self, req).   
-0000c9b0: 2020 2020 2023 2052 6563 6965 7665 206d       # Recieve m
-0000c9c0: 6573 7361 6765 0a20 2020 2020 2020 2072  essage.        r
-0000c9d0: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
-0000c9e0: 656c 662c 2070 726f 746f 2e43 6c69 656e  elf, proto.Clien
-0000c9f0: 7443 6f6e 6e65 6374 696f 6e52 6566 7265  tConnectionRefre
-0000ca00: 7368 5365 7373 696f 6e52 6573 706f 6e73  shSessionRespons
-0000ca10: 6528 2929 0a0a 2020 2020 2020 2020 6966  e())..        if
-0000ca20: 2072 7370 2e72 6573 706f 6e73 652e 7479   rsp.response.ty
-0000ca30: 7065 203d 3d20 7072 6f74 6f2e 436f 6e66  pe == proto.Conf
-0000ca40: 6972 6d61 7469 6f6e 5265 7370 6f6e 7365  irmationResponse
-0000ca50: 2e52 4553 504f 4e53 455f 5741 524e 3a0a  .RESPONSE_WARN:.
-0000ca60: 2020 2020 2020 2020 2020 2020 7761 726e              warn
-0000ca70: 2872 7370 2e72 6573 706f 6e73 652e 7265  (rsp.response.re
-0000ca80: 6173 6f6e 290a 2020 2020 2020 2020 656c  ason).        el
-0000ca90: 6966 2072 7370 2e72 6573 706f 6e73 652e  if rsp.response.
-0000caa0: 7479 7065 203d 3d20 7072 6f74 6f2e 436f  type == proto.Co
-0000cab0: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
-0000cac0: 7365 2e52 4553 504f 4e53 455f 4f4b 3a0a  se.RESPONSE_OK:.
-0000cad0: 2020 2020 2020 2020 2020 2020 2320 4361              # Ca
-0000cae0: 7074 7572 6520 7468 6520 7365 7373 696f  pture the sessio
-0000caf0: 6e20 6964 0a20 2020 2020 2020 2020 2020  n id.           
-0000cb00: 2073 656c 662e 7365 7276 6572 5365 7373   self.serverSess
-0000cb10: 696f 6e49 6420 3d20 7273 702e 7365 7373  ionId = rsp.sess
-0000cb20: 696f 6e49 6e66 6f2e 7365 7276 6572 5365  ionInfo.serverSe
-0000cb30: 7373 696f 6e49 640a 2020 2020 2020 2020  ssionId.        
-0000cb40: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000cb50: 2866 2243 6f6e 6e65 6374 6564 2074 6f20  (f"Connected to 
-0000cb60: 7365 7276 6572 2073 6573 7369 6f6e 2049  server session I
-0000cb70: 643a 207b 7365 6c66 2e73 6572 7665 7253  d: {self.serverS
-0000cb80: 6573 7369 6f6e 4964 7d22 290a 2020 2020  essionId}").    
-0000cb90: 2020 2020 2020 2020 7265 6365 6976 6564          received
-0000cba0: 5f74 6f6b 656e 203d 2072 7370 2e73 6573  _token = rsp.ses
-0000cbb0: 7369 6f6e 496e 666f 2e73 6563 7572 6974  sionInfo.securit
-0000cbc0: 7954 6f6b 656e 0a20 2020 2020 2020 2020  yToken.         
-0000cbd0: 2020 2069 6620 7365 6c66 2e73 6573 7369     if self.sessi
-0000cbe0: 6f6e 2e73 6563 7572 6974 7954 6f6b 656e  on.securityToken
-0000cbf0: 2021 3d20 4e6f 6e65 3a0a 2020 2020 2020   != None:.      
-0000cc00: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000cc10: 6573 7369 6f6e 203d 2053 6573 7369 6f6e  ession = Session
-0000cc20: 2873 6563 7572 6974 7954 6f6b 656e 3d53  (securityToken=S
-0000cc30: 6563 7572 6974 7954 6f6b 656e 2872 6563  ecurityToken(rec
-0000cc40: 6569 7665 645f 746f 6b65 6e2e 6461 7461  eived_token.data
-0000cc50: 2c20 7265 6365 6976 6564 5f74 6f6b 656e  , received_token
-0000cc60: 2e73 6967 6e61 7475 7265 2c20 7265 6365  .signature, rece
-0000cc70: 6976 6564 5f74 6f6b 656e 2e69 7373 7565  ived_token.issue
-0000cc80: 7246 696e 6765 7270 7269 6e74 2929 0a20  rFingerprint)). 
-0000cc90: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000cca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ccb0: 2023 2049 676e 6f72 6520 7468 6520 7365   # Ignore the se
-0000ccc0: 6375 7269 7479 2074 6f6b 656e 0a20 2020  curity token.   
-0000ccd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000cce0: 662e 7365 7373 696f 6e20 3d20 5365 7373  f.session = Sess
-0000ccf0: 696f 6e28 7573 6572 416e 6450 6173 7377  ion(userAndPassw
-0000cd00: 6f72 643d 5573 6572 416e 6450 6173 7377  ord=UserAndPassw
-0000cd10: 6f72 6428 7365 6c66 2e75 7365 722c 2073  ord(self.user, s
-0000cd20: 656c 662e 7061 7373 776f 7264 2929 0a20  elf.password)). 
-0000cd30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000cd40: 6e0a 2020 2020 2020 2020 2320 536f 6d65  n.        # Some
-0000cd50: 7468 696e 6720 6261 6420 6861 7070 656e  thing bad happen
-0000cd60: 6564 2077 6974 6820 7468 6520 7265 6672  ed with the refr
-0000cd70: 6573 6820 6174 7465 6d70 742e 0a20 2020  esh attempt..   
-0000cd80: 2020 2020 2072 6169 7365 205f 636f 6e76       raise _conv
-0000cd90: 6572 745f 6578 6365 7074 696f 6e28 7273  ert_exception(rs
-0000cda0: 702e 7265 7370 6f6e 7365 290a 0a0a 636c  p.response)...cl
-0000cdb0: 6173 7320 4375 7273 6f72 3a0a 2020 2020  ass Cursor:.    
-0000cdc0: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-0000cdd0: 653d 746f 6f2d 6d61 6e79 2d69 6e73 7461  e=too-many-insta
-0000cde0: 6e63 652d 6174 7472 6962 7574 6573 0a20  nce-attributes. 
-0000cdf0: 2020 2022 2222 4120 6461 7461 6261 7365     """A database
-0000ce00: 2063 7572 736f 722c 2077 6869 6368 2069   cursor, which i
-0000ce10: 7320 7573 6564 2074 6f20 6d61 6e61 6765  s used to manage
-0000ce20: 2061 2071 7565 7269 6520 616e 6420 6974   a querie and it
-0000ce30: 7320 7265 7475 726e 6564 2072 6573 756c  s returned resul
-0000ce40: 7473 2222 220a 0a20 2020 2064 6566 205f  ts"""..    def _
-0000ce50: 5f69 6e69 745f 5f28 7365 6c66 2c20 636f  _init__(self, co
-0000ce60: 6e6e 293a 0a20 2020 2020 2020 2022 2222  nn):.        """
-0000ce70: 4375 7273 6f72 7320 6172 6520 6e6f 726d  Cursors are norm
-0000ce80: 616c 6c79 2063 7265 6174 6564 2062 7920  ally created by 
-0000ce90: 7468 6520 6375 7273 6f72 2829 2063 616c  the cursor() cal
-0000cea0: 6c20 6f6e 2061 2063 6f6e 6e65 6374 696f  l on a connectio
-0000ceb0: 6e2c 2062 7574 2063 616e 0a20 2020 2020  n, but can.     
-0000cec0: 2020 2062 6520 6372 6561 7465 6420 6469     be created di
-0000ced0: 7265 6374 6c79 2062 7920 7072 6f76 6964  rectly by provid
-0000cee0: 696e 6720 6120 636f 6e6e 6563 7469 6f6e  ing a connection
-0000cef0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000cf00: 2020 2020 2073 656c 662e 636f 6e6e 6563       self.connec
-0000cf10: 7469 6f6e 203d 2063 6f6e 6e0a 2020 2020  tion = conn.    
-0000cf20: 2020 2020 7365 6c66 2e61 7272 6179 7369      self.arraysi
-0000cf30: 7a65 203d 2031 0a0a 2020 2020 2020 2020  ze = 1..        
-0000cf40: 7365 6c66 2e5f 7265 696e 6974 6961 6c69  self._reinitiali
-0000cf50: 7a65 2829 0a0a 2020 2020 6465 6620 5f5f  ze()..    def __
-0000cf60: 6465 6c5f 5f28 7365 6c66 293a 0a20 2020  del__(self):.   
-0000cf70: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0000cf80: 2020 2020 2020 7365 6c66 2e5f 636c 6f73        self._clos
-0000cf90: 655f 7265 7375 6c74 7365 7428 290a 2020  e_resultset().  
-0000cfa0: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-0000cfb0: 2020 2020 2020 2020 2020 7061 7373 0a0a            pass..
-0000cfc0: 2020 2020 6465 6620 5f72 6569 6e69 7469      def _reiniti
-0000cfd0: 616c 697a 6528 7365 6c66 293a 0a20 2020  alize(self):.   
-0000cfe0: 2020 2020 2022 2222 496e 7465 726e 616c       """Internal
-0000cff0: 2066 756e 6374 696f 6e20 746f 2069 6e69   function to ini
-0000d000: 7469 616c 697a 6520 6120 6375 7273 6f72  tialize a cursor
-0000d010: 2222 220a 2020 2020 2020 2020 2320 5365  """.        # Se
-0000d020: 7420 7468 6520 7374 6174 650a 2020 2020  t the state.    
-0000d030: 2020 2020 7365 6c66 2e71 7565 7279 5f69      self.query_i
-0000d040: 6420 3d20 4e6f 6e65 0a20 2020 2020 2020  d = None.       
-0000d050: 2073 656c 662e 726f 7763 6f75 6e74 203d   self.rowcount =
-0000d060: 202d 310a 2020 2020 2020 2020 7365 6c66   -1.        self
-0000d070: 2e72 6f77 6e75 6d62 6572 203d 204e 6f6e  .rownumber = Non
-0000d080: 650a 2020 2020 2020 2020 7365 6c66 2e72  e.        self.r
-0000d090: 6573 756c 7473 6574 5f74 7570 6c65 203d  esultset_tuple =
-0000d0a0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-0000d0b0: 6c66 2e64 6573 6372 6970 7469 6f6e 203d  lf.description =
-0000d0c0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-0000d0d0: 6c66 2e65 6e64 5f6f 665f 6461 7461 203d  lf.end_of_data =
-0000d0e0: 2046 616c 7365 0a20 2020 2020 2020 2073   False.        s
-0000d0f0: 656c 662e 6578 706c 6169 6e5f 7265 7375  elf.explain_resu
-0000d100: 6c74 203d 204e 6f6e 650a 2020 2020 2020  lt = None.      
-0000d110: 2020 7365 6c66 2e6c 6973 745f 7265 7375    self.list_resu
-0000d120: 6c74 203d 204e 6f6e 650a 2020 2020 2020  lt = None.      
-0000d130: 2020 7365 6c66 2e5f 6275 6666 6572 7320    self._buffers 
-0000d140: 3d20 5b5d 0a20 2020 2020 2020 2073 656c  = [].        sel
-0000d150: 662e 5f6f 6666 7365 7420 3d20 300a 2020  f._offset = 0.  
-0000d160: 2020 2020 2020 7365 6c66 2e5f 7065 6e64        self._pend
-0000d170: 696e 675f 6f70 7320 3d20 5b5d 0a0a 2020  ing_ops = []..  
-0000d180: 2020 6465 6620 7365 7469 6e70 7574 7369    def setinputsi
-0000d190: 7a65 7328 7365 6c66 2c20 7369 7a65 7329  zes(self, sizes)
-0000d1a0: 3a0a 2020 2020 2020 2020 2222 2254 6869  :.        """Thi
-0000d1b0: 7320 6361 6e20 6265 2075 7365 6420 6265  s can be used be
-0000d1c0: 666f 7265 2061 2063 616c 6c20 746f 202e  fore a call to .
-0000d1d0: 6578 6563 7574 652a 2829 2074 6f20 7072  execute*() to pr
-0000d1e0: 6564 6566 696e 650a 2020 2020 2020 2020  edefine.        
-0000d1f0: 6d65 6d6f 7279 2061 7265 6173 2066 6f72  memory areas for
-0000d200: 2074 6865 206f 7065 7261 7469 6f6e 2773   the operation's
-0000d210: 2070 6172 616d 6574 6572 732e 2043 7572   parameters. Cur
-0000d220: 7265 6e74 6c79 2069 676e 6f72 6564 0a20  rently ignored. 
-0000d230: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-0000d240: 6465 6620 7365 746f 7574 7075 7473 697a  def setoutputsiz
-0000d250: 6528 7365 6c66 2c20 7369 7a65 2c20 636f  e(self, size, co
-0000d260: 6c75 6d6e 3d4e 6f6e 6529 3a0a 2020 2020  lumn=None):.    
-0000d270: 2020 2020 2222 2253 6574 2061 2063 6f6c      """Set a col
-0000d280: 756d 6e20 6275 6666 6572 2073 697a 6520  umn buffer size 
-0000d290: 666f 7220 6665 7463 6865 7320 6f66 206c  for fetches of l
-0000d2a0: 6172 6765 2063 6f6c 756d 6e73 0a20 2020  arge columns.   
-0000d2b0: 2020 2020 2028 652e 672e 204c 4f4e 4773       (e.g. LONGs
-0000d2c0: 2c20 424c 4f42 732c 2065 7463 2e29 2e20  , BLOBs, etc.). 
-0000d2d0: 5468 6520 636f 6c75 6d6e 2069 7320 7370  The column is sp
-0000d2e0: 6563 6966 6965 6420 6173 2061 6e0a 2020  ecified as an.  
-0000d2f0: 2020 2020 2020 696e 6465 7820 696e 746f        index into
-0000d300: 2074 6865 2072 6573 756c 7420 7365 7175   the result sequ
-0000d310: 656e 6365 2e20 4375 7272 656e 746c 7920  ence. Currently 
-0000d320: 6967 6e6f 7265 640a 2020 2020 2020 2020  ignored.        
-0000d330: 2222 220a 0a20 2020 2064 6566 2063 6c6f  """..    def clo
-0000d340: 7365 2873 656c 6629 3a0a 2020 2020 2020  se(self):.      
-0000d350: 2020 2222 2243 6c6f 7365 2074 6869 7320    """Close this 
-0000d360: 6375 7273 6f72 2e20 2054 6865 2063 7572  cursor.  The cur
-0000d370: 7265 6e74 2072 6573 756c 7420 7365 7420  rent result set 
-0000d380: 6973 2063 6c6f 7365 642c 2062 7574 0a20  is closed, but. 
-0000d390: 2020 2020 2020 2074 6865 2063 7572 736f         the curso
-0000d3a0: 7220 6361 6e20 6265 2072 6575 7365 6420  r can be reused 
-0000d3b0: 666f 7220 7375 6273 6571 7565 6e74 2065  for subsequent e
-0000d3c0: 7865 6375 7465 2829 2063 616c 6c73 2e0a  xecute() calls..
-0000d3d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000d3e0: 2020 2020 6966 2073 656c 662e 5f62 7566      if self._buf
-0000d3f0: 6665 7273 3a0a 2020 2020 2020 2020 2020  fers:.          
-0000d400: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0000d410: 2020 2020 2020 2073 656c 662e 5f63 6c6f         self._clo
-0000d420: 7365 5f72 6573 756c 7473 6574 2829 0a20  se_resultset(). 
-0000d430: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-0000d440: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0000d450: 2020 2070 6173 730a 0a20 2020 2020 2020     pass..       
-0000d460: 2073 656c 662e 5f72 6569 6e69 7469 616c   self._reinitial
-0000d470: 697a 6528 290a 0a20 2020 2064 6566 2065  ize()..    def e
-0000d480: 7865 6375 7465 6d61 6e79 2873 656c 662c  xecutemany(self,
-0000d490: 206f 7065 7261 7469 6f6e 2c20 7061 7261   operation, para
-0000d4a0: 6d65 7465 726c 6973 7429 3a0a 2020 2020  meterlist):.    
-0000d4b0: 2020 2020 2222 2250 7265 7061 7265 2061      """Prepare a
-0000d4c0: 2064 6174 6162 6173 6520 6f70 6572 6174   database operat
-0000d4d0: 696f 6e20 2871 7565 7279 206f 7220 636f  ion (query or co
-0000d4e0: 6d6d 616e 6429 2061 6e64 2074 6865 6e20  mmand) and then 
-0000d4f0: 6578 6563 7574 6520 6974 2061 6761 696e  execute it again
-0000d500: 7374 0a20 2020 2020 2020 2061 6c6c 2070  st.        all p
-0000d510: 6172 616d 6574 6572 2073 6571 7565 6e63  arameter sequenc
-0000d520: 6573 206f 7220 6d61 7070 696e 6773 2066  es or mappings f
-0000d530: 6f75 6e64 2069 6e20 7468 6520 7365 7175  ound in the sequ
-0000d540: 656e 6365 2070 6172 616d 6574 6572 6c69  ence parameterli
-0000d550: 7374 2e0a 0a20 2020 2020 2020 2050 6172  st...        Par
-0000d560: 616d 6574 6572 7320 6d61 7920 6265 2070  ameters may be p
-0000d570: 726f 7669 6465 6420 6173 2061 206d 6170  rovided as a map
-0000d580: 7069 6e67 2061 6e64 2077 696c 6c20 6265  ping and will be
-0000d590: 2062 6f75 6e64 2074 6f20 7661 7269 6162   bound to variab
-0000d5a0: 6c65 730a 2020 2020 2020 2020 696e 2074  les.        in t
-0000d5b0: 6865 206f 7065 7261 7469 6f6e 2e20 5661  he operation. Va
-0000d5c0: 7269 6162 6c65 7320 6172 6520 7370 6563  riables are spec
-0000d5d0: 6966 6965 6420 696e 2050 7974 686f 6e20  ified in Python 
-0000d5e0: 6578 7465 6e64 6564 2066 6f72 6d61 7420  extended format 
-0000d5f0: 636f 6465 732c 0a20 2020 2020 2020 2065  codes,.        e
-0000d600: 2e67 2e20 2e2e 2e57 4845 5245 206e 616d  .g. ...WHERE nam
-0000d610: 653d 2528 6e61 6d65 290a 2020 2020 2020  e=%(name).      
-0000d620: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
-0000d630: 6c66 2e5f 7265 696e 6974 6961 6c69 7a65  lf._reinitialize
-0000d640: 2829 0a0a 2020 2020 2020 2020 2320 7765  ()..        # we
-0000d650: 2063 616e 2774 206a 7573 7420 6578 6563   can't just exec
-0000d660: 7574 6520 616c 6c20 7468 6520 7175 6572  ute all the quer
-0000d670: 6965 7320 6174 206f 6e63 652e 2e2e 2e6f  ies at once....o
-0000d680: 6369 656e 7420 6f6e 6c79 2061 6c6c 6f77  cient only allow
-0000d690: 730a 2020 2020 2020 2020 2320 6f6e 6520  s.        # one 
-0000d6a0: 7175 6572 7920 6174 2061 2074 696d 6520  query at a time 
-0000d6b0: 6f6e 2061 2063 6f6e 6e65 6374 696f 6e2e  on a connection.
-0000d6c0: 2020 536f 2071 7565 7565 2075 7020 616c    So queue up al
-0000d6d0: 6c20 7468 6520 7175 6572 6965 7320 616e  l the queries an
-0000d6e0: 640a 2020 2020 2020 2020 2320 7765 276c  d.        # we'l
-0000d6f0: 6c20 6361 6c6c 2074 6865 6d20 6c61 7465  l call them late
-0000d700: 720a 2020 2020 2020 2020 666f 7220 7061  r.        for pa
-0000d710: 7261 6d20 696e 2070 6172 616d 6574 6572  ram in parameter
-0000d720: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
-0000d730: 2020 7365 6c66 2e5f 7065 6e64 696e 675f    self._pending_
-0000d740: 6f70 732e 6170 7065 6e64 286f 7065 7261  ops.append(opera
-0000d750: 7469 6f6e 2025 2070 6172 616d 290a 0a20  tion % param).. 
-0000d760: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0000d770: 7065 6e64 696e 675f 6f70 733a 0a20 2020  pending_ops:.   
-0000d780: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
-0000d790: 7865 6375 7465 5f69 6e74 6572 6e61 6c28  xecute_internal(
-0000d7a0: 7365 6c66 2e5f 7065 6e64 696e 675f 6f70  self._pending_op
-0000d7b0: 732e 706f 7028 3029 290a 0a20 2020 2020  s.pop(0))..     
-0000d7c0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0000d7d0: 2020 2020 6465 6620 6578 6563 7574 6528      def execute(
-0000d7e0: 7365 6c66 2c20 6f70 6572 6174 696f 6e2c  self, operation,
-0000d7f0: 2070 6172 616d 6574 6572 733d 4e6f 6e65   parameters=None
-0000d800: 293a 0a20 2020 2020 2020 2022 2222 5072  ):.        """Pr
-0000d810: 6570 6172 6520 616e 6420 6578 6563 7574  epare and execut
-0000d820: 6520 6120 6461 7461 6261 7365 206f 7065  e a database ope
-0000d830: 7261 7469 6f6e 2028 7175 6572 7920 6f72  ration (query or
-0000d840: 2063 6f6d 6d61 6e64 292e 0a0a 2020 2020   command)...    
-0000d850: 2020 2020 5061 7261 6d65 7465 7273 206d      Parameters m
-0000d860: 6179 2062 6520 7072 6f76 6964 6564 2061  ay be provided a
-0000d870: 7320 6120 6d61 7070 696e 6720 616e 6420  s a mapping and 
-0000d880: 7769 6c6c 2062 6520 626f 756e 6420 746f  will be bound to
-0000d890: 2076 6172 6961 626c 6573 0a20 2020 2020   variables.     
-0000d8a0: 2020 2069 6e20 7468 6520 6f70 6572 6174     in the operat
-0000d8b0: 696f 6e2e 2056 6172 6961 626c 6573 2061  ion. Variables a
-0000d8c0: 7265 2073 7065 6369 6669 6564 2069 6e20  re specified in 
-0000d8d0: 5079 7468 6f6e 2065 7874 656e 6465 6420  Python extended 
-0000d8e0: 666f 726d 6174 2063 6f64 6573 2c0a 2020  format codes,.  
-0000d8f0: 2020 2020 2020 652e 672e 202e 2e2e 5748        e.g. ...WH
-0000d900: 4552 4520 6e61 6d65 3d25 286e 616d 6529  ERE name=%(name)
-0000d910: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d920: 2020 2020 2073 656c 662e 5f72 6569 6e69       self._reini
-0000d930: 7469 616c 697a 6528 290a 2020 2020 2020  tialize().      
-0000d940: 2020 7365 6c66 2e5f 6578 6563 7574 655f    self._execute_
-0000d950: 696e 7465 726e 616c 286f 7065 7261 7469  internal(operati
-0000d960: 6f6e 2c20 7061 7261 6d65 7465 7273 290a  on, parameters).
-0000d970: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000d980: 7365 6c66 0a0a 2020 2020 6465 6620 5f65  self..    def _e
-0000d990: 7865 6375 7465 5f69 6e74 6572 6e61 6c28  xecute_internal(
-0000d9a0: 7365 6c66 2c20 6f70 6572 6174 696f 6e2c  self, operation,
-0000d9b0: 2070 6172 616d 6574 6572 733d 4e6f 6e65   parameters=None
-0000d9c0: 293a 0a20 2020 2020 2020 2022 2222 496e  ):.        """In
-0000d9d0: 7465 726e 616c 2065 7865 6375 7465 2072  ternal execute r
-0000d9e0: 6f75 7469 6e65 2074 6861 7420 6765 7473  outine that gets
-0000d9f0: 2063 616c 6c65 6420 6672 6f6d 2065 7865   called from exe
-0000da00: 6375 7465 2061 6e64 2065 7865 6375 7465  cute and execute
-0000da10: 6d61 6e79 2222 220a 2020 2020 2020 2020  many""".        
-0000da20: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-0000da30: 653d 746f 6f2d 6d61 6e79 2d62 7261 6e63  e=too-many-branc
-0000da40: 6865 730a 0a20 2020 2020 2020 2069 6620  hes..        if 
-0000da50: 6861 7361 7474 7228 6f70 6572 6174 696f  hasattr(operatio
-0000da60: 6e2c 2022 6465 636f 6465 2229 3a0a 2020  n, "decode"):.  
-0000da70: 2020 2020 2020 2020 2020 6f70 6572 6174            operat
-0000da80: 696f 6e20 3d20 6f70 6572 6174 696f 6e2e  ion = operation.
-0000da90: 6465 636f 6465 2829 0a0a 2020 2020 2020  decode()..      
-0000daa0: 2020 6966 2070 6172 616d 6574 6572 7320    if parameters 
-0000dab0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000dac0: 2020 2020 2020 2020 2069 6620 6861 7361           if hasa
-0000dad0: 7474 7228 6c69 7374 2870 6172 616d 6574  ttr(list(paramet
-0000dae0: 6572 732e 6b65 7973 2829 295b 305d 2c20  ers.keys())[0], 
-0000daf0: 2264 6563 6f64 6522 293a 0a20 2020 2020  "decode"):.     
-0000db00: 2020 2020 2020 2020 2020 2070 6172 616d             param
-0000db10: 6574 6572 7320 3d20 7b6b 6579 2e64 6563  eters = {key.dec
-0000db20: 6f64 6528 293a 2076 616c 7565 2066 6f72  ode(): value for
-0000db30: 2028 6b65 792c 2076 616c 7565 2920 696e   (key, value) in
-0000db40: 2070 6172 616d 6574 6572 732e 6974 656d   parameters.item
-0000db50: 7328 297d 0a20 2020 2020 2020 2020 2020  s()}.           
-0000db60: 206f 7065 7261 7469 6f6e 203d 206f 7065   operation = ope
-0000db70: 7261 7469 6f6e 2025 2070 6172 616d 6574  ration % paramet
-0000db80: 6572 730a 0a20 2020 2020 2020 2023 2057  ers..        # W
-0000db90: 6520 6e65 6564 2074 6f20 6669 6775 7265  e need to figure
-0000dba0: 206f 7574 2077 6865 7468 6572 2077 6520   out whether we 
-0000dbb0: 7368 6f75 6c64 2063 616c 6c0a 2020 2020  should call.    
-0000dbc0: 2020 2020 2320 6578 6563 7574 655f 7175      # execute_qu
-0000dbd0: 6572 7920 6f72 2065 7865 6375 7465 5f75  ery or execute_u
-0000dbe0: 7064 6174 650a 2020 2020 2020 2020 7374  pdate.        st
-0000dbf0: 7269 7070 6564 203d 206f 7065 7261 7469  ripped = operati
-0000dc00: 6f6e 0a0a 2020 2020 2020 2020 2320 4c6f  on..        # Lo
-0000dc10: 6f70 2075 6e74 696c 2077 6520 6861 7665  op until we have
-0000dc20: 2073 6f6d 6520 7374 6172 7469 6e67 2077   some starting w
-0000dc30: 6f72 6473 2e20 4e6f 7465 2074 6869 730a  ords. Note this.
-0000dc40: 2020 2020 2020 2020 2320 646f 6573 6e27          # doesn'
-0000dc50: 7420 6163 7475 616c 6c79 2068 616e 646c  t actually handl
-0000dc60: 6520 7468 6520 6361 7365 206f 6620 2777  e the case of 'w
-0000dc70: 6f72 6431 202f 2a20 636f 6d6d 656e 7420  ord1 /* comment 
-0000dc80: 2a2f 2077 6f72 6432 272c 0a20 2020 2020  */ word2',.     
-0000dc90: 2020 2023 2062 7574 206e 6f6e 6520 6f66     # but none of
-0000dca0: 2074 6865 206f 7468 6572 2063 6c69 656e   the other clien
-0000dcb0: 7473 2064 6f20 6569 7468 6572 2e2e 2e0a  ts do either....
-0000dcc0: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
-0000dcd0: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
-0000dce0: 2320 7374 7269 7020 6f66 6620 7374 6172  # strip off star
-0000dcf0: 7469 6e67 2073 7061 6365 730a 2020 2020  ting spaces.    
-0000dd00: 2020 2020 2020 2020 7374 7269 7070 6564          stripped
-0000dd10: 203d 2073 7472 6970 7065 642e 6c73 7472   = stripped.lstr
-0000dd20: 6970 2829 0a0a 2020 2020 2020 2020 2020  ip()..          
-0000dd30: 2020 2320 6966 2074 6869 7320 7374 6172    # if this star
-0000dd40: 7473 2077 6974 6820 2d2d 2c20 7374 7269  ts with --, stri
-0000dd50: 7020 7468 6520 7265 7374 206f 6620 7468  p the rest of th
-0000dd60: 6520 6c69 6e65 0a20 2020 2020 2020 2020  e line.         
-0000dd70: 2020 2069 6620 7374 7269 7070 6564 2e73     if stripped.s
-0000dd80: 7461 7274 7377 6974 6828 222d 2d22 293a  tartswith("--"):
-0000dd90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dda0: 2070 6f73 203d 2073 7472 6970 7065 642e   pos = stripped.
-0000ddb0: 6669 6e64 2822 5c6e 2229 0a20 2020 2020  find("\n").     
-0000ddc0: 2020 2020 2020 2020 2020 2069 6620 706f             if po
-0000ddd0: 7320 3d3d 202d 313a 0a20 2020 2020 2020  s == -1:.       
-0000dde0: 2020 2020 2020 2020 2020 2020 2073 7472               str
-0000ddf0: 6970 7065 6420 3d20 2222 0a20 2020 2020  ipped = "".     
-0000de00: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000de10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000de20: 2020 2020 2073 7472 6970 7065 6420 3d20       stripped = 
-0000de30: 7374 7269 7070 6564 5b70 6f73 202b 2031  stripped[pos + 1
-0000de40: 203a 5d0a 0a20 2020 2020 2020 2020 2020   :]..           
-0000de50: 2023 2069 6620 7468 6973 2073 7461 7274   # if this start
-0000de60: 7320 7769 7468 202f 2a2c 2073 7472 6970  s with /*, strip
-0000de70: 2075 6e74 696c 202a 2f0a 2020 2020 2020   until */.      
-0000de80: 2020 2020 2020 656c 6966 2073 7472 6970        elif strip
-0000de90: 7065 642e 7374 6172 7473 7769 7468 2822  ped.startswith("
-0000dea0: 2f2a 2229 3a0a 2020 2020 2020 2020 2020  /*"):.          
-0000deb0: 2020 2020 2020 706f 7320 3d20 7374 7269        pos = stri
-0000dec0: 7070 6564 2e66 696e 6428 222a 2f22 290a  pped.find("*/").
-0000ded0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dee0: 6966 2070 6f73 203d 3d20 2d31 3a0a 2020  if pos == -1:.  
-0000def0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df00: 2020 7374 7269 7070 6564 203d 2022 220a    stripped = "".
-0000df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000df30: 2020 2020 2020 2020 2020 7374 7269 7070            stripp
-0000df40: 6564 203d 2073 7472 6970 7065 645b 706f  ed = stripped[po
-0000df50: 7320 2b20 3220 3a5d 0a20 2020 2020 2020  s + 2 :].       
-0000df60: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000df70: 2020 2020 2020 2020 2020 2023 2079 6179             # yay
-0000df80: 2c20 6e6f 2063 6f6d 6d65 6e74 732c 206d  , no comments, m
-0000df90: 6f76 6520 746f 2074 6865 206e 6578 7420  ove to the next 
-0000dfa0: 7068 6173 650a 2020 2020 2020 2020 2020  phase.          
-0000dfb0: 2020 2020 2020 6272 6561 6b0a 0a20 2020        break..   
-0000dfc0: 2020 2020 2023 2069 6620 7765 2064 6f6e       # if we don
-0000dfd0: 2774 2068 6176 6520 616e 7974 6869 6e67  't have anything
-0000dfe0: 206c 6566 742c 206a 7573 7420 7265 7475   left, just retu
-0000dff0: 726e 205b 5d0a 2020 2020 2020 2020 6966  rn [].        if
-0000e000: 206e 6f74 2073 7472 6970 7065 643a 0a20   not stripped:. 
-0000e010: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000e020: 6e0a 0a20 2020 2020 2020 2023 206e 6f77  n..        # now
-0000e030: 2073 706c 6974 206f 7574 2074 6865 2077   split out the w
-0000e040: 6f72 6473 0a20 2020 2020 2020 2077 6f72  ords.        wor
-0000e050: 6473 203d 2073 7472 6970 7065 642e 7370  ds = stripped.sp
-0000e060: 6c69 7428 4e6f 6e65 2c20 3329 0a0a 2020  lit(None, 3)..  
-0000e070: 2020 2020 2020 2320 5369 6e67 6c65 2077        # Single w
-0000e080: 6f72 6420 6d61 7463 6865 730a 2020 2020  ord matches.    
-0000e090: 2020 2020 7175 6572 795f 7479 7065 203d      query_type =
-0000e0a0: 2077 6f72 6473 5b30 5d2e 7570 7065 7228   words[0].upper(
-0000e0b0: 290a 2020 2020 2020 2020 6966 2071 7565  ).        if que
-0000e0c0: 7279 5f74 7970 6520 696e 205b 2253 454c  ry_type in ["SEL
-0000e0d0: 4543 5422 2c20 2257 4954 4822 2c20 2245  ECT", "WITH", "E
-0000e0e0: 5850 4f52 5422 2c20 2243 4845 434b 225d  XPORT", "CHECK"]
-0000e0f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000e100: 7475 726e 2073 656c 662e 5f65 7865 6375  turn self._execu
-0000e110: 7465 5f71 7565 7279 286f 7065 7261 7469  te_query(operati
-0000e120: 6f6e 3d6f 7065 7261 7469 6f6e 2c20 7175  on=operation, qu
-0000e130: 6572 795f 7479 7065 3d71 7565 7279 5f74  ery_type=query_t
-0000e140: 7970 6529 0a20 2020 2020 2020 2065 6c69  ype).        eli
-0000e150: 6620 7175 6572 795f 7479 7065 2069 6e20  f query_type in 
-0000e160: 5b22 4558 504c 4149 4e22 5d3a 0a20 2020  ["EXPLAIN"]:.   
-0000e170: 2020 2020 2020 2020 2023 2065 7870 6c61           # expla
-0000e180: 696e 2070 6970 656c 696e 650a 2020 2020  in pipeline.    
-0000e190: 2020 2020 2020 2020 6966 206c 656e 2877          if len(w
-0000e1a0: 6f72 6473 2920 3e20 3120 616e 6420 776f  ords) > 1 and wo
-0000e1b0: 7264 735b 315d 2e75 7070 6572 2829 203d  rds[1].upper() =
-0000e1c0: 3d20 2250 4950 454c 494e 4522 3a0a 2020  = "PIPELINE":.  
-0000e1d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000e1e0: 7475 726e 2073 656c 662e 5f65 7865 6375  turn self._execu
-0000e1f0: 7465 5f71 7565 7279 286f 7065 7261 7469  te_query(operati
-0000e200: 6f6e 3d6f 7065 7261 7469 6f6e 2c20 7175  on=operation, qu
-0000e210: 6572 795f 7479 7065 3d71 7565 7279 5f74  ery_type=query_t
-0000e220: 7970 6520 2b20 2220 5049 5045 4c49 4e45  ype + " PIPELINE
-0000e230: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
-0000e240: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000e250: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000e260: 2e5f 6578 6563 7574 655f 7175 6572 7928  ._execute_query(
-0000e270: 6f70 6572 6174 696f 6e3d 6f70 6572 6174  operation=operat
-0000e280: 696f 6e2c 2071 7565 7279 5f74 7970 653d  ion, query_type=
-0000e290: 7175 6572 795f 7479 7065 290a 2020 2020  query_type).    
-0000e2a0: 2020 2020 656c 6966 2071 7565 7279 5f74      elif query_t
-0000e2b0: 7970 6520 696e 205b 224c 4953 5422 5d3a  ype in ["LIST"]:
-0000e2c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000e2d0: 6f70 6572 6174 696f 6e2e 7570 7065 7228  operation.upper(
-0000e2e0: 2920 3d3d 2022 4c49 5354 2041 4c4c 2051  ) == "LIST ALL Q
-0000e2f0: 5545 5249 4553 223a 0a20 2020 2020 2020  UERIES":.       
-0000e300: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000e310: 7365 6c66 2e5f 6578 6563 7574 655f 7175  self._execute_qu
-0000e320: 6572 7928 6f70 6572 6174 696f 6e3d 2253  ery(operation="S
-0000e330: 454c 4543 5420 2a20 4652 4f4d 2053 5953  ELECT * FROM SYS
-0000e340: 2e51 5545 5249 4553 222c 2071 7565 7279  .QUERIES", query
-0000e350: 5f74 7970 653d 2253 454c 4543 5422 290a  _type="SELECT").
-0000e360: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0000e370: 206f 7065 7261 7469 6f6e 2e75 7070 6572   operation.upper
-0000e380: 2829 203d 3d20 224c 4953 5420 414c 4c20  () == "LIST ALL 
-0000e390: 434f 4d50 4c45 5445 4420 5155 4552 4945  COMPLETED QUERIE
-0000e3a0: 5322 3a0a 2020 2020 2020 2020 2020 2020  S":.            
-0000e3b0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000e3c0: 5f65 7865 6375 7465 5f71 7565 7279 286f  _execute_query(o
-0000e3d0: 7065 7261 7469 6f6e 3d22 5345 4c45 4354  peration="SELECT
-0000e3e0: 202a 2046 524f 4d20 5359 532e 434f 4d50   * FROM SYS.COMP
-0000e3f0: 4c45 5445 445f 5155 4552 4945 5322 2c20  LETED_QUERIES", 
-0000e400: 7175 6572 795f 7479 7065 3d22 5345 4c45  query_type="SELE
-0000e410: 4354 2229 0a20 2020 2020 2020 2020 2020  CT").           
-0000e420: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000e430: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000e440: 6c66 2e5f 6578 6563 7574 655f 6c69 7374  lf._execute_list
-0000e450: 286f 7065 7261 7469 6f6e 3d6f 7065 7261  (operation=opera
-0000e460: 7469 6f6e 290a 2020 2020 2020 2020 656c  tion).        el
-0000e470: 6966 2071 7565 7279 5f74 7970 6520 3d3d  if query_type ==
-0000e480: 2022 464f 5243 4522 3a0a 2020 2020 2020   "FORCE":.      
-0000e490: 2020 2020 2020 7365 6c66 2e5f 6578 6563        self._exec
-0000e4a0: 7574 655f 666f 7263 6528 6f70 6572 6174  ute_force(operat
-0000e4b0: 696f 6e3d 6f70 6572 6174 696f 6e29 0a20  ion=operation). 
-0000e4c0: 2020 2020 2020 2065 6c69 6620 7175 6572         elif quer
-0000e4d0: 795f 7479 7065 203d 3d20 2253 4554 223a  y_type == "SET":
-0000e4e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000e4f0: 662e 5f65 7865 6375 7465 5f73 6574 2877  f._execute_set(w
-0000e500: 6f72 6473 5b31 3a5d 290a 2020 2020 2020  ords[1:]).      
-0000e510: 2020 656c 6966 2071 7565 7279 5f74 7970    elif query_typ
-0000e520: 6520 3d3d 2022 4745 5422 3a0a 2020 2020  e == "GET":.    
-0000e530: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
-0000e540: 6563 7574 655f 6765 7428 776f 7264 735b  ecute_get(words[
-0000e550: 313a 5d29 0a20 2020 2020 2020 2065 6c69  1:]).        eli
-0000e560: 6620 7175 6572 795f 7479 7065 203d 3d20  f query_type == 
-0000e570: 224b 494c 4c22 206f 7220 7175 6572 795f  "KILL" or query_
-0000e580: 7479 7065 203d 3d20 2243 414e 4345 4c22  type == "CANCEL"
-0000e590: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000e5a0: 6c66 2e5f 6578 6563 7574 655f 6361 6e63  lf._execute_canc
-0000e5b0: 656c 6b69 6c6c 2871 7565 7279 5f74 7970  elkill(query_typ
-0000e5c0: 652c 2077 6f72 6473 5b31 3a5d 290a 2020  e, words[1:]).  
-0000e5d0: 2020 2020 2020 656c 6966 2071 7565 7279        elif query
-0000e5e0: 5f74 7970 6520 3d3d 2022 434c 4541 5222  _type == "CLEAR"
-0000e5f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000e600: 6c66 2e5f 6578 6563 7574 655f 636c 6561  lf._execute_clea
-0000e610: 7228 776f 7264 735b 313a 5d29 0a20 2020  r(words[1:]).   
-0000e620: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000e630: 2020 2020 2020 2023 206f 6b2c 2074 6869         # ok, thi
-0000e640: 7320 6973 2061 6e20 7570 6461 7465 0a20  s is an update. 
-0000e650: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e660: 5f65 7865 6375 7465 5f75 7064 6174 6528  _execute_update(
-0000e670: 6f70 6572 6174 696f 6e29 0a0a 2020 2020  operation)..    
-0000e680: 6465 6620 7461 626c 6573 2873 656c 662c  def tables(self,
-0000e690: 2073 6368 656d 613d 2225 222c 2074 6162   schema="%", tab
-0000e6a0: 6c65 3d22 2522 293a 0a20 2020 2020 2020  le="%"):.       
-0000e6b0: 2022 2222 4765 7420 7468 6520 6461 7461   """Get the data
-0000e6c0: 6261 7365 2074 6162 6c65 7322 2222 0a20  base tables""". 
-0000e6d0: 2020 2020 2020 2023 2070 796c 696e 743a         # pylint:
-0000e6e0: 2064 6973 6162 6c65 3d6e 6f2d 6d65 6d62   disable=no-memb
-0000e6f0: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
-0000e700: 5f6d 6574 6164 6174 615f 7265 7128 7072  _metadata_req(pr
-0000e710: 6f74 6f2e 4665 7463 6853 7973 7465 6d4d  oto.FetchSystemM
-0000e720: 6574 6164 6174 612e 4745 545f 5441 424c  etadata.GET_TABL
-0000e730: 4553 2c20 7363 6865 6d61 3d73 6368 656d  ES, schema=schem
-0000e740: 612c 2074 6162 6c65 3d74 6162 6c65 290a  a, table=table).
-0000e750: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000e760: 656c 660a 0a20 2020 2064 6566 2073 7973  elf..    def sys
-0000e770: 7465 6d5f 7461 626c 6573 2873 656c 662c  tem_tables(self,
-0000e780: 2074 6162 6c65 3d22 2522 293a 0a20 2020   table="%"):.   
-0000e790: 2020 2020 2022 2222 4765 7420 7468 6520       """Get the 
-0000e7a0: 6461 7461 6261 7365 2073 7973 7465 6d20  database system 
-0000e7b0: 7461 626c 6573 2222 220a 2020 2020 2020  tables""".      
-0000e7c0: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-0000e7d0: 626c 653d 6e6f 2d6d 656d 6265 720a 2020  ble=no-member.  
-0000e7e0: 2020 2020 2020 7365 6c66 2e5f 6d65 7461        self._meta
-0000e7f0: 6461 7461 5f72 6571 2870 726f 746f 2e46  data_req(proto.F
-0000e800: 6574 6368 5379 7374 656d 4d65 7461 6461  etchSystemMetada
-0000e810: 7461 2e47 4554 5f53 5953 5445 4d5f 5441  ta.GET_SYSTEM_TA
-0000e820: 424c 4553 2c20 7461 626c 653d 7461 626c  BLES, table=tabl
-0000e830: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
-0000e840: 6e20 7365 6c66 0a0a 2020 2020 6465 6620  n self..    def 
-0000e850: 7669 6577 7328 7365 6c66 2c20 7669 6577  views(self, view
-0000e860: 3d22 2522 293a 0a20 2020 2020 2020 2022  ="%"):.        "
-0000e870: 2222 4765 7420 7468 6520 6461 7461 6261  ""Get the databa
-0000e880: 7365 2076 6965 7773 2222 220a 2020 2020  se views""".    
-0000e890: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
-0000e8a0: 7361 626c 653d 6e6f 2d6d 656d 6265 720a  sable=no-member.
-0000e8b0: 2020 2020 2020 2020 7365 6c66 2e5f 6d65          self._me
-0000e8c0: 7461 6461 7461 5f72 6571 2870 726f 746f  tadata_req(proto
-0000e8d0: 2e46 6574 6368 5379 7374 656d 4d65 7461  .FetchSystemMeta
-0000e8e0: 6461 7461 2e47 4554 5f56 4945 5753 2c20  data.GET_VIEWS, 
-0000e8f0: 7669 6577 3d76 6965 7729 0a20 2020 2020  view=view).     
-0000e900: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0000e910: 2020 2020 6465 6620 636f 6c75 6d6e 7328      def columns(
-0000e920: 7365 6c66 2c20 7363 6865 6d61 3d22 2522  self, schema="%"
-0000e930: 2c20 7461 626c 653d 2225 222c 2063 6f6c  , table="%", col
-0000e940: 756d 6e3d 2225 2229 3a0a 2020 2020 2020  umn="%"):.      
-0000e950: 2020 2222 2247 6574 2074 6865 2064 6174    """Get the dat
-0000e960: 6162 6173 6520 636f 6c75 6d6e 7322 2222  abase columns"""
-0000e970: 0a20 2020 2020 2020 2023 2070 796c 696e  .        # pylin
-0000e980: 743a 2064 6973 6162 6c65 3d6e 6f2d 6d65  t: disable=no-me
-0000e990: 6d62 6572 0a20 2020 2020 2020 2073 656c  mber.        sel
-0000e9a0: 662e 5f6d 6574 6164 6174 615f 7265 7128  f._metadata_req(
-0000e9b0: 7072 6f74 6f2e 4665 7463 6853 7973 7465  proto.FetchSyste
-0000e9c0: 6d4d 6574 6164 6174 612e 4745 545f 434f  mMetadata.GET_CO
-0000e9d0: 4c55 4d4e 532c 2073 6368 656d 613d 7363  LUMNS, schema=sc
-0000e9e0: 6865 6d61 2c20 7461 626c 653d 7461 626c  hema, table=tabl
-0000e9f0: 652c 2063 6f6c 756d 6e3d 636f 6c75 6d6e  e, column=column
-0000ea00: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000ea10: 2073 656c 660a 0a20 2020 2064 6566 2069   self..    def i
-0000ea20: 6e64 6578 6573 2873 656c 662c 2073 6368  ndexes(self, sch
-0000ea30: 656d 613d 2225 222c 2074 6162 6c65 3d22  ema="%", table="
-0000ea40: 2522 293a 0a20 2020 2020 2020 2022 2222  %"):.        """
-0000ea50: 4765 7420 7468 6520 6461 7461 6261 7365  Get the database
-0000ea60: 2069 6e64 6578 6573 2222 220a 2020 2020   indexes""".    
-0000ea70: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
-0000ea80: 7361 626c 653d 6e6f 2d6d 656d 6265 720a  sable=no-member.
-0000ea90: 2020 2020 2020 2020 7365 6c66 2e5f 6d65          self._me
-0000eaa0: 7461 6461 7461 5f72 6571 2870 726f 746f  tadata_req(proto
-0000eab0: 2e46 6574 6368 5379 7374 656d 4d65 7461  .FetchSystemMeta
-0000eac0: 6461 7461 2e47 4554 5f49 4e44 4558 4553  data.GET_INDEXES
-0000ead0: 2c20 7363 6865 6d61 3d73 6368 656d 612c  , schema=schema,
-0000eae0: 2074 6162 6c65 3d74 6162 6c65 290a 2020   table=table).  
-0000eaf0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000eb00: 660a 0a20 2020 2064 6566 2067 6574 5479  f..    def getTy
-0000eb10: 7065 496e 666f 2873 656c 6629 3a20 2023  peInfo(self):  #
-0000eb20: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
-0000eb30: 3d69 6e76 616c 6964 2d6e 616d 650a 2020  =invalid-name.  
-0000eb40: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
-0000eb50: 2064 6174 6162 6173 6520 7479 7065 2069   database type i
-0000eb60: 6e66 6f22 2222 0a20 2020 2020 2020 2023  nfo""".        #
-0000eb70: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
-0000eb80: 3d6e 6f2d 6d65 6d62 6572 0a20 2020 2020  =no-member.     
-0000eb90: 2020 2073 656c 662e 5f6d 6574 6164 6174     self._metadat
-0000eba0: 615f 7265 7128 7072 6f74 6f2e 4665 7463  a_req(proto.Fetc
-0000ebb0: 6853 7973 7465 6d4d 6574 6164 6174 612e  hSystemMetadata.
-0000ebc0: 4745 545f 5459 5045 5f49 4e46 4f29 0a20  GET_TYPE_INFO). 
-0000ebd0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000ebe0: 6c66 0a0a 2020 2020 6465 6620 6765 7453  lf..    def getS
-0000ebf0: 7973 7465 6d56 6572 7369 6f6e 2873 656c  ystemVersion(sel
-0000ec00: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-0000ec10: 726e 2073 656c 662e 5f65 7865 6375 7465  rn self._execute
-0000ec20: 5f73 7973 7465 6d6d 6574 6164 6174 6128  _systemmetadata(
-0000ec30: 7072 6f74 6f2e 4665 7463 6853 7973 7465  proto.FetchSyste
-0000ec40: 6d4d 6574 6164 6174 612e 4745 545f 4441  mMetadata.GET_DA
-0000ec50: 5441 4241 5345 5f50 524f 4455 4354 5f56  TABASE_PRODUCT_V
-0000ec60: 4552 5349 4f4e 290a 0a20 2020 2064 6566  ERSION)..    def
-0000ec70: 205f 6d65 7461 6461 7461 5f72 6571 2873   _metadata_req(s
-0000ec80: 656c 662c 2072 6571 7479 7065 2c20 7363  elf, reqtype, sc
-0000ec90: 6865 6d61 3d22 2522 2c20 7461 626c 653d  hema="%", table=
-0000eca0: 2225 222c 2063 6f6c 756d 6e3d 2225 222c  "%", column="%",
-0000ecb0: 2076 6965 773d 2225 2229 3a0a 2020 2020   view="%"):.    
-0000ecc0: 2020 2020 2222 2249 6e74 6572 6e61 6c20      """Internal 
-0000ecd0: 6675 6e63 7469 6f6e 2074 6f20 6765 7420  function to get 
-0000ece0: 6461 7461 6261 7365 206d 6574 6164 6174  database metadat
-0000ecf0: 6122 2222 0a20 2020 2020 2020 2023 2070  a""".        # p
-0000ed00: 796c 696e 743a 2064 6973 6162 6c65 3d6e  ylint: disable=n
-0000ed10: 6f2d 6d65 6d62 6572 2c74 6f6f 2d6d 616e  o-member,too-man
-0000ed20: 792d 6172 6775 6d65 6e74 730a 2020 2020  y-arguments.    
-0000ed30: 2020 2020 7365 6c66 2e5f 7265 696e 6974      self._reinit
-0000ed40: 6961 6c69 7a65 2829 0a20 2020 2020 2020  ialize().       
-0000ed50: 2023 2072 6571 2e66 6574 6368 5f73 7973   # req.fetch_sys
-0000ed60: 7465 6d5f 6d65 7461 6461 7461 2e47 4554  tem_metadata.GET
-0000ed70: 5f54 4142 4c45 530a 2020 2020 2020 2020  _TABLES.        
-0000ed80: 7265 7120 3d20 7072 6f74 6f2e 5265 7175  req = proto.Requ
-0000ed90: 6573 7428 290a 2020 2020 2020 2020 7265  est().        re
-0000eda0: 712e 7479 7065 203d 2072 6571 2e46 4554  q.type = req.FET
-0000edb0: 4348 5f53 5953 5445 4d5f 4d45 5441 4441  CH_SYSTEM_METADA
-0000edc0: 5441 0a20 2020 2020 2020 2072 6571 2e66  TA.        req.f
-0000edd0: 6574 6368 5f73 7973 7465 6d5f 6d65 7461  etch_system_meta
-0000ede0: 6461 7461 2e63 616c 6c20 3d20 7265 7174  data.call = reqt
-0000edf0: 7970 650a 2020 2020 2020 2020 7265 712e  ype.        req.
-0000ee00: 6665 7463 685f 7379 7374 656d 5f6d 6574  fetch_system_met
-0000ee10: 6164 6174 612e 7363 6865 6d61 203d 2073  adata.schema = s
-0000ee20: 6368 656d 610a 2020 2020 2020 2020 7265  chema.        re
-0000ee30: 712e 6665 7463 685f 7379 7374 656d 5f6d  q.fetch_system_m
-0000ee40: 6574 6164 6174 612e 7461 626c 6520 3d20  etadata.table = 
-0000ee50: 7461 626c 650a 2020 2020 2020 2020 7265  table.        re
-0000ee60: 712e 6665 7463 685f 7379 7374 656d 5f6d  q.fetch_system_m
-0000ee70: 6574 6164 6174 612e 636f 6c75 6d6e 203d  etadata.column =
-0000ee80: 2063 6f6c 756d 6e0a 2020 2020 2020 2020   column.        
-0000ee90: 7265 712e 6665 7463 685f 7379 7374 656d  req.fetch_system
-0000eea0: 5f6d 6574 6164 6174 612e 7669 6577 203d  _metadata.view =
-0000eeb0: 2076 6965 770a 2020 2020 2020 2020 7265   view.        re
-0000eec0: 712e 6665 7463 685f 7379 7374 656d 5f6d  q.fetch_system_m
-0000eed0: 6574 6164 6174 612e 7465 7374 203d 2054  etadata.test = T
-0000eee0: 7275 650a 0a20 2020 2020 2020 205f 7365  rue..        _se
-0000eef0: 6e64 5f6d 7367 2873 656c 662e 636f 6e6e  nd_msg(self.conn
-0000ef00: 6563 7469 6f6e 2c20 7265 7129 0a0a 2020  ection, req)..  
-0000ef10: 2020 2020 2020 7273 7020 3d20 5f72 6563        rsp = _rec
-0000ef20: 765f 6d73 6728 7365 6c66 2e63 6f6e 6e65  v_msg(self.conne
-0000ef30: 6374 696f 6e2c 2070 726f 746f 2e46 6574  ction, proto.Fet
-0000ef40: 6368 5379 7374 656d 4d65 7461 6461 7461  chSystemMetadata
-0000ef50: 5265 7370 6f6e 7365 2829 290a 0a20 2020  Response())..   
-0000ef60: 2020 2020 2069 6620 7273 702e 7265 7370       if rsp.resp
-0000ef70: 6f6e 7365 2e74 7970 6520 3d3d 2070 726f  onse.type == pro
-0000ef80: 746f 2e43 6f6e 6669 726d 6174 696f 6e52  to.ConfirmationR
-0000ef90: 6573 706f 6e73 652e 5245 5350 4f4e 5345  esponse.RESPONSE
-0000efa0: 5f45 5252 4f52 3a0a 2020 2020 2020 2020  _ERROR:.        
-0000efb0: 2020 2020 6966 2072 7370 2e72 6573 706f      if rsp.respo
-0000efc0: 6e73 652e 7665 6e64 6f72 5f63 6f64 6520  nse.vendor_code 
-0000efd0: 3d3d 2053 4553 5349 4f4e 5f45 5850 4952  == SESSION_EXPIR
-0000efe0: 4544 5f43 4f44 453a 0a20 2020 2020 2020  ED_CODE:.       
-0000eff0: 2020 2020 2020 2020 2023 204e 6565 6420           # Need 
-0000f000: 746f 2072 6566 7265 7368 2074 6865 2073  to refresh the s
-0000f010: 6573 7369 6f6e 0a20 2020 2020 2020 2020  ession.         
-0000f020: 2020 2020 2020 2073 656c 662e 636f 6e6e         self.conn
-0000f030: 6563 7469 6f6e 2e72 6566 7265 7368 2829  ection.refresh()
-0000f040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f050: 2023 2061 6e64 2074 7279 2061 6761 696e   # and try again
-0000f060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f070: 205f 6d65 7461 6461 7461 5f72 6571 2872   _metadata_req(r
-0000f080: 6571 7479 7065 2c20 7363 6865 6d61 3d73  eqtype, schema=s
-0000f090: 6368 656d 612c 2074 6162 6c65 3d74 6162  chema, table=tab
-0000f0a0: 6c65 2c20 636f 6c75 6d6e 3d63 6f6c 756d  le, column=colum
-0000f0b0: 6e2c 2076 6965 773d 7669 6577 290a 2020  n, view=view).  
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000f0d0: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-0000f0e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000f0f0: 2020 2020 2020 2072 6169 7365 205f 636f         raise _co
-0000f100: 6e76 6572 745f 6578 6365 7074 696f 6e28  nvert_exception(
-0000f110: 7273 702e 7265 7370 6f6e 7365 290a 0a20  rsp.response).. 
-0000f120: 2020 2020 2020 2073 656c 662e 5f67 6574         self._get
-0000f130: 5f72 6573 756c 745f 6d65 7461 6461 7461  _result_metadata
-0000f140: 2829 0a0a 2020 2020 2020 2020 7365 6c66  ()..        self
-0000f150: 2e72 6f77 6e75 6d62 6572 203d 2030 0a20  .rownumber = 0. 
-0000f160: 2020 2020 2020 2066 6f72 2062 6c6f 6220         for blob 
-0000f170: 696e 2072 7370 2e72 6573 756c 745f 7365  in rsp.result_se
-0000f180: 745f 7661 6c2e 626c 6f62 733a 0a20 2020  t_val.blobs:.   
-0000f190: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0000f1a0: 7365 6c66 2e5f 6275 6666 6572 733a 0a20  self._buffers:. 
-0000f1b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f1c0: 656c 662e 5f6f 6666 7365 7420 3d20 300a  elf._offset = 0.
-0000f1d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f1e0: 2e5f 6275 6666 6572 732e 6170 7065 6e64  ._buffers.append
-0000f1f0: 2862 6c6f 6229 0a0a 2020 2020 6465 6620  (blob)..    def 
-0000f200: 5f65 7865 6375 7465 5f71 7565 7279 2873  _execute_query(s
-0000f210: 656c 662c 206f 7065 7261 7469 6f6e 2c20  elf, operation, 
-0000f220: 7175 6572 795f 7479 7065 3a20 7374 7220  query_type: str 
-0000f230: 3d20 2253 454c 4543 5422 293a 0a20 2020  = "SELECT"):.   
-0000f240: 2020 2020 2022 2222 4578 6563 7574 6520       """Execute 
-0000f250: 6120 7175 6572 7922 2222 0a20 2020 2020  a query""".     
-0000f260: 2020 2023 2070 796c 696e 743a 2064 6973     # pylint: dis
-0000f270: 6162 6c65 3d6e 6f2d 6d65 6d62 6572 0a0a  able=no-member..
-0000f280: 2020 2020 2020 2020 6661 6374 6f72 7920          factory 
-0000f290: 3d20 5f4f 4349 454e 545f 5245 5155 4553  = _OCIENT_REQUES
-0000f2a0: 545f 4641 4354 4f52 4945 532e 6765 7428  T_FACTORIES.get(
-0000f2b0: 7175 6572 795f 7479 7065 2e75 7070 6572  query_type.upper
-0000f2c0: 2829 2c20 4e6f 6e65 290a 0a20 2020 2020  (), None)..     
-0000f2d0: 2020 2069 6620 6661 6374 6f72 7920 6973     if factory is
-0000f2e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000f2f0: 2020 2072 6169 7365 204e 6f74 5375 7070     raise NotSupp
-0000f300: 6f72 7465 6445 7272 6f72 2866 2251 7565  ortedError(f"Que
-0000f310: 7279 2074 7970 6520 277b 7175 6572 795f  ry type '{query_
-0000f320: 7479 7065 7d27 206e 6f74 2073 7570 706f  type}' not suppo
-0000f330: 7274 6564 2062 7920 7079 6f63 6965 6e74  rted by pyocient
-0000f340: 2722 290a 0a20 2020 2020 2020 2023 2067  '")..        # g
-0000f350: 656e 6572 6174 6520 7468 6520 6170 7072  enerate the appr
-0000f360: 6f70 7269 6174 6520 7265 7175 6573 740a  opriate request.
-0000f370: 2020 2020 2020 2020 7265 7120 3d20 6661          req = fa
-0000f380: 6374 6f72 792e 7265 7175 6573 7428 6f70  ctory.request(op
-0000f390: 6572 6174 696f 6e29 0a0a 2020 2020 2020  eration)..      
-0000f3a0: 2020 2320 4c6f 6f70 2077 6869 6c65 2077    # Loop while w
-0000f3b0: 6520 7265 7472 7920 7265 6469 7265 6374  e retry redirect
-0000f3c0: 7320 616e 6420 7265 636f 6e6e 6563 7473  s and reconnects
-0000f3d0: 0a20 2020 2020 2020 2077 6869 6c65 2054  .        while T
-0000f3e0: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
-0000f3f0: 2069 6620 7265 712e 7479 7065 203d 3d20   if req.type == 
-0000f400: 7072 6f74 6f2e 5265 7175 6573 742e 5265  proto.Request.Re
-0000f410: 7175 6573 7454 7970 652e 5661 6c75 6528  questType.Value(
-0000f420: 2245 5845 4355 5445 5f51 5545 5259 2229  "EXECUTE_QUERY")
-0000f430: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f440: 2020 7265 712e 6578 6563 7574 655f 7175    req.execute_qu
-0000f450: 6572 792e 666f 7263 6520 3d20 7365 6c66  ery.force = self
-0000f460: 2e63 6f6e 6e65 6374 696f 6e2e 666f 7263  .connection.forc
-0000f470: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000f480: 2020 7265 712e 6578 6563 7574 655f 7175    req.execute_qu
-0000f490: 6572 792e 666f 7263 6552 6564 6972 6563  ery.forceRedirec
-0000f4a0: 7420 3d20 7365 6c66 2e63 6f6e 6e65 6374  t = self.connect
-0000f4b0: 696f 6e2e 666f 7263 655f 6e65 7874 5f72  ion.force_next_r
-0000f4c0: 6564 6972 6563 740a 2020 2020 2020 2020  edirect.        
-0000f4d0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-0000f4e0: 6e65 6374 696f 6e2e 666f 7263 655f 6e65  nection.force_ne
-0000f4f0: 7874 5f72 6564 6972 6563 7420 3d20 4661  xt_redirect = Fa
-0000f500: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-0000f510: 656c 6966 2072 6571 2e74 7970 6520 3d3d  elif req.type ==
-0000f520: 2070 726f 746f 2e52 6571 7565 7374 2e52   proto.Request.R
-0000f530: 6571 7565 7374 5479 7065 2e56 616c 7565  equestType.Value
-0000f540: 2822 4558 4543 5554 455f 4558 504c 4149  ("EXECUTE_EXPLAI
-0000f550: 4e22 293a 0a20 2020 2020 2020 2020 2020  N"):.           
-0000f560: 2020 2020 2072 6571 2e65 7865 6375 7465       req.execute
-0000f570: 5f65 7870 6c61 696e 2e66 6f72 6365 203d  _explain.force =
-0000f580: 2073 656c 662e 636f 6e6e 6563 7469 6f6e   self.connection
-0000f590: 2e66 6f72 6365 0a20 2020 2020 2020 2020  .force.         
-0000f5a0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000f5b0: 2020 2020 2020 2020 5f73 656e 645f 6d73          _send_ms
-0000f5c0: 6728 7365 6c66 2e63 6f6e 6e65 6374 696f  g(self.connectio
-0000f5d0: 6e2c 2072 6571 290a 0a20 2020 2020 2020  n, req)..       
-0000f5e0: 2020 2020 2020 2020 2072 7370 203d 205f           rsp = _
-0000f5f0: 7265 6376 5f6d 7367 2873 656c 662e 636f  recv_msg(self.co
-0000f600: 6e6e 6563 7469 6f6e 2c20 6661 6374 6f72  nnection, factor
-0000f610: 792e 7265 7370 6f6e 7365 2829 290a 2020  y.response()).  
-0000f620: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0000f630: 2049 4f45 7272 6f72 3a0a 2020 2020 2020   IOError:.      
-0000f640: 2020 2020 2020 2020 2020 2320 7265 6d61            # rema
-0000f650: 6b65 206f 7572 2063 6f6e 6e65 6374 696f  ke our connectio
-0000f660: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-0000f670: 2020 7365 6c66 2e63 6f6e 6e65 6374 696f    self.connectio
-0000f680: 6e20 3d20 436f 6e6e 6563 7469 6f6e 280a  n = Connection(.
-0000f690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6a0: 2020 2020 7573 6572 3d73 656c 662e 636f      user=self.co
-0000f6b0: 6e6e 6563 7469 6f6e 2e75 7365 722c 0a20  nnection.user,. 
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6d0: 2020 2070 6173 7377 6f72 643d 7365 6c66     password=self
-0000f6e0: 2e63 6f6e 6e65 6374 696f 6e2e 7061 7373  .connection.pass
-0000f6f0: 776f 7264 2c0a 2020 2020 2020 2020 2020  word,.          
-0000f700: 2020 2020 2020 2020 2020 686f 7374 3d66            host=f
-0000f710: 227b 272c 272e 6a6f 696e 2873 656c 662e  "{','.join(self.
-0000f720: 636f 6e6e 6563 7469 6f6e 2e68 6f73 7473  connection.hosts
-0000f730: 297d 3a7b 7365 6c66 2e63 6f6e 6e65 6374  )}:{self.connect
-0000f740: 696f 6e2e 706f 7274 7d22 2c0a 2020 2020  ion.port}",.    
-0000f750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f760: 6461 7461 6261 7365 3d73 656c 662e 636f  database=self.co
-0000f770: 6e6e 6563 7469 6f6e 2e64 6174 6162 6173  nnection.databas
-0000f780: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000f790: 2020 2020 2020 2074 6c73 3d73 656c 662e         tls=self.
-0000f7a0: 636f 6e6e 6563 7469 6f6e 2e74 6c73 2c0a  connection.tls,.
-0000f7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7c0: 2020 2020 6861 6e64 7368 616b 653d 7365      handshake=se
-0000f7d0: 6c66 2e63 6f6e 6e65 6374 696f 6e2e 6861  lf.connection.ha
-0000f7e0: 6e64 7368 616b 652c 0a20 2020 2020 2020  ndshake,.       
-0000f7f0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000f800: 6365 3d73 656c 662e 636f 6e6e 6563 7469  ce=self.connecti
-0000f810: 6f6e 2e66 6f72 6365 2c0a 2020 2020 2020  on.force,.      
-0000f820: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f830: 7373 696f 6e3d 7365 6c66 2e63 6f6e 6e65  ssion=self.conne
-0000f840: 6374 696f 6e2e 7365 7373 696f 6e2c 0a20  ction.session,. 
-0000f850: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000f860: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f870: 2020 636f 6e74 696e 7565 0a0a 2020 2020    continue..    
-0000f880: 2020 2020 2020 2020 6966 2072 7370 2e72          if rsp.r
-0000f890: 6573 706f 6e73 652e 7479 7065 203d 3d20  esponse.type == 
-0000f8a0: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
-0000f8b0: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
-0000f8c0: 4e53 455f 5741 524e 3a0a 2020 2020 2020  NSE_WARN:.      
-0000f8d0: 2020 2020 2020 2020 2020 7761 726e 2872            warn(r
-0000f8e0: 7370 2e72 6573 706f 6e73 652e 7265 6173  sp.response.reas
-0000f8f0: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
-0000f900: 656c 6966 206e 6f74 2072 7370 2e72 6573  elif not rsp.res
-0000f910: 706f 6e73 652e 7479 7065 203d 3d20 7072  ponse.type == pr
-0000f920: 6f74 6f2e 436f 6e66 6972 6d61 7469 6f6e  oto.Confirmation
-0000f930: 5265 7370 6f6e 7365 2e52 4553 504f 4e53  Response.RESPONS
-0000f940: 455f 4f4b 3a0a 2020 2020 2020 2020 2020  E_OK:.          
-0000f950: 2020 2020 2020 6966 2072 7370 2e72 6573        if rsp.res
-0000f960: 706f 6e73 652e 7665 6e64 6f72 5f63 6f64  ponse.vendor_cod
-0000f970: 6520 3d3d 2053 4553 5349 4f4e 5f45 5850  e == SESSION_EXP
-0000f980: 4952 4544 5f43 4f44 453a 0a20 2020 2020  IRED_CODE:.     
-0000f990: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000f9a0: 204e 6565 6420 746f 2072 6566 7265 7368   Need to refresh
-0000f9b0: 2074 6865 2073 6573 7369 6f6e 0a20 2020   the session.   
-0000f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9d0: 2073 656c 662e 636f 6e6e 6563 7469 6f6e   self.connection
-0000f9e0: 2e72 6566 7265 7368 2829 0a20 2020 2020  .refresh().     
-0000f9f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000fa00: 2061 6e64 2074 7279 2061 6761 696e 0a20   and try again. 
-0000fa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa20: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-0000fa30: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000fa40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000fa50: 2020 2020 2020 7261 6973 6520 5f63 6f6e        raise _con
-0000fa60: 7665 7274 5f65 7863 6570 7469 6f6e 2872  vert_exception(r
-0000fa70: 7370 2e72 6573 706f 6e73 6529 0a0a 2020  sp.response)..  
-0000fa80: 2020 2020 2020 2020 2020 2320 7365 6520            # see 
-0000fa90: 6966 2077 6520 6172 6520 6265 696e 6720  if we are being 
-0000faa0: 746f 6c64 2074 6f20 7265 6469 7265 6374  told to redirect
-0000fab0: 0a20 2020 2020 2020 2020 2020 2072 6564  .            red
-0000fac0: 6972 6563 7420 3d20 6765 7461 7474 7228  irect = getattr(
-0000fad0: 7273 702c 2022 7265 6469 7265 6374 222c  rsp, "redirect",
-0000fae0: 2046 616c 7365 290a 2020 2020 2020 2020   False).        
-0000faf0: 2020 2020 6966 206e 6f74 2072 6564 6972      if not redir
-0000fb00: 6563 743a 0a20 2020 2020 2020 2020 2020  ect:.           
-0000fb10: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
-0000fb20: 2020 2020 2020 2020 2320 7265 6d61 6b65          # remake
-0000fb30: 206f 7572 2063 6f6e 6e65 6374 696f 6e0a   our connection.
-0000fb40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fb50: 2e63 6f6e 6e65 6374 696f 6e2e 636c 6f73  .connection.clos
-0000fb60: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0000fb70: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e20  self.connection 
-0000fb80: 3d20 7365 6c66 2e63 6f6e 6e65 6374 696f  = self.connectio
-0000fb90: 6e2e 7265 6469 7265 6374 2872 7370 2e72  n.redirect(rsp.r
-0000fba0: 6564 6972 6563 7448 6f73 742c 2072 7370  edirectHost, rsp
-0000fbb0: 2e72 6564 6972 6563 7450 6f72 7429 0a0a  .redirectPort)..
-0000fbc0: 2020 2020 2020 2020 7175 6572 795f 6964          query_id
-0000fbd0: 203d 2067 6574 6174 7472 2872 7370 2c20   = getattr(rsp, 
-0000fbe0: 2271 7565 7279 4964 222c 204e 6f6e 6529  "queryId", None)
-0000fbf0: 0a20 2020 2020 2020 2069 6620 7175 6572  .        if quer
-0000fc00: 795f 6964 2069 7320 6e6f 7420 4e6f 6e65  y_id is not None
-0000fc10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000fc20: 6c66 2e71 7565 7279 5f69 6420 3d20 7175  lf.query_id = qu
-0000fc30: 6572 795f 6964 0a0a 2020 2020 2020 2020  ery_id..        
-0000fc40: 7365 6c66 2e72 6f77 6e75 6d62 6572 203d  self.rownumber =
-0000fc50: 2030 0a0a 2020 2020 2020 2020 6966 2071   0..        if q
-0000fc60: 7565 7279 5f74 7970 6520 696e 205b 2253  uery_type in ["S
-0000fc70: 454c 4543 5422 2c20 2257 4954 4822 5d3a  ELECT", "WITH"]:
-0000fc80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000fc90: 662e 5f67 6574 5f72 6573 756c 745f 6d65  f._get_result_me
-0000fca0: 7461 6461 7461 2829 0a0a 2020 2020 2020  tadata()..      
-0000fcb0: 2020 656c 6966 2071 7565 7279 5f74 7970    elif query_typ
-0000fcc0: 6520 3d3d 2022 4558 504c 4149 4e22 3a0a  e == "EXPLAIN":.
-0000fcd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fce0: 2e64 6573 6372 6970 7469 6f6e 203d 205b  .description = [
-0000fcf0: 2822 6578 706c 6169 6e22 2c20 5479 7065  ("explain", Type
-0000fd00: 436f 6465 732e 4348 4152 2c20 4e6f 6e65  Codes.CHAR, None
-0000fd10: 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f  , None, None, No
-0000fd20: 6e65 2c20 4e6f 6e65 295d 2020 2320 6469  ne, None)]  # di
-0000fd30: 7370 6c61 795f 7369 7a65 2020 2320 696e  splay_size  # in
-0000fd40: 7465 726e 616c 5f73 697a 6520 2023 2070  ternal_size  # p
-0000fd50: 7265 6369 7369 6f6e 2020 2320 7363 616c  recision  # scal
-0000fd60: 6520 2023 206e 756c 6c5f 6f6b 0a0a 2020  e  # null_ok..  
-0000fd70: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-0000fd80: 7870 6c61 696e 5f72 6573 756c 7420 3d20  xplain_result = 
-0000fd90: 7273 702e 706c 616e 0a0a 2020 2020 2320  rsp.plan..    # 
-0000fda0: 4166 7465 7220 6c69 7374 2061 6c6c 2071  After list all q
-0000fdb0: 7565 7269 6573 2061 6e64 206c 6973 7420  ueries and list 
-0000fdc0: 616c 6c20 636f 6d70 6c65 7465 6420 7175  all completed qu
-0000fdd0: 6572 6965 7320 6861 7665 2062 6565 6e20  eries have been 
-0000fde0: 7265 6d61 7070 6564 2c20 7468 6973 2069  remapped, this i
-0000fdf0: 7320 6e6f 206c 6f6e 6765 7220 7573 6564  s no longer used
-0000fe00: 2e20 4275 7420 6974 2063 616e 2062 6520  . But it can be 
-0000fe10: 7573 6564 2066 6f72 206f 7468 6572 2074  used for other t
-0000fe20: 6869 6e67 732e 0a20 2020 2023 2045 783a  hings..    # Ex:
-0000fe30: 206c 6973 7420 7461 626c 6573 2c20 6c69   list tables, li
-0000fe40: 7374 2076 6965 7773 2c20 6c69 7374 2074  st views, list t
-0000fe50: 6162 6c65 2070 7269 7669 6c65 6765 732e  able privileges.
-0000fe60: 204e 6f6e 6520 6f66 2074 6865 7365 2061   None of these a
-0000fe70: 7265 2069 6d70 6c65 6d65 6e74 6564 2079  re implemented y
-0000fe80: 6574 2e0a 2020 2020 6465 6620 5f65 7865  et..    def _exe
-0000fe90: 6375 7465 5f6c 6973 7428 7365 6c66 2c20  cute_list(self, 
-0000fea0: 6f70 6572 6174 696f 6e3a 2073 7472 203d  operation: str =
-0000feb0: 2022 4c49 5354 2041 4c4c 2051 5545 5249   "LIST ALL QUERI
-0000fec0: 4553 2229 3a0a 2020 2020 2020 2020 2222  ES"):.        ""
-0000fed0: 2245 7865 6375 7465 204c 4953 545f 414c  "Execute LIST_AL
-0000fee0: 4c5f 5155 4552 4945 5322 2222 0a20 2020  L_QUERIES""".   
-0000fef0: 2020 2020 2023 2070 796c 696e 743a 2064       # pylint: d
-0000ff00: 6973 6162 6c65 3d6e 6f2d 6d65 6d62 6572  isable=no-member
-0000ff10: 0a0a 2020 2020 2020 2020 6661 6374 6f72  ..        factor
-0000ff20: 7920 3d20 5f4f 4349 454e 545f 5245 5155  y = _OCIENT_REQU
-0000ff30: 4553 545f 4641 4354 4f52 4945 532e 6765  EST_FACTORIES.ge
-0000ff40: 7428 6f70 6572 6174 696f 6e2e 7570 7065  t(operation.uppe
-0000ff50: 7228 292c 204e 6f6e 6529 0a0a 2020 2020  r(), None)..    
-0000ff60: 2020 2020 6966 2066 6163 746f 7279 2069      if factory i
-0000ff70: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000ff80: 2020 2020 7261 6973 6520 4e6f 7453 7570      raise NotSup
-0000ff90: 706f 7274 6564 4572 726f 7228 6622 4c69  portedError(f"Li
-0000ffa0: 7374 2071 7565 7279 2027 7b6f 7065 7261  st query '{opera
-0000ffb0: 7469 6f6e 7d27 206e 6f74 2073 7570 706f  tion}' not suppo
-0000ffc0: 7274 6564 2062 7920 7079 6f63 6965 6e74  rted by pyocient
-0000ffd0: 2722 290a 0a20 2020 2020 2020 2023 2067  '")..        # g
-0000ffe0: 6565 7261 7465 2074 6865 2061 7070 726f  eerate the appro
-0000fff0: 7072 6961 7465 2072 6571 7565 7374 0a20  priate request. 
-00010000: 2020 2020 2020 2072 6571 203d 2066 6163         req = fac
-00010010: 746f 7279 2e72 6571 7565 7374 286f 7065  tory.request(ope
-00010020: 7261 7469 6f6e 290a 0a20 2020 2020 2020  ration)..       
-00010030: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
-00010040: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00010050: 2020 2020 2020 2020 2020 2020 2020 5f73                _s
-00010060: 656e 645f 6d73 6728 7365 6c66 2e63 6f6e  end_msg(self.con
-00010070: 6e65 6374 696f 6e2c 2072 6571 290a 0a20  nection, req).. 
-00010080: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00010090: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
-000100a0: 656c 662e 636f 6e6e 6563 7469 6f6e 2c20  elf.connection, 
-000100b0: 6661 6374 6f72 792e 7265 7370 6f6e 7365  factory.response
-000100c0: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-000100d0: 6578 6365 7074 2049 4f45 7272 6f72 3a0a  except IOError:.
-000100e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100f0: 2320 7265 6d61 6b65 206f 7572 2063 6f6e  # remake our con
-00010100: 6e65 6374 696f 6e0a 2020 2020 2020 2020  nection.        
-00010110: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00010120: 6e65 6374 696f 6e20 3d20 436f 6e6e 6563  nection = Connec
-00010130: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-00010140: 2020 2020 2020 2020 2020 7573 6572 3d73            user=s
-00010150: 656c 662e 636f 6e6e 6563 7469 6f6e 2e75  elf.connection.u
-00010160: 7365 722c 0a20 2020 2020 2020 2020 2020  ser,.           
-00010170: 2020 2020 2020 2020 2070 6173 7377 6f72           passwor
-00010180: 643d 7365 6c66 2e63 6f6e 6e65 6374 696f  d=self.connectio
-00010190: 6e2e 7061 7373 776f 7264 2c0a 2020 2020  n.password,.    
-000101a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101b0: 686f 7374 3d66 227b 272c 272e 6a6f 696e  host=f"{','.join
-000101c0: 2873 656c 662e 636f 6e6e 6563 7469 6f6e  (self.connection
-000101d0: 2e68 6f73 7473 297d 3a7b 7365 6c66 2e63  .hosts)}:{self.c
-000101e0: 6f6e 6e65 6374 696f 6e2e 706f 7274 7d22  onnection.port}"
-000101f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010200: 2020 2020 2020 6461 7461 6261 7365 3d73        database=s
-00010210: 656c 662e 636f 6e6e 6563 7469 6f6e 2e64  elf.connection.d
-00010220: 6174 6162 6173 652c 0a20 2020 2020 2020  atabase,.       
-00010230: 2020 2020 2020 2020 2020 2020 2074 6c73               tls
-00010240: 3d73 656c 662e 636f 6e6e 6563 7469 6f6e  =self.connection
-00010250: 2e74 6c73 2c0a 2020 2020 2020 2020 2020  .tls,.          
-00010260: 2020 2020 2020 2020 2020 6861 6e64 7368            handsh
-00010270: 616b 653d 7365 6c66 2e63 6f6e 6e65 6374  ake=self.connect
-00010280: 696f 6e2e 6861 6e64 7368 616b 652c 0a20  ion.handshake,. 
-00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102a0: 2020 2066 6f72 6365 3d73 656c 662e 636f     force=self.co
-000102b0: 6e6e 6563 7469 6f6e 2e66 6f72 6365 2c0a  nnection.force,.
-000102c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102d0: 2020 2020 7365 7373 696f 6e3d 7365 6c66      session=self
-000102e0: 2e63 6f6e 6e65 6374 696f 6e2e 7365 7373  .connection.sess
-000102f0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00010300: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00010310: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00010320: 0a20 2020 2020 2020 2020 2020 2062 7265  .            bre
-00010330: 616b 0a0a 2020 2020 2020 2020 6966 2072  ak..        if r
-00010340: 7370 2e72 6573 706f 6e73 652e 7479 7065  sp.response.type
-00010350: 203d 3d20 7072 6f74 6f2e 436f 6e66 6972   == proto.Confir
-00010360: 6d61 7469 6f6e 5265 7370 6f6e 7365 2e52  mationResponse.R
-00010370: 4553 504f 4e53 455f 5741 524e 3a0a 2020  ESPONSE_WARN:.  
-00010380: 2020 2020 2020 2020 2020 7761 726e 2872            warn(r
-00010390: 7370 2e72 6573 706f 6e73 652e 7265 6173  sp.response.reas
-000103a0: 6f6e 290a 2020 2020 2020 2020 656c 6966  on).        elif
-000103b0: 206e 6f74 2072 7370 2e72 6573 706f 6e73   not rsp.respons
-000103c0: 652e 7479 7065 203d 3d20 7072 6f74 6f2e  e.type == proto.
-000103d0: 436f 6e66 6972 6d61 7469 6f6e 5265 7370  ConfirmationResp
-000103e0: 6f6e 7365 2e52 4553 504f 4e53 455f 4f4b  onse.RESPONSE_OK
-000103f0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00010400: 2072 7370 2e72 6573 706f 6e73 652e 7665   rsp.response.ve
-00010410: 6e64 6f72 5f63 6f64 6520 3d3d 2053 4553  ndor_code == SES
-00010420: 5349 4f4e 5f45 5850 4952 4544 5f43 4f44  SION_EXPIRED_COD
-00010430: 453a 0a20 2020 2020 2020 2020 2020 2020  E:.             
-00010440: 2020 2023 204e 6565 6420 746f 2072 6566     # Need to ref
-00010450: 7265 7368 2074 6865 2073 6573 7369 6f6e  resh the session
-00010460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010470: 2073 656c 662e 636f 6e6e 6563 7469 6f6e   self.connection
-00010480: 2e72 6566 7265 7368 2829 0a20 2020 2020  .refresh().     
-00010490: 2020 2020 2020 2020 2020 2023 2061 6e64             # and
-000104a0: 2074 7279 2061 6761 696e 0a20 2020 2020   try again.     
-000104b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000104c0: 5f65 7865 6375 7465 5f6c 6973 7428 6f70  _execute_list(op
-000104d0: 6572 6174 696f 6e3d 6f70 6572 6174 696f  eration=operatio
-000104e0: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-000104f0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00010500: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00010510: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00010520: 6520 5f63 6f6e 7665 7274 5f65 7863 6570  e _convert_excep
-00010530: 7469 6f6e 2872 7370 2e72 6573 706f 6e73  tion(rsp.respons
-00010540: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
-00010550: 2e64 6573 6372 6970 7469 6f6e 203d 205b  .description = [
-00010560: 5d0a 0a20 2020 2020 2020 2072 6f77 7320  ]..        rows 
-00010570: 3d20 6661 6374 6f72 792e 7072 6f63 6573  = factory.proces
-00010580: 7328 7273 7029 0a20 2020 2020 2020 2069  s(rsp).        i
-00010590: 6620 6e6f 7420 726f 7773 3a0a 2020 2020  f not rows:.    
-000105a0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000105b0: 745f 7265 7375 6c74 203d 205b 5d0a 2020  t_result = [].  
-000105c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000105d0: 0a0a 2020 2020 2020 2020 2320 4372 6561  ..        # Crea
-000105e0: 7465 2074 6865 2063 6f6c 756d 6e20 6465  te the column de
-000105f0: 7363 7269 7074 696f 6e73 0a20 2020 2020  scriptions.     
-00010600: 2020 2072 6f77 203d 2072 6f77 735b 305d     row = rows[0]
-00010610: 0a20 2020 2020 2020 2066 6f72 2066 6965  .        for fie
-00010620: 6c64 2069 6e20 726f 772e 5f66 6965 6c64  ld in row._field
-00010630: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00010640: 656c 662e 6465 7363 7269 7074 696f 6e2e  elf.description.
-00010650: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
-00010660: 2020 2020 2020 2020 2866 6965 6c64 2c20          (field, 
-00010670: 5479 7065 436f 6465 732e 636c 735f 746f  TypeCodes.cls_to
-00010680: 5f74 7970 6528 726f 772e 5f66 6965 6c64  _type(row._field
-00010690: 5f74 7970 6573 5b66 6965 6c64 5d29 2c20  _types[field]), 
-000106a0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
-000106b0: 2c20 4e6f 6e65 2c20 4e6f 6e65 2920 2023  , None, None)  #
-000106c0: 2064 6973 706c 6179 5f73 697a 6520 2023   display_size  #
-000106d0: 2069 6e74 6572 6e61 6c5f 7369 7a65 2020   internal_size  
-000106e0: 2320 7072 6563 6973 696f 6e20 2023 2073  # precision  # s
-000106f0: 6361 6c65 2020 2320 6e75 6c6c 5f6f 6b0a  cale  # null_ok.
-00010700: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00010710: 2020 2020 2020 2023 2061 6e64 2073 6574         # and set
-00010720: 2074 6865 2072 6573 756c 7473 0a20 2020   the results.   
-00010730: 2020 2020 2073 656c 662e 6c69 7374 5f72       self.list_r
-00010740: 6573 756c 7420 3d20 726f 7773 0a0a 2020  esult = rows..  
-00010750: 2020 6465 6620 5f67 6574 5f72 6573 756c    def _get_resul
-00010760: 745f 6d65 7461 6461 7461 2873 656c 6629  t_metadata(self)
-00010770: 3a0a 2020 2020 2020 2020 2222 2249 6e74  :.        """Int
-00010780: 6572 6e61 6c20 726f 7574 696e 6520 746f  ernal routine to
-00010790: 2067 6574 206d 6574 6164 6174 6120 666f   get metadata fo
-000107a0: 7220 6120 7265 7375 6c74 2073 6574 2222  r a result set""
-000107b0: 220a 2020 2020 2020 2020 2320 7079 6c69  ".        # pyli
-000107c0: 6e74 3a20 6469 7361 626c 653d 6e6f 2d6d  nt: disable=no-m
-000107d0: 656d 6265 720a 2020 2020 2020 2020 7265  ember.        re
-000107e0: 7120 3d20 7072 6f74 6f2e 5265 7175 6573  q = proto.Reques
-000107f0: 7428 290a 2020 2020 2020 2020 7265 712e  t().        req.
-00010800: 7479 7065 203d 2072 6571 2e46 4554 4348  type = req.FETCH
-00010810: 5f4d 4554 4144 4154 410a 0a20 2020 2020  _METADATA..     
-00010820: 2020 205f 7365 6e64 5f6d 7367 2873 656c     _send_msg(sel
-00010830: 662e 636f 6e6e 6563 7469 6f6e 2c20 7265  f.connection, re
-00010840: 7129 0a0a 2020 2020 2020 2020 7273 7020  q)..        rsp 
-00010850: 3d20 5f72 6563 765f 6d73 6728 7365 6c66  = _recv_msg(self
-00010860: 2e63 6f6e 6e65 6374 696f 6e2c 2070 726f  .connection, pro
-00010870: 746f 2e46 6574 6368 4d65 7461 6461 7461  to.FetchMetadata
-00010880: 5265 7370 6f6e 7365 2829 290a 2020 2020  Response()).    
-00010890: 2020 2020 6966 2072 7370 2e72 6573 706f      if rsp.respo
-000108a0: 6e73 652e 7479 7065 203d 3d20 7072 6f74  nse.type == prot
-000108b0: 6f2e 436f 6e66 6972 6d61 7469 6f6e 5265  o.ConfirmationRe
-000108c0: 7370 6f6e 7365 2e52 4553 504f 4e53 455f  sponse.RESPONSE_
-000108d0: 5741 524e 3a0a 2020 2020 2020 2020 2020  WARN:.          
-000108e0: 2020 7761 726e 2872 7370 2e72 6573 706f    warn(rsp.respo
-000108f0: 6e73 652e 7265 6173 6f6e 290a 2020 2020  nse.reason).    
-00010900: 2020 2020 656c 6966 206e 6f74 2072 7370      elif not rsp
-00010910: 2e72 6573 706f 6e73 652e 7479 7065 203d  .response.type =
-00010920: 3d20 7072 6f74 6f2e 436f 6e66 6972 6d61  = proto.Confirma
-00010930: 7469 6f6e 5265 7370 6f6e 7365 2e52 4553  tionResponse.RES
-00010940: 504f 4e53 455f 4f4b 3a0a 2020 2020 2020  PONSE_OK:.      
-00010950: 2020 2020 2020 7261 6973 6520 5f63 6f6e        raise _con
-00010960: 7665 7274 5f65 7863 6570 7469 6f6e 2872  vert_exception(r
-00010970: 7370 2e72 6573 706f 6e73 6529 0a0a 2020  sp.response)..  
-00010980: 2020 2020 2020 636f 6c73 203d 207b 7d0a        cols = {}.
-00010990: 2020 2020 2020 2020 666f 7220 286b 6579          for (key
-000109a0: 2c20 7661 6c75 6529 2069 6e20 7273 702e  , value) in rsp.
-000109b0: 636f 6c73 3270 6f73 2e69 7465 6d73 2829  cols2pos.items()
-000109c0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-000109d0: 6c73 5b76 616c 7565 5d20 3d20 6b65 790a  ls[value] = key.
-000109e0: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
-000109f0: 7363 7269 7074 696f 6e20 3d20 5b5d 0a20  scription = []. 
-00010a00: 2020 2020 2020 2063 6f6c 6e61 6d65 7320         colnames 
-00010a10: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
-00010a20: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00010a30: 636f 6c73 2929 3a20 2023 2070 796c 696e  cols)):  # pylin
-00010a40: 743a 2064 6973 6162 6c65 3d63 6f6e 7369  t: disable=consi
-00010a50: 6465 722d 7573 696e 672d 656e 756d 6572  der-using-enumer
-00010a60: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
-00010a70: 6e61 6d65 203d 2063 6f6c 735b 695d 0a20  name = cols[i]. 
-00010a80: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
-00010a90: 7320 7475 706c 6520 6973 2064 6566 696e  s tuple is defin
-00010aa0: 6564 2069 6e20 5045 5020 3234 390a 2020  ed in PEP 249.  
-00010ab0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00010ac0: 6573 6372 6970 7469 6f6e 2e61 7070 656e  escription.appen
-00010ad0: 6428 286e 616d 652c 2054 7970 6543 6f64  d((name, TypeCod
-00010ae0: 6573 2e74 6f5f 7479 7065 2872 7370 2e63  es.to_type(rsp.c
-00010af0: 6f6c 7332 5479 7065 735b 6e61 6d65 5d29  ols2Types[name])
-00010b00: 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f  , None, None, No
-00010b10: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 2929  ne, None, None))
-00010b20: 2020 2320 6469 7370 6c61 795f 7369 7a65    # display_size
-00010b30: 2020 2320 696e 7465 726e 616c 5f73 697a    # internal_siz
-00010b40: 6520 2023 2070 7265 6369 7369 6f6e 2020  e  # precision  
-00010b50: 2320 7363 616c 6520 2023 206e 756c 6c5f  # scale  # null_
-00010b60: 6f6b 0a20 2020 2020 2020 2020 2020 2063  ok.            c
-00010b70: 6f6c 6e61 6d65 732e 6170 7065 6e64 286e  olnames.append(n
-00010b80: 616d 6529 0a20 2020 2020 2020 2073 656c  ame).        sel
-00010b90: 662e 7265 7375 6c74 7365 745f 7475 706c  f.resultset_tupl
-00010ba0: 6520 3d20 6e61 6d65 6474 7570 6c65 2822  e = namedtuple("
-00010bb0: 526f 7722 2c20 636f 6c6e 616d 6573 2c20  Row", colnames, 
-00010bc0: 7265 6e61 6d65 3d54 7275 6529 0a0a 2020  rename=True)..  
-00010bd0: 2020 6465 6620 5f65 7865 6375 7465 5f75    def _execute_u
-00010be0: 7064 6174 6528 7365 6c66 2c20 6f70 6572  pdate(self, oper
-00010bf0: 6174 696f 6e29 3a0a 2020 2020 2020 2020  ation):.        
-00010c00: 2222 2245 7865 6375 7465 2061 6e20 7570  """Execute an up
-00010c10: 6461 7465 2073 7461 7465 6d65 6e74 2222  date statement""
-00010c20: 220a 2020 2020 2020 2020 2320 7079 6c69  ".        # pyli
-00010c30: 6e74 3a20 6469 7361 626c 653d 6e6f 2d6d  nt: disable=no-m
-00010c40: 656d 6265 720a 2020 2020 2020 2020 2320  ember.        # 
-00010c50: 5768 696c 6520 7765 2061 7265 2072 6564  While we are red
-00010c60: 6972 6563 7469 6e67 2e2e 2e0a 0a20 2020  irecting.....   
-00010c70: 2020 2020 2023 2054 6865 7265 2069 7320       # There is 
-00010c80: 6e6f 2072 6573 756c 7473 6574 2064 6174  no resultset dat
-00010c90: 6120 6672 6f6d 2061 6e20 7570 6461 7465  a from an update
-00010ca0: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
-00010cb0: 645f 6f66 5f64 6174 6120 3d20 5472 7565  d_of_data = True
-00010cc0: 0a0a 2020 2020 2020 2020 7768 696c 6520  ..        while 
-00010cd0: 5472 7565 3a0a 2020 2020 2020 2020 2020  True:.          
-00010ce0: 2020 7265 7120 3d20 7072 6f74 6f2e 5265    req = proto.Re
-00010cf0: 7175 6573 7428 290a 2020 2020 2020 2020  quest().        
-00010d00: 2020 2020 7265 712e 7479 7065 203d 2072      req.type = r
-00010d10: 6571 2e45 5845 4355 5445 5f55 5044 4154  eq.EXECUTE_UPDAT
-00010d20: 450a 2020 2020 2020 2020 2020 2020 7265  E.            re
-00010d30: 712e 6578 6563 7574 655f 7570 6461 7465  q.execute_update
-00010d40: 2e73 716c 203d 206f 7065 7261 7469 6f6e  .sql = operation
-00010d50: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-00010d60: 2e65 7865 6375 7465 5f75 7064 6174 652e  .execute_update.
-00010d70: 666f 7263 6520 3d20 7365 6c66 2e63 6f6e  force = self.con
-00010d80: 6e65 6374 696f 6e2e 666f 7263 650a 0a20  nection.force.. 
-00010d90: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010db0: 5f73 656e 645f 6d73 6728 7365 6c66 2e63  _send_msg(self.c
-00010dc0: 6f6e 6e65 6374 696f 6e2c 2072 6571 290a  onnection, req).
-00010dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010de0: 2072 7370 203d 205f 7265 6376 5f6d 7367   rsp = _recv_msg
-00010df0: 2873 656c 662e 636f 6e6e 6563 7469 6f6e  (self.connection
-00010e00: 2c20 7072 6f74 6f2e 4578 6563 7574 6555  , proto.ExecuteU
-00010e10: 7064 6174 6552 6573 706f 6e73 6528 2929  pdateResponse())
-00010e20: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-00010e30: 6570 7420 494f 4572 726f 723a 0a20 2020  ept IOError:.   
-00010e40: 2020 2020 2020 2020 2020 2020 2023 2072               # r
-00010e50: 656d 616b 6520 6f75 7220 636f 6e6e 6563  emake our connec
-00010e60: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00010e70: 2020 2020 2073 656c 662e 636f 6e6e 6563       self.connec
-00010e80: 7469 6f6e 203d 2043 6f6e 6e65 6374 696f  tion = Connectio
-00010e90: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00010ea0: 2020 2020 2020 2075 7365 723d 7365 6c66         user=self
-00010eb0: 2e63 6f6e 6e65 6374 696f 6e2e 7573 6572  .connection.user
-00010ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010ed0: 2020 2020 2020 7061 7373 776f 7264 3d73        password=s
-00010ee0: 656c 662e 636f 6e6e 6563 7469 6f6e 2e70  elf.connection.p
-00010ef0: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
-00010f00: 2020 2020 2020 2020 2020 2020 2068 6f73               hos
-00010f10: 743d 6622 7b27 2c27 2e6a 6f69 6e28 7365  t=f"{','.join(se
-00010f20: 6c66 2e63 6f6e 6e65 6374 696f 6e2e 686f  lf.connection.ho
-00010f30: 7374 7329 7d3a 7b73 656c 662e 636f 6e6e  sts)}:{self.conn
-00010f40: 6563 7469 6f6e 2e70 6f72 747d 222c 0a20  ection.port}",. 
+0000bb60: 2073 656c 662e 686f 7374 7320 3d20 7061   self.hosts = pa
+0000bb70: 7274 735b 305d 2e73 706c 6974 2822 2c22  rts[0].split(","
+0000bb80: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000bb90: 6966 206c 656e 2870 6172 7473 2920 3d3d  if len(parts) ==
+0000bba0: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+0000bbb0: 2020 2020 7365 6c66 2e68 6f73 7473 203d      self.hosts =
+0000bbc0: 2070 6172 7473 5b30 5d2e 7370 6c69 7428   parts[0].split(
+0000bbd0: 222c 2229 0a20 2020 2020 2020 2020 2020  ",").           
+0000bbe0: 2020 2020 2073 656c 662e 706f 7274 203d       self.port =
+0000bbf0: 2069 6e74 2870 6172 7473 5b31 5d29 0a20   int(parts[1]). 
+0000bc00: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000bc10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bc20: 2072 6169 7365 204d 616c 666f 726d 6564   raise Malformed
+0000bc30: 5552 4c28 6622 496e 7661 6c69 6420 686f  URL(f"Invalid ho
+0000bc40: 7374 2076 616c 7565 3a20 7b68 6f73 747d  st value: {host}
+0000bc50: 2229 0a0a 2020 2020 2020 2020 6966 2064  ")..        if d
+0000bc60: 6174 6162 6173 653a 0a20 2020 2020 2020  atabase:.       
+0000bc70: 2020 2020 2073 656c 662e 6461 7461 6261       self.databa
+0000bc80: 7365 203d 2064 6174 6162 6173 650a 0a20  se = database.. 
+0000bc90: 2020 2020 2020 2069 6620 746c 7320 6973         if tls is
+0000bca0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000bcb0: 2020 2020 2020 2073 656c 662e 746c 7320         self.tls 
+0000bcc0: 3d20 746c 730a 0a20 2020 2020 2020 2069  = tls..        i
+0000bcd0: 6620 6861 6e64 7368 616b 6520 6973 206e  f handshake is n
+0000bce0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000bcf0: 2020 2020 2073 656c 662e 6861 6e64 7368       self.handsh
+0000bd00: 616b 6520 3d20 6861 6e64 7368 616b 650a  ake = handshake.
+0000bd10: 0a20 2020 2020 2020 2023 2053 6574 2074  .        # Set t
+0000bd20: 6865 2064 6566 6175 6c74 2068 6f73 7420  he default host 
+0000bd30: 6e6f 772c 2073 696e 6365 2077 6520 7573  now, since we us
+0000bd40: 6520 7468 6174 2061 7320 6120 6b65 7920  e that as a key 
+0000bd50: 696e 746f 2074 6865 0a20 2020 2020 2020  into the.       
+0000bd60: 2023 2063 6f6e 6669 6720 6669 6c65 0a20   # config file. 
+0000bd70: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+0000bd80: 6f73 7473 2069 7320 4e6f 6e65 3a0a 2020  osts is None:.  
+0000bd90: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+0000bda0: 6f73 7473 203d 205b 7365 6c66 2e44 4546  osts = [self.DEF
+0000bdb0: 4155 4c54 5f48 4f53 545d 0a0a 2020 2020  AULT_HOST]..    
+0000bdc0: 2020 2020 2320 4e6f 7720 6275 696c 6420      # Now build 
+0000bdd0: 6120 636f 6e66 6967 7061 7273 6572 2077  a configparser w
+0000bde0: 6974 6820 6465 6661 756c 7420 7661 6c75  ith default valu
+0000bdf0: 6573 0a20 2020 2020 2020 2063 6f6e 6669  es.        confi
+0000be00: 6720 3d20 636f 6e66 6967 7061 7273 6572  g = configparser
+0000be10: 2e43 6f6e 6669 6750 6172 7365 7228 0a20  .ConfigParser(. 
+0000be20: 2020 2020 2020 2020 2020 2064 6566 6175             defau
+0000be30: 6c74 733d 7b22 706f 7274 223a 2073 7472  lts={"port": str
+0000be40: 2873 656c 662e 4445 4641 554c 545f 504f  (self.DEFAULT_PO
+0000be50: 5254 292c 2022 6461 7461 6261 7365 223a  RT), "database":
+0000be60: 2073 656c 662e 4445 4641 554c 545f 4441   self.DEFAULT_DA
+0000be70: 5441 4241 5345 2c20 2274 6c73 223a 2022  TABASE, "tls": "
+0000be80: 756e 7665 7269 6669 6564 222c 2022 666f  unverified", "fo
+0000be90: 7263 6522 3a20 2266 616c 7365 222c 2022  rce": "false", "
+0000bea0: 6861 6e64 7368 616b 6522 3a20 2222 7d2c  handshake": ""},
+0000beb0: 2069 6e74 6572 706f 6c61 7469 6f6e 3d4e   interpolation=N
+0000bec0: 6f6e 650a 2020 2020 2020 2020 290a 2020  one.        ).  
+0000bed0: 2020 2020 2020 636f 6e66 6967 7661 6c73        configvals
+0000bee0: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+0000bef0: 2023 2049 6620 7765 2068 6176 6520 6120   # If we have a 
+0000bf00: 636f 6e66 6967 2066 696c 6520 7472 7920  config file try 
+0000bf10: 6c6f 6164 696e 6720 7468 6174 0a20 2020  loading that.   
+0000bf20: 2020 2020 2069 6620 636f 6e66 6967 6669       if configfi
+0000bf30: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  le is not None:.
+0000bf40: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+0000bf50: 6669 672e 7265 6164 2863 6f6e 6669 6766  fig.read(configf
+0000bf60: 696c 6529 0a0a 2020 2020 2020 2020 2020  ile)..          
+0000bf70: 2020 2320 576f 726b 206f 7574 2074 6865    # Work out the
+0000bf80: 2068 6f73 742f 6461 7461 6261 7365 2069   host/database i
+0000bf90: 6620 7765 206b 6e6f 7720 6974 0a20 2020  f we know it.   
+0000bfa0: 2020 2020 2020 2020 2068 6f73 745f 6462           host_db
+0000bfb0: 203d 2022 2c22 2e6a 6f69 6e28 7365 6c66   = ",".join(self
+0000bfc0: 2e68 6f73 7473 290a 2020 2020 2020 2020  .hosts).        
+0000bfd0: 2020 2020 6966 2073 656c 662e 6461 7461      if self.data
+0000bfe0: 6261 7365 2069 7320 6e6f 7420 4e6f 6e65  base is not None
+0000bff0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c000: 2020 686f 7374 5f64 6220 3d20 686f 7374    host_db = host
+0000c010: 5f64 6220 2b20 222f 2220 2b20 7365 6c66  _db + "/" + self
+0000c020: 2e64 6174 6162 6173 650a 0a20 2020 2020  .database..     
+0000c030: 2020 2020 2020 2023 2054 7279 2061 6e64         # Try and
+0000c040: 206d 6174 6368 2065 6163 6820 7365 6374   match each sect
+0000c050: 696f 6e20 696e 2074 6865 2049 4e49 2066  ion in the INI f
+0000c060: 696c 6520 7769 7468 2074 6865 2068 6f73  ile with the hos
+0000c070: 742f 6461 7461 6261 7365 0a20 2020 2020  t/database.     
+0000c080: 2020 2020 2020 2066 6f72 2073 2069 6e20         for s in 
+0000c090: 636f 6e66 6967 2e73 6563 7469 6f6e 7328  config.sections(
+0000c0a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000c0b0: 2020 2069 6620 7265 2e6d 6174 6368 2873     if re.match(s
+0000c0c0: 2c20 686f 7374 5f64 6229 3a0a 2020 2020  , host_db):.    
+0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0e0: 636f 6e66 6967 7661 6c73 203d 2063 6f6e  configvals = con
+0000c0f0: 6669 675b 735d 0a20 2020 2020 2020 2020  fig[s].         
+0000c100: 2020 2020 2020 2020 2020 2062 7265 616b             break
+0000c110: 0a0a 2020 2020 2020 2020 2320 6966 2077  ..        # if w
+0000c120: 6520 6469 646e 2774 2066 696e 6420 6120  e didn't find a 
+0000c130: 6d61 7463 6869 6e67 2068 6f73 7420 286f  matching host (o
+0000c140: 7220 7468 6572 6520 6973 206e 6f20 6669  r there is no fi
+0000c150: 6c65 292e 2075 7365 2074 6865 2064 6566  le). use the def
+0000c160: 6175 6c74 730a 2020 2020 2020 2020 6966  aults.        if
+0000c170: 2063 6f6e 6669 6776 616c 7320 6973 204e   configvals is N
+0000c180: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000c190: 2063 6f6e 6669 6776 616c 7320 3d20 636f   configvals = co
+0000c1a0: 6e66 6967 5b22 4445 4641 554c 5422 5d0a  nfig["DEFAULT"].
+0000c1b0: 2020 2020 2020 2020 2320 466f 7263 6520          # Force 
+0000c1c0: 6973 206e 6f74 2070 6c61 6365 7320 6865  is not places he
+0000c1d0: 7265 2073 6f20 6974 2063 616e 2067 6574  re so it can get
+0000c1e0: 2070 6172 7365 6420 6265 6c6f 772e 0a20   parsed below.. 
+0000c1f0: 2020 2020 2020 2066 6f72 2061 7474 7220         for attr 
+0000c200: 696e 205b 2270 6f72 7422 2c20 2264 6174  in ["port", "dat
+0000c210: 6162 6173 6522 2c20 2274 6c73 222c 2022  abase", "tls", "
+0000c220: 6861 6e64 7368 616b 6522 5d3a 0a20 2020  handshake"]:.   
+0000c230: 2020 2020 2020 2020 2069 6620 6765 7461           if geta
+0000c240: 7474 7228 7365 6c66 2c20 6174 7472 2920  ttr(self, attr) 
+0000c250: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000c260: 2020 2020 2020 2020 2073 6574 6174 7472           setattr
+0000c270: 2873 656c 662c 2061 7474 722c 2063 6f6e  (self, attr, con
+0000c280: 6669 6776 616c 735b 6174 7472 5d29 0a0a  figvals[attr])..
+0000c290: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+0000c2a0: 656c 662e 7573 6572 3a0a 2020 2020 2020  elf.user:.      
+0000c2b0: 2020 2020 2020 7365 6c66 2e75 7365 7220        self.user 
+0000c2c0: 3d20 636f 6e66 6967 7661 6c73 2e67 6574  = configvals.get
+0000c2d0: 2822 7573 6572 222c 2022 2229 0a0a 2020  ("user", "")..  
+0000c2e0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+0000c2f0: 662e 7061 7373 776f 7264 3a0a 2020 2020  f.password:.    
+0000c300: 2020 2020 2020 2020 7365 6c66 2e70 6173          self.pas
+0000c310: 7377 6f72 6420 3d20 636f 6e66 6967 7661  sword = configva
+0000c320: 6c73 2e67 6574 2822 7061 7373 776f 7264  ls.get("password
+0000c330: 222c 2022 2229 0a0a 2020 2020 2020 2020  ", "")..        
+0000c340: 6966 2073 656c 662e 666f 7263 6520 6973  if self.force is
+0000c350: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000c360: 2020 2073 656c 662e 666f 7263 6520 3d20     self.force = 
+0000c370: 636f 6e66 6967 7661 6c73 2e67 6574 626f  configvals.getbo
+0000c380: 6f6c 6561 6e28 2266 6f72 6365 2229 0a0a  olean("force")..
+0000c390: 2020 2020 2020 2020 2320 416e 6420 6669          # And fi
+0000c3a0: 6e61 6c6c 7920 7469 6479 2075 7020 736f  nally tidy up so
+0000c3b0: 6d65 2074 6869 6e67 730a 2020 2020 2020  me things.      
+0000c3c0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000c3d0: 7365 6c66 2e70 6f72 742c 2073 7472 293a  self.port, str):
+0000c3e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c3f0: 662e 706f 7274 203d 2069 6e74 2873 656c  f.port = int(sel
+0000c400: 662e 706f 7274 290a 0a20 2020 2020 2020  f.port)..       
+0000c410: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
+0000c420: 656c 662e 746c 732c 2073 7472 293a 0a20  elf.tls, str):. 
+0000c430: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000c440: 6c66 2e74 6c73 2e6c 6f77 6572 2829 203d  lf.tls.lower() =
+0000c450: 3d20 226f 6666 223a 0a20 2020 2020 2020  = "off":.       
+0000c460: 2020 2020 2020 2020 2073 656c 662e 746c           self.tl
+0000c470: 7320 3d20 7365 6c66 2e54 4c53 5f4e 4f4e  s = self.TLS_NON
+0000c480: 450a 2020 2020 2020 2020 2020 2020 656c  E.            el
+0000c490: 6966 2073 656c 662e 746c 732e 6c6f 7765  if self.tls.lowe
+0000c4a0: 7228 2920 3d3d 2022 756e 7665 7269 6669  r() == "unverifi
+0000c4b0: 6564 223a 0a20 2020 2020 2020 2020 2020  ed":.           
+0000c4c0: 2020 2020 2073 656c 662e 746c 7320 3d20       self.tls = 
+0000c4d0: 7365 6c66 2e54 4c53 5f55 4e56 4552 4946  self.TLS_UNVERIF
+0000c4e0: 4945 440a 2020 2020 2020 2020 2020 2020  IED.            
+0000c4f0: 656c 6966 2073 656c 662e 746c 732e 6c6f  elif self.tls.lo
+0000c500: 7765 7228 2920 3d3d 2022 6f6e 223a 0a20  wer() == "on":. 
+0000c510: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c520: 656c 662e 746c 7320 3d20 7365 6c66 2e54  elf.tls = self.T
+0000c530: 4c53 5f4f 4e0a 2020 2020 2020 2020 2020  LS_ON.          
+0000c540: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000c550: 2020 2020 2020 2020 7261 6973 6520 4d61          raise Ma
+0000c560: 6c66 6f72 6d65 6455 524c 2866 2249 6e76  lformedURL(f"Inv
+0000c570: 616c 6964 2074 6c73 2076 616c 7565 3a20  alid tls value: 
+0000c580: 7b73 656c 662e 746c 737d 2229 0a20 2020  {self.tls}").   
+0000c590: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+0000c5a0: 616e 6365 2873 656c 662e 746c 732c 206c  ance(self.tls, l
+0000c5b0: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
+0000c5c0: 2020 7261 6973 6520 4d61 6c66 6f72 6d65    raise Malforme
+0000c5d0: 6455 524c 2866 224d 756c 7469 706c 6520  dURL(f"Multiple 
+0000c5e0: 544c 5320 7661 6c75 6573 2064 6574 6563  TLS values detec
+0000c5f0: 7465 643a 207b 7365 6c66 2e74 6c73 7d22  ted: {self.tls}"
+0000c600: 290a 0a20 2020 2020 2020 2069 6620 6973  )..        if is
+0000c610: 696e 7374 616e 6365 2873 656c 662e 6861  instance(self.ha
+0000c620: 6e64 7368 616b 652c 2073 7472 293a 0a20  ndshake, str):. 
+0000c630: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000c640: 6c66 2e68 616e 6473 6861 6b65 2e6c 6f77  lf.handshake.low
+0000c650: 6572 2829 203d 3d20 2263 6263 223a 0a20  er() == "cbc":. 
+0000c660: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c670: 656c 662e 6861 6e64 7368 616b 6520 3d20  elf.handshake = 
+0000c680: 7365 6c66 2e48 414e 4453 4841 4b45 5f43  self.HANDSHAKE_C
+0000c690: 4243 0a20 2020 2020 2020 2020 2020 2065  BC.            e
+0000c6a0: 6c69 6620 7365 6c66 2e68 616e 6473 6861  lif self.handsha
+0000c6b0: 6b65 2e6c 6f77 6572 2829 203d 3d20 2273  ke.lower() == "s
+0000c6c0: 736f 223a 0a20 2020 2020 2020 2020 2020  so":.           
+0000c6d0: 2020 2020 2073 656c 662e 6861 6e64 7368       self.handsh
+0000c6e0: 616b 6520 3d20 7365 6c66 2e48 414e 4453  ake = self.HANDS
+0000c6f0: 4841 4b45 5f53 534f 0a20 2020 2020 2020  HAKE_SSO.       
+0000c700: 2020 2020 2023 2049 6620 7468 6579 2064       # If they d
+0000c710: 6964 6e27 7420 7370 6563 6966 7920 6861  idn't specify ha
+0000c720: 6e64 7368 616b 652c 2069 7420 7769 6c6c  ndshake, it will
+0000c730: 2062 6520 626c 616e 6b20 616e 6420 7468   be blank and th
+0000c740: 7573 2073 686f 756c 6420 6265 2047 434d  us should be GCM
+0000c750: 2e0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+0000c760: 6966 2073 656c 662e 6861 6e64 7368 616b  if self.handshak
+0000c770: 652e 6c6f 7765 7228 2920 3d3d 2022 6763  e.lower() == "gc
+0000c780: 6d22 206f 7220 7365 6c66 2e68 616e 6473  m" or self.hands
+0000c790: 6861 6b65 2e6c 6f77 6572 2829 203d 3d20  hake.lower() == 
+0000c7a0: 2222 3a0a 2020 2020 2020 2020 2020 2020  "":.            
+0000c7b0: 2020 2020 7365 6c66 2e68 616e 6473 6861      self.handsha
+0000c7c0: 6b65 203d 2073 656c 662e 4841 4e44 5348  ke = self.HANDSH
+0000c7d0: 414b 455f 4743 4d0a 2020 2020 2020 2020  AKE_GCM.        
+0000c7e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000c7f0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000c800: 7365 6c66 2e68 616e 6473 6861 6b65 290a  self.handshake).
+0000c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c820: 7261 6973 6520 4d61 6c66 6f72 6d65 6455  raise MalformedU
+0000c830: 524c 2866 2249 6e76 616c 6964 2068 616e  RL(f"Invalid han
+0000c840: 6473 6861 6b65 2076 616c 7565 3a20 7b73  dshake value: {s
+0000c850: 656c 662e 6861 6e64 7368 616b 657d 2229  elf.handshake}")
+0000c860: 0a0a 2020 2020 2020 2020 2320 446f 6e27  ..        # Don'
+0000c870: 7420 6173 7365 7274 2061 2075 7365 7220  t assert a user 
+0000c880: 7061 7261 6d65 7465 7220 6861 7320 6265  parameter has be
+0000c890: 656e 2073 6574 2e20 416e 2065 6d70 7479  en set. An empty
+0000c8a0: 0a20 2020 2020 2020 2023 2073 7472 696e  .        # strin
+0000c8b0: 6720 666f 7220 7468 6973 2066 6965 6c64  g for this field
+0000c8c0: 2069 7320 7573 6564 2066 6f72 2061 7574   is used for aut
+0000c8d0: 6865 6e74 6963 6174 696e 6720 5353 4f20  henticating SSO 
+0000c8e0: 7573 6572 730a 0a20 2020 2020 2020 2023  users..        #
+0000c8f0: 2044 6f6e 2774 2061 7373 6572 7420 6120   Don't assert a 
+0000c900: 7061 7373 776f 7264 2070 6172 616d 6574  password paramet
+0000c910: 6572 2068 6173 2062 6565 6e20 7365 742e  er has been set.
+0000c920: 2041 7420 656d 7074 790a 2020 2020 2020   At empty.      
+0000c930: 2020 2320 7573 6572 2061 6e64 2070 6173    # user and pas
+0000c940: 7377 6f72 6420 6973 2066 6f72 2061 7574  sword is for aut
+0000c950: 6865 6e74 6963 6174 696f 6e20 666c 6f77  hentication flow
+0000c960: 2077 6974 6820 5353 4f2e 0a0a 2020 2020   with SSO...    
+0000c970: 6465 6620 636c 6f73 6528 7365 6c66 293a  def close(self):
+0000c980: 0a20 2020 2020 2020 2022 2222 436c 6f73  .        """Clos
+0000c990: 6520 7468 6520 636f 6e6e 6563 7469 6f6e  e the connection
+0000c9a0: 2e20 5375 6273 6571 7565 6e74 2071 7565  . Subsequent que
+0000c9b0: 7269 6573 206f 6e20 7468 6973 2063 6f6e  ries on this con
+0000c9c0: 6e65 6374 696f 6e0a 2020 2020 2020 2020  nection.        
+0000c9d0: 7769 6c6c 2066 6169 6c0a 2020 2020 2020  will fail.      
+0000c9e0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+0000c9f0: 206e 6f74 2073 656c 662e 736f 636b 3a0a   not self.sock:.
+0000ca00: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000ca10: 6520 4572 726f 7228 224e 6f20 636f 6e6e  e Error("No conn
+0000ca20: 6563 7469 6f6e 2229 0a0a 2020 2020 2020  ection")..      
+0000ca30: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
+0000ca40: 2243 6c6f 7369 6e67 2063 6f6e 6e65 6374  "Closing connect
+0000ca50: 696f 6e20 6f6e 2073 6f63 6b65 7420 7b73  ion on socket {s
+0000ca60: 656c 662e 736f 636b 7d22 290a 2020 2020  elf.sock}").    
+0000ca70: 2020 2020 2320 446f 2074 6869 7320 6c69      # Do this li
+0000ca80: 7474 6c65 2064 616e 6365 2073 6f20 7468  ttle dance so th
+0000ca90: 6174 2065 7665 6e20 6966 2074 6865 2063  at even if the c
+0000caa0: 6c6f 7365 2829 2063 616c 6c0a 2020 2020  lose() call.    
+0000cab0: 2020 2020 2320 626c 6f77 7320 7570 2c20      # blows up, 
+0000cac0: 7765 2068 6176 6520 616c 7265 6164 7920  we have already 
+0000cad0: 7365 7420 7365 6c66 2e73 6f63 6b20 746f  set self.sock to
+0000cae0: 204e 6f6e 650a 2020 2020 2020 2020 736f   None.        so
+0000caf0: 636b 203d 2073 656c 662e 736f 636b 0a20  ck = self.sock. 
+0000cb00: 2020 2020 2020 2073 656c 662e 736f 636b         self.sock
+0000cb10: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000cb20: 736f 636b 2e63 6c6f 7365 2829 0a0a 2020  sock.close()..  
+0000cb30: 2020 6465 6620 636f 6d6d 6974 2873 656c    def commit(sel
+0000cb40: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
+0000cb50: 6f6d 6d69 7420 6120 7472 616e 7361 6374  ommit a transact
+0000cb60: 696f 6e2e 2043 7572 7265 6e74 6c79 2069  ion. Currently i
+0000cb70: 676e 6f72 6564 2222 220a 0a20 2020 2064  gnored"""..    d
+0000cb80: 6566 2063 7572 736f 7228 7365 6c66 293a  ef cursor(self):
+0000cb90: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+0000cba0: 726e 2061 206e 6577 2063 7572 736f 7220  rn a new cursor 
+0000cbb0: 666f 7220 7468 6973 2063 6f6e 6e65 6374  for this connect
+0000cbc0: 696f 6e22 2222 0a20 2020 2020 2020 2069  ion""".        i
+0000cbd0: 6620 6e6f 7420 7365 6c66 2e73 6f63 6b3a  f not self.sock:
+0000cbe0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0000cbf0: 7365 2045 7272 6f72 2822 4e6f 2063 6f6e  se Error("No con
+0000cc00: 6e65 6374 696f 6e22 290a 2020 2020 2020  nection").      
+0000cc10: 2020 7265 7475 726e 2043 7572 736f 7228    return Cursor(
+0000cc20: 7365 6c66 290a 0a20 2020 2064 6566 205f  self)..    def _
+0000cc30: 5f64 656c 5f5f 2873 656c 6629 3a0a 2020  _del__(self):.  
+0000cc40: 2020 2020 2020 6966 2073 656c 662e 736f        if self.so
+0000cc50: 636b 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ck is not None:.
+0000cc60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cc70: 2e63 6c6f 7365 2829 0a0a 2020 2020 6465  .close()..    de
+0000cc80: 6620 7265 736f 6c76 655f 6e65 775f 656e  f resolve_new_en
+0000cc90: 6470 6f69 6e74 2873 656c 662c 206e 6577  dpoint(self, new
+0000cca0: 5f68 6f73 742c 206e 6577 5f70 6f72 7429  _host, new_port)
+0000ccb0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000ccc0: 2020 2020 2020 4861 6e64 6c65 7320 6d61        Handles ma
+0000ccd0: 7070 696e 6720 746f 2061 2073 6563 6f6e  pping to a secon
+0000cce0: 6461 7279 2069 6e74 6572 6661 6365 2062  dary interface b
+0000ccf0: 6173 6564 206f 6e20 7468 6520 7365 636f  ased on the seco
+0000cd00: 6e64 6172 7920 696e 7465 7266 6163 6520  ndary interface 
+0000cd10: 6d61 7070 696e 6720 7361 7665 6420 6f6e  mapping saved on
+0000cd20: 2074 6869 7320 636f 6e6e 6563 7469 6f6e   this connection
+0000cd30: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+0000cd40: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+0000cd50: 5f68 6f73 745b 7374 7269 6e67 5d3a 2074  _host[string]: t
+0000cd60: 6865 206e 6577 2068 6f73 7420 746f 2062  he new host to b
+0000cd70: 6520 7265 6d61 7070 6564 0a20 2020 2020  e remapped.     
+0000cd80: 2020 2020 2020 206e 6577 5f70 6f72 745b         new_port[
+0000cd90: 696e 745d 3a20 7468 6520 6e65 7720 706f  int]: the new po
+0000cda0: 7274 2074 6f20 6265 2072 656d 6170 7065  rt to be remappe
+0000cdb0: 640a 0a20 2020 2020 2020 2052 6574 7572  d..        Retur
+0000cdc0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000cdd0: 5b74 7570 6c65 2873 7472 696e 672c 2069  [tuple(string, i
+0000cde0: 6e74 295d 3a20 5468 6520 6163 7475 616c  nt)]: The actual
+0000cdf0: 2065 6e64 706f 696e 7420 746f 2063 6f6e   endpoint to con
+0000ce00: 6e65 6374 2074 6f20 696e 2074 6865 2066  nect to in the f
+0000ce10: 6f72 6d61 743a 2028 686f 7374 2c20 706f  ormat: (host, po
+0000ce20: 7274 292e 0a20 2020 2020 2020 2022 2222  rt)..        """
+0000ce30: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000ce40: 6465 6275 6728 6622 5265 736f 6c76 696e  debug(f"Resolvin
+0000ce50: 6720 6e65 7720 656e 6470 6f69 6e74 207b  g new endpoint {
+0000ce60: 6e65 775f 686f 7374 7d3a 7b6e 6577 5f70  new_host}:{new_p
+0000ce70: 6f72 747d 2077 6974 6820 7365 636f 6e64  ort} with second
+0000ce80: 6172 795f 696e 6465 7820 7b73 656c 662e  ary_index {self.
+0000ce90: 7365 636f 6e64 6172 795f 696e 6465 787d  secondary_index}
+0000cea0: 2061 6e64 2073 6563 6f6e 6461 7279 5f69   and secondary_i
+0000ceb0: 6e74 6572 6661 6365 207b 7365 6c66 2e73  nterface {self.s
+0000cec0: 6563 6f6e 6461 7279 5f69 6e74 6572 6661  econdary_interfa
+0000ced0: 6365 737d 2229 0a0a 2020 2020 2020 2020  ces}")..        
+0000cee0: 6e65 775f 656e 6470 6f69 6e74 203d 2028  new_endpoint = (
+0000cef0: 6e65 775f 686f 7374 2c20 6e65 775f 706f  new_host, new_po
+0000cf00: 7274 290a 2020 2020 2020 2020 656e 6470  rt).        endp
+0000cf10: 6f69 6e74 5f74 6f5f 636f 6e6e 6563 7420  oint_to_connect 
+0000cf20: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
+0000cf30: 6620 7365 6c66 2e73 6563 6f6e 6461 7279  f self.secondary
+0000cf40: 5f69 6e64 6578 2021 3d20 2d31 3a0a 2020  _index != -1:.  
+0000cf50: 2020 2020 2020 2020 2020 6f75 7465 725f            outer_
+0000cf60: 696e 6465 7820 3d20 300a 2020 2020 2020  index = 0.      
+0000cf70: 2020 2020 2020 666f 7220 6f75 7465 725f        for outer_
+0000cf80: 6c69 7374 2069 6e20 7365 6c66 2e73 6563  list in self.sec
+0000cf90: 6f6e 6461 7279 5f69 6e74 6572 6661 6365  ondary_interface
+0000cfa0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000cfb0: 2020 2069 6620 6f75 7465 725f 6c69 7374     if outer_list
+0000cfc0: 5b30 5d20 3d3d 206e 6577 5f65 6e64 706f  [0] == new_endpo
+0000cfd0: 696e 743a 0a20 2020 2020 2020 2020 2020  int:.           
+0000cfe0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+0000cff0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000d000: 7574 6572 5f69 6e64 6578 202b 3d20 310a  uter_index += 1.
+0000d010: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+0000d020: 7574 6572 5f69 6e64 6578 203c 206c 656e  uter_index < len
+0000d030: 2873 656c 662e 7365 636f 6e64 6172 795f  (self.secondary_
+0000d040: 696e 7465 7266 6163 6573 293a 0a20 2020  interfaces):.   
+0000d050: 2020 2020 2020 2020 2020 2020 2065 6e64               end
+0000d060: 706f 696e 745f 746f 5f63 6f6e 6e65 6374  point_to_connect
+0000d070: 203d 2073 656c 662e 7365 636f 6e64 6172   = self.secondar
+0000d080: 795f 696e 7465 7266 6163 6573 5b6f 7574  y_interfaces[out
+0000d090: 6572 5f69 6e64 6578 5d5b 7365 6c66 2e73  er_index][self.s
+0000d0a0: 6563 6f6e 6461 7279 5f69 6e64 6578 5d0a  econdary_index].
+0000d0b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000d0c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d0d0: 2020 656e 6470 6f69 6e74 5f74 6f5f 636f    endpoint_to_co
+0000d0e0: 6e6e 6563 7420 3d20 6e65 775f 656e 6470  nnect = new_endp
+0000d0f0: 6f69 6e74 0a0a 2020 2020 2020 2020 656c  oint..        el
+0000d100: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000d110: 656e 6470 6f69 6e74 5f74 6f5f 636f 6e6e  endpoint_to_conn
+0000d120: 6563 7420 3d20 6e65 775f 656e 6470 6f69  ect = new_endpoi
+0000d130: 6e74 0a0a 2020 2020 2020 2020 6c6f 6767  nt..        logg
+0000d140: 6572 2e64 6562 7567 2866 2252 6573 6f6c  er.debug(f"Resol
+0000d150: 7665 6420 6e65 7720 656e 6470 6f69 6e74  ved new endpoint
+0000d160: 207b 6e65 775f 686f 7374 7d3a 7b6e 6577   {new_host}:{new
+0000d170: 5f70 6f72 747d 2074 6f20 7b65 6e64 706f  _port} to {endpo
+0000d180: 696e 745f 746f 5f63 6f6e 6e65 6374 7d22  int_to_connect}"
+0000d190: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0000d1a0: 6e20 656e 6470 6f69 6e74 5f74 6f5f 636f  n endpoint_to_co
+0000d1b0: 6e6e 6563 740a 0a20 2020 2064 6566 2072  nnect..    def r
+0000d1c0: 6564 6972 6563 7428 7365 6c66 2c20 6e65  edirect(self, ne
+0000d1d0: 775f 686f 7374 2c20 6e65 775f 706f 7274  w_host, new_port
+0000d1e0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000d1f0: 2020 2020 2020 2052 6564 6972 6563 7473         Redirects
+0000d200: 2074 6f20 7468 6520 7072 6f70 6572 2073   to the proper s
+0000d210: 6563 6f6e 6461 7279 2069 6e74 6572 6661  econdary interfa
+0000d220: 6365 2067 6976 656e 2061 206e 6577 2065  ce given a new e
+0000d230: 6e64 706f 696e 742e 0a0a 2020 2020 2020  ndpoint...      
+0000d240: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000d250: 2020 2020 6e65 775f 686f 7374 5b73 7472      new_host[str
+0000d260: 696e 675d 3a20 7468 6520 6e65 7720 686f  ing]: the new ho
+0000d270: 7374 2074 6f20 6265 2072 656d 6170 7065  st to be remappe
+0000d280: 640a 2020 2020 2020 2020 2020 2020 6e65  d.            ne
+0000d290: 775f 706f 7274 5b69 6e74 5d3a 2074 6865  w_port[int]: the
+0000d2a0: 206e 6577 2070 6f72 7420 746f 2062 6520   new port to be 
+0000d2b0: 7265 6d61 7070 6564 0a0a 2020 2020 2020  remapped..      
+0000d2c0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000d2d0: 2020 2020 2020 205b 436f 6e6e 6563 7469         [Connecti
+0000d2e0: 6f6e 5d3a 2041 206e 6577 2063 6f6e 6e65  on]: A new conne
+0000d2f0: 6374 696f 6e2e 0a20 2020 2020 2020 2022  ction..        "
+0000d300: 2222 0a20 2020 2020 2020 2072 656d 6170  "".        remap
+0000d310: 7065 645f 686f 7374 2c20 7265 6d61 7070  ped_host, remapp
+0000d320: 6564 5f70 6f72 7420 3d20 7365 6c66 2e72  ed_port = self.r
+0000d330: 6573 6f6c 7665 5f6e 6577 5f65 6e64 706f  esolve_new_endpo
+0000d340: 696e 7428 6e65 775f 686f 7374 2c20 6e65  int(new_host, ne
+0000d350: 775f 706f 7274 290a 2020 2020 2020 2020  w_port).        
+0000d360: 6e65 775f 656e 6470 6f69 6e74 203d 2066  new_endpoint = f
+0000d370: 227b 7265 6d61 7070 6564 5f68 6f73 747d  "{remapped_host}
+0000d380: 3a7b 7265 6d61 7070 6564 5f70 6f72 747d  :{remapped_port}
+0000d390: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000d3a0: 2e64 6562 7567 2866 2252 6564 6972 6563  .debug(f"Redirec
+0000d3b0: 7469 6e67 2063 6f6e 6e65 6374 696f 6e20  ting connection 
+0000d3c0: 746f 207b 6e65 775f 686f 7374 7d3a 7b6e  to {new_host}:{n
+0000d3d0: 6577 5f70 6f72 747d 2c20 7768 6963 6820  ew_port}, which 
+0000d3e0: 6d61 7073 2074 6f20 7b72 656d 6170 7065  maps to {remappe
+0000d3f0: 645f 686f 7374 7d3a 7b72 656d 6170 7065  d_host}:{remappe
+0000d400: 645f 706f 7274 7d22 290a 0a20 2020 2020  d_port}")..     
+0000d410: 2020 2072 6574 7572 6e20 436f 6e6e 6563     return Connec
+0000d420: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+0000d430: 2020 7573 6572 3d73 656c 662e 7573 6572    user=self.user
+0000d440: 2c20 7061 7373 776f 7264 3d73 656c 662e  , password=self.
+0000d450: 7061 7373 776f 7264 2c20 686f 7374 3d6e  password, host=n
+0000d460: 6577 5f65 6e64 706f 696e 742c 2064 6174  ew_endpoint, dat
+0000d470: 6162 6173 653d 7365 6c66 2e64 6174 6162  abase=self.datab
+0000d480: 6173 652c 2074 6c73 3d73 656c 662e 746c  ase, tls=self.tl
+0000d490: 732c 2068 616e 6473 6861 6b65 3d73 656c  s, handshake=sel
+0000d4a0: 662e 6861 6e64 7368 616b 652c 2066 6f72  f.handshake, for
+0000d4b0: 6365 3d73 656c 662e 666f 7263 652c 2073  ce=self.force, s
+0000d4c0: 6573 7369 6f6e 3d73 656c 662e 7365 7373  ession=self.sess
+0000d4d0: 696f 6e0a 2020 2020 2020 2020 290a 0a20  ion.        ).. 
+0000d4e0: 2020 2064 6566 2072 6566 7265 7368 2873     def refresh(s
+0000d4f0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000d500: 220a 2020 2020 2020 2020 5573 6564 2074  ".        Used t
+0000d510: 6f20 7265 6672 6573 6820 7468 6520 7365  o refresh the se
+0000d520: 7373 696f 6e20 6173 736f 6369 6174 6564  ssion associated
+0000d530: 2077 6974 6820 7468 6973 2063 6f6e 6e65   with this conne
+0000d540: 6374 696f 6e2e 2054 6865 2073 6572 7665  ction. The serve
+0000d550: 7220 7769 6c6c 0a20 2020 2020 2020 2072  r will.        r
+0000d560: 6574 7572 6e20 6120 6e65 7720 7365 7276  eturn a new serv
+0000d570: 6572 2073 6573 7369 6f6e 2069 6420 616e  er session id an
+0000d580: 6420 7365 6375 7269 7479 2074 6f6b 656e  d security token
+0000d590: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000d5a0: 2020 2020 2020 7265 7120 3d20 7072 6f74        req = prot
+0000d5b0: 6f2e 5265 7175 6573 7428 290a 2020 2020  o.Request().    
+0000d5c0: 2020 2020 7265 712e 7479 7065 203d 2072      req.type = r
+0000d5d0: 6571 2e43 4c49 454e 545f 434f 4e4e 4543  eq.CLIENT_CONNEC
+0000d5e0: 5449 4f4e 5f52 4546 5245 5348 5f53 4553  TION_REFRESH_SES
+0000d5f0: 5349 4f4e 0a20 2020 2020 2020 2063 6c69  SION.        cli
+0000d600: 656e 745f 636f 6e6e 6563 7469 6f6e 203d  ent_connection =
+0000d610: 2072 6571 2e63 6c69 656e 745f 636f 6e6e   req.client_conn
+0000d620: 6563 7469 6f6e 5f72 6566 7265 7368 5f73  ection_refresh_s
+0000d630: 6573 7369 6f6e 0a0a 2020 2020 2020 2020  ession..        
+0000d640: 2320 5365 6e64 206d 6573 7361 6765 0a20  # Send message. 
+0000d650: 2020 2020 2020 205f 7365 6e64 5f6d 7367         _send_msg
+0000d660: 2873 656c 662c 2072 6571 290a 2020 2020  (self, req).    
+0000d670: 2020 2020 2320 5265 6365 6976 6520 6d65      # Receive me
+0000d680: 7373 6167 650a 2020 2020 2020 2020 7273  ssage.        rs
+0000d690: 7020 3d20 5f72 6563 765f 6d73 6728 7365  p = _recv_msg(se
+0000d6a0: 6c66 2c20 7072 6f74 6f2e 436c 6965 6e74  lf, proto.Client
+0000d6b0: 436f 6e6e 6563 7469 6f6e 5265 6672 6573  ConnectionRefres
+0000d6c0: 6853 6573 7369 6f6e 5265 7370 6f6e 7365  hSessionResponse
+0000d6d0: 2829 290a 0a20 2020 2020 2020 2069 6620  ())..        if 
+0000d6e0: 7273 702e 7265 7370 6f6e 7365 2e74 7970  rsp.response.typ
+0000d6f0: 6520 3d3d 2070 726f 746f 2e43 6f6e 6669  e == proto.Confi
+0000d700: 726d 6174 696f 6e52 6573 706f 6e73 652e  rmationResponse.
+0000d710: 5245 5350 4f4e 5345 5f57 4152 4e3a 0a20  RESPONSE_WARN:. 
+0000d720: 2020 2020 2020 2020 2020 2077 6172 6e28             warn(
+0000d730: 7273 702e 7265 7370 6f6e 7365 2e72 6561  rsp.response.rea
+0000d740: 736f 6e29 0a20 2020 2020 2020 2065 6c69  son).        eli
+0000d750: 6620 7273 702e 7265 7370 6f6e 7365 2e74  f rsp.response.t
+0000d760: 7970 6520 3d3d 2070 726f 746f 2e43 6f6e  ype == proto.Con
+0000d770: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
+0000d780: 652e 5245 5350 4f4e 5345 5f4f 4b3a 0a20  e.RESPONSE_OK:. 
+0000d790: 2020 2020 2020 2020 2020 2023 2043 6170             # Cap
+0000d7a0: 7475 7265 2074 6865 2073 6573 7369 6f6e  ture the session
+0000d7b0: 2069 640a 2020 2020 2020 2020 2020 2020   id.            
+0000d7c0: 7365 6c66 2e73 6572 7665 7253 6573 7369  self.serverSessi
+0000d7d0: 6f6e 4964 203d 2072 7370 2e73 6573 7369  onId = rsp.sessi
+0000d7e0: 6f6e 496e 666f 2e73 6572 7665 7253 6573  onInfo.serverSes
+0000d7f0: 7369 6f6e 4964 0a20 2020 2020 2020 2020  sionId.         
+0000d800: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000d810: 6622 436f 6e6e 6563 7465 6420 746f 2073  f"Connected to s
+0000d820: 6572 7665 7220 7365 7373 696f 6e20 4964  erver session Id
+0000d830: 3a20 7b73 656c 662e 7365 7276 6572 5365  : {self.serverSe
+0000d840: 7373 696f 6e49 647d 2229 0a20 2020 2020  ssionId}").     
+0000d850: 2020 2020 2020 2072 6563 6569 7665 645f         received_
+0000d860: 746f 6b65 6e20 3d20 7273 702e 7365 7373  token = rsp.sess
+0000d870: 696f 6e49 6e66 6f2e 7365 6375 7269 7479  ionInfo.security
+0000d880: 546f 6b65 6e0a 2020 2020 2020 2020 2020  Token.          
+0000d890: 2020 6966 2073 656c 662e 7365 7373 696f    if self.sessio
+0000d8a0: 6e2e 7365 6375 7269 7479 546f 6b65 6e20  n.securityToken 
+0000d8b0: 213d 204e 6f6e 653a 0a20 2020 2020 2020  != None:.       
+0000d8c0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000d8d0: 7373 696f 6e20 3d20 5365 7373 696f 6e28  ssion = Session(
+0000d8e0: 7365 6375 7269 7479 546f 6b65 6e3d 5365  securityToken=Se
+0000d8f0: 6375 7269 7479 546f 6b65 6e28 7265 6365  curityToken(rece
+0000d900: 6976 6564 5f74 6f6b 656e 2e64 6174 612c  ived_token.data,
+0000d910: 2072 6563 6569 7665 645f 746f 6b65 6e2e   received_token.
+0000d920: 7369 676e 6174 7572 652c 2072 6563 6569  signature, recei
+0000d930: 7665 645f 746f 6b65 6e2e 6973 7375 6572  ved_token.issuer
+0000d940: 4669 6e67 6572 7072 696e 7429 290a 2020  Fingerprint)).  
+0000d950: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d970: 2320 4967 6e6f 7265 2074 6865 2073 6563  # Ignore the sec
+0000d980: 7572 6974 7920 746f 6b65 6e0a 2020 2020  urity token.    
+0000d990: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d9a0: 2e73 6573 7369 6f6e 203d 2053 6573 7369  .session = Sessi
+0000d9b0: 6f6e 2875 7365 7241 6e64 5061 7373 776f  on(userAndPasswo
+0000d9c0: 7264 3d55 7365 7241 6e64 5061 7373 776f  rd=UserAndPasswo
+0000d9d0: 7264 2873 656c 662e 7573 6572 2c20 7365  rd(self.user, se
+0000d9e0: 6c66 2e70 6173 7377 6f72 6429 290a 2020  lf.password)).  
+0000d9f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000da00: 0a20 2020 2020 2020 2023 2053 6f6d 6574  .        # Somet
+0000da10: 6869 6e67 2062 6164 2068 6170 7065 6e65  hing bad happene
+0000da20: 6420 7769 7468 2074 6865 2072 6566 7265  d with the refre
+0000da30: 7368 2061 7474 656d 7074 2e0a 2020 2020  sh attempt..    
+0000da40: 2020 2020 7261 6973 6520 5f63 6f6e 7665      raise _conve
+0000da50: 7274 5f65 7863 6570 7469 6f6e 2872 7370  rt_exception(rsp
+0000da60: 2e72 6573 706f 6e73 6529 0a0a 0a63 6c61  .response)...cla
+0000da70: 7373 2043 7572 736f 723a 0a20 2020 2023  ss Cursor:.    #
+0000da80: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
+0000da90: 3d74 6f6f 2d6d 616e 792d 696e 7374 616e  =too-many-instan
+0000daa0: 6365 2d61 7474 7269 6275 7465 730a 2020  ce-attributes.  
+0000dab0: 2020 2222 2241 2064 6174 6162 6173 6520    """A database 
+0000dac0: 6375 7273 6f72 2c20 7768 6963 6820 6973  cursor, which is
+0000dad0: 2075 7365 6420 746f 206d 616e 6167 6520   used to manage 
+0000dae0: 6120 7175 6572 7920 616e 6420 6974 7320  a query and its 
+0000daf0: 7265 7475 726e 6564 2072 6573 756c 7473  returned results
+0000db00: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
+0000db10: 6e69 745f 5f28 7365 6c66 2c20 636f 6e6e  nit__(self, conn
+0000db20: 293a 0a20 2020 2020 2020 2022 2222 4375  ):.        """Cu
+0000db30: 7273 6f72 7320 6172 6520 6e6f 726d 616c  rsors are normal
+0000db40: 6c79 2063 7265 6174 6564 2062 7920 7468  ly created by th
+0000db50: 6520 6375 7273 6f72 2829 2063 616c 6c20  e cursor() call 
+0000db60: 6f6e 2061 2063 6f6e 6e65 6374 696f 6e2c  on a connection,
+0000db70: 2062 7574 2063 616e 0a20 2020 2020 2020   but can.       
+0000db80: 2062 6520 6372 6561 7465 6420 6469 7265   be created dire
+0000db90: 6374 6c79 2062 7920 7072 6f76 6964 696e  ctly by providin
+0000dba0: 6720 6120 636f 6e6e 6563 7469 6f6e 0a20  g a connection. 
+0000dbb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000dbc0: 2020 2073 656c 662e 636f 6e6e 6563 7469     self.connecti
+0000dbd0: 6f6e 203d 2063 6f6e 6e0a 2020 2020 2020  on = conn.      
+0000dbe0: 2020 7365 6c66 2e61 7272 6179 7369 7a65    self.arraysize
+0000dbf0: 203d 2031 0a0a 2020 2020 2020 2020 7365   = 1..        se
+0000dc00: 6c66 2e5f 7265 696e 6974 6961 6c69 7a65  lf._reinitialize
+0000dc10: 2829 0a0a 2020 2020 6465 6620 5f5f 6465  ()..    def __de
+0000dc20: 6c5f 5f28 7365 6c66 293a 0a20 2020 2020  l__(self):.     
+0000dc30: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000dc40: 2020 2020 7365 6c66 2e5f 636c 6f73 655f      self._close_
+0000dc50: 7265 7375 6c74 7365 7428 290a 2020 2020  resultset().    
+0000dc60: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+0000dc70: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+0000dc80: 2020 6465 6620 5f72 6569 6e69 7469 616c    def _reinitial
+0000dc90: 697a 6528 7365 6c66 293a 0a20 2020 2020  ize(self):.     
+0000dca0: 2020 2022 2222 496e 7465 726e 616c 2066     """Internal f
+0000dcb0: 756e 6374 696f 6e20 746f 2069 6e69 7469  unction to initi
+0000dcc0: 616c 697a 6520 6120 6375 7273 6f72 2222  alize a cursor""
+0000dcd0: 220a 2020 2020 2020 2020 2320 5365 7420  ".        # Set 
+0000dce0: 7468 6520 7374 6174 650a 2020 2020 2020  the state.      
+0000dcf0: 2020 7365 6c66 2e71 7565 7279 5f69 6420    self.query_id 
+0000dd00: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+0000dd10: 656c 662e 726f 7763 6f75 6e74 203d 202d  elf.rowcount = -
+0000dd20: 310a 2020 2020 2020 2020 7365 6c66 2e72  1.        self.r
+0000dd30: 6f77 6e75 6d62 6572 203d 204e 6f6e 650a  ownumber = None.
+0000dd40: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
+0000dd50: 756c 7473 6574 5f74 7570 6c65 203d 204e  ultset_tuple = N
+0000dd60: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000dd70: 2e64 6573 6372 6970 7469 6f6e 203d 204e  .description = N
+0000dd80: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000dd90: 2e65 6e64 5f6f 665f 6461 7461 203d 2046  .end_of_data = F
+0000dda0: 616c 7365 0a20 2020 2020 2020 2073 656c  alse.        sel
+0000ddb0: 662e 6578 706c 6169 6e5f 7265 7375 6c74  f.explain_result
+0000ddc0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000ddd0: 7365 6c66 2e6c 6973 745f 7265 7375 6c74  self.list_result
+0000dde0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000ddf0: 7365 6c66 2e5f 6275 6666 6572 7320 3d20  self._buffers = 
+0000de00: 5b5d 0a20 2020 2020 2020 2073 656c 662e  [].        self.
+0000de10: 5f6f 6666 7365 7420 3d20 300a 2020 2020  _offset = 0.    
+0000de20: 2020 2020 7365 6c66 2e5f 7065 6e64 696e      self._pendin
+0000de30: 675f 6f70 7320 3d20 5b5d 0a0a 2020 2020  g_ops = []..    
+0000de40: 6465 6620 7365 7469 6e70 7574 7369 7a65  def setinputsize
+0000de50: 7328 7365 6c66 2c20 7369 7a65 7329 3a0a  s(self, sizes):.
+0000de60: 2020 2020 2020 2020 2222 2254 6869 7320          """This 
+0000de70: 6361 6e20 6265 2075 7365 6420 6265 666f  can be used befo
+0000de80: 7265 2061 2063 616c 6c20 746f 202e 6578  re a call to .ex
+0000de90: 6563 7574 652a 2829 2074 6f20 7072 6564  ecute*() to pred
+0000dea0: 6566 696e 650a 2020 2020 2020 2020 6d65  efine.        me
+0000deb0: 6d6f 7279 2061 7265 6173 2066 6f72 2074  mory areas for t
+0000dec0: 6865 206f 7065 7261 7469 6f6e 2773 2070  he operation's p
+0000ded0: 6172 616d 6574 6572 732e 2043 7572 7265  arameters. Curre
+0000dee0: 6e74 6c79 2069 676e 6f72 6564 0a20 2020  ntly ignored.   
+0000def0: 2020 2020 2022 2222 0a0a 2020 2020 6465       """..    de
+0000df00: 6620 7365 746f 7574 7075 7473 697a 6528  f setoutputsize(
+0000df10: 7365 6c66 2c20 7369 7a65 2c20 636f 6c75  self, size, colu
+0000df20: 6d6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  mn=None):.      
+0000df30: 2020 2222 2253 6574 2061 2063 6f6c 756d    """Set a colum
+0000df40: 6e20 6275 6666 6572 2073 697a 6520 666f  n buffer size fo
+0000df50: 7220 6665 7463 6865 7320 6f66 206c 6172  r fetches of lar
+0000df60: 6765 2063 6f6c 756d 6e73 0a20 2020 2020  ge columns.     
+0000df70: 2020 2028 652e 672e 204c 4f4e 4773 2c20     (e.g. LONGs, 
+0000df80: 424c 4f42 732c 2065 7463 2e29 2e20 5468  BLOBs, etc.). Th
+0000df90: 6520 636f 6c75 6d6e 2069 7320 7370 6563  e column is spec
+0000dfa0: 6966 6965 6420 6173 2061 6e0a 2020 2020  ified as an.    
+0000dfb0: 2020 2020 696e 6465 7820 696e 746f 2074      index into t
+0000dfc0: 6865 2072 6573 756c 7420 7365 7175 656e  he result sequen
+0000dfd0: 6365 2e20 4375 7272 656e 746c 7920 6967  ce. Currently ig
+0000dfe0: 6e6f 7265 640a 2020 2020 2020 2020 2222  nored.        ""
+0000dff0: 220a 0a20 2020 2064 6566 2063 6c6f 7365  "..    def close
+0000e000: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000e010: 2222 2243 6c6f 7365 2074 6869 7320 6375  """Close this cu
+0000e020: 7273 6f72 2e20 2054 6865 2063 7572 7265  rsor.  The curre
+0000e030: 6e74 2072 6573 756c 7420 7365 7420 6973  nt result set is
+0000e040: 2063 6c6f 7365 642c 2062 7574 0a20 2020   closed, but.   
+0000e050: 2020 2020 2074 6865 2063 7572 736f 7220       the cursor 
+0000e060: 6361 6e20 6265 2072 6575 7365 6420 666f  can be reused fo
+0000e070: 7220 7375 6273 6571 7565 6e74 2065 7865  r subsequent exe
+0000e080: 6375 7465 2829 2063 616c 6c73 2e0a 2020  cute() calls..  
+0000e090: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000e0a0: 2020 6966 2073 656c 662e 5f62 7566 6665    if self._buffe
+0000e0b0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+0000e0c0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000e0d0: 2020 2020 2073 656c 662e 5f63 6c6f 7365       self._close
+0000e0e0: 5f72 6573 756c 7473 6574 2829 0a20 2020  _resultset().   
+0000e0f0: 2020 2020 2020 2020 2065 7863 6570 743a           except:
+0000e100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e110: 2070 6173 730a 0a20 2020 2020 2020 2073   pass..        s
+0000e120: 656c 662e 5f72 6569 6e69 7469 616c 697a  elf._reinitializ
+0000e130: 6528 290a 0a20 2020 2064 6566 2065 7865  e()..    def exe
+0000e140: 6375 7465 6d61 6e79 2873 656c 662c 206f  cutemany(self, o
+0000e150: 7065 7261 7469 6f6e 2c20 7061 7261 6d65  peration, parame
+0000e160: 7465 726c 6973 7429 3a0a 2020 2020 2020  terlist):.      
+0000e170: 2020 2222 2250 7265 7061 7265 2061 2064    """Prepare a d
+0000e180: 6174 6162 6173 6520 6f70 6572 6174 696f  atabase operatio
+0000e190: 6e20 2871 7565 7279 206f 7220 636f 6d6d  n (query or comm
+0000e1a0: 616e 6429 2061 6e64 2074 6865 6e20 6578  and) and then ex
+0000e1b0: 6563 7574 6520 6974 2061 6761 696e 7374  ecute it against
+0000e1c0: 0a20 2020 2020 2020 2061 6c6c 2070 6172  .        all par
+0000e1d0: 616d 6574 6572 2073 6571 7565 6e63 6573  ameter sequences
+0000e1e0: 206f 7220 6d61 7070 696e 6773 2066 6f75   or mappings fou
+0000e1f0: 6e64 2069 6e20 7468 6520 7365 7175 656e  nd in the sequen
+0000e200: 6365 2070 6172 616d 6574 6572 6c69 7374  ce parameterlist
+0000e210: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0000e220: 6574 6572 7320 6d61 7920 6265 2070 726f  eters may be pro
+0000e230: 7669 6465 6420 6173 2061 206d 6170 7069  vided as a mappi
+0000e240: 6e67 2061 6e64 2077 696c 6c20 6265 2062  ng and will be b
+0000e250: 6f75 6e64 2074 6f20 7661 7269 6162 6c65  ound to variable
+0000e260: 730a 2020 2020 2020 2020 696e 2074 6865  s.        in the
+0000e270: 206f 7065 7261 7469 6f6e 2e20 5661 7269   operation. Vari
+0000e280: 6162 6c65 7320 6172 6520 7370 6563 6966  ables are specif
+0000e290: 6965 6420 696e 2050 7974 686f 6e20 6578  ied in Python ex
+0000e2a0: 7465 6e64 6564 2066 6f72 6d61 7420 636f  tended format co
+0000e2b0: 6465 732c 0a20 2020 2020 2020 2065 2e67  des,.        e.g
+0000e2c0: 2e20 2e2e 2e57 4845 5245 206e 616d 653d  . ...WHERE name=
+0000e2d0: 2528 6e61 6d65 290a 2020 2020 2020 2020  %(name).        
+0000e2e0: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+0000e2f0: 2e5f 7265 696e 6974 6961 6c69 7a65 2829  ._reinitialize()
+0000e300: 0a0a 2020 2020 2020 2020 2320 7765 2063  ..        # we c
+0000e310: 616e 2774 206a 7573 7420 6578 6563 7574  an't just execut
+0000e320: 6520 616c 6c20 7468 6520 7175 6572 6965  e all the querie
+0000e330: 7320 6174 206f 6e63 652e 2e2e 2e6f 6369  s at once....oci
+0000e340: 656e 7420 6f6e 6c79 2061 6c6c 6f77 730a  ent only allows.
+0000e350: 2020 2020 2020 2020 2320 6f6e 6520 7175          # one qu
+0000e360: 6572 7920 6174 2061 2074 696d 6520 6f6e  ery at a time on
+0000e370: 2061 2063 6f6e 6e65 6374 696f 6e2e 2020   a connection.  
+0000e380: 536f 2071 7565 7565 2075 7020 616c 6c20  So queue up all 
+0000e390: 7468 6520 7175 6572 6965 7320 616e 640a  the queries and.
+0000e3a0: 2020 2020 2020 2020 2320 7765 276c 6c20          # we'll 
+0000e3b0: 6361 6c6c 2074 6865 6d20 6c61 7465 720a  call them later.
+0000e3c0: 2020 2020 2020 2020 666f 7220 7061 7261          for para
+0000e3d0: 6d20 696e 2070 6172 616d 6574 6572 6c69  m in parameterli
+0000e3e0: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+0000e3f0: 7365 6c66 2e5f 7065 6e64 696e 675f 6f70  self._pending_op
+0000e400: 732e 6170 7065 6e64 286f 7065 7261 7469  s.append(operati
+0000e410: 6f6e 2025 2070 6172 616d 290a 0a20 2020  on % param)..   
+0000e420: 2020 2020 2069 6620 7365 6c66 2e5f 7065       if self._pe
+0000e430: 6e64 696e 675f 6f70 733a 0a20 2020 2020  nding_ops:.     
+0000e440: 2020 2020 2020 2073 656c 662e 5f65 7865         self._exe
+0000e450: 6375 7465 5f69 6e74 6572 6e61 6c28 7365  cute_internal(se
+0000e460: 6c66 2e5f 7065 6e64 696e 675f 6f70 732e  lf._pending_ops.
+0000e470: 706f 7028 3029 290a 0a20 2020 2020 2020  pop(0))..       
+0000e480: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
+0000e490: 2020 6465 6620 6578 6563 7574 6528 7365    def execute(se
+0000e4a0: 6c66 2c20 6f70 6572 6174 696f 6e2c 2070  lf, operation, p
+0000e4b0: 6172 616d 6574 6572 733d 4e6f 6e65 293a  arameters=None):
+0000e4c0: 0a20 2020 2020 2020 2022 2222 5072 6570  .        """Prep
+0000e4d0: 6172 6520 616e 6420 6578 6563 7574 6520  are and execute 
+0000e4e0: 6120 6461 7461 6261 7365 206f 7065 7261  a database opera
+0000e4f0: 7469 6f6e 2028 7175 6572 7920 6f72 2063  tion (query or c
+0000e500: 6f6d 6d61 6e64 292e 0a0a 2020 2020 2020  ommand)...      
+0000e510: 2020 5061 7261 6d65 7465 7273 206d 6179    Parameters may
+0000e520: 2062 6520 7072 6f76 6964 6564 2061 7320   be provided as 
+0000e530: 6120 6d61 7070 696e 6720 616e 6420 7769  a mapping and wi
+0000e540: 6c6c 2062 6520 626f 756e 6420 746f 2076  ll be bound to v
+0000e550: 6172 6961 626c 6573 0a20 2020 2020 2020  ariables.       
+0000e560: 2069 6e20 7468 6520 6f70 6572 6174 696f   in the operatio
+0000e570: 6e2e 2056 6172 6961 626c 6573 2061 7265  n. Variables are
+0000e580: 2073 7065 6369 6669 6564 2069 6e20 5079   specified in Py
+0000e590: 7468 6f6e 2065 7874 656e 6465 6420 666f  thon extended fo
+0000e5a0: 726d 6174 2063 6f64 6573 2c0a 2020 2020  rmat codes,.    
+0000e5b0: 2020 2020 652e 672e 202e 2e2e 5748 4552      e.g. ...WHER
+0000e5c0: 4520 6e61 6d65 3d25 286e 616d 6529 0a20  E name=%(name). 
+0000e5d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000e5e0: 2020 2073 656c 662e 5f72 6569 6e69 7469     self._reiniti
+0000e5f0: 616c 697a 6528 290a 2020 2020 2020 2020  alize().        
+0000e600: 7365 6c66 2e5f 6578 6563 7574 655f 696e  self._execute_in
+0000e610: 7465 726e 616c 286f 7065 7261 7469 6f6e  ternal(operation
+0000e620: 2c20 7061 7261 6d65 7465 7273 290a 0a20  , parameters).. 
+0000e630: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000e640: 6c66 0a0a 2020 2020 6465 6620 5f65 7865  lf..    def _exe
+0000e650: 6375 7465 5f69 6e74 6572 6e61 6c28 7365  cute_internal(se
+0000e660: 6c66 2c20 6f70 6572 6174 696f 6e2c 2070  lf, operation, p
+0000e670: 6172 616d 6574 6572 733d 4e6f 6e65 293a  arameters=None):
+0000e680: 0a20 2020 2020 2020 2022 2222 496e 7465  .        """Inte
+0000e690: 726e 616c 2065 7865 6375 7465 2072 6f75  rnal execute rou
+0000e6a0: 7469 6e65 2074 6861 7420 6765 7473 2063  tine that gets c
+0000e6b0: 616c 6c65 6420 6672 6f6d 2065 7865 6375  alled from execu
+0000e6c0: 7465 2061 6e64 2065 7865 6375 7465 6d61  te and executema
+0000e6d0: 6e79 2222 220a 2020 2020 2020 2020 2320  ny""".        # 
+0000e6e0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+0000e6f0: 746f 6f2d 6d61 6e79 2d62 7261 6e63 6865  too-many-branche
+0000e700: 730a 0a20 2020 2020 2020 2069 6620 6861  s..        if ha
+0000e710: 7361 7474 7228 6f70 6572 6174 696f 6e2c  sattr(operation,
+0000e720: 2022 6465 636f 6465 2229 3a0a 2020 2020   "decode"):.    
+0000e730: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
+0000e740: 6e20 3d20 6f70 6572 6174 696f 6e2e 6465  n = operation.de
+0000e750: 636f 6465 2829 0a0a 2020 2020 2020 2020  code()..        
+0000e760: 6966 2070 6172 616d 6574 6572 7320 6973  if parameters is
+0000e770: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000e780: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+0000e790: 7228 6c69 7374 2870 6172 616d 6574 6572  r(list(parameter
+0000e7a0: 732e 6b65 7973 2829 295b 305d 2c20 2264  s.keys())[0], "d
+0000e7b0: 6563 6f64 6522 293a 0a20 2020 2020 2020  ecode"):.       
+0000e7c0: 2020 2020 2020 2020 2070 6172 616d 6574           paramet
+0000e7d0: 6572 7320 3d20 7b6b 6579 2e64 6563 6f64  ers = {key.decod
+0000e7e0: 6528 293a 2076 616c 7565 2066 6f72 2028  e(): value for (
+0000e7f0: 6b65 792c 2076 616c 7565 2920 696e 2070  key, value) in p
+0000e800: 6172 616d 6574 6572 732e 6974 656d 7328  arameters.items(
+0000e810: 297d 0a20 2020 2020 2020 2020 2020 206f  )}.            o
+0000e820: 7065 7261 7469 6f6e 203d 206f 7065 7261  peration = opera
+0000e830: 7469 6f6e 2025 2070 6172 616d 6574 6572  tion % parameter
+0000e840: 730a 0a20 2020 2020 2020 2023 2057 6520  s..        # We 
+0000e850: 6e65 6564 2074 6f20 6669 6775 7265 206f  need to figure o
+0000e860: 7574 2077 6865 7468 6572 2077 6520 7368  ut whether we sh
+0000e870: 6f75 6c64 2063 616c 6c0a 2020 2020 2020  ould call.      
+0000e880: 2020 2320 6578 6563 7574 655f 7175 6572    # execute_quer
+0000e890: 7920 6f72 2065 7865 6375 7465 5f75 7064  y or execute_upd
+0000e8a0: 6174 650a 2020 2020 2020 2020 7374 7269  ate.        stri
+0000e8b0: 7070 6564 203d 206f 7065 7261 7469 6f6e  pped = operation
+0000e8c0: 0a0a 2020 2020 2020 2020 2320 4c6f 6f70  ..        # Loop
+0000e8d0: 2075 6e74 696c 2077 6520 6861 7665 2073   until we have s
+0000e8e0: 6f6d 6520 7374 6172 7469 6e67 2077 6f72  ome starting wor
+0000e8f0: 6473 2e20 4e6f 7465 2074 6869 730a 2020  ds. Note this.  
+0000e900: 2020 2020 2020 2320 646f 6573 6e27 7420        # doesn't 
+0000e910: 6163 7475 616c 6c79 2068 616e 646c 6520  actually handle 
+0000e920: 7468 6520 6361 7365 206f 6620 2777 6f72  the case of 'wor
+0000e930: 6431 202f 2a20 636f 6d6d 656e 7420 2a2f  d1 /* comment */
+0000e940: 2077 6f72 6432 272c 0a20 2020 2020 2020   word2',.       
+0000e950: 2023 2062 7574 206e 6f6e 6520 6f66 2074   # but none of t
+0000e960: 6865 206f 7468 6572 2063 6c69 656e 7473  he other clients
+0000e970: 2064 6f20 6569 7468 6572 2e2e 2e0a 2020   do either....  
+0000e980: 2020 2020 2020 7768 696c 6520 5472 7565        while True
+0000e990: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000e9a0: 7374 7269 7020 6f66 6620 7374 6172 7469  strip off starti
+0000e9b0: 6e67 2073 7061 6365 730a 2020 2020 2020  ng spaces.      
+0000e9c0: 2020 2020 2020 7374 7269 7070 6564 203d        stripped =
+0000e9d0: 2073 7472 6970 7065 642e 6c73 7472 6970   stripped.lstrip
+0000e9e0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+0000e9f0: 2320 6966 2074 6869 7320 7374 6172 7473  # if this starts
+0000ea00: 2077 6974 6820 2d2d 2c20 7374 7269 7020   with --, strip 
+0000ea10: 7468 6520 7265 7374 206f 6620 7468 6520  the rest of the 
+0000ea20: 6c69 6e65 0a20 2020 2020 2020 2020 2020  line.           
+0000ea30: 2069 6620 7374 7269 7070 6564 2e73 7461   if stripped.sta
+0000ea40: 7274 7377 6974 6828 222d 2d22 293a 0a20  rtswith("--"):. 
+0000ea50: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000ea60: 6f73 203d 2073 7472 6970 7065 642e 6669  os = stripped.fi
+0000ea70: 6e64 2822 5c6e 2229 0a20 2020 2020 2020  nd("\n").       
+0000ea80: 2020 2020 2020 2020 2069 6620 706f 7320           if pos 
+0000ea90: 3d3d 202d 313a 0a20 2020 2020 2020 2020  == -1:.         
+0000eaa0: 2020 2020 2020 2020 2020 2073 7472 6970             strip
+0000eab0: 7065 6420 3d20 2222 0a20 2020 2020 2020  ped = "".       
+0000eac0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eae0: 2020 2073 7472 6970 7065 6420 3d20 7374     stripped = st
+0000eaf0: 7269 7070 6564 5b70 6f73 202b 2031 203a  ripped[pos + 1 :
+0000eb00: 5d0a 0a20 2020 2020 2020 2020 2020 2023  ]..            #
+0000eb10: 2069 6620 7468 6973 2073 7461 7274 7320   if this starts 
+0000eb20: 7769 7468 202f 2a2c 2073 7472 6970 2075  with /*, strip u
+0000eb30: 6e74 696c 202a 2f0a 2020 2020 2020 2020  ntil */.        
+0000eb40: 2020 2020 656c 6966 2073 7472 6970 7065      elif strippe
+0000eb50: 642e 7374 6172 7473 7769 7468 2822 2f2a  d.startswith("/*
+0000eb60: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+0000eb70: 2020 2020 706f 7320 3d20 7374 7269 7070      pos = stripp
+0000eb80: 6564 2e66 696e 6428 222a 2f22 290a 2020  ed.find("*/").  
+0000eb90: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000eba0: 2070 6f73 203d 3d20 2d31 3a0a 2020 2020   pos == -1:.    
+0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebc0: 7374 7269 7070 6564 203d 2022 220a 2020  stripped = "".  
+0000ebd0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000ebe0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000ebf0: 2020 2020 2020 2020 7374 7269 7070 6564          stripped
+0000ec00: 203d 2073 7472 6970 7065 645b 706f 7320   = stripped[pos 
+0000ec10: 2b20 3220 3a5d 0a20 2020 2020 2020 2020  + 2 :].         
+0000ec20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000ec30: 2020 2020 2020 2020 2023 2079 6179 2c20           # yay, 
+0000ec40: 6e6f 2063 6f6d 6d65 6e74 732c 206d 6f76  no comments, mov
+0000ec50: 6520 746f 2074 6865 206e 6578 7420 7068  e to the next ph
+0000ec60: 6173 650a 2020 2020 2020 2020 2020 2020  ase.            
+0000ec70: 2020 2020 6272 6561 6b0a 0a20 2020 2020      break..     
+0000ec80: 2020 2023 2069 6620 7765 2064 6f6e 2774     # if we don't
+0000ec90: 2068 6176 6520 616e 7974 6869 6e67 206c   have anything l
+0000eca0: 6566 742c 206a 7573 7420 7265 7475 726e  eft, just return
+0000ecb0: 205b 5d0a 2020 2020 2020 2020 6966 206e   [].        if n
+0000ecc0: 6f74 2073 7472 6970 7065 643a 0a20 2020  ot stripped:.   
+0000ecd0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000ece0: 0a20 2020 2020 2020 2023 206e 6f77 2073  .        # now s
+0000ecf0: 706c 6974 206f 7574 2074 6865 2077 6f72  plit out the wor
+0000ed00: 6473 0a20 2020 2020 2020 2077 6f72 6473  ds.        words
+0000ed10: 203d 2073 7472 6970 7065 642e 7370 6c69   = stripped.spli
+0000ed20: 7428 4e6f 6e65 2c20 3329 0a0a 2020 2020  t(None, 3)..    
+0000ed30: 2020 2020 2320 5369 6e67 6c65 2077 6f72      # Single wor
+0000ed40: 6420 6d61 7463 6865 730a 2020 2020 2020  d matches.      
+0000ed50: 2020 7175 6572 795f 7479 7065 203d 2077    query_type = w
+0000ed60: 6f72 6473 5b30 5d2e 7570 7065 7228 290a  ords[0].upper().
+0000ed70: 2020 2020 2020 2020 6966 2071 7565 7279          if query
+0000ed80: 5f74 7970 6520 696e 205b 2253 454c 4543  _type in ["SELEC
+0000ed90: 5422 2c20 2257 4954 4822 2c20 2245 5850  T", "WITH", "EXP
+0000eda0: 4f52 5422 2c20 2243 4845 434b 225d 3a0a  ORT", "CHECK"]:.
+0000edb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000edc0: 726e 2073 656c 662e 5f65 7865 6375 7465  rn self._execute
+0000edd0: 5f71 7565 7279 286f 7065 7261 7469 6f6e  _query(operation
+0000ede0: 3d6f 7065 7261 7469 6f6e 2c20 7175 6572  =operation, quer
+0000edf0: 795f 7479 7065 3d71 7565 7279 5f74 7970  y_type=query_typ
+0000ee00: 6529 0a20 2020 2020 2020 2065 6c69 6620  e).        elif 
+0000ee10: 7175 6572 795f 7479 7065 2069 6e20 5b22  query_type in ["
+0000ee20: 4558 504c 4149 4e22 5d3a 0a20 2020 2020  EXPLAIN"]:.     
+0000ee30: 2020 2020 2020 2023 2065 7870 6c61 696e         # explain
+0000ee40: 2070 6970 656c 696e 650a 2020 2020 2020   pipeline.      
+0000ee50: 2020 2020 2020 6966 206c 656e 2877 6f72        if len(wor
+0000ee60: 6473 2920 3e20 3120 616e 6420 776f 7264  ds) > 1 and word
+0000ee70: 735b 315d 2e75 7070 6572 2829 203d 3d20  s[1].upper() == 
+0000ee80: 2250 4950 454c 494e 4522 3a0a 2020 2020  "PIPELINE":.    
+0000ee90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000eea0: 726e 2073 656c 662e 5f65 7865 6375 7465  rn self._execute
+0000eeb0: 5f71 7565 7279 286f 7065 7261 7469 6f6e  _query(operation
+0000eec0: 3d6f 7065 7261 7469 6f6e 2c20 7175 6572  =operation, quer
+0000eed0: 795f 7479 7065 3d71 7565 7279 5f74 7970  y_type=query_typ
+0000eee0: 6520 2b20 2220 5049 5045 4c49 4e45 2229  e + " PIPELINE")
+0000eef0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000ef00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000ef10: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000ef20: 6578 6563 7574 655f 7175 6572 7928 6f70  execute_query(op
+0000ef30: 6572 6174 696f 6e3d 6f70 6572 6174 696f  eration=operatio
+0000ef40: 6e2c 2071 7565 7279 5f74 7970 653d 7175  n, query_type=qu
+0000ef50: 6572 795f 7479 7065 290a 2020 2020 2020  ery_type).      
+0000ef60: 2020 656c 6966 2071 7565 7279 5f74 7970    elif query_typ
+0000ef70: 6520 696e 205b 224c 4953 5422 5d3a 0a20  e in ["LIST"]:. 
+0000ef80: 2020 2020 2020 2020 2020 2069 6620 6f70             if op
+0000ef90: 6572 6174 696f 6e2e 7570 7065 7228 2920  eration.upper() 
+0000efa0: 3d3d 2022 4c49 5354 2041 4c4c 2051 5545  == "LIST ALL QUE
+0000efb0: 5249 4553 223a 0a20 2020 2020 2020 2020  RIES":.         
+0000efc0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000efd0: 6c66 2e5f 6578 6563 7574 655f 7175 6572  lf._execute_quer
+0000efe0: 7928 6f70 6572 6174 696f 6e3d 2253 454c  y(operation="SEL
+0000eff0: 4543 5420 2a20 4652 4f4d 2053 5953 2e51  ECT * FROM SYS.Q
+0000f000: 5545 5249 4553 222c 2071 7565 7279 5f74  UERIES", query_t
+0000f010: 7970 653d 2253 454c 4543 5422 290a 2020  ype="SELECT").  
+0000f020: 2020 2020 2020 2020 2020 656c 6966 206f            elif o
+0000f030: 7065 7261 7469 6f6e 2e75 7070 6572 2829  peration.upper()
+0000f040: 203d 3d20 224c 4953 5420 414c 4c20 434f   == "LIST ALL CO
+0000f050: 4d50 4c45 5445 4420 5155 4552 4945 5322  MPLETED QUERIES"
+0000f060: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f070: 2020 7265 7475 726e 2073 656c 662e 5f65    return self._e
+0000f080: 7865 6375 7465 5f71 7565 7279 286f 7065  xecute_query(ope
+0000f090: 7261 7469 6f6e 3d22 5345 4c45 4354 202a  ration="SELECT *
+0000f0a0: 2046 524f 4d20 5359 532e 434f 4d50 4c45   FROM SYS.COMPLE
+0000f0b0: 5445 445f 5155 4552 4945 5322 2c20 7175  TED_QUERIES", qu
+0000f0c0: 6572 795f 7479 7065 3d22 5345 4c45 4354  ery_type="SELECT
+0000f0d0: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
+0000f0e0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000f0f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000f100: 2e5f 6578 6563 7574 655f 6c69 7374 286f  ._execute_list(o
+0000f110: 7065 7261 7469 6f6e 3d6f 7065 7261 7469  peration=operati
+0000f120: 6f6e 290a 2020 2020 2020 2020 656c 6966  on).        elif
+0000f130: 2071 7565 7279 5f74 7970 6520 3d3d 2022   query_type == "
+0000f140: 464f 5243 4522 3a0a 2020 2020 2020 2020  FORCE":.        
+0000f150: 2020 2020 7365 6c66 2e5f 6578 6563 7574      self._execut
+0000f160: 655f 666f 7263 6528 6f70 6572 6174 696f  e_force(operatio
+0000f170: 6e3d 6f70 6572 6174 696f 6e29 0a20 2020  n=operation).   
+0000f180: 2020 2020 2065 6c69 6620 7175 6572 795f       elif query_
+0000f190: 7479 7065 203d 3d20 2253 4554 223a 0a20  type == "SET":. 
+0000f1a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f1b0: 5f65 7865 6375 7465 5f73 6574 2877 6f72  _execute_set(wor
+0000f1c0: 6473 5b31 3a5d 290a 2020 2020 2020 2020  ds[1:]).        
+0000f1d0: 656c 6966 2071 7565 7279 5f74 7970 6520  elif query_type 
+0000f1e0: 3d3d 2022 4745 5422 3a0a 2020 2020 2020  == "GET":.      
+0000f1f0: 2020 2020 2020 7365 6c66 2e5f 6578 6563        self._exec
+0000f200: 7574 655f 6765 7428 776f 7264 735b 313a  ute_get(words[1:
+0000f210: 5d29 0a20 2020 2020 2020 2065 6c69 6620  ]).        elif 
+0000f220: 7175 6572 795f 7479 7065 203d 3d20 224b  query_type == "K
+0000f230: 494c 4c22 206f 7220 7175 6572 795f 7479  ILL" or query_ty
+0000f240: 7065 203d 3d20 2243 414e 4345 4c22 3a0a  pe == "CANCEL":.
+0000f250: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f260: 2e5f 6578 6563 7574 655f 6361 6e63 656c  ._execute_cancel
+0000f270: 6b69 6c6c 2871 7565 7279 5f74 7970 652c  kill(query_type,
+0000f280: 2077 6f72 6473 5b31 3a5d 290a 2020 2020   words[1:]).    
+0000f290: 2020 2020 656c 6966 2071 7565 7279 5f74      elif query_t
+0000f2a0: 7970 6520 3d3d 2022 434c 4541 5222 3a0a  ype == "CLEAR":.
+0000f2b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f2c0: 2e5f 6578 6563 7574 655f 636c 6561 7228  ._execute_clear(
+0000f2d0: 776f 7264 735b 313a 5d29 0a20 2020 2020  words[1:]).     
+0000f2e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000f2f0: 2020 2020 2023 206f 6b2c 2074 6869 7320       # ok, this 
+0000f300: 6973 2061 6e20 7570 6461 7465 0a20 2020  is an update.   
+0000f310: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
+0000f320: 7865 6375 7465 5f75 7064 6174 6528 6f70  xecute_update(op
+0000f330: 6572 6174 696f 6e29 0a0a 2020 2020 6465  eration)..    de
+0000f340: 6620 7461 626c 6573 2873 656c 662c 2073  f tables(self, s
+0000f350: 6368 656d 613d 2225 222c 2074 6162 6c65  chema="%", table
+0000f360: 3d22 2522 293a 0a20 2020 2020 2020 2022  ="%"):.        "
+0000f370: 2222 4765 7420 7468 6520 6461 7461 6261  ""Get the databa
+0000f380: 7365 2074 6162 6c65 7322 2222 0a20 2020  se tables""".   
+0000f390: 2020 2020 2023 2070 796c 696e 743a 2064       # pylint: d
+0000f3a0: 6973 6162 6c65 3d6e 6f2d 6d65 6d62 6572  isable=no-member
+0000f3b0: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
+0000f3c0: 6574 6164 6174 615f 7265 7128 7072 6f74  etadata_req(prot
+0000f3d0: 6f2e 4665 7463 6853 7973 7465 6d4d 6574  o.FetchSystemMet
+0000f3e0: 6164 6174 612e 4745 545f 5441 424c 4553  adata.GET_TABLES
+0000f3f0: 2c20 7363 6865 6d61 3d73 6368 656d 612c  , schema=schema,
+0000f400: 2074 6162 6c65 3d74 6162 6c65 290a 2020   table=table).  
+0000f410: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000f420: 660a 0a20 2020 2064 6566 2073 7973 7465  f..    def syste
+0000f430: 6d5f 7461 626c 6573 2873 656c 662c 2074  m_tables(self, t
+0000f440: 6162 6c65 3d22 2522 293a 0a20 2020 2020  able="%"):.     
+0000f450: 2020 2022 2222 4765 7420 7468 6520 6461     """Get the da
+0000f460: 7461 6261 7365 2073 7973 7465 6d20 7461  tabase system ta
+0000f470: 626c 6573 2222 220a 2020 2020 2020 2020  bles""".        
+0000f480: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+0000f490: 653d 6e6f 2d6d 656d 6265 720a 2020 2020  e=no-member.    
+0000f4a0: 2020 2020 7365 6c66 2e5f 6d65 7461 6461      self._metada
+0000f4b0: 7461 5f72 6571 2870 726f 746f 2e46 6574  ta_req(proto.Fet
+0000f4c0: 6368 5379 7374 656d 4d65 7461 6461 7461  chSystemMetadata
+0000f4d0: 2e47 4554 5f53 5953 5445 4d5f 5441 424c  .GET_SYSTEM_TABL
+0000f4e0: 4553 2c20 7461 626c 653d 7461 626c 6529  ES, table=table)
+0000f4f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000f500: 7365 6c66 0a0a 2020 2020 6465 6620 7669  self..    def vi
+0000f510: 6577 7328 7365 6c66 2c20 7669 6577 3d22  ews(self, view="
+0000f520: 2522 293a 0a20 2020 2020 2020 2022 2222  %"):.        """
+0000f530: 4765 7420 7468 6520 6461 7461 6261 7365  Get the database
+0000f540: 2076 6965 7773 2222 220a 2020 2020 2020   views""".      
+0000f550: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
+0000f560: 626c 653d 6e6f 2d6d 656d 6265 720a 2020  ble=no-member.  
+0000f570: 2020 2020 2020 7365 6c66 2e5f 6d65 7461        self._meta
+0000f580: 6461 7461 5f72 6571 2870 726f 746f 2e46  data_req(proto.F
+0000f590: 6574 6368 5379 7374 656d 4d65 7461 6461  etchSystemMetada
+0000f5a0: 7461 2e47 4554 5f56 4945 5753 2c20 7669  ta.GET_VIEWS, vi
+0000f5b0: 6577 3d76 6965 7729 0a20 2020 2020 2020  ew=view).       
+0000f5c0: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
+0000f5d0: 2020 6465 6620 636f 6c75 6d6e 7328 7365    def columns(se
+0000f5e0: 6c66 2c20 7363 6865 6d61 3d22 2522 2c20  lf, schema="%", 
+0000f5f0: 7461 626c 653d 2225 222c 2063 6f6c 756d  table="%", colum
+0000f600: 6e3d 2225 2229 3a0a 2020 2020 2020 2020  n="%"):.        
+0000f610: 2222 2247 6574 2074 6865 2064 6174 6162  """Get the datab
+0000f620: 6173 6520 636f 6c75 6d6e 7322 2222 0a20  ase columns""". 
+0000f630: 2020 2020 2020 2023 2070 796c 696e 743a         # pylint:
+0000f640: 2064 6973 6162 6c65 3d6e 6f2d 6d65 6d62   disable=no-memb
+0000f650: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
+0000f660: 5f6d 6574 6164 6174 615f 7265 7128 7072  _metadata_req(pr
+0000f670: 6f74 6f2e 4665 7463 6853 7973 7465 6d4d  oto.FetchSystemM
+0000f680: 6574 6164 6174 612e 4745 545f 434f 4c55  etadata.GET_COLU
+0000f690: 4d4e 532c 2073 6368 656d 613d 7363 6865  MNS, schema=sche
+0000f6a0: 6d61 2c20 7461 626c 653d 7461 626c 652c  ma, table=table,
+0000f6b0: 2063 6f6c 756d 6e3d 636f 6c75 6d6e 290a   column=column).
+0000f6c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000f6d0: 656c 660a 0a20 2020 2064 6566 2069 6e64  elf..    def ind
+0000f6e0: 6578 6573 2873 656c 662c 2073 6368 656d  exes(self, schem
+0000f6f0: 613d 2225 222c 2074 6162 6c65 3d22 2522  a="%", table="%"
+0000f700: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
+0000f710: 7420 7468 6520 6461 7461 6261 7365 2069  t the database i
+0000f720: 6e64 6578 6573 2222 220a 2020 2020 2020  ndexes""".      
+0000f730: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
+0000f740: 626c 653d 6e6f 2d6d 656d 6265 720a 2020  ble=no-member.  
+0000f750: 2020 2020 2020 7365 6c66 2e5f 6d65 7461        self._meta
+0000f760: 6461 7461 5f72 6571 2870 726f 746f 2e46  data_req(proto.F
+0000f770: 6574 6368 5379 7374 656d 4d65 7461 6461  etchSystemMetada
+0000f780: 7461 2e47 4554 5f49 4e44 4558 4553 2c20  ta.GET_INDEXES, 
+0000f790: 7363 6865 6d61 3d73 6368 656d 612c 2074  schema=schema, t
+0000f7a0: 6162 6c65 3d74 6162 6c65 290a 2020 2020  able=table).    
+0000f7b0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0000f7c0: 0a20 2020 2064 6566 2067 6574 5479 7065  .    def getType
+0000f7d0: 496e 666f 2873 656c 6629 3a20 2023 2070  Info(self):  # p
+0000f7e0: 796c 696e 743a 2064 6973 6162 6c65 3d69  ylint: disable=i
+0000f7f0: 6e76 616c 6964 2d6e 616d 650a 2020 2020  nvalid-name.    
+0000f800: 2020 2020 2222 2247 6574 2074 6865 2064      """Get the d
+0000f810: 6174 6162 6173 6520 7479 7065 2069 6e66  atabase type inf
+0000f820: 6f22 2222 0a20 2020 2020 2020 2023 2070  o""".        # p
+0000f830: 796c 696e 743a 2064 6973 6162 6c65 3d6e  ylint: disable=n
+0000f840: 6f2d 6d65 6d62 6572 0a20 2020 2020 2020  o-member.       
+0000f850: 2073 656c 662e 5f6d 6574 6164 6174 615f   self._metadata_
+0000f860: 7265 7128 7072 6f74 6f2e 4665 7463 6853  req(proto.FetchS
+0000f870: 7973 7465 6d4d 6574 6164 6174 612e 4745  ystemMetadata.GE
+0000f880: 545f 5459 5045 5f49 4e46 4f29 0a20 2020  T_TYPE_INFO).   
+0000f890: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000f8a0: 0a0a 2020 2020 6465 6620 6765 7453 7973  ..    def getSys
+0000f8b0: 7465 6d56 6572 7369 6f6e 2873 656c 6629  temVersion(self)
+0000f8c0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0000f8d0: 2073 656c 662e 5f65 7865 6375 7465 5f73   self._execute_s
+0000f8e0: 7973 7465 6d6d 6574 6164 6174 6128 7072  ystemmetadata(pr
+0000f8f0: 6f74 6f2e 4665 7463 6853 7973 7465 6d4d  oto.FetchSystemM
+0000f900: 6574 6164 6174 612e 4745 545f 4441 5441  etadata.GET_DATA
+0000f910: 4241 5345 5f50 524f 4455 4354 5f56 4552  BASE_PRODUCT_VER
+0000f920: 5349 4f4e 290a 0a20 2020 2064 6566 205f  SION)..    def _
+0000f930: 6d65 7461 6461 7461 5f72 6571 2873 656c  metadata_req(sel
+0000f940: 662c 2072 6571 7479 7065 2c20 7363 6865  f, reqtype, sche
+0000f950: 6d61 3d22 2522 2c20 7461 626c 653d 2225  ma="%", table="%
+0000f960: 222c 2063 6f6c 756d 6e3d 2225 222c 2076  ", column="%", v
+0000f970: 6965 773d 2225 2229 3a0a 2020 2020 2020  iew="%"):.      
+0000f980: 2020 2222 2249 6e74 6572 6e61 6c20 6675    """Internal fu
+0000f990: 6e63 7469 6f6e 2074 6f20 6765 7420 6461  nction to get da
+0000f9a0: 7461 6261 7365 206d 6574 6164 6174 6122  tabase metadata"
+0000f9b0: 2222 0a20 2020 2020 2020 2023 2070 796c  "".        # pyl
+0000f9c0: 696e 743a 2064 6973 6162 6c65 3d6e 6f2d  int: disable=no-
+0000f9d0: 6d65 6d62 6572 2c74 6f6f 2d6d 616e 792d  member,too-many-
+0000f9e0: 6172 6775 6d65 6e74 730a 2020 2020 2020  arguments.      
+0000f9f0: 2020 7365 6c66 2e5f 7265 696e 6974 6961    self._reinitia
+0000fa00: 6c69 7a65 2829 0a20 2020 2020 2020 2023  lize().        #
+0000fa10: 2072 6571 2e66 6574 6368 5f73 7973 7465   req.fetch_syste
+0000fa20: 6d5f 6d65 7461 6461 7461 2e47 4554 5f54  m_metadata.GET_T
+0000fa30: 4142 4c45 530a 2020 2020 2020 2020 7265  ABLES.        re
+0000fa40: 7120 3d20 7072 6f74 6f2e 5265 7175 6573  q = proto.Reques
+0000fa50: 7428 290a 2020 2020 2020 2020 7265 712e  t().        req.
+0000fa60: 7479 7065 203d 2072 6571 2e46 4554 4348  type = req.FETCH
+0000fa70: 5f53 5953 5445 4d5f 4d45 5441 4441 5441  _SYSTEM_METADATA
+0000fa80: 0a20 2020 2020 2020 2072 6571 2e66 6574  .        req.fet
+0000fa90: 6368 5f73 7973 7465 6d5f 6d65 7461 6461  ch_system_metada
+0000faa0: 7461 2e63 616c 6c20 3d20 7265 7174 7970  ta.call = reqtyp
+0000fab0: 650a 2020 2020 2020 2020 7265 712e 6665  e.        req.fe
+0000fac0: 7463 685f 7379 7374 656d 5f6d 6574 6164  tch_system_metad
+0000fad0: 6174 612e 7363 6865 6d61 203d 2073 6368  ata.schema = sch
+0000fae0: 656d 610a 2020 2020 2020 2020 7265 712e  ema.        req.
+0000faf0: 6665 7463 685f 7379 7374 656d 5f6d 6574  fetch_system_met
+0000fb00: 6164 6174 612e 7461 626c 6520 3d20 7461  adata.table = ta
+0000fb10: 626c 650a 2020 2020 2020 2020 7265 712e  ble.        req.
+0000fb20: 6665 7463 685f 7379 7374 656d 5f6d 6574  fetch_system_met
+0000fb30: 6164 6174 612e 636f 6c75 6d6e 203d 2063  adata.column = c
+0000fb40: 6f6c 756d 6e0a 2020 2020 2020 2020 7265  olumn.        re
+0000fb50: 712e 6665 7463 685f 7379 7374 656d 5f6d  q.fetch_system_m
+0000fb60: 6574 6164 6174 612e 7669 6577 203d 2076  etadata.view = v
+0000fb70: 6965 770a 2020 2020 2020 2020 7265 712e  iew.        req.
+0000fb80: 6665 7463 685f 7379 7374 656d 5f6d 6574  fetch_system_met
+0000fb90: 6164 6174 612e 7465 7374 203d 2054 7275  adata.test = Tru
+0000fba0: 650a 0a20 2020 2020 2020 205f 7365 6e64  e..        _send
+0000fbb0: 5f6d 7367 2873 656c 662e 636f 6e6e 6563  _msg(self.connec
+0000fbc0: 7469 6f6e 2c20 7265 7129 0a0a 2020 2020  tion, req)..    
+0000fbd0: 2020 2020 7273 7020 3d20 5f72 6563 765f      rsp = _recv_
+0000fbe0: 6d73 6728 7365 6c66 2e63 6f6e 6e65 6374  msg(self.connect
+0000fbf0: 696f 6e2c 2070 726f 746f 2e46 6574 6368  ion, proto.Fetch
+0000fc00: 5379 7374 656d 4d65 7461 6461 7461 5265  SystemMetadataRe
+0000fc10: 7370 6f6e 7365 2829 290a 0a20 2020 2020  sponse())..     
+0000fc20: 2020 2069 6620 7273 702e 7265 7370 6f6e     if rsp.respon
+0000fc30: 7365 2e74 7970 6520 3d3d 2070 726f 746f  se.type == proto
+0000fc40: 2e43 6f6e 6669 726d 6174 696f 6e52 6573  .ConfirmationRes
+0000fc50: 706f 6e73 652e 5245 5350 4f4e 5345 5f45  ponse.RESPONSE_E
+0000fc60: 5252 4f52 3a0a 2020 2020 2020 2020 2020  RROR:.          
+0000fc70: 2020 6966 2072 7370 2e72 6573 706f 6e73    if rsp.respons
+0000fc80: 652e 7665 6e64 6f72 5f63 6f64 6520 3d3d  e.vendor_code ==
+0000fc90: 2053 4553 5349 4f4e 5f45 5850 4952 4544   SESSION_EXPIRED
+0000fca0: 5f43 4f44 453a 0a20 2020 2020 2020 2020  _CODE:.         
+0000fcb0: 2020 2020 2020 2023 204e 6565 6420 746f         # Need to
+0000fcc0: 2072 6566 7265 7368 2074 6865 2073 6573   refresh the ses
+0000fcd0: 7369 6f6e 0a20 2020 2020 2020 2020 2020  sion.           
+0000fce0: 2020 2020 2073 656c 662e 636f 6e6e 6563       self.connec
+0000fcf0: 7469 6f6e 2e72 6566 7265 7368 2829 0a20  tion.refresh(). 
+0000fd00: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000fd10: 2061 6e64 2074 7279 2061 6761 696e 0a20   and try again. 
+0000fd20: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+0000fd30: 6d65 7461 6461 7461 5f72 6571 2872 6571  metadata_req(req
+0000fd40: 7479 7065 2c20 7363 6865 6d61 3d73 6368  type, schema=sch
+0000fd50: 656d 612c 2074 6162 6c65 3d74 6162 6c65  ema, table=table
+0000fd60: 2c20 636f 6c75 6d6e 3d63 6f6c 756d 6e2c  , column=column,
+0000fd70: 2076 6965 773d 7669 6577 290a 2020 2020   view=view).    
+0000fd80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000fd90: 726e 0a20 2020 2020 2020 2020 2020 2065  rn.            e
+0000fda0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000fdb0: 2020 2020 2072 6169 7365 205f 636f 6e76       raise _conv
+0000fdc0: 6572 745f 6578 6365 7074 696f 6e28 7273  ert_exception(rs
+0000fdd0: 702e 7265 7370 6f6e 7365 290a 0a20 2020  p.response)..   
+0000fde0: 2020 2020 2073 656c 662e 5f67 6574 5f72       self._get_r
+0000fdf0: 6573 756c 745f 6d65 7461 6461 7461 2829  esult_metadata()
+0000fe00: 0a0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
+0000fe10: 6f77 6e75 6d62 6572 203d 2030 0a20 2020  ownumber = 0.   
+0000fe20: 2020 2020 2066 6f72 2062 6c6f 6220 696e       for blob in
+0000fe30: 2072 7370 2e72 6573 756c 745f 7365 745f   rsp.result_set_
+0000fe40: 7661 6c2e 626c 6f62 733a 0a20 2020 2020  val.blobs:.     
+0000fe50: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0000fe60: 6c66 2e5f 6275 6666 6572 733a 0a20 2020  lf._buffers:.   
+0000fe70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fe80: 662e 5f6f 6666 7365 7420 3d20 300a 2020  f._offset = 0.  
+0000fe90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000fea0: 6275 6666 6572 732e 6170 7065 6e64 2862  buffers.append(b
+0000feb0: 6c6f 6229 0a0a 2020 2020 6465 6620 5f65  lob)..    def _e
+0000fec0: 7865 6375 7465 5f71 7565 7279 2873 656c  xecute_query(sel
+0000fed0: 662c 206f 7065 7261 7469 6f6e 2c20 7175  f, operation, qu
+0000fee0: 6572 795f 7479 7065 3a20 7374 7220 3d20  ery_type: str = 
+0000fef0: 2253 454c 4543 5422 293a 0a20 2020 2020  "SELECT"):.     
+0000ff00: 2020 2022 2222 4578 6563 7574 6520 6120     """Execute a 
+0000ff10: 7175 6572 7922 2222 0a20 2020 2020 2020  query""".       
+0000ff20: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+0000ff30: 6c65 3d6e 6f2d 6d65 6d62 6572 0a0a 2020  le=no-member..  
+0000ff40: 2020 2020 2020 6661 6374 6f72 7920 3d20        factory = 
+0000ff50: 5f4f 4349 454e 545f 5245 5155 4553 545f  _OCIENT_REQUEST_
+0000ff60: 4641 4354 4f52 4945 532e 6765 7428 7175  FACTORIES.get(qu
+0000ff70: 6572 795f 7479 7065 2e75 7070 6572 2829  ery_type.upper()
+0000ff80: 2c20 4e6f 6e65 290a 0a20 2020 2020 2020  , None)..       
+0000ff90: 2069 6620 6661 6374 6f72 7920 6973 204e   if factory is N
+0000ffa0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000ffb0: 2072 6169 7365 204e 6f74 5375 7070 6f72   raise NotSuppor
+0000ffc0: 7465 6445 7272 6f72 2866 2251 7565 7279  tedError(f"Query
+0000ffd0: 2074 7970 6520 277b 7175 6572 795f 7479   type '{query_ty
+0000ffe0: 7065 7d27 206e 6f74 2073 7570 706f 7274  pe}' not support
+0000fff0: 6564 2062 7920 7079 6f63 6965 6e74 2722  ed by pyocient'"
+00010000: 290a 0a20 2020 2020 2020 2023 2067 656e  )..        # gen
+00010010: 6572 6174 6520 7468 6520 6170 7072 6f70  erate the approp
+00010020: 7269 6174 6520 7265 7175 6573 740a 2020  riate request.  
+00010030: 2020 2020 2020 7265 7120 3d20 6661 6374        req = fact
+00010040: 6f72 792e 7265 7175 6573 7428 6f70 6572  ory.request(oper
+00010050: 6174 696f 6e29 0a0a 2020 2020 2020 2020  ation)..        
+00010060: 2320 4c6f 6f70 2077 6869 6c65 2077 6520  # Loop while we 
+00010070: 7265 7472 7920 7265 6469 7265 6374 7320  retry redirects 
+00010080: 616e 6420 7265 636f 6e6e 6563 7473 0a20  and reconnects. 
+00010090: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
+000100a0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+000100b0: 6620 7265 712e 7479 7065 203d 3d20 7072  f req.type == pr
+000100c0: 6f74 6f2e 5265 7175 6573 742e 5265 7175  oto.Request.Requ
+000100d0: 6573 7454 7970 652e 5661 6c75 6528 2245  estType.Value("E
+000100e0: 5845 4355 5445 5f51 5545 5259 2229 3a0a  XECUTE_QUERY"):.
+000100f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010100: 7265 712e 6578 6563 7574 655f 7175 6572  req.execute_quer
+00010110: 792e 666f 7263 6520 3d20 7365 6c66 2e63  y.force = self.c
+00010120: 6f6e 6e65 6374 696f 6e2e 666f 7263 650a  onnection.force.
+00010130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010140: 7265 712e 6578 6563 7574 655f 7175 6572  req.execute_quer
+00010150: 792e 666f 7263 6552 6564 6972 6563 7420  y.forceRedirect 
+00010160: 3d20 7365 6c66 2e63 6f6e 6e65 6374 696f  = self.connectio
+00010170: 6e2e 666f 7263 655f 6e65 7874 5f72 6564  n.force_next_red
+00010180: 6972 6563 740a 2020 2020 2020 2020 2020  irect.          
+00010190: 2020 2020 2020 7365 6c66 2e63 6f6e 6e65        self.conne
+000101a0: 6374 696f 6e2e 666f 7263 655f 6e65 7874  ction.force_next
+000101b0: 5f72 6564 6972 6563 7420 3d20 4661 6c73  _redirect = Fals
+000101c0: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
+000101d0: 6966 2072 6571 2e74 7970 6520 3d3d 2070  if req.type == p
+000101e0: 726f 746f 2e52 6571 7565 7374 2e52 6571  roto.Request.Req
+000101f0: 7565 7374 5479 7065 2e56 616c 7565 2822  uestType.Value("
+00010200: 4558 4543 5554 455f 4558 504c 4149 4e22  EXECUTE_EXPLAIN"
+00010210: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00010220: 2020 2072 6571 2e65 7865 6375 7465 5f65     req.execute_e
+00010230: 7870 6c61 696e 2e66 6f72 6365 203d 2073  xplain.force = s
+00010240: 656c 662e 636f 6e6e 6563 7469 6f6e 2e66  elf.connection.f
+00010250: 6f72 6365 0a20 2020 2020 2020 2020 2020  orce.           
+00010260: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00010270: 2020 2020 2020 5f73 656e 645f 6d73 6728        _send_msg(
+00010280: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2c  self.connection,
+00010290: 2072 6571 290a 0a20 2020 2020 2020 2020   req)..         
+000102a0: 2020 2020 2020 2072 7370 203d 205f 7265         rsp = _re
+000102b0: 6376 5f6d 7367 2873 656c 662e 636f 6e6e  cv_msg(self.conn
+000102c0: 6563 7469 6f6e 2c20 6661 6374 6f72 792e  ection, factory.
+000102d0: 7265 7370 6f6e 7365 2829 290a 2020 2020  response()).    
+000102e0: 2020 2020 2020 2020 6578 6365 7074 2049          except I
+000102f0: 4f45 7272 6f72 3a0a 2020 2020 2020 2020  OError:.        
+00010300: 2020 2020 2020 2020 2320 7265 6d61 6b65          # remake
+00010310: 206f 7572 2063 6f6e 6e65 6374 696f 6e0a   our connection.
+00010320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010330: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e20  self.connection 
+00010340: 3d20 436f 6e6e 6563 7469 6f6e 280a 2020  = Connection(.  
+00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010360: 2020 7573 6572 3d73 656c 662e 636f 6e6e    user=self.conn
+00010370: 6563 7469 6f6e 2e75 7365 722c 0a20 2020  ection.user,.   
+00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010390: 2070 6173 7377 6f72 643d 7365 6c66 2e63   password=self.c
+000103a0: 6f6e 6e65 6374 696f 6e2e 7061 7373 776f  onnection.passwo
+000103b0: 7264 2c0a 2020 2020 2020 2020 2020 2020  rd,.            
+000103c0: 2020 2020 2020 2020 686f 7374 3d66 227b          host=f"{
+000103d0: 272c 272e 6a6f 696e 2873 656c 662e 636f  ','.join(self.co
+000103e0: 6e6e 6563 7469 6f6e 2e68 6f73 7473 297d  nnection.hosts)}
+000103f0: 3a7b 7365 6c66 2e63 6f6e 6e65 6374 696f  :{self.connectio
+00010400: 6e2e 706f 7274 7d22 2c0a 2020 2020 2020  n.port}",.      
+00010410: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00010420: 7461 6261 7365 3d73 656c 662e 636f 6e6e  tabase=self.conn
+00010430: 6563 7469 6f6e 2e64 6174 6162 6173 652c  ection.database,
+00010440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010450: 2020 2020 2074 6c73 3d73 656c 662e 636f       tls=self.co
+00010460: 6e6e 6563 7469 6f6e 2e74 6c73 2c0a 2020  nnection.tls,.  
+00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010480: 2020 6861 6e64 7368 616b 653d 7365 6c66    handshake=self
+00010490: 2e63 6f6e 6e65 6374 696f 6e2e 6861 6e64  .connection.hand
+000104a0: 7368 616b 652c 0a20 2020 2020 2020 2020  shake,.         
+000104b0: 2020 2020 2020 2020 2020 2066 6f72 6365             force
+000104c0: 3d73 656c 662e 636f 6e6e 6563 7469 6f6e  =self.connection
+000104d0: 2e66 6f72 6365 2c0a 2020 2020 2020 2020  .force,.        
+000104e0: 2020 2020 2020 2020 2020 2020 7365 7373              sess
+000104f0: 696f 6e3d 7365 6c66 2e63 6f6e 6e65 6374  ion=self.connect
+00010500: 696f 6e2e 7365 7373 696f 6e2c 0a20 2020  ion.session,.   
+00010510: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010530: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
+00010540: 2020 2020 2020 6966 2072 7370 2e72 6573        if rsp.res
+00010550: 706f 6e73 652e 7479 7065 203d 3d20 7072  ponse.type == pr
+00010560: 6f74 6f2e 436f 6e66 6972 6d61 7469 6f6e  oto.Confirmation
+00010570: 5265 7370 6f6e 7365 2e52 4553 504f 4e53  Response.RESPONS
+00010580: 455f 5741 524e 3a0a 2020 2020 2020 2020  E_WARN:.        
+00010590: 2020 2020 2020 2020 7761 726e 2872 7370          warn(rsp
+000105a0: 2e72 6573 706f 6e73 652e 7265 6173 6f6e  .response.reason
+000105b0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+000105c0: 6966 206e 6f74 2072 7370 2e72 6573 706f  if not rsp.respo
+000105d0: 6e73 652e 7479 7065 203d 3d20 7072 6f74  nse.type == prot
+000105e0: 6f2e 436f 6e66 6972 6d61 7469 6f6e 5265  o.ConfirmationRe
+000105f0: 7370 6f6e 7365 2e52 4553 504f 4e53 455f  sponse.RESPONSE_
+00010600: 4f4b 3a0a 2020 2020 2020 2020 2020 2020  OK:.            
+00010610: 2020 2020 6966 2072 7370 2e72 6573 706f      if rsp.respo
+00010620: 6e73 652e 7665 6e64 6f72 5f63 6f64 6520  nse.vendor_code 
+00010630: 3d3d 2053 4553 5349 4f4e 5f45 5850 4952  == SESSION_EXPIR
+00010640: 4544 5f43 4f44 453a 0a20 2020 2020 2020  ED_CODE:.       
+00010650: 2020 2020 2020 2020 2020 2020 2023 204e               # N
+00010660: 6565 6420 746f 2072 6566 7265 7368 2074  eed to refresh t
+00010670: 6865 2073 6573 7369 6f6e 0a20 2020 2020  he session.     
+00010680: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010690: 656c 662e 636f 6e6e 6563 7469 6f6e 2e72  elf.connection.r
+000106a0: 6566 7265 7368 2829 0a20 2020 2020 2020  efresh().       
+000106b0: 2020 2020 2020 2020 2020 2020 2023 2061               # a
+000106c0: 6e64 2074 7279 2061 6761 696e 0a20 2020  nd try again.   
+000106d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106e0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+000106f0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010710: 2020 2020 7261 6973 6520 5f63 6f6e 7665      raise _conve
+00010720: 7274 5f65 7863 6570 7469 6f6e 2872 7370  rt_exception(rsp
+00010730: 2e72 6573 706f 6e73 6529 0a0a 2020 2020  .response)..    
+00010740: 2020 2020 2020 2020 2320 7365 6520 6966          # see if
+00010750: 2077 6520 6172 6520 6265 696e 6720 746f   we are being to
+00010760: 6c64 2074 6f20 7265 6469 7265 6374 0a20  ld to redirect. 
+00010770: 2020 2020 2020 2020 2020 2072 6564 6972             redir
+00010780: 6563 7420 3d20 6765 7461 7474 7228 7273  ect = getattr(rs
+00010790: 702c 2022 7265 6469 7265 6374 222c 2046  p, "redirect", F
+000107a0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+000107b0: 2020 6966 206e 6f74 2072 6564 6972 6563    if not redirec
+000107c0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+000107d0: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
+000107e0: 2020 2020 2020 2320 7265 6d61 6b65 206f        # remake o
+000107f0: 7572 2063 6f6e 6e65 6374 696f 6e0a 2020  ur connection.  
+00010800: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00010810: 6f6e 6e65 6374 696f 6e2e 636c 6f73 6528  onnection.close(
+00010820: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00010830: 6c66 2e63 6f6e 6e65 6374 696f 6e20 3d20  lf.connection = 
+00010840: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2e  self.connection.
+00010850: 7265 6469 7265 6374 2872 7370 2e72 6564  redirect(rsp.red
+00010860: 6972 6563 7448 6f73 742c 2072 7370 2e72  irectHost, rsp.r
+00010870: 6564 6972 6563 7450 6f72 7429 0a0a 2020  edirectPort)..  
+00010880: 2020 2020 2020 7175 6572 795f 6964 203d        query_id =
+00010890: 2067 6574 6174 7472 2872 7370 2c20 2271   getattr(rsp, "q
+000108a0: 7565 7279 4964 222c 204e 6f6e 6529 0a20  ueryId", None). 
+000108b0: 2020 2020 2020 2069 6620 7175 6572 795f         if query_
+000108c0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+000108d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000108e0: 2e71 7565 7279 5f69 6420 3d20 7175 6572  .query_id = quer
+000108f0: 795f 6964 0a0a 2020 2020 2020 2020 7365  y_id..        se
+00010900: 6c66 2e72 6f77 6e75 6d62 6572 203d 2030  lf.rownumber = 0
+00010910: 0a0a 2020 2020 2020 2020 6966 2071 7565  ..        if que
+00010920: 7279 5f74 7970 6520 696e 205b 2253 454c  ry_type in ["SEL
+00010930: 4543 5422 2c20 2257 4954 4822 5d3a 0a20  ECT", "WITH"]:. 
+00010940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010950: 5f67 6574 5f72 6573 756c 745f 6d65 7461  _get_result_meta
+00010960: 6461 7461 2829 0a0a 2020 2020 2020 2020  data()..        
+00010970: 656c 6966 2071 7565 7279 5f74 7970 6520  elif query_type 
+00010980: 3d3d 2022 4558 504c 4149 4e22 3a0a 2020  == "EXPLAIN":.  
+00010990: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+000109a0: 6573 6372 6970 7469 6f6e 203d 205b 2822  escription = [("
+000109b0: 6578 706c 6169 6e22 2c20 5479 7065 436f  explain", TypeCo
+000109c0: 6465 732e 4348 4152 2c20 4e6f 6e65 2c20  des.CHAR, None, 
+000109d0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
+000109e0: 2c20 4e6f 6e65 295d 2020 2320 6469 7370  , None)]  # disp
+000109f0: 6c61 795f 7369 7a65 2020 2320 696e 7465  lay_size  # inte
+00010a00: 726e 616c 5f73 697a 6520 2023 2070 7265  rnal_size  # pre
+00010a10: 6369 7369 6f6e 2020 2320 7363 616c 6520  cision  # scale 
+00010a20: 2023 206e 756c 6c5f 6f6b 0a0a 2020 2020   # null_ok..    
+00010a30: 2020 2020 2020 2020 7365 6c66 2e65 7870          self.exp
+00010a40: 6c61 696e 5f72 6573 756c 7420 3d20 7273  lain_result = rs
+00010a50: 702e 706c 616e 0a0a 2020 2020 2320 4166  p.plan..    # Af
+00010a60: 7465 7220 6c69 7374 2061 6c6c 2071 7565  ter list all que
+00010a70: 7269 6573 2061 6e64 206c 6973 7420 616c  ries and list al
+00010a80: 6c20 636f 6d70 6c65 7465 6420 7175 6572  l completed quer
+00010a90: 6965 7320 6861 7665 2062 6565 6e20 7265  ies have been re
+00010aa0: 6d61 7070 6564 2c20 7468 6973 2069 7320  mapped, this is 
+00010ab0: 6e6f 206c 6f6e 6765 7220 7573 6564 2e20  no longer used. 
+00010ac0: 4275 7420 6974 2063 616e 2062 6520 7573  But it can be us
+00010ad0: 6564 2066 6f72 206f 7468 6572 2074 6869  ed for other thi
+00010ae0: 6e67 732e 0a20 2020 2023 2045 783a 206c  ngs..    # Ex: l
+00010af0: 6973 7420 7461 626c 6573 2c20 6c69 7374  ist tables, list
+00010b00: 2076 6965 7773 2c20 6c69 7374 2074 6162   views, list tab
+00010b10: 6c65 2070 7269 7669 6c65 6765 732e 204e  le privileges. N
+00010b20: 6f6e 6520 6f66 2074 6865 7365 2061 7265  one of these are
+00010b30: 2069 6d70 6c65 6d65 6e74 6564 2079 6574   implemented yet
+00010b40: 2e0a 2020 2020 6465 6620 5f65 7865 6375  ..    def _execu
+00010b50: 7465 5f6c 6973 7428 7365 6c66 2c20 6f70  te_list(self, op
+00010b60: 6572 6174 696f 6e3a 2073 7472 203d 2022  eration: str = "
+00010b70: 4c49 5354 2041 4c4c 2051 5545 5249 4553  LIST ALL QUERIES
+00010b80: 2229 3a0a 2020 2020 2020 2020 2222 2245  "):.        """E
+00010b90: 7865 6375 7465 204c 4953 545f 414c 4c5f  xecute LIST_ALL_
+00010ba0: 5155 4552 4945 5322 2222 0a20 2020 2020  QUERIES""".     
+00010bb0: 2020 2023 2070 796c 696e 743a 2064 6973     # pylint: dis
+00010bc0: 6162 6c65 3d6e 6f2d 6d65 6d62 6572 0a0a  able=no-member..
+00010bd0: 2020 2020 2020 2020 6661 6374 6f72 7920          factory 
+00010be0: 3d20 5f4f 4349 454e 545f 5245 5155 4553  = _OCIENT_REQUES
+00010bf0: 545f 4641 4354 4f52 4945 532e 6765 7428  T_FACTORIES.get(
+00010c00: 6f70 6572 6174 696f 6e2e 7570 7065 7228  operation.upper(
+00010c10: 292c 204e 6f6e 6529 0a0a 2020 2020 2020  ), None)..      
+00010c20: 2020 6966 2066 6163 746f 7279 2069 7320    if factory is 
+00010c30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00010c40: 2020 7261 6973 6520 4e6f 7453 7570 706f    raise NotSuppo
+00010c50: 7274 6564 4572 726f 7228 6622 4c69 7374  rtedError(f"List
+00010c60: 2071 7565 7279 2027 7b6f 7065 7261 7469   query '{operati
+00010c70: 6f6e 7d27 206e 6f74 2073 7570 706f 7274  on}' not support
+00010c80: 6564 2062 7920 7079 6f63 6965 6e74 2722  ed by pyocient'"
+00010c90: 290a 0a20 2020 2020 2020 2023 2067 6565  )..        # gee
+00010ca0: 7261 7465 2074 6865 2061 7070 726f 7072  rate the appropr
+00010cb0: 6961 7465 2072 6571 7565 7374 0a20 2020  iate request.   
+00010cc0: 2020 2020 2072 6571 203d 2066 6163 746f       req = facto
+00010cd0: 7279 2e72 6571 7565 7374 286f 7065 7261  ry.request(opera
+00010ce0: 7469 6f6e 290a 0a20 2020 2020 2020 2077  tion)..        w
+00010cf0: 6869 6c65 2054 7275 653a 0a20 2020 2020  hile True:.     
+00010d00: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00010d10: 2020 2020 2020 2020 2020 2020 5f73 656e              _sen
+00010d20: 645f 6d73 6728 7365 6c66 2e63 6f6e 6e65  d_msg(self.conne
+00010d30: 6374 696f 6e2c 2072 6571 290a 0a20 2020  ction, req)..   
+00010d40: 2020 2020 2020 2020 2020 2020 2072 7370               rsp
+00010d50: 203d 205f 7265 6376 5f6d 7367 2873 656c   = _recv_msg(sel
+00010d60: 662e 636f 6e6e 6563 7469 6f6e 2c20 6661  f.connection, fa
+00010d70: 6374 6f72 792e 7265 7370 6f6e 7365 2829  ctory.response()
+00010d80: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+00010d90: 6365 7074 2049 4f45 7272 6f72 3a0a 2020  cept IOError:.  
+00010da0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00010db0: 7265 6d61 6b65 206f 7572 2063 6f6e 6e65  remake our conne
+00010dc0: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
+00010dd0: 2020 2020 2020 7365 6c66 2e63 6f6e 6e65        self.conne
+00010de0: 6374 696f 6e20 3d20 436f 6e6e 6563 7469  ction = Connecti
+00010df0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00010e00: 2020 2020 2020 2020 7573 6572 3d73 656c          user=sel
+00010e10: 662e 636f 6e6e 6563 7469 6f6e 2e75 7365  f.connection.use
+00010e20: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+00010e30: 2020 2020 2020 2070 6173 7377 6f72 643d         password=
+00010e40: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2e  self.connection.
+00010e50: 7061 7373 776f 7264 2c0a 2020 2020 2020  password,.      
+00010e60: 2020 2020 2020 2020 2020 2020 2020 686f                ho
+00010e70: 7374 3d66 227b 272c 272e 6a6f 696e 2873  st=f"{','.join(s
+00010e80: 656c 662e 636f 6e6e 6563 7469 6f6e 2e68  elf.connection.h
+00010e90: 6f73 7473 297d 3a7b 7365 6c66 2e63 6f6e  osts)}:{self.con
+00010ea0: 6e65 6374 696f 6e2e 706f 7274 7d22 2c0a  nection.port}",.
+00010eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ec0: 2020 2020 6461 7461 6261 7365 3d73 656c      database=sel
+00010ed0: 662e 636f 6e6e 6563 7469 6f6e 2e64 6174  f.connection.dat
+00010ee0: 6162 6173 652c 0a20 2020 2020 2020 2020  abase,.         
+00010ef0: 2020 2020 2020 2020 2020 2074 6c73 3d73             tls=s
+00010f00: 656c 662e 636f 6e6e 6563 7469 6f6e 2e74  elf.connection.t
+00010f10: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
+00010f20: 2020 2020 2020 2020 6861 6e64 7368 616b          handshak
+00010f30: 653d 7365 6c66 2e63 6f6e 6e65 6374 696f  e=self.connectio
+00010f40: 6e2e 6861 6e64 7368 616b 652c 0a20 2020  n.handshake,.   
 00010f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f60: 2020 2064 6174 6162 6173 653d 7365 6c66     database=self
-00010f70: 2e63 6f6e 6e65 6374 696f 6e2e 6461 7461  .connection.data
-00010f80: 6261 7365 2c0a 2020 2020 2020 2020 2020  base,.          
-00010f90: 2020 2020 2020 2020 2020 746c 733d 7365            tls=se
-00010fa0: 6c66 2e63 6f6e 6e65 6374 696f 6e2e 746c  lf.connection.tl
-00010fb0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00010fc0: 2020 2020 2020 2068 616e 6473 6861 6b65         handshake
-00010fd0: 3d73 656c 662e 636f 6e6e 6563 7469 6f6e  =self.connection
-00010fe0: 2e68 616e 6473 6861 6b65 2c0a 2020 2020  .handshake,.    
-00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011000: 666f 7263 653d 7365 6c66 2e63 6f6e 6e65  force=self.conne
-00011010: 6374 696f 6e2e 666f 7263 652c 0a20 2020  ction.force,.   
-00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011030: 2073 6573 7369 6f6e 3d73 656c 662e 636f   session=self.co
-00011040: 6e6e 6563 7469 6f6e 2e73 6573 7369 6f6e  nnection.session
-00011050: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011060: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-00011070: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-00011080: 2020 2020 2020 2020 2020 2069 6620 7273             if rs
-00011090: 702e 7265 7370 6f6e 7365 2e74 7970 6520  p.response.type 
-000110a0: 3d3d 2070 726f 746f 2e43 6f6e 6669 726d  == proto.Confirm
-000110b0: 6174 696f 6e52 6573 706f 6e73 652e 5245  ationResponse.RE
-000110c0: 5350 4f4e 5345 5f57 4152 4e3a 0a20 2020  SPONSE_WARN:.   
-000110d0: 2020 2020 2020 2020 2020 2020 2077 6172               war
-000110e0: 6e28 7273 702e 7265 7370 6f6e 7365 2e72  n(rsp.response.r
-000110f0: 6561 736f 6e29 0a20 2020 2020 2020 2020  eason).         
-00011100: 2020 2065 6c69 6620 6e6f 7420 7273 702e     elif not rsp.
-00011110: 7265 7370 6f6e 7365 2e74 7970 6520 3d3d  response.type ==
-00011120: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
-00011130: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
-00011140: 4f4e 5345 5f4f 4b3a 0a20 2020 2020 2020  ONSE_OK:.       
-00011150: 2020 2020 2020 2020 2069 6620 7273 702e           if rsp.
-00011160: 7265 7370 6f6e 7365 2e76 656e 646f 725f  response.vendor_
-00011170: 636f 6465 203d 3d20 5345 5353 494f 4e5f  code == SESSION_
-00011180: 4558 5049 5245 445f 434f 4445 3a0a 2020  EXPIRED_CODE:.  
-00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111a0: 2020 2320 4e65 6564 2074 6f20 7265 6672    # Need to refr
-000111b0: 6573 6820 7468 6520 7365 7373 696f 6e0a  esh the session.
-000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111d0: 2020 2020 7365 6c66 2e63 6f6e 6e65 6374      self.connect
-000111e0: 696f 6e2e 7265 6672 6573 6828 290a 2020  ion.refresh().  
-000111f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011200: 2020 2320 616e 6420 7472 7920 6167 6169    # and try agai
-00011210: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00011220: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-00011230: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00011240: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00011250: 2020 2020 2020 2020 2072 6169 7365 205f           raise _
-00011260: 636f 6e76 6572 745f 6578 6365 7074 696f  convert_exceptio
-00011270: 6e28 7273 702e 7265 7370 6f6e 7365 290a  n(rsp.response).
-00011280: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-00011290: 6565 2069 6620 7765 2061 7265 2062 6569  ee if we are bei
-000112a0: 6e67 2074 6f6c 6420 746f 2072 6564 6972  ng told to redir
-000112b0: 6563 740a 2020 2020 2020 2020 2020 2020  ect.            
-000112c0: 6966 206e 6f74 2072 7370 2e72 6564 6972  if not rsp.redir
-000112d0: 6563 743a 0a20 2020 2020 2020 2020 2020  ect:.           
-000112e0: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
-000112f0: 2020 2020 2020 2020 2320 7265 6d61 6b65          # remake
-00011300: 206f 7572 2063 6f6e 6e65 6374 696f 6e0a   our connection.
-00011310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011320: 2e63 6f6e 6e65 6374 696f 6e20 3d20 7365  .connection = se
-00011330: 6c66 2e63 6f6e 6e65 6374 696f 6e2e 7265  lf.connection.re
-00011340: 6469 7265 6374 2872 7370 2e72 6564 6972  direct(rsp.redir
-00011350: 6563 7448 6f73 742c 2072 7370 2e72 6564  ectHost, rsp.red
-00011360: 6972 6563 7450 6f72 7429 0a0a 2020 2020  irectPort)..    
-00011370: 6465 6620 5f65 7865 6375 7465 5f66 6f72  def _execute_for
-00011380: 6365 2873 656c 662c 206f 7065 7261 7469  ce(self, operati
-00011390: 6f6e 2920 2d3e 204e 6f6e 653a 0a20 2020  on) -> None:.   
-000113a0: 2020 2020 2069 6620 6f70 6572 6174 696f       if operatio
-000113b0: 6e2e 7374 7269 7028 292e 7570 7065 7228  n.strip().upper(
-000113c0: 2920 3d3d 2022 464f 5243 4520 5245 4449  ) == "FORCE REDI
-000113d0: 5245 4354 223a 0a20 2020 2020 2020 2020  RECT":.         
-000113e0: 2020 2023 2053 6574 7320 7468 6520 6e65     # Sets the ne
-000113f0: 7874 2063 6f6d 6d61 6e64 2074 6861 7420  xt command that 
-00011400: 6973 2065 7865 6375 7465 2071 7565 7279  is execute query
-00011410: 2074 6f20 7265 6469 7265 6374 0a20 2020   to redirect.   
-00011420: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00011430: 6e6e 6563 7469 6f6e 2e66 6f72 6365 5f6e  nnection.force_n
-00011440: 6578 745f 7265 6469 7265 6374 203d 2054  ext_redirect = T
-00011450: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-00011460: 7365 6c66 2e65 6e64 5f6f 665f 6461 7461  self.end_of_data
-00011470: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00011480: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00011490: 2020 2320 466f 7263 6520 6578 7465 726e    # Force extern
-000114a0: 616c 2063 6f6d 6d61 6e64 0a20 2020 2020  al command.     
-000114b0: 2020 2020 2020 2073 656c 662e 5f65 7865         self._exe
-000114c0: 6375 7465 5f66 6f72 6365 5f65 7874 6572  cute_force_exter
-000114d0: 6e61 6c28 6f70 6572 6174 696f 6e29 0a0a  nal(operation)..
-000114e0: 2020 2020 6465 6620 5f65 7865 6375 7465      def _execute
-000114f0: 5f66 6f72 6365 5f65 7874 6572 6e61 6c28  _force_external(
-00011500: 7365 6c66 2c20 6f70 6572 6174 696f 6e29  self, operation)
-00011510: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00011520: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-00011530: 626c 653d 6e6f 2d6d 656d 6265 720a 2020  ble=no-member.  
-00011540: 2020 2020 2020 2320 5768 696c 6520 7765        # While we
-00011550: 2061 7265 2072 6564 6972 6563 7469 6e67   are redirecting
-00011560: 2e2e 2e0a 2020 2020 2020 2020 6661 6374  ....        fact
-00011570: 6f72 7920 3d20 5f4f 4349 454e 545f 5245  ory = _OCIENT_RE
-00011580: 5155 4553 545f 4641 4354 4f52 4945 535b  QUEST_FACTORIES[
-00011590: 2246 4f52 4345 225d 0a20 2020 2020 2020  "FORCE"].       
-000115a0: 2072 6571 203d 2066 6163 746f 7279 2e72   req = factory.r
-000115b0: 6571 7565 7374 286f 7065 7261 7469 6f6e  equest(operation
-000115c0: 3d6f 7065 7261 7469 6f6e 290a 0a20 2020  =operation)..   
-000115d0: 2020 2020 205f 7365 6e64 5f6d 7367 2873       _send_msg(s
-000115e0: 656c 662e 636f 6e6e 6563 7469 6f6e 2c20  elf.connection, 
-000115f0: 7265 7129 0a0a 2020 2020 2020 2020 7273  req)..        rs
-00011600: 7020 3d20 5f72 6563 765f 6d73 6728 7365  p = _recv_msg(se
-00011610: 6c66 2e63 6f6e 6e65 6374 696f 6e2c 2070  lf.connection, p
-00011620: 726f 746f 2e43 6f6e 6669 726d 6174 696f  roto.Confirmatio
-00011630: 6e52 6573 706f 6e73 6528 2929 0a0a 2020  nResponse())..  
-00011640: 2020 2020 2020 6966 2072 7370 2e74 7970        if rsp.typ
-00011650: 6520 3d3d 2070 726f 746f 2e43 6f6e 6669  e == proto.Confi
-00011660: 726d 6174 696f 6e52 6573 706f 6e73 652e  rmationResponse.
-00011670: 5245 5350 4f4e 5345 5f57 4152 4e3a 0a20  RESPONSE_WARN:. 
-00011680: 2020 2020 2020 2020 2020 2077 6172 6e28             warn(
-00011690: 7273 702e 7265 6173 6f6e 290a 2020 2020  rsp.reason).    
-000116a0: 2020 2020 656c 6966 206e 6f74 2072 7370      elif not rsp
-000116b0: 2e74 7970 6520 3d3d 2070 726f 746f 2e43  .type == proto.C
-000116c0: 6f6e 6669 726d 6174 696f 6e52 6573 706f  onfirmationRespo
-000116d0: 6e73 652e 5245 5350 4f4e 5345 5f4f 4b3a  nse.RESPONSE_OK:
-000116e0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000116f0: 7365 205f 636f 6e76 6572 745f 6578 6365  se _convert_exce
-00011700: 7074 696f 6e28 7273 7029 0a0a 2020 2020  ption(rsp)..    
-00011710: 6465 6620 5f65 7865 6375 7465 5f73 6574  def _execute_set
-00011720: 2873 656c 662c 2070 6172 616d 7329 202d  (self, params) -
-00011730: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00011740: 6966 206c 656e 2870 6172 616d 7329 2021  if len(params) !
-00011750: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
-00011760: 2072 6169 7365 2050 726f 6772 616d 6d69   raise Programmi
-00011770: 6e67 4572 726f 7228 7265 6173 6f6e 3d22  ngError(reason="
-00011780: 5379 6e74 6178 2065 7272 6f72 2229 0a0a  Syntax error")..
-00011790: 2020 2020 2020 2020 2320 5468 6572 6520          # There 
-000117a0: 6973 206e 6f20 7265 7375 6c74 7365 7420  is no resultset 
-000117b0: 6461 7461 2066 726f 6d20 616e 2075 7064  data from an upd
-000117c0: 6174 650a 2020 2020 2020 2020 7365 6c66  ate.        self
-000117d0: 2e65 6e64 5f6f 665f 6461 7461 203d 2054  .end_of_data = T
-000117e0: 7275 650a 0a20 2020 2020 2020 206f 7020  rue..        op 
-000117f0: 3d20 7061 7261 6d73 5b30 5d2e 7570 7065  = params[0].uppe
-00011800: 7228 290a 2020 2020 2020 2020 7661 6c20  r().        val 
-00011810: 3d20 7061 7261 6d73 5b31 5d2e 7374 7269  = params[1].stri
-00011820: 7028 290a 0a20 2020 2020 2020 2069 6620  p()..        if 
-00011830: 6f70 203d 3d20 2253 4348 454d 4122 3a0a  op == "SCHEMA":.
-00011840: 2020 2020 2020 2020 2020 2020 6661 6374              fact
-00011850: 6f72 7920 3d20 5f4f 4349 454e 545f 5245  ory = _OCIENT_RE
-00011860: 5155 4553 545f 4641 4354 4f52 4945 535b  QUEST_FACTORIES[
-00011870: 2253 4554 2053 4348 454d 4122 5d0a 2020  "SET SCHEMA"].  
-00011880: 2020 2020 2020 2020 2020 7265 7120 3d20            req = 
-00011890: 6661 6374 6f72 792e 7265 7175 6573 7428  factory.request(
-000118a0: 7661 6c29 0a20 2020 2020 2020 2065 6c73  val).        els
-000118b0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-000118c0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-000118d0: 2020 2020 7661 6c20 3d20 696e 7428 7661      val = int(va
-000118e0: 6c29 0a20 2020 2020 2020 2020 2020 2065  l).            e
-000118f0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
-00011900: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011910: 2020 7261 6973 6520 5072 6f67 7261 6d6d    raise Programm
-00011920: 696e 6745 7272 6f72 2872 6561 736f 6e3d  ingError(reason=
-00011930: 2253 796e 7461 7820 6572 726f 7220 696e  "Syntax error in
-00011940: 2053 4554 2e20 5661 6c75 6520 6d75 7374   SET. Value must
-00011950: 2062 6520 6e75 6d65 7269 6322 290a 0a20   be numeric").. 
-00011960: 2020 2020 2020 2020 2020 2066 6163 746f             facto
-00011970: 7279 203d 205f 4f43 4945 4e54 5f52 4551  ry = _OCIENT_REQ
-00011980: 5545 5354 5f46 4143 544f 5249 4553 5b22  UEST_FACTORIES["
-00011990: 5345 5422 5d0a 2020 2020 2020 2020 2020  SET"].          
-000119a0: 2020 7265 7120 3d20 6661 6374 6f72 792e    req = factory.
-000119b0: 7265 7175 6573 7428 6f70 2c20 7661 6c29  request(op, val)
-000119c0: 0a0a 2020 2020 2020 2020 5f73 656e 645f  ..        _send_
-000119d0: 6d73 6728 7365 6c66 2e63 6f6e 6e65 6374  msg(self.connect
-000119e0: 696f 6e2c 2072 6571 290a 0a20 2020 2020  ion, req)..     
-000119f0: 2020 2072 7370 203d 205f 7265 6376 5f6d     rsp = _recv_m
-00011a00: 7367 2873 656c 662e 636f 6e6e 6563 7469  sg(self.connecti
-00011a10: 6f6e 2c20 6661 6374 6f72 792e 7265 7370  on, factory.resp
-00011a20: 6f6e 7365 2829 290a 0a20 2020 2020 2020  onse())..       
-00011a30: 2069 6620 7273 702e 7479 7065 203d 3d20   if rsp.type == 
-00011a40: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
-00011a50: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
-00011a60: 4e53 455f 5741 524e 3a0a 2020 2020 2020  NSE_WARN:.      
-00011a70: 2020 2020 2020 7761 726e 2872 7370 2e72        warn(rsp.r
-00011a80: 6561 736f 6e29 0a20 2020 2020 2020 2065  eason).        e
-00011a90: 6c69 6620 6e6f 7420 7273 702e 7479 7065  lif not rsp.type
-00011aa0: 203d 3d20 7072 6f74 6f2e 436f 6e66 6972   == proto.Confir
-00011ab0: 6d61 7469 6f6e 5265 7370 6f6e 7365 2e52  mationResponse.R
-00011ac0: 4553 504f 4e53 455f 4f4b 3a0a 2020 2020  ESPONSE_OK:.    
-00011ad0: 2020 2020 2020 2020 6966 2072 7370 2e72          if rsp.r
-00011ae0: 6573 706f 6e73 652e 7665 6e64 6f72 5f63  esponse.vendor_c
-00011af0: 6f64 6520 3d3d 2053 4553 5349 4f4e 5f45  ode == SESSION_E
-00011b00: 5850 4952 4544 5f43 4f44 453a 0a20 2020  XPIRED_CODE:.   
-00011b10: 2020 2020 2020 2020 2020 2020 2023 204e               # N
-00011b20: 6565 6420 746f 2072 6566 7265 7368 2074  eed to refresh t
-00011b30: 6865 2073 6573 7369 6f6e 0a20 2020 2020  he session.     
-00011b40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011b50: 636f 6e6e 6563 7469 6f6e 2e72 6566 7265  connection.refre
-00011b60: 7368 2829 0a20 2020 2020 2020 2020 2020  sh().           
-00011b70: 2020 2020 2023 2061 6e64 2074 7279 2061       # and try a
-00011b80: 6761 696e 0a20 2020 2020 2020 2020 2020  gain.           
-00011b90: 2020 2020 2073 656c 662e 5f65 7865 6375       self._execu
-00011ba0: 7465 5f73 6574 2870 6172 616d 7329 0a20  te_set(params). 
-00011bb0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00011bc0: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-00011bd0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00011be0: 2020 2020 2020 2020 7261 6973 6520 5f63          raise _c
-00011bf0: 6f6e 7665 7274 5f65 7863 6570 7469 6f6e  onvert_exception
-00011c00: 2872 7370 290a 0a20 2020 2064 6566 205f  (rsp)..    def _
-00011c10: 6578 6563 7574 655f 6765 745f 7363 6865  execute_get_sche
-00011c20: 6d61 2873 656c 6629 202d 3e20 4e6f 6e65  ma(self) -> None
-00011c30: 3a0a 2020 2020 2020 2020 6661 6374 6f72  :.        factor
-00011c40: 7920 3d20 5f4f 4349 454e 545f 5245 5155  y = _OCIENT_REQU
-00011c50: 4553 545f 4641 4354 4f52 4945 535b 2247  EST_FACTORIES["G
-00011c60: 4554 2053 4348 454d 4122 5d0a 2020 2020  ET SCHEMA"].    
-00011c70: 2020 2020 7265 7120 3d20 6661 6374 6f72      req = factor
-00011c80: 792e 7265 7175 6573 7428 290a 0a20 2020  y.request()..   
-00011c90: 2020 2020 205f 7365 6e64 5f6d 7367 2873       _send_msg(s
-00011ca0: 656c 662e 636f 6e6e 6563 7469 6f6e 2c20  elf.connection, 
-00011cb0: 7265 7129 0a0a 2020 2020 2020 2020 7273  req)..        rs
-00011cc0: 7020 3d20 5f72 6563 765f 6d73 6728 7365  p = _recv_msg(se
-00011cd0: 6c66 2e63 6f6e 6e65 6374 696f 6e2c 2066  lf.connection, f
-00011ce0: 6163 746f 7279 2e72 6573 706f 6e73 6528  actory.response(
-00011cf0: 2929 0a0a 2020 2020 2020 2020 6966 2072  ))..        if r
-00011d00: 7370 2e72 6573 706f 6e73 652e 7479 7065  sp.response.type
-00011d10: 203d 3d20 7072 6f74 6f2e 436f 6e66 6972   == proto.Confir
-00011d20: 6d61 7469 6f6e 5265 7370 6f6e 7365 2e52  mationResponse.R
-00011d30: 4553 504f 4e53 455f 5741 524e 3a0a 2020  ESPONSE_WARN:.  
-00011d40: 2020 2020 2020 2020 2020 7761 726e 2872            warn(r
-00011d50: 7370 2e72 6573 706f 6e73 652e 7265 6173  sp.response.reas
-00011d60: 6f6e 290a 2020 2020 2020 2020 656c 6966  on).        elif
-00011d70: 206e 6f74 2072 7370 2e72 6573 706f 6e73   not rsp.respons
-00011d80: 652e 7479 7065 203d 3d20 7072 6f74 6f2e  e.type == proto.
-00011d90: 436f 6e66 6972 6d61 7469 6f6e 5265 7370  ConfirmationResp
-00011da0: 6f6e 7365 2e52 4553 504f 4e53 455f 4f4b  onse.RESPONSE_OK
-00011db0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00011dc0: 2072 7370 2e72 6573 706f 6e73 652e 7665   rsp.response.ve
-00011dd0: 6e64 6f72 5f63 6f64 6520 3d3d 2053 4553  ndor_code == SES
-00011de0: 5349 4f4e 5f45 5850 4952 4544 5f43 4f44  SION_EXPIRED_COD
-00011df0: 453a 0a20 2020 2020 2020 2020 2020 2020  E:.             
-00011e00: 2020 2023 204e 6565 6420 746f 2072 6566     # Need to ref
-00011e10: 7265 7368 2074 6865 2073 6573 7369 6f6e  resh the session
-00011e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011e30: 2073 656c 662e 636f 6e6e 6563 7469 6f6e   self.connection
-00011e40: 2e72 6566 7265 7368 2829 0a20 2020 2020  .refresh().     
-00011e50: 2020 2020 2020 2020 2020 2023 2061 6e64             # and
-00011e60: 2074 7279 2061 6761 696e 0a20 2020 2020   try again.     
-00011e70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011e80: 5f65 7865 6375 7465 5f67 6574 5f73 6368  _execute_get_sch
-00011e90: 656d 6128 290a 2020 2020 2020 2020 2020  ema().          
-00011ea0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00011eb0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00011ec0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00011ed0: 6169 7365 205f 636f 6e76 6572 745f 6578  aise _convert_ex
-00011ee0: 6365 7074 696f 6e28 7273 702e 7265 7370  ception(rsp.resp
-00011ef0: 6f6e 7365 290a 0a20 2020 2020 2020 2073  onse)..        s
-00011f00: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
-00011f10: 3d20 5b28 2273 6368 656d 6122 2c20 5479  = [("schema", Ty
-00011f20: 7065 436f 6465 732e 4348 4152 2c20 4e6f  peCodes.CHAR, No
-00011f30: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20  ne, None, None, 
-00011f40: 4e6f 6e65 2c20 4e6f 6e65 295d 2020 2320  None, None)]  # 
-00011f50: 6469 7370 6c61 795f 7369 7a65 2020 2320  display_size  # 
-00011f60: 696e 7465 726e 616c 5f73 697a 6520 2023  internal_size  #
-00011f70: 2070 7265 6369 7369 6f6e 2020 2320 7363   precision  # sc
-00011f80: 616c 6520 2023 206e 756c 6c5f 6f6b 0a0a  ale  # null_ok..
-00011f90: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00011fa0: 745f 7265 7375 6c74 203d 205b 0a20 2020  t_result = [.   
-00011fb0: 2020 2020 2020 2020 206e 616d 6564 7475           namedtu
-00011fc0: 706c 6528 2252 6f77 222c 2028 2273 6368  ple("Row", ("sch
-00011fd0: 656d 6122 2929 280a 2020 2020 2020 2020  ema"))(.        
-00011fe0: 2020 2020 2020 2020 7273 702e 7363 6865          rsp.sche
-00011ff0: 6d61 2c0a 2020 2020 2020 2020 2020 2020  ma,.            
-00012000: 290a 2020 2020 2020 2020 5d0a 0a20 2020  ).        ]..   
-00012010: 2023 2049 6620 7765 206e 6565 6420 746f   # If we need to
-00012020: 2069 6d70 6c65 6d65 6e74 206d 6f72 6520   implement more 
-00012030: 6f66 2074 6865 7365 2073 6f72 7473 206f  of these sorts o
-00012040: 6620 6375 7374 6f6d 2063 6f6d 6d61 6e64  f custom command
-00012050: 732c 2063 6f6e 7369 6465 720a 2020 2020  s, consider.    
-00012060: 2320 6d61 6b69 6e67 2061 2066 6163 746f  # making a facto
-00012070: 7279 2066 6f72 2074 6865 2064 6573 6372  ry for the descr
-00012080: 6970 7469 6f6e 2061 6e64 2072 6573 756c  iption and resul
-00012090: 7473 2e0a 2020 2020 6465 6620 5f65 7865  ts..    def _exe
-000120a0: 6375 7465 5f67 6574 5f73 6572 7665 725f  cute_get_server_
-000120b0: 7365 7373 696f 6e5f 6964 2873 656c 6629  session_id(self)
-000120c0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000120d0: 2020 7365 6c66 2e64 6573 6372 6970 7469    self.descripti
-000120e0: 6f6e 203d 205b 2822 7365 7276 6572 5f73  on = [("server_s
-000120f0: 6573 7369 6f6e 5f69 6422 2c20 5479 7065  ession_id", Type
-00012100: 436f 6465 732e 4348 4152 2c20 4e6f 6e65  Codes.CHAR, None
-00012110: 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f  , None, None, No
-00012120: 6e65 2c20 4e6f 6e65 295d 2020 2320 6469  ne, None)]  # di
-00012130: 7370 6c61 795f 7369 7a65 2020 2320 696e  splay_size  # in
-00012140: 7465 726e 616c 5f73 697a 6520 2023 2070  ternal_size  # p
-00012150: 7265 6369 7369 6f6e 2020 2320 7363 616c  recision  # scal
-00012160: 6520 2023 206e 756c 6c5f 6f6b 0a20 2020  e  # null_ok.   
-00012170: 2020 2020 2073 656c 662e 6c69 7374 5f72       self.list_r
-00012180: 6573 756c 7420 3d20 5b0a 2020 2020 2020  esult = [.      
-00012190: 2020 2020 2020 6e61 6d65 6474 7570 6c65        namedtuple
-000121a0: 2822 526f 7722 2c20 2822 7365 7276 6572  ("Row", ("server
-000121b0: 5f73 6573 7369 6f6e 5f69 6422 2929 280a  _session_id"))(.
-000121c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121d0: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2e  self.connection.
-000121e0: 7365 7276 6572 5365 7373 696f 6e49 642c  serverSessionId,
-000121f0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00012200: 2020 2020 2020 205d 0a0a 2020 2020 6465         ]..    de
-00012210: 6620 5f65 7865 6375 7465 5f67 6574 2873  f _execute_get(s
-00012220: 656c 662c 2070 6172 616d 7329 202d 3e20  elf, params) -> 
-00012230: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
-00012240: 206c 656e 2870 6172 616d 7329 203d 3d20   len(params) == 
-00012250: 3120 616e 6420 7061 7261 6d73 5b30 5d2e  1 and params[0].
-00012260: 7570 7065 7228 2920 3d3d 2022 5343 4845  upper() == "SCHE
-00012270: 4d41 223a 0a20 2020 2020 2020 2020 2020  MA":.           
-00012280: 2073 656c 662e 5f65 7865 6375 7465 5f67   self._execute_g
-00012290: 6574 5f73 6368 656d 6128 290a 2020 2020  et_schema().    
-000122a0: 2020 2020 656c 6966 206c 656e 2870 6172      elif len(par
-000122b0: 616d 7329 203d 3d20 3320 616e 6420 7061  ams) == 3 and pa
-000122c0: 7261 6d73 5b30 5d2e 7570 7065 7228 2920  rams[0].upper() 
-000122d0: 3d3d 2022 5345 5256 4552 2220 616e 6420  == "SERVER" and 
-000122e0: 7061 7261 6d73 5b31 5d2e 7570 7065 7228  params[1].upper(
-000122f0: 2920 3d3d 2022 5345 5353 494f 4e22 2061  ) == "SESSION" a
-00012300: 6e64 2070 6172 616d 735b 325d 2e75 7070  nd params[2].upp
-00012310: 6572 2829 203d 3d20 2249 4422 3a0a 2020  er() == "ID":.  
-00012320: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00012330: 6578 6563 7574 655f 6765 745f 7365 7276  execute_get_serv
-00012340: 6572 5f73 6573 7369 6f6e 5f69 6428 290a  er_session_id().
-00012350: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00012360: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00012370: 5072 6f67 7261 6d6d 696e 6745 7272 6f72  ProgrammingError
-00012380: 2872 6561 736f 6e3d 2253 796e 7461 7820  (reason="Syntax 
-00012390: 6572 726f 7222 290a 0a20 2020 2064 6566  error")..    def
-000123a0: 205f 6578 6563 7574 655f 636c 6561 7228   _execute_clear(
-000123b0: 7365 6c66 2c20 7061 7261 6d73 2920 2d3e  self, params) ->
-000123c0: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
-000123d0: 6620 6c65 6e28 7061 7261 6d73 2920 213d  f len(params) !=
-000123e0: 2031 206f 7220 7061 7261 6d73 5b30 5d2e   1 or params[0].
-000123f0: 7570 7065 7228 2920 213d 2022 4341 4348  upper() != "CACH
-00012400: 4522 3a0a 2020 2020 2020 2020 2020 2020  E":.            
-00012410: 7261 6973 6520 5072 6f67 7261 6d6d 696e  raise Programmin
-00012420: 6745 7272 6f72 2872 6561 736f 6e3d 2253  gError(reason="S
-00012430: 796e 7461 7820 6572 726f 7222 290a 0a20  yntax error").. 
-00012440: 2020 2020 2020 2023 2054 6865 7265 2069         # There i
-00012450: 7320 6e6f 2072 6573 756c 7473 6574 2064  s no resultset d
-00012460: 6174 6120 6672 6f6d 2061 6e20 7570 6461  ata from an upda
-00012470: 7465 0a20 2020 2020 2020 2073 656c 662e  te.        self.
-00012480: 656e 645f 6f66 5f64 6174 6120 3d20 5472  end_of_data = Tr
-00012490: 7565 0a0a 2020 2020 2020 2020 6661 6374  ue..        fact
-000124a0: 6f72 7920 3d20 5f4f 4349 454e 545f 5245  ory = _OCIENT_RE
-000124b0: 5155 4553 545f 4641 4354 4f52 4945 535b  QUEST_FACTORIES[
-000124c0: 2243 4c45 4152 2043 4143 4845 225d 0a20  "CLEAR CACHE"]. 
-000124d0: 2020 2020 2020 2072 6571 203d 2066 6163         req = fac
-000124e0: 746f 7279 2e72 6571 7565 7374 2829 0a0a  tory.request()..
-000124f0: 2020 2020 2020 2020 5f73 656e 645f 6d73          _send_ms
-00012500: 6728 7365 6c66 2e63 6f6e 6e65 6374 696f  g(self.connectio
-00012510: 6e2c 2072 6571 290a 0a20 2020 2020 2020  n, req)..       
-00012520: 2072 7370 203d 205f 7265 6376 5f6d 7367   rsp = _recv_msg
-00012530: 2873 656c 662e 636f 6e6e 6563 7469 6f6e  (self.connection
-00012540: 2c20 6661 6374 6f72 792e 7265 7370 6f6e  , factory.respon
-00012550: 7365 2829 290a 0a20 2020 2020 2020 2069  se())..        i
-00012560: 6620 7273 702e 7479 7065 203d 3d20 7072  f rsp.type == pr
-00012570: 6f74 6f2e 436f 6e66 6972 6d61 7469 6f6e  oto.Confirmation
-00012580: 5265 7370 6f6e 7365 2e52 4553 504f 4e53  Response.RESPONS
-00012590: 455f 5741 524e 3a0a 2020 2020 2020 2020  E_WARN:.        
-000125a0: 2020 2020 7761 726e 2872 7370 2e72 6561      warn(rsp.rea
-000125b0: 736f 6e29 0a20 2020 2020 2020 2065 6c69  son).        eli
-000125c0: 6620 6e6f 7420 7273 702e 7479 7065 203d  f not rsp.type =
-000125d0: 3d20 7072 6f74 6f2e 436f 6e66 6972 6d61  = proto.Confirma
-000125e0: 7469 6f6e 5265 7370 6f6e 7365 2e52 4553  tionResponse.RES
-000125f0: 504f 4e53 455f 4f4b 3a0a 2020 2020 2020  PONSE_OK:.      
-00012600: 2020 2020 2020 6966 2072 7370 2e76 656e        if rsp.ven
-00012610: 646f 725f 636f 6465 203d 3d20 5345 5353  dor_code == SESS
-00012620: 494f 4e5f 4558 5049 5245 445f 434f 4445  ION_EXPIRED_CODE
-00012630: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012640: 2020 2320 4e65 6564 2074 6f20 7265 6672    # Need to refr
-00012650: 6573 6820 7468 6520 7365 7373 696f 6e0a  esh the session.
-00012660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012670: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2e  self.connection.
-00012680: 7265 6672 6573 6828 290a 2020 2020 2020  refresh().      
-00012690: 2020 2020 2020 2020 2020 2320 616e 6420            # and 
-000126a0: 7472 7920 6167 6169 6e0a 2020 2020 2020  try again.      
-000126b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000126c0: 6578 6563 7574 655f 636c 6561 7228 7061  execute_clear(pa
-000126d0: 7261 6d73 290a 2020 2020 2020 2020 2020  rams).          
-000126e0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-000126f0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00012700: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00012710: 6169 7365 205f 636f 6e76 6572 745f 6578  aise _convert_ex
-00012720: 6365 7074 696f 6e28 7273 7029 0a0a 2020  ception(rsp)..  
-00012730: 2020 6465 6620 5f65 7865 6375 7465 5f63    def _execute_c
-00012740: 616e 6365 6c6b 696c 6c28 7365 6c66 2c20  ancelkill(self, 
-00012750: 6f70 2c20 6964 2920 2d3e 204e 6f6e 653a  op, id) -> None:
-00012760: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00012770: 6964 2920 213d 2031 3a0a 2020 2020 2020  id) != 1:.      
-00012780: 2020 2020 2020 7261 6973 6520 5072 6f67        raise Prog
-00012790: 7261 6d6d 696e 6745 7272 6f72 2872 6561  rammingError(rea
-000127a0: 736f 6e3d 2253 796e 7461 7820 6572 726f  son="Syntax erro
-000127b0: 7222 290a 0a20 2020 2020 2020 2023 2054  r")..        # T
-000127c0: 6865 7265 2069 7320 6e6f 2072 6573 756c  here is no resul
-000127d0: 7473 6574 2064 6174 6120 6672 6f6d 2061  tset data from a
-000127e0: 6e20 7570 6461 7465 0a20 2020 2020 2020  n update.       
-000127f0: 2073 656c 662e 656e 645f 6f66 5f64 6174   self.end_of_dat
-00012800: 6120 3d20 5472 7565 0a0a 2020 2020 2020  a = True..      
-00012810: 2020 6661 6374 6f72 7920 3d20 5f4f 4349    factory = _OCI
-00012820: 454e 545f 5245 5155 4553 545f 4641 4354  ENT_REQUEST_FACT
-00012830: 4f52 4945 535b 6f70 5d0a 2020 2020 2020  ORIES[op].      
-00012840: 2020 7265 7120 3d20 6661 6374 6f72 792e    req = factory.
-00012850: 7265 7175 6573 7428 6964 5b30 5d29 0a0a  request(id[0])..
-00012860: 2020 2020 2020 2020 5f73 656e 645f 6d73          _send_ms
-00012870: 6728 7365 6c66 2e63 6f6e 6e65 6374 696f  g(self.connectio
-00012880: 6e2c 2072 6571 290a 0a20 2020 2020 2020  n, req)..       
-00012890: 2072 7370 203d 205f 7265 6376 5f6d 7367   rsp = _recv_msg
-000128a0: 2873 656c 662e 636f 6e6e 6563 7469 6f6e  (self.connection
-000128b0: 2c20 6661 6374 6f72 792e 7265 7370 6f6e  , factory.respon
-000128c0: 7365 2829 290a 0a20 2020 2020 2020 2069  se())..        i
-000128d0: 6620 7273 702e 7265 7370 6f6e 7365 2e74  f rsp.response.t
-000128e0: 7970 6520 3d3d 2070 726f 746f 2e43 6f6e  ype == proto.Con
-000128f0: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
-00012900: 652e 5245 5350 4f4e 5345 5f57 4152 4e3a  e.RESPONSE_WARN:
-00012910: 0a20 2020 2020 2020 2020 2020 2077 6172  .            war
-00012920: 6e28 7273 702e 7265 7370 6f6e 7365 2e72  n(rsp.response.r
-00012930: 6561 736f 6e29 0a20 2020 2020 2020 2065  eason).        e
-00012940: 6c69 6620 6e6f 7420 7273 702e 7265 7370  lif not rsp.resp
-00012950: 6f6e 7365 2e74 7970 6520 3d3d 2070 726f  onse.type == pro
-00012960: 746f 2e43 6f6e 6669 726d 6174 696f 6e52  to.ConfirmationR
-00012970: 6573 706f 6e73 652e 5245 5350 4f4e 5345  esponse.RESPONSE
-00012980: 5f4f 4b3a 0a20 2020 2020 2020 2020 2020  _OK:.           
-00012990: 2069 6620 7273 702e 7265 7370 6f6e 7365   if rsp.response
-000129a0: 2e76 656e 646f 725f 636f 6465 203d 3d20  .vendor_code == 
-000129b0: 5345 5353 494f 4e5f 4558 5049 5245 445f  SESSION_EXPIRED_
-000129c0: 434f 4445 3a0a 2020 2020 2020 2020 2020  CODE:.          
-000129d0: 2020 2020 2020 2320 4e65 6564 2074 6f20        # Need to 
-000129e0: 7265 6672 6573 6820 7468 6520 7365 7373  refresh the sess
-000129f0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00012a00: 2020 2020 7365 6c66 2e63 6f6e 6e65 6374      self.connect
-00012a10: 696f 6e2e 7265 6672 6573 6828 290a 2020  ion.refresh().  
-00012a20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00012a30: 616e 6420 7472 7920 6167 6169 6e0a 2020  and try again.  
-00012a40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012a50: 6c66 2e5f 6578 6563 7574 655f 6361 6e63  lf._execute_canc
-00012a60: 656c 6b69 6c6c 286f 702c 2069 6429 0a20  elkill(op, id). 
-00012a70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00012a80: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-00012a90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00012aa0: 2020 2020 2020 2020 7261 6973 6520 5f63          raise _c
-00012ab0: 6f6e 7665 7274 5f65 7863 6570 7469 6f6e  onvert_exception
-00012ac0: 2872 7370 2e72 6573 706f 6e73 6529 0a0a  (rsp.response)..
-00012ad0: 2020 2020 2320 544f 444f 3a20 7265 706c      # TODO: repl
-00012ae0: 6163 6520 7468 6520 6f74 6865 7220 6d65  ace the other me
-00012af0: 7461 6461 7461 2063 616c 6c0a 2020 2020  tadata call.    
-00012b00: 6465 6620 5f65 7865 6375 7465 5f73 7973  def _execute_sys
-00012b10: 7465 6d6d 6574 6164 6174 6128 7365 6c66  temmetadata(self
-00012b20: 2c20 6f70 2c20 7363 6865 6d61 3d4e 6f6e  , op, schema=Non
-00012b30: 652c 2074 6162 6c65 3d4e 6f6e 652c 2063  e, table=None, c
-00012b40: 6f6c 756d 6e3d 4e6f 6e65 2c20 7669 6577  olumn=None, view
-00012b50: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00012b60: 6661 6374 6f72 7920 3d20 5f4f 4349 454e  factory = _OCIEN
-00012b70: 545f 5245 5155 4553 545f 4641 4354 4f52  T_REQUEST_FACTOR
-00012b80: 4945 535b 2247 4554 2053 5953 5445 4d20  IES["GET SYSTEM 
-00012b90: 4d45 5441 4441 5441 225d 0a20 2020 2020  METADATA"].     
-00012ba0: 2020 2072 6571 203d 2066 6163 746f 7279     req = factory
-00012bb0: 2e72 6571 7565 7374 286f 702c 2073 6368  .request(op, sch
-00012bc0: 656d 612c 2074 6162 6c65 2c20 636f 6c75  ema, table, colu
-00012bd0: 6d6e 2c20 7669 6577 290a 0a20 2020 2020  mn, view)..     
-00012be0: 2020 205f 7365 6e64 5f6d 7367 2873 656c     _send_msg(sel
-00012bf0: 662e 636f 6e6e 6563 7469 6f6e 2c20 7265  f.connection, re
-00012c00: 7129 0a0a 2020 2020 2020 2020 7273 7020  q)..        rsp 
-00012c10: 3d20 5f72 6563 765f 6d73 6728 7365 6c66  = _recv_msg(self
-00012c20: 2e63 6f6e 6e65 6374 696f 6e2c 2066 6163  .connection, fac
-00012c30: 746f 7279 2e72 6573 706f 6e73 6528 2929  tory.response())
-00012c40: 0a0a 2020 2020 2020 2020 6966 2072 7370  ..        if rsp
-00012c50: 2e72 6573 706f 6e73 652e 7479 7065 203d  .response.type =
-00012c60: 3d20 7072 6f74 6f2e 436f 6e66 6972 6d61  = proto.Confirma
-00012c70: 7469 6f6e 5265 7370 6f6e 7365 2e52 4553  tionResponse.RES
-00012c80: 504f 4e53 455f 5741 524e 3a0a 2020 2020  PONSE_WARN:.    
-00012c90: 2020 2020 2020 2020 7761 726e 2872 7370          warn(rsp
-00012ca0: 2e72 6573 706f 6e73 652e 7265 6173 6f6e  .response.reason
-00012cb0: 290a 2020 2020 2020 2020 656c 6966 206e  ).        elif n
-00012cc0: 6f74 2072 7370 2e72 6573 706f 6e73 652e  ot rsp.response.
-00012cd0: 7479 7065 203d 3d20 7072 6f74 6f2e 436f  type == proto.Co
-00012ce0: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
-00012cf0: 7365 2e52 4553 504f 4e53 455f 4f4b 3a0a  se.RESPONSE_OK:.
-00012d00: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00012d10: 7370 2e72 6573 706f 6e73 652e 7665 6e64  sp.response.vend
-00012d20: 6f72 5f63 6f64 6520 3d3d 2053 4553 5349  or_code == SESSI
-00012d30: 4f4e 5f45 5850 4952 4544 5f43 4f44 453a  ON_EXPIRED_CODE:
-00012d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012d50: 2023 204e 6565 6420 746f 2072 6566 7265   # Need to refre
-00012d60: 7368 2074 6865 2073 6573 7369 6f6e 0a20  sh the session. 
-00012d70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012d80: 656c 662e 636f 6e6e 6563 7469 6f6e 2e72  elf.connection.r
-00012d90: 6566 7265 7368 2829 0a20 2020 2020 2020  efresh().       
-00012da0: 2020 2020 2020 2020 2023 2061 6e64 2074           # and t
-00012db0: 7279 2061 6761 696e 0a20 2020 2020 2020  ry again.       
-00012dc0: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
-00012dd0: 7865 6375 7465 5f73 7973 7465 6d6d 6574  xecute_systemmet
-00012de0: 6164 6174 6128 6f70 2c20 7363 6865 6d61  adata(op, schema
-00012df0: 3d73 6368 656d 612c 2074 6162 6c65 3d74  =schema, table=t
-00012e00: 6162 6c65 2c20 636f 6c75 6d6e 3d63 6f6c  able, column=col
-00012e10: 756d 6e2c 2076 6965 773d 7669 6577 290a  umn, view=view).
-00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e30: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-00012e40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00012e50: 2020 2020 2020 2020 2072 6169 7365 205f           raise _
-00012e60: 636f 6e76 6572 745f 6578 6365 7074 696f  convert_exceptio
-00012e70: 6e28 7273 702e 7265 7370 6f6e 7365 290a  n(rsp.response).
-00012e80: 0a20 2020 2020 2020 2069 6620 7273 702e  .        if rsp.
-00012e90: 4861 7346 6965 6c64 2822 7265 7375 6c74  HasField("result
-00012ea0: 5f73 6574 5f76 616c 2229 3a0a 2020 2020  _set_val"):.    
-00012eb0: 2020 2020 2020 2020 7365 6c66 2e5f 6765          self._ge
-00012ec0: 745f 7265 7375 6c74 5f6d 6574 6164 6174  t_result_metadat
-00012ed0: 6128 290a 0a20 2020 2020 2020 2020 2020  a()..           
-00012ee0: 2066 6f72 2062 6c6f 6220 696e 2072 7370   for blob in rsp
-00012ef0: 2e72 6573 756c 745f 7365 745f 7661 6c2e  .result_set_val.
-00012f00: 626c 6f62 733a 0a20 2020 2020 2020 2020  blobs:.         
-00012f10: 2020 2020 2020 2073 656c 662e 5f62 7566         self._buf
-00012f20: 6665 7273 2e61 7070 656e 6428 626c 6f62  fers.append(blob
-00012f30: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00012f40: 7475 726e 204e 6f6e 650a 0a20 2020 2020  turn None..     
-00012f50: 2020 2069 6620 7273 702e 4861 7346 6965     if rsp.HasFie
-00012f60: 6c64 2822 7374 7269 6e67 5f76 616c 2229  ld("string_val")
-00012f70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00012f80: 7475 726e 2072 7370 2e73 7472 696e 675f  turn rsp.string_
-00012f90: 7661 6c0a 0a20 2020 2020 2020 2072 6574  val..        ret
-00012fa0: 7572 6e20 7273 702e 696e 745f 7661 6c0a  urn rsp.int_val.
-00012fb0: 0a20 2020 2064 6566 205f 6765 745f 6d6f  .    def _get_mo
-00012fc0: 7265 5f64 6174 6128 7365 6c66 293a 0a20  re_data(self):. 
-00012fd0: 2020 2020 2020 2022 2222 496e 7465 726e         """Intern
-00012fe0: 616c 2072 6f75 7469 6e65 2074 6f20 6765  al routine to ge
-00012ff0: 7420 6d6f 7265 2064 6174 6120 6672 6f6d  t more data from
-00013000: 2061 2071 7565 7279 2222 220a 2020 2020   a query""".    
-00013010: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
-00013020: 7361 626c 653d 6e6f 2d6d 656d 6265 720a  sable=no-member.
-00013030: 2020 2020 2020 2020 7265 7120 3d20 7072          req = pr
-00013040: 6f74 6f2e 5265 7175 6573 7428 290a 2020  oto.Request().  
-00013050: 2020 2020 2020 7265 712e 7479 7065 203d        req.type =
-00013060: 2072 6571 2e46 4554 4348 5f44 4154 410a   req.FETCH_DATA.
-00013070: 2020 2020 2020 2020 7265 712e 6665 7463          req.fetc
-00013080: 685f 6461 7461 2e66 6574 6368 5f73 697a  h_data.fetch_siz
-00013090: 6520 3d20 7365 6c66 2e61 7272 6179 7369  e = self.arraysi
-000130a0: 7a65 0a20 2020 2020 2020 205f 7365 6e64  ze.        _send
-000130b0: 5f6d 7367 2873 656c 662e 636f 6e6e 6563  _msg(self.connec
-000130c0: 7469 6f6e 2c20 7265 7129 0a0a 2020 2020  tion, req)..    
-000130d0: 2020 2020 7273 7020 3d20 5f72 6563 765f      rsp = _recv_
-000130e0: 6d73 6728 7365 6c66 2e63 6f6e 6e65 6374  msg(self.connect
-000130f0: 696f 6e2c 2070 726f 746f 2e46 6574 6368  ion, proto.Fetch
-00013100: 4461 7461 5265 7370 6f6e 7365 2829 290a  DataResponse()).
-00013110: 0a20 2020 2020 2020 2069 6620 7273 702e  .        if rsp.
-00013120: 7265 7370 6f6e 7365 2e74 7970 6520 3d3d  response.type ==
-00013130: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
-00013140: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
-00013150: 4f4e 5345 5f45 5252 4f52 3a0a 2020 2020  ONSE_ERROR:.    
-00013160: 2020 2020 2020 2020 7261 6973 6520 5f63          raise _c
-00013170: 6f6e 7665 7274 5f65 7863 6570 7469 6f6e  onvert_exception
-00013180: 2872 7370 2e72 6573 706f 6e73 6529 0a0a  (rsp.response)..
-00013190: 2020 2020 2020 2020 666f 7220 626c 6f62          for blob
-000131a0: 2069 6e20 7273 702e 7265 7375 6c74 5f73   in rsp.result_s
-000131b0: 6574 2e62 6c6f 6273 3a0a 2020 2020 2020  et.blobs:.      
-000131c0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-000131d0: 662e 5f62 7566 6665 7273 3a0a 2020 2020  f._buffers:.    
-000131e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000131f0: 2e5f 6f66 6673 6574 203d 2030 0a20 2020  ._offset = 0.   
-00013200: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
-00013210: 7566 6665 7273 2e61 7070 656e 6428 626c  uffers.append(bl
-00013220: 6f62 290a 0a20 2020 2064 6566 2066 6574  ob)..    def fet
-00013230: 6368 6d61 6e79 2873 656c 662c 2073 697a  chmany(self, siz
-00013240: 653d 4e6f 6e65 293a 0a20 2020 2020 2020  e=None):.       
-00013250: 2022 2222 4665 7463 6820 7468 6520 6e65   """Fetch the ne
-00013260: 7874 2073 6574 206f 6620 726f 7773 206f  xt set of rows o
-00013270: 6620 6120 7175 6572 7920 7265 7375 6c74  f a query result
-00013280: 2c20 7265 7475 726e 696e 6720 6120 7365  , returning a se
-00013290: 7175 656e 6365 206f 660a 2020 2020 2020  quence of.      
-000132a0: 2020 7365 7175 656e 6365 7320 2865 2e67    sequences (e.g
-000132b0: 2e20 6120 6c69 7374 206f 6620 7475 706c  . a list of tupl
-000132c0: 6573 292e 2041 6e20 656d 7074 7920 7365  es). An empty se
-000132d0: 7175 656e 6365 2069 7320 7265 7475 726e  quence is return
-000132e0: 6564 2077 6865 6e20 6e6f 0a20 2020 2020  ed when no.     
-000132f0: 2020 206d 6f72 6520 726f 7773 2061 7265     more rows are
-00013300: 2061 7661 696c 6162 6c65 2e0a 0a20 2020   available...   
-00013310: 2020 2020 2054 6865 206e 756d 6265 7220       The number 
-00013320: 6f66 2072 6f77 7320 746f 2066 6574 6368  of rows to fetch
-00013330: 2070 6572 2063 616c 6c20 6973 2073 7065   per call is spe
-00013340: 6369 6669 6564 2062 7920 7468 6520 7061  cified by the pa
-00013350: 7261 6d65 7465 722e 2049 6620 6974 0a20  rameter. If it. 
-00013360: 2020 2020 2020 2069 7320 6e6f 7420 6769         is not gi
-00013370: 7665 6e2c 2074 6865 2063 7572 736f 7227  ven, the cursor'
-00013380: 7320 6172 7261 7973 697a 6520 6465 7465  s arraysize dete
-00013390: 726d 696e 6573 2074 6865 206e 756d 6265  rmines the numbe
-000133a0: 7220 6f66 2072 6f77 7320 746f 2062 650a  r of rows to be.
-000133b0: 2020 2020 2020 2020 6665 7463 6865 642e          fetched.
-000133c0: 2054 6865 206d 6574 686f 6420 7769 6c6c   The method will
-000133d0: 2074 7279 2074 6f20 6665 7463 6820 6173   try to fetch as
-000133e0: 206d 616e 7920 726f 7773 2061 7320 696e   many rows as in
-000133f0: 6469 6361 7465 6420 6279 2074 6865 2073  dicated by the s
-00013400: 697a 650a 2020 2020 2020 2020 7061 7261  ize.        para
-00013410: 6d65 7465 722e 2049 6620 7468 6973 2069  meter. If this i
-00013420: 7320 6e6f 7420 706f 7373 6962 6c65 2064  s not possible d
-00013430: 7565 2074 6f20 7468 6520 7370 6563 6966  ue to the specif
-00013440: 6965 6420 6e75 6d62 6572 206f 6620 726f  ied number of ro
-00013450: 7773 206e 6f74 0a20 2020 2020 2020 2062  ws not.        b
-00013460: 6569 6e67 2061 7661 696c 6162 6c65 2c20  eing available, 
-00013470: 6665 7765 7220 726f 7773 206d 6179 2062  fewer rows may b
-00013480: 6520 7265 7475 726e 6564 2e0a 2020 2020  e returned..    
-00013490: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000134a0: 6966 2073 697a 6520 6973 204e 6f6e 653a  if size is None:
-000134b0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-000134c0: 6520 3d20 7365 6c66 2e61 7272 6179 7369  e = self.arraysi
-000134d0: 7a65 0a0a 2020 2020 2020 2020 726f 7773  ze..        rows
-000134e0: 203d 205b 5d0a 2020 2020 2020 2020 7768   = [].        wh
-000134f0: 696c 6520 7369 7a65 203e 2030 3a0a 2020  ile size > 0:.  
-00013500: 2020 2020 2020 2020 2020 615f 726f 7720            a_row 
-00013510: 3d20 7365 6c66 2e66 6574 6368 6f6e 6528  = self.fetchone(
-00013520: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00013530: 2061 5f72 6f77 2069 7320 4e6f 6e65 3a0a   a_row is None:.
-00013540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013550: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
-00013560: 2020 726f 7773 2e61 7070 656e 6428 615f    rows.append(a_
-00013570: 726f 7729 0a20 2020 2020 2020 2020 2020  row).           
-00013580: 2073 697a 6520 2d3d 2031 0a20 2020 2020   size -= 1.     
-00013590: 2020 2072 6574 7572 6e20 726f 7773 0a0a     return rows..
-000135a0: 2020 2020 6465 6620 6665 7463 6861 6c6c      def fetchall
-000135b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000135c0: 2222 2246 6574 6368 2061 6c6c 2028 7265  """Fetch all (re
-000135d0: 6d61 696e 696e 6729 2072 6f77 7320 6f66  maining) rows of
-000135e0: 2061 2071 7565 7279 2072 6573 756c 742c   a query result,
-000135f0: 2072 6574 7572 6e69 6e67 2074 6865 6d20   returning them 
-00013600: 6173 2061 0a20 2020 2020 2020 2073 6571  as a.        seq
-00013610: 7565 6e63 6520 6f66 2073 6571 7565 6e63  uence of sequenc
-00013620: 6573 2028 652e 672e 2061 206c 6973 7420  es (e.g. a list 
-00013630: 6f66 2074 7570 6c65 7329 2e20 4e6f 7465  of tuples). Note
-00013640: 2074 6861 7420 7468 6520 6375 7273 6f72   that the cursor
-00013650: 2773 0a20 2020 2020 2020 2061 7272 6179  's.        array
-00013660: 7369 7a65 2061 7474 7269 6275 7465 2063  size attribute c
-00013670: 616e 2061 6666 6563 7420 7468 6520 7065  an affect the pe
-00013680: 7266 6f72 6d61 6e63 6520 6f66 2074 6869  rformance of thi
-00013690: 7320 6f70 6572 6174 696f 6e2e 0a20 2020  s operation..   
-000136a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000136b0: 2072 6574 7572 6e20 7365 6c66 2e66 6574   return self.fet
-000136c0: 6368 6d61 6e79 2873 697a 653d 7379 732e  chmany(size=sys.
-000136d0: 6d61 7873 697a 6529 0a0a 2020 2020 6465  maxsize)..    de
-000136e0: 6620 5f5f 6e65 7874 5f5f 2873 656c 6629  f __next__(self)
-000136f0: 3a0a 2020 2020 2020 2020 615f 726f 7720  :.        a_row 
-00013700: 3d20 7365 6c66 2e66 6574 6368 6f6e 6528  = self.fetchone(
-00013710: 290a 2020 2020 2020 2020 6966 2061 5f72  ).        if a_r
-00013720: 6f77 2069 7320 4e6f 6e65 3a0a 2020 2020  ow is None:.    
-00013730: 2020 2020 2020 2020 7261 6973 6520 5374          raise St
-00013740: 6f70 4974 6572 6174 696f 6e0a 2020 2020  opIteration.    
-00013750: 2020 2020 7265 7475 726e 2061 5f72 6f77      return a_row
-00013760: 0a0a 2020 2020 6465 6620 5f5f 6974 6572  ..    def __iter
-00013770: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-00013780: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
-00013790: 2020 2064 6566 2066 6574 6368 7661 6c28     def fetchval(
-000137a0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000137b0: 2222 5468 6520 6665 7463 6876 616c 2829  ""The fetchval()
-000137c0: 2063 6f6e 7665 6e69 656e 6365 206d 6574   convenience met
-000137d0: 686f 6420 7265 7475 726e 7320 7468 6520  hod returns the 
-000137e0: 6669 7273 7420 636f 6c75 6d6e 206f 6620  first column of 
-000137f0: 7468 650a 2020 2020 2020 2020 6669 7273  the.        firs
-00013800: 7420 726f 7720 6966 2074 6865 7265 2061  t row if there a
-00013810: 7265 2072 6573 756c 7473 2c20 6f74 6865  re results, othe
-00013820: 7277 6973 6520 6974 2072 6574 7572 6e73  rwise it returns
-00013830: 204e 6f6e 652e 0a20 2020 2020 2020 2022   None..        "
-00013840: 2222 0a20 2020 2020 2020 2061 726f 7720  "".        arow 
-00013850: 3d20 7365 6c66 2e66 6574 6368 6f6e 6528  = self.fetchone(
-00013860: 290a 2020 2020 2020 2020 6966 2061 726f  ).        if aro
-00013870: 773a 0a20 2020 2020 2020 2020 2020 2072  w:.            r
-00013880: 6574 7572 6e20 6172 6f77 5b30 5d0a 2020  eturn arow[0].  
-00013890: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-000138a0: 650a 0a20 2020 2064 6566 2066 6574 6368  e..    def fetch
-000138b0: 6f6e 6528 7365 6c66 293a 0a20 2020 2020  one(self):.     
-000138c0: 2020 2022 2222 4665 7463 6820 7468 6520     """Fetch the 
-000138d0: 6e65 7874 2072 6f77 206f 6620 6120 7175  next row of a qu
-000138e0: 6572 7920 7265 7375 6c74 2073 6574 2c20  ery result set, 
-000138f0: 7265 7475 726e 696e 6720 6120 7369 6e67  returning a sing
-00013900: 6c65 2073 6571 7565 6e63 652c 0a20 2020  le sequence,.   
-00013910: 2020 2020 206f 7220 4e6f 6e65 2077 6865       or None whe
-00013920: 6e20 6e6f 206d 6f72 6520 6461 7461 2069  n no more data i
-00013930: 7320 6176 6169 6c61 626c 652e 0a20 2020  s available..   
-00013940: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013950: 2023 2049 6620 7468 6572 6520 7761 7320   # If there was 
-00013960: 6e65 7665 7220 6120 7175 6572 7920 6578  never a query ex
-00013970: 6563 7574 6564 2c20 7468 726f 7720 616e  ecuted, throw an
-00013980: 2065 7272 6f72 0a20 2020 2020 2020 2069   error.        i
-00013990: 6620 7365 6c66 2e64 6573 6372 6970 7469  f self.descripti
-000139a0: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
-000139b0: 2020 2020 2020 2020 7261 6973 6520 5072          raise Pr
-000139c0: 6f67 7261 6d6d 696e 6745 7272 6f72 2822  ogrammingError("
-000139d0: 4e6f 2072 6573 756c 7420 7365 7420 6176  No result set av
-000139e0: 6169 6c61 626c 6522 290a 0a20 2020 2020  ailable")..     
-000139f0: 2020 2023 2070 796c 696e 743a 2064 6973     # pylint: dis
-00013a00: 6162 6c65 203d 2074 6f6f 2d6d 616e 792d  able = too-many-
-00013a10: 6272 616e 6368 6573 0a20 2020 2020 2020  branches.       
-00013a20: 2069 6620 7365 6c66 2e65 6e64 5f6f 665f   if self.end_of_
-00013a30: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-00013a40: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
-00013a50: 2020 2020 2020 2023 2073 7065 6369 616c         # special
-00013a60: 2063 6173 6520 6578 706c 6169 6e2e 0a20   case explain.. 
-00013a70: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-00013a80: 7870 6c61 696e 5f72 6573 756c 7420 6973  xplain_result is
-00013a90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00013aa0: 2020 2020 2020 2072 6574 203d 2073 656c         ret = sel
-00013ab0: 662e 6578 706c 6169 6e5f 7265 7375 6c74  f.explain_result
-00013ac0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00013ad0: 662e 656e 645f 6f66 5f64 6174 6120 3d20  f.end_of_data = 
-00013ae0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-00013af0: 2072 6574 7572 6e20 5b72 6574 5d0a 0a20   return [ret].. 
-00013b00: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
-00013b10: 6973 745f 7265 7375 6c74 2069 7320 6e6f  ist_result is no
-00013b20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00013b30: 2020 2020 6966 2073 656c 662e 5f6f 6666      if self._off
-00013b40: 7365 7420 3e3d 206c 656e 2873 656c 662e  set >= len(self.
-00013b50: 6c69 7374 5f72 6573 756c 7429 3a0a 2020  list_result):.  
-00013b60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013b70: 6c66 2e65 6e64 5f6f 665f 6461 7461 203d  lf.end_of_data =
-00013b80: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-00013b90: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00013ba0: 650a 2020 2020 2020 2020 2020 2020 615f  e.            a_
-00013bb0: 726f 7720 3d20 7365 6c66 2e6c 6973 745f  row = self.list_
-00013bc0: 7265 7375 6c74 5b73 656c 662e 5f6f 6666  result[self._off
-00013bd0: 7365 745d 0a20 2020 2020 2020 2020 2020  set].           
-00013be0: 2073 656c 662e 5f6f 6666 7365 7420 2b3d   self._offset +=
-00013bf0: 2031 0a20 2020 2020 2020 2020 2020 2072   1.            r
-00013c00: 6574 7572 6e20 615f 726f 770a 0a20 2020  eturn a_row..   
-00013c10: 2020 2020 2069 6620 7365 6c66 2e72 6f77       if self.row
-00013c20: 636f 756e 7420 3c20 303a 0a20 2020 2020  count < 0:.     
-00013c30: 2020 2020 2020 2073 656c 662e 726f 7763         self.rowc
-00013c40: 6f75 6e74 203d 2030 0a0a 2020 2020 2020  ount = 0..      
-00013c50: 2020 7768 696c 6520 6e6f 7420 7365 6c66    while not self
-00013c60: 2e5f 6275 6666 6572 733a 0a20 2020 2020  ._buffers:.     
-00013c70: 2020 2020 2020 2073 656c 662e 5f67 6574         self._get
-00013c80: 5f6d 6f72 655f 6461 7461 2829 0a20 2020  _more_data().   
-00013c90: 2020 2020 2020 2020 2077 6869 6c65 2073           while s
-00013ca0: 656c 662e 5f62 7566 6665 7273 2061 6e64  elf._buffers and
-00013cb0: 2073 656c 662e 5f62 7566 2829 203d 3d20   self._buf() == 
-00013cc0: 6222 5c30 5c30 5c30 5c30 223a 0a20 2020  b"\0\0\0\0":.   
-00013cd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013ce0: 662e 5f62 7566 6665 7273 2e70 6f70 2830  f._buffers.pop(0
-00013cf0: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00013d00: 6620 6e6f 7420 7365 6c66 2e5f 6275 6666  f not self._buff
-00013d10: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
-00013d20: 2020 2020 2023 206e 6f20 6461 7461 2079       # no data y
-00013d30: 6574 2e2e 2e77 6169 7420 736f 2077 6520  et...wait so we 
-00013d40: 646f 6e27 7420 6861 6d6d 6572 2074 6865  don't hammer the
-00013d50: 2068 6f73 7420 6265 666f 7265 2061 736b   host before ask
-00013d60: 696e 6720 666f 7220 6d6f 7265 0a20 2020  ing for more.   
-00013d70: 2020 2020 2020 2020 2020 2020 2073 6c65               sle
-00013d80: 6570 2830 2e32 3529 0a0a 2020 2020 2020  ep(0.25)..      
-00013d90: 2020 6966 2073 656c 662e 5f6f 6666 7365    if self._offse
-00013da0: 7420 3d3d 2030 3a0a 2020 2020 2020 2020  t == 0:.        
-00013db0: 2020 2020 7365 6c66 2e5f 6765 745f 6e75      self._get_nu
-00013dc0: 6d5f 726f 7773 2829 0a0a 2020 2020 2020  m_rows()..      
-00013dd0: 2020 726f 775f 6c65 6e67 7468 203d 2073    row_length = s
-00013de0: 656c 662e 5f67 6574 5f69 6e74 2829 202d  elf._get_int() -
-00013df0: 2034 2020 2320 726f 775f 6c65 6e67 7468   4  # row_length
-00013e00: 2069 6e63 6c75 6465 7320 7468 6520 3420   includes the 4 
-00013e10: 6279 7465 7320 7765 206a 7573 7420 636f  bytes we just co
-00013e20: 6e73 756d 6564 0a20 2020 2020 2020 2065  nsumed.        e
-00013e30: 6e64 5f6f 6666 7365 7420 3d20 7365 6c66  nd_offset = self
-00013e40: 2e5f 6f66 6673 6574 202b 2072 6f77 5f6c  ._offset + row_l
-00013e50: 656e 6774 680a 0a20 2020 2020 2020 2069  ength..        i
-00013e60: 6620 7365 6c66 2e5f 6279 7465 735f 7265  f self._bytes_re
-00013e70: 6d61 696e 696e 6728 2920 3d3d 2031 2061  maining() == 1 a
-00013e80: 6e64 2073 656c 662e 5f62 7566 2829 5b73  nd self._buf()[s
-00013e90: 656c 662e 5f6f 6666 7365 745d 203d 3d20  elf._offset] == 
-00013ea0: 5479 7065 436f 6465 732e 4445 4d3a 0a20  TypeCodes.DEM:. 
-00013eb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013ec0: 726f 7763 6f75 6e74 202d 3d20 310a 2020  rowcount -= 1.  
-00013ed0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00013ee0: 6275 6666 6572 732e 706f 7028 3029 0a20  buffers.pop(0). 
-00013ef0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013f00: 5f63 6c6f 7365 5f72 6573 756c 7473 6574  _close_resultset
-00013f10: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
-00013f20: 6574 7572 6e20 7365 6c66 2e5f 7072 6f63  eturn self._proc
-00013f30: 6573 735f 7065 6e64 696e 6728 290a 0a20  ess_pending().. 
-00013f40: 2020 2020 2020 2061 5f72 6f77 203d 205b         a_row = [
-00013f50: 5d0a 2020 2020 2020 2020 7768 696c 6520  ].        while 
-00013f60: 7365 6c66 2e5f 6f66 6673 6574 203c 2065  self._offset < e
-00013f70: 6e64 5f6f 6666 7365 743a 0a20 2020 2020  nd_offset:.     
-00013f80: 2020 2020 2020 2061 5f72 6f77 2e61 7070         a_row.app
-00013f90: 656e 6428 7365 6c66 2e5f 6465 636f 6465  end(self._decode
-00013fa0: 5f65 6e74 7279 2829 290a 0a20 2020 2020  _entry())..     
-00013fb0: 2020 2069 6620 7365 6c66 2e5f 6f66 6673     if self._offs
-00013fc0: 6574 203e 3d20 6c65 6e28 7365 6c66 2e5f  et >= len(self._
-00013fd0: 6275 6628 2929 3a0a 2020 2020 2020 2020  buf()):.        
-00013fe0: 2020 2020 7365 6c66 2e5f 6275 6666 6572      self._buffer
-00013ff0: 732e 706f 7028 3029 0a20 2020 2020 2020  s.pop(0).       
-00014000: 2020 2020 2073 656c 662e 5f6f 6666 7365       self._offse
-00014010: 7420 3d20 300a 2020 2020 2020 2020 7365  t = 0.        se
-00014020: 6c66 2e72 6f77 6e75 6d62 6572 202b 3d20  lf.rownumber += 
-00014030: 310a 2020 2020 2020 2020 7265 7475 726e  1.        return
-00014040: 2073 656c 662e 7265 7375 6c74 7365 745f   self.resultset_
-00014050: 7475 706c 652e 5f6d 616b 6528 615f 726f  tuple._make(a_ro
-00014060: 7729 0a0a 2020 2020 6465 6620 5f70 726f  w)..    def _pro
-00014070: 6365 7373 5f70 656e 6469 6e67 2873 656c  cess_pending(sel
-00014080: 6629 3a0a 2020 2020 2020 2020 2320 6966  f):.        # if
-00014090: 2077 6520 6861 7665 2061 6e79 2070 656e   we have any pen
-000140a0: 6469 6e67 2071 7565 7269 6573 2074 6f20  ding queries to 
-000140b0: 6578 6563 7574 652c 206b 6963 6b20 6f6e  execute, kick on
-000140c0: 6520 6f66 6620 6e6f 770a 2020 2020 2020  e off now.      
-000140d0: 2020 6966 2073 656c 662e 5f70 656e 6469    if self._pendi
-000140e0: 6e67 5f6f 7073 3a0a 2020 2020 2020 2020  ng_ops:.        
-000140f0: 2020 2020 7365 6c66 2e5f 6275 6666 6572      self._buffer
-00014100: 7320 3d20 5b5d 0a20 2020 2020 2020 2020  s = [].         
-00014110: 2020 2073 656c 662e 5f6f 6666 7365 7420     self._offset 
-00014120: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
-00014130: 7365 6c66 2e5f 6578 6563 7574 655f 696e  self._execute_in
-00014140: 7465 726e 616c 2873 656c 662e 5f70 656e  ternal(self._pen
-00014150: 6469 6e67 5f6f 7073 2e70 6f70 2830 2929  ding_ops.pop(0))
-00014160: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00014170: 7572 6e20 7365 6c66 2e66 6574 6368 6f6e  urn self.fetchon
-00014180: 6528 290a 0a20 2020 2020 2020 2073 656c  e()..        sel
-00014190: 662e 656e 645f 6f66 5f64 6174 6120 3d20  f.end_of_data = 
-000141a0: 5472 7565 0a20 2020 2020 2020 2072 6574  True.        ret
-000141b0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 6465  urn None..    de
-000141c0: 6620 5f62 7566 2873 656c 6629 3a0a 2020  f _buf(self):.  
-000141d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000141e0: 662e 5f62 7566 6665 7273 5b30 5d0a 0a20  f._buffers[0].. 
-000141f0: 2020 2064 6566 205f 6279 7465 735f 7265     def _bytes_re
-00014200: 6d61 696e 696e 6728 7365 6c66 293a 0a20  maining(self):. 
-00014210: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00014220: 6c66 2e5f 6275 6666 6572 733a 0a20 2020  lf._buffers:.   
-00014230: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00014240: 300a 2020 2020 2020 2020 7265 7475 726e  0.        return
-00014250: 206c 656e 2873 656c 662e 5f62 7566 6665   len(self._buffe
-00014260: 7273 5b30 5d29 202d 2073 656c 662e 5f6f  rs[0]) - self._o
-00014270: 6666 7365 740a 0a20 2020 2064 6566 205f  ffset..    def _
-00014280: 6765 745f 6e75 6d5f 726f 7773 2873 656c  get_num_rows(sel
-00014290: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-000142a0: 656c 662e 5f62 7974 6573 5f72 656d 6169  elf._bytes_remai
-000142b0: 6e69 6e67 2829 203e 3d20 343a 0a20 2020  ning() >= 4:.   
-000142c0: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
-000142d0: 7763 6f75 6e74 202b 3d20 7365 6c66 2e5f  wcount += self._
-000142e0: 6765 745f 696e 7428 290a 0a20 2020 2064  get_int()..    d
-000142f0: 6566 205f 6465 636f 6465 5f65 6e74 7279  ef _decode_entry
-00014300: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00014310: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-00014320: 653d 746f 6f2d 6d61 6e79 2d6c 6f63 616c  e=too-many-local
-00014330: 732c 746f 6f2d 6d61 6e79 2d72 6574 7572  s,too-many-retur
-00014340: 6e2d 7374 6174 656d 656e 7473 2c74 6f6f  n-statements,too
-00014350: 2d6d 616e 792d 6272 616e 6368 6573 2c74  -many-branches,t
-00014360: 6f6f 2d6d 616e 792d 7374 6174 656d 656e  oo-many-statemen
-00014370: 7473 0a20 2020 2020 2020 2063 6f6c 7479  ts.        colty
-00014380: 7065 203d 2073 656c 662e 5f67 6574 5f62  pe = self._get_b
-00014390: 7974 6528 290a 0a20 2020 2020 2020 2023  yte()..        #
-000143a0: 2065 6173 7920 636f 6e76 6572 7369 6f6e   easy conversion
-000143b0: 7320 7765 2063 616e 2064 6f20 7769 7468  s we can do with
-000143c0: 2073 7472 7563 7473 0a20 2020 2020 2020   structs.       
-000143d0: 2074 7970 655f 6d61 7020 3d20 7b54 7970   type_map = {Typ
-000143e0: 6543 6f64 6573 2e49 4e54 3a20 2221 6922  eCodes.INT: "!i"
-000143f0: 2c20 5479 7065 436f 6465 732e 4c4f 4e47  , TypeCodes.LONG
-00014400: 3a20 2221 7122 2c20 5479 7065 436f 6465  : "!q", TypeCode
-00014410: 732e 464c 4f41 543a 2022 2166 222c 2054  s.FLOAT: "!f", T
-00014420: 7970 6543 6f64 6573 2e44 4f55 424c 453a  ypeCodes.DOUBLE:
-00014430: 2022 2164 222c 2054 7970 6543 6f64 6573   "!d", TypeCodes
-00014440: 2e42 4f4f 4c45 414e 3a20 223f 222c 2054  .BOOLEAN: "?", T
-00014450: 7970 6543 6f64 6573 2e53 484f 5254 3a20  ypeCodes.SHORT: 
-00014460: 2221 6822 7d0a 0a20 2020 2020 2020 2023  "!h"}..        #
-00014470: 2069 6620 7468 6973 2069 7320 7468 6520   if this is the 
-00014480: 6561 7379 2063 6f6e 7665 7273 696f 6e2c  easy conversion,
-00014490: 206a 7573 7420 646f 2069 740a 2020 2020   just do it.    
-000144a0: 2020 2020 6966 2063 6f6c 7479 7065 2069      if coltype i
-000144b0: 6e20 7479 7065 5f6d 6170 3a0a 2020 2020  n type_map:.    
-000144c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000144d0: 656c 662e 5f67 6574 5f74 7970 6528 7479  elf._get_type(ty
-000144e0: 7065 5f6d 6170 5b63 6f6c 7479 7065 5d29  pe_map[coltype])
-000144f0: 0a0a 2020 2020 2020 2020 6966 2063 6f6c  ..        if col
-00014500: 7479 7065 203d 3d20 5479 7065 436f 6465  type == TypeCode
-00014510: 732e 5354 5249 4e47 3a0a 2020 2020 2020  s.STRING:.      
-00014520: 2020 2020 2020 7374 726c 656e 203d 2073        strlen = s
-00014530: 656c 662e 5f67 6574 5f69 6e74 2829 0a20  elf._get_int(). 
-00014540: 2020 2020 2020 2020 2020 206f 6666 7365             offse
-00014550: 7420 3d20 7365 6c66 2e5f 6f66 6673 6574  t = self._offset
-00014560: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014570: 662e 5f6f 6666 7365 7420 2b3d 2073 7472  f._offset += str
-00014580: 6c65 6e0a 2020 2020 2020 2020 2020 2020  len.            
-00014590: 7265 7475 726e 2073 656c 662e 5f62 7566  return self._buf
-000145a0: 2829 5b6f 6666 7365 7420 3a20 6f66 6673  ()[offset : offs
-000145b0: 6574 202b 2073 7472 6c65 6e5d 2e64 6563  et + strlen].dec
-000145c0: 6f64 6528 2275 7466 2d38 222c 2065 7272  ode("utf-8", err
-000145d0: 6f72 733d 2272 6570 6c61 6365 2229 0a0a  ors="replace")..
-000145e0: 2020 2020 2020 2020 6966 2063 6f6c 7479          if colty
-000145f0: 7065 203d 3d20 5479 7065 436f 6465 732e  pe == TypeCodes.
-00014600: 5449 4d45 5354 414d 503a 0a20 2020 2020  TIMESTAMP:.     
-00014610: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-00014620: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
-00014630: 7574 6366 726f 6d74 696d 6573 7461 6d70  utcfromtimestamp
-00014640: 2873 656c 662e 5f67 6574 5f6c 6f6e 6728  (self._get_long(
-00014650: 2929 0a0a 2020 2020 2020 2020 6966 2063  ))..        if c
-00014660: 6f6c 7479 7065 203d 3d20 5479 7065 436f  oltype == TypeCo
-00014670: 6465 732e 4e55 4c4c 3a0a 2020 2020 2020  des.NULL:.      
-00014680: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00014690: 650a 0a20 2020 2020 2020 2069 6620 636f  e..        if co
-000146a0: 6c74 7970 6520 3d3d 2054 7970 6543 6f64  ltype == TypeCod
-000146b0: 6573 2e42 5954 453a 0a20 2020 2020 2020  es.BYTE:.       
-000146c0: 2020 2020 2072 6574 7572 6e20 696e 742e       return int.
-000146d0: 6672 6f6d 5f62 7974 6573 2873 656c 662e  from_bytes(self.
-000146e0: 5f67 6574 5f74 7970 6528 2263 2229 2c20  _get_type("c"), 
-000146f0: 2262 6967 222c 2073 6967 6e65 643d 5472  "big", signed=Tr
-00014700: 7565 290a 0a20 2020 2020 2020 2069 6620  ue)..        if 
-00014710: 636f 6c74 7970 6520 3d3d 2054 7970 6543  coltype == TypeC
-00014720: 6f64 6573 2e54 494d 453a 0a20 2020 2020  odes.TIME:.     
-00014730: 2020 2020 2020 2073 6563 6f6e 6473 203d         seconds =
-00014740: 2073 656c 662e 5f67 6574 5f6c 6f6e 6728   self._get_long(
-00014750: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00014760: 636f 6e64 203d 2069 6e74 2873 6563 6f6e  cond = int(secon
-00014770: 6473 2025 2036 3029 0a20 2020 2020 2020  ds % 60).       
-00014780: 2020 2020 206d 696e 7574 6573 203d 2073       minutes = s
-00014790: 6563 6f6e 6473 202f 2036 300a 2020 2020  econds / 60.    
-000147a0: 2020 2020 2020 2020 6d69 6e75 7465 203d          minute =
-000147b0: 2069 6e74 286d 696e 7574 6573 2025 2036   int(minutes % 6
-000147c0: 3029 0a20 2020 2020 2020 2020 2020 2068  0).            h
-000147d0: 6f75 7273 203d 206d 696e 7574 6573 202f  ours = minutes /
-000147e0: 2036 300a 2020 2020 2020 2020 2020 2020   60.            
-000147f0: 686f 7572 203d 2069 6e74 2868 6f75 7273  hour = int(hours
-00014800: 2025 2032 3429 0a20 2020 2020 2020 2020   % 24).         
-00014810: 2020 2072 6574 7572 6e20 6461 7465 7469     return dateti
-00014820: 6d65 2e74 696d 6528 686f 7572 2c20 6d69  me.time(hour, mi
-00014830: 6e75 7465 2c20 7365 636f 6e64 290a 0a20  nute, second).. 
-00014840: 2020 2020 2020 2069 6620 636f 6c74 7970         if coltyp
-00014850: 6520 3d3d 2054 7970 6543 6f64 6573 2e42  e == TypeCodes.B
-00014860: 494e 4152 593a 0a20 2020 2020 2020 2020  INARY:.         
-00014870: 2020 2073 7472 6c65 6e20 3d20 7365 6c66     strlen = self
-00014880: 2e5f 6765 745f 696e 7428 290a 2020 2020  ._get_int().    
-00014890: 2020 2020 2020 2020 6f66 6673 6574 203d          offset =
-000148a0: 2073 656c 662e 5f6f 6666 7365 740a 2020   self._offset.  
-000148b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000148c0: 6f66 6673 6574 202b 3d20 7374 726c 656e  offset += strlen
-000148d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000148e0: 7572 6e20 7365 6c66 2e5f 6275 6628 295b  urn self._buf()[
-000148f0: 6f66 6673 6574 203a 206f 6666 7365 7420  offset : offset 
-00014900: 2b20 7374 726c 656e 5d0a 0a20 2020 2020  + strlen]..     
-00014910: 2020 2069 6620 636f 6c74 7970 6520 3d3d     if coltype ==
-00014920: 2054 7970 6543 6f64 6573 2e44 4543 494d   TypeCodes.DECIM
-00014930: 414c 3a0a 2020 2020 2020 2020 2020 2020  AL:.            
-00014940: 7072 6563 6973 696f 6e20 3d20 7365 6c66  precision = self
-00014950: 2e5f 6765 745f 6279 7465 2829 0a20 2020  ._get_byte().   
-00014960: 2020 2020 2020 2020 2073 6361 6c65 203d           scale =
-00014970: 2073 656c 662e 5f67 6574 5f62 7974 6528   self._get_byte(
-00014980: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00014990: 6620 7072 6563 6973 696f 6e20 2520 3220  f precision % 2 
-000149a0: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-000149b0: 2020 2020 2020 7374 726c 656e 203d 2069        strlen = i
-000149c0: 6e74 2828 7072 6563 6973 696f 6e20 2f20  nt((precision / 
-000149d0: 3229 202b 2031 290a 2020 2020 2020 2020  2) + 1).        
-000149e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000149f0: 2020 2020 2020 2020 2020 7374 726c 656e            strlen
-00014a00: 203d 2069 6e74 2828 7072 6563 6973 696f   = int((precisio
-00014a10: 6e20 2b20 3129 202f 2032 290a 0a20 2020  n + 1) / 2)..   
-00014a20: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-00014a30: 7365 6c66 2e5f 6275 6628 295b 7365 6c66  self._buf()[self
-00014a40: 2e5f 6f66 6673 6574 203a 2028 7365 6c66  ._offset : (self
-00014a50: 2e5f 6f66 6673 6574 202b 2073 7472 6c65  ._offset + strle
-00014a60: 6e20 2d20 3129 5d0a 2020 2020 2020 2020  n - 1)].        
-00014a70: 2020 2020 6469 6769 7473 203d 205b 5d0a      digits = [].
-00014a80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00014a90: 6279 7465 2069 6e20 6461 7461 3a0a 2020  byte in data:.  
-00014aa0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00014ab0: 6769 7473 2e61 7070 656e 6428 2862 7974  gits.append((byt
-00014ac0: 6520 2620 3078 4630 2920 3e3e 2034 290a  e & 0xF0) >> 4).
-00014ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ae0: 6469 6769 7473 2e61 7070 656e 6428 6279  digits.append(by
-00014af0: 7465 2026 2030 7830 4629 0a0a 2020 2020  te & 0x0F)..    
-00014b00: 2020 2020 2020 2020 7369 676e 203d 2073          sign = s
-00014b10: 656c 662e 5f62 7566 2829 5b73 656c 662e  elf._buf()[self.
-00014b20: 5f6f 6666 7365 7420 2b20 7374 726c 656e  _offset + strlen
-00014b30: 202d 2031 5d0a 0a20 2020 2020 2020 2020   - 1]..         
-00014b40: 2020 2064 6967 6974 732e 6170 7065 6e64     digits.append
-00014b50: 2873 6967 6e20 3e3e 2034 290a 2020 2020  (sign >> 4).    
-00014b60: 2020 2020 2020 2020 7369 676e 203d 2073          sign = s
-00014b70: 6967 6e20 2620 3078 3046 0a0a 2020 2020  ign & 0x0F..    
-00014b80: 2020 2020 2020 2020 6966 2073 6967 6e20          if sign 
-00014b90: 3d3d 2031 323a 0a20 2020 2020 2020 2020  == 12:.         
-00014ba0: 2020 2020 2020 2073 6967 6e20 3d20 300a         sign = 0.
-00014bb0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00014bc0: 2073 6967 6e20 3d3d 2031 333a 0a20 2020   sign == 13:.   
-00014bd0: 2020 2020 2020 2020 2020 2020 2073 6967               sig
-00014be0: 6e20 3d20 310a 2020 2020 2020 2020 2020  n = 1.          
-00014bf0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00014c00: 2020 2020 2020 2020 7261 6973 6520 4572          raise Er
-00014c10: 726f 7228 7265 6173 6f6e 3d66 2255 6e6b  ror(reason=f"Unk
-00014c20: 6e6f 776e 2064 6563 696d 616c 2073 6967  nown decimal sig
-00014c30: 6e20 7661 6c75 6520 7b73 6967 6e7d 2229  n value {sign}")
-00014c40: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00014c50: 6c66 2e5f 6f66 6673 6574 202b 3d20 7374  lf._offset += st
-00014c60: 726c 656e 0a20 2020 2020 2020 2020 2020  rlen.           
-00014c70: 2072 6574 7572 6e20 6465 6369 6d61 6c2e   return decimal.
-00014c80: 4465 6369 6d61 6c28 2873 6967 6e2c 2064  Decimal((sign, d
-00014c90: 6967 6974 732c 202d 7363 616c 6529 290a  igits, -scale)).
-00014ca0: 0a20 2020 2020 2020 2069 6620 636f 6c74  .        if colt
-00014cb0: 7970 6520 3d3d 2054 7970 6543 6f64 6573  ype == TypeCodes
-00014cc0: 2e41 5252 4159 3a0a 2020 2020 2020 2020  .ARRAY:.        
-00014cd0: 2020 2020 6e65 7374 6564 5f6c 6576 656c      nested_level
-00014ce0: 203d 2030 0a0a 2020 2020 2020 2020 2020   = 0..          
-00014cf0: 2020 6172 7261 7974 7970 6520 3d20 7365    arraytype = se
-00014d00: 6c66 2e5f 6765 745f 6279 7465 2829 0a0a  lf._get_byte()..
-00014d10: 2020 2020 2020 2020 2020 2020 7768 696c              whil
-00014d20: 6520 6172 7261 7974 7970 6520 3d3d 2054  e arraytype == T
-00014d30: 7970 6543 6f64 6573 2e41 5252 4159 3a0a  ypeCodes.ARRAY:.
-00014d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d50: 6172 7261 7974 7970 6520 3d20 7365 6c66  arraytype = self
-00014d60: 2e5f 6765 745f 6279 7465 2829 0a20 2020  ._get_byte().   
-00014d70: 2020 2020 2020 2020 2020 2020 206e 6573               nes
-00014d80: 7465 645f 6c65 7665 6c20 2b3d 2031 0a0a  ted_level += 1..
-00014d90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00014da0: 726e 2073 656c 662e 5f67 6574 5f61 7272  rn self._get_arr
-00014db0: 6179 286e 6573 7465 645f 6c65 7665 6c29  ay(nested_level)
-00014dc0: 0a0a 2020 2020 2020 2020 6966 2063 6f6c  ..        if col
-00014dd0: 7479 7065 203d 3d20 5479 7065 436f 6465  type == TypeCode
-00014de0: 732e 5555 4944 3a0a 2020 2020 2020 2020  s.UUID:.        
-00014df0: 2020 2020 7365 6c66 2e5f 6f66 6673 6574      self._offset
-00014e00: 202b 3d20 3136 0a20 2020 2020 2020 2020   += 16.         
-00014e10: 2020 2072 6574 7572 6e20 7575 6964 2e55     return uuid.U
-00014e20: 5549 4428 6279 7465 733d 7365 6c66 2e5f  UID(bytes=self._
-00014e30: 6275 6628 295b 7365 6c66 2e5f 6f66 6673  buf()[self._offs
-00014e40: 6574 202d 2031 3620 3a20 7365 6c66 2e5f  et - 16 : self._
-00014e50: 6f66 6673 6574 5d29 0a0a 2020 2020 2020  offset])..      
-00014e60: 2020 6966 2063 6f6c 7479 7065 203d 3d20    if coltype == 
-00014e70: 5479 7065 436f 6465 732e 5354 5f50 4f49  TypeCodes.ST_POI
-00014e80: 4e54 3a0a 2020 2020 2020 2020 2020 2020  NT:.            
-00014e90: 6c6f 6e67 203d 2073 656c 662e 5f67 6574  long = self._get
-00014ea0: 5f74 7970 6528 2221 6422 290a 2020 2020  _type("!d").    
-00014eb0: 2020 2020 2020 2020 6c61 7420 3d20 7365          lat = se
-00014ec0: 6c66 2e5f 6765 745f 7479 7065 2822 2164  lf._get_type("!d
-00014ed0: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
-00014ee0: 6620 6973 696e 6628 6c6f 6e67 2920 6f72  f isinf(long) or
-00014ef0: 2069 7369 6e66 286c 6174 293a 0a20 2020   isinf(lat):.   
-00014f00: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00014f10: 7572 6e20 2250 4f49 4e54 2045 4d50 5459  urn "POINT EMPTY
-00014f20: 220a 2020 2020 2020 2020 2020 2020 7265  ".            re
-00014f30: 7475 726e 2022 504f 494e 5428 2220 2b20  turn "POINT(" + 
-00014f40: 7374 7228 6c6f 6e67 2920 2b20 2220 2220  str(long) + " " 
-00014f50: 2b20 7374 7228 6c61 7429 202b 2022 2922  + str(lat) + ")"
-00014f60: 0a0a 2020 2020 2020 2020 6966 2063 6f6c  ..        if col
-00014f70: 7479 7065 203d 3d20 5479 7065 436f 6465  type == TypeCode
-00014f80: 732e 4441 5445 3a0a 2020 2020 2020 2020  s.DATE:.        
-00014f90: 2020 2020 6420 3d20 6461 7465 7469 6d65      d = datetime
-00014fa0: 2e64 6174 6574 696d 652e 7574 6366 726f  .datetime.utcfro
-00014fb0: 6d74 696d 6573 7461 6d70 2873 656c 662e  mtimestamp(self.
-00014fc0: 5f67 6574 5f6c 6f6e 6728 2920 2f20 3130  _get_long() / 10
-00014fd0: 3030 2e30 290a 2020 2020 2020 2020 2020  00.0).          
-00014fe0: 2020 7265 7475 726e 2064 6174 6574 696d    return datetim
-00014ff0: 652e 6461 7465 2864 2e79 6561 722c 2064  e.date(d.year, d
-00015000: 2e6d 6f6e 7468 2c20 642e 6461 7929 0a0a  .month, d.day)..
-00015010: 2020 2020 2020 2020 6966 2063 6f6c 7479          if colty
-00015020: 7065 203d 3d20 5479 7065 436f 6465 732e  pe == TypeCodes.
-00015030: 4950 3a0a 2020 2020 2020 2020 2020 2020  IP:.            
-00015040: 6f66 6620 3d20 7365 6c66 2e5f 6f66 6673  off = self._offs
-00015050: 6574 0a20 2020 2020 2020 2020 2020 2073  et.            s
-00015060: 656c 662e 5f6f 6666 7365 7420 2b3d 2031  elf._offset += 1
-00015070: 360a 2020 2020 2020 2020 2020 2020 7265  6.            re
-00015080: 7475 726e 2069 7061 6464 7265 7373 2e69  turn ipaddress.i
-00015090: 705f 6164 6472 6573 7328 7365 6c66 2e5f  p_address(self._
-000150a0: 6275 6628 295b 6f66 6620 3a20 6f66 6620  buf()[off : off 
-000150b0: 2b20 3136 5d29 0a0a 2020 2020 2020 2020  + 16])..        
-000150c0: 6966 2063 6f6c 7479 7065 203d 3d20 5479  if coltype == Ty
-000150d0: 7065 436f 6465 732e 4950 5634 3a0a 2020  peCodes.IPV4:.  
-000150e0: 2020 2020 2020 2020 2020 6f66 6620 3d20            off = 
-000150f0: 7365 6c66 2e5f 6f66 6673 6574 0a20 2020  self._offset.   
-00015100: 2020 2020 2020 2020 2073 656c 662e 5f6f           self._o
-00015110: 6666 7365 7420 2b3d 2034 0a20 2020 2020  ffset += 4.     
-00015120: 2020 2020 2020 2072 6574 7572 6e20 6970         return ip
-00015130: 6164 6472 6573 732e 6970 5f61 6464 7265  address.ip_addre
-00015140: 7373 2873 656c 662e 5f62 7566 2829 5b6f  ss(self._buf()[o
-00015150: 6666 203a 206f 6666 202b 2034 5d29 0a0a  ff : off + 4])..
-00015160: 2020 2020 2020 2020 6966 2063 6f6c 7479          if colty
-00015170: 7065 203d 3d20 5479 7065 436f 6465 732e  pe == TypeCodes.
-00015180: 5449 4d45 5354 414d 505f 4e41 4e4f 533a  TIMESTAMP_NANOS:
-00015190: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
-000151a0: 6573 7461 6d70 203d 2073 656c 662e 5f67  estamp = self._g
-000151b0: 6574 5f6c 6f6e 6728 2920 2f20 3130 3030  et_long() / 1000
-000151c0: 3030 3030 3030 2e30 0a20 2020 2020 2020  000000.0.       
-000151d0: 2020 2020 2072 6574 7572 6e20 6461 7465       return date
-000151e0: 7469 6d65 2e64 6174 6574 696d 652e 7574  time.datetime.ut
-000151f0: 6366 726f 6d74 696d 6573 7461 6d70 2874  cfromtimestamp(t
-00015200: 696d 6573 7461 6d70 290a 0a20 2020 2020  imestamp)..     
-00015210: 2020 2069 6620 636f 6c74 7970 6520 3d3d     if coltype ==
-00015220: 2054 7970 6543 6f64 6573 2e54 494d 455f   TypeCodes.TIME_
-00015230: 4e41 4e4f 533a 0a20 2020 2020 2020 2020  NANOS:.         
-00015240: 2020 206e 616e 6f73 203d 2073 656c 662e     nanos = self.
-00015250: 5f67 6574 5f6c 6f6e 6728 290a 2020 2020  _get_long().    
-00015260: 2020 2020 2020 2020 6d69 6372 6f73 203d          micros =
-00015270: 2069 6e74 2828 6e61 6e6f 7320 2f20 3130   int((nanos / 10
-00015280: 3030 2920 2520 3130 3030 3030 3029 0a20  00) % 1000000). 
-00015290: 2020 2020 2020 2020 2020 2073 6563 6f6e             secon
-000152a0: 6473 203d 206e 616e 6f73 202f 2031 3030  ds = nanos / 100
-000152b0: 3030 3030 3030 300a 2020 2020 2020 2020  0000000.        
-000152c0: 2020 2020 7365 636f 6e64 203d 2069 6e74      second = int
-000152d0: 2873 6563 6f6e 6473 2025 2036 3029 0a20  (seconds % 60). 
-000152e0: 2020 2020 2020 2020 2020 206d 696e 7574             minut
-000152f0: 6573 203d 2073 6563 6f6e 6473 202f 2036  es = seconds / 6
-00015300: 300a 2020 2020 2020 2020 2020 2020 6d69  0.            mi
-00015310: 6e75 7465 203d 2069 6e74 286d 696e 7574  nute = int(minut
-00015320: 6573 2025 2036 3029 0a20 2020 2020 2020  es % 60).       
-00015330: 2020 2020 2068 6f75 7273 203d 206d 696e       hours = min
-00015340: 7574 6573 202f 2036 300a 2020 2020 2020  utes / 60.      
-00015350: 2020 2020 2020 686f 7572 203d 2069 6e74        hour = int
-00015360: 2868 6f75 7273 2025 2032 3429 0a0a 2020  (hours % 24)..  
-00015370: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00015380: 2064 6174 6574 696d 652e 7469 6d65 2868   datetime.time(h
-00015390: 6f75 722c 206d 696e 7574 652c 2073 6563  our, minute, sec
-000153a0: 6f6e 642c 206d 6963 726f 7329 0a0a 2020  ond, micros)..  
-000153b0: 2020 2020 2020 6966 2063 6f6c 7479 7065        if coltype
-000153c0: 203d 3d20 5479 7065 436f 6465 732e 5455   == TypeCodes.TU
-000153d0: 504c 453a 0a20 2020 2020 2020 2020 2020  PLE:.           
-000153e0: 2072 6574 7572 6e20 7365 6c66 2e5f 6765   return self._ge
-000153f0: 745f 7475 706c 6528 290a 0a20 2020 2020  t_tuple()..     
-00015400: 2020 2069 6620 636f 6c74 7970 6520 3d3d     if coltype ==
-00015410: 2054 7970 6543 6f64 6573 2e53 545f 4c49   TypeCodes.ST_LI
-00015420: 4e45 5354 5249 4e47 3a0a 2020 2020 2020  NESTRING:.      
-00015430: 2020 2020 2020 706f 696e 7473 203d 205b        points = [
-00015440: 5d0a 2020 2020 2020 2020 2020 2020 6e75  ].            nu
-00015450: 6d5f 656c 656d 656e 7473 203d 2073 656c  m_elements = sel
-00015460: 662e 5f67 6574 5f69 6e74 2829 0a20 2020  f._get_int().   
-00015470: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00015480: 6e20 7261 6e67 6528 6e75 6d5f 656c 656d  n range(num_elem
-00015490: 656e 7473 293a 0a20 2020 2020 2020 2020  ents):.         
-000154a0: 2020 2020 2020 206c 6f6e 6720 3d20 7365         long = se
-000154b0: 6c66 2e5f 6765 745f 7479 7065 2822 2164  lf._get_type("!d
-000154c0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-000154d0: 2020 206c 6174 203d 2073 656c 662e 5f67     lat = self._g
-000154e0: 6574 5f74 7970 6528 2221 6422 290a 2020  et_type("!d").  
-000154f0: 2020 2020 2020 2020 2020 2020 2020 706f                po
-00015500: 696e 7473 2e61 7070 656e 6428 286c 6f6e  ints.append((lon
-00015510: 672c 206c 6174 2929 0a20 2020 2020 2020  g, lat)).       
-00015520: 2020 2020 2072 6574 7572 6e20 706f 696e       return poin
-00015530: 7473 0a0a 2020 2020 2020 2020 6966 2063  ts..        if c
-00015540: 6f6c 7479 7065 203d 3d20 5479 7065 436f  oltype == TypeCo
-00015550: 6465 732e 5354 5f50 4f4c 5947 4f4e 3a0a  des.ST_POLYGON:.
-00015560: 2020 2020 2020 2020 2020 2020 6578 7465              exte
-00015570: 7269 6f72 203d 205b 5d0a 2020 2020 2020  rior = [].      
-00015580: 2020 2020 2020 6e75 6d5f 656c 656d 656e        num_elemen
-00015590: 7473 203d 2073 656c 662e 5f67 6574 5f69  ts = self._get_i
-000155a0: 6e74 2829 0a20 2020 2020 2020 2020 2020  nt().           
-000155b0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-000155c0: 6e75 6d5f 656c 656d 656e 7473 293a 0a20  num_elements):. 
-000155d0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000155e0: 6f6e 6720 3d20 7365 6c66 2e5f 6765 745f  ong = self._get_
-000155f0: 7479 7065 2822 2164 2229 0a20 2020 2020  type("!d").     
-00015600: 2020 2020 2020 2020 2020 206c 6174 203d             lat =
-00015610: 2073 656c 662e 5f67 6574 5f74 7970 6528   self._get_type(
-00015620: 2221 6422 290a 2020 2020 2020 2020 2020  "!d").          
-00015630: 2020 2020 2020 6578 7465 7269 6f72 2e61        exterior.a
-00015640: 7070 656e 6428 286c 6f6e 672c 206c 6174  ppend((long, lat
-00015650: 2929 0a20 2020 2020 2020 2020 2020 2068  )).            h
-00015660: 6f6c 6573 203d 205b 5d0a 2020 2020 2020  oles = [].      
-00015670: 2020 2020 2020 6e75 6d5f 7269 6e67 7320        num_rings 
-00015680: 3d20 7365 6c66 2e5f 6765 745f 696e 7428  = self._get_int(
-00015690: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-000156a0: 7220 6920 696e 2072 616e 6765 286e 756d  r i in range(num
-000156b0: 5f72 696e 6773 293a 0a20 2020 2020 2020  _rings):.       
-000156c0: 2020 2020 2020 2020 206e 756d 5f65 6c65           num_ele
-000156d0: 6d65 6e74 7320 3d20 7365 6c66 2e5f 6765  ments = self._ge
-000156e0: 745f 696e 7428 290a 2020 2020 2020 2020  t_int().        
-000156f0: 2020 2020 2020 2020 7269 6e67 203d 205b          ring = [
-00015700: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00015710: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
-00015720: 286e 756d 5f65 6c65 6d65 6e74 7329 3a0a  (num_elements):.
-00015730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015740: 2020 2020 6c6f 6e67 203d 2073 656c 662e      long = self.
-00015750: 5f67 6574 5f74 7970 6528 2221 6422 290a  _get_type("!d").
-00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015770: 2020 2020 6c61 7420 3d20 7365 6c66 2e5f      lat = self._
-00015780: 6765 745f 7479 7065 2822 2164 2229 0a20  get_type("!d"). 
-00015790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157a0: 2020 2072 696e 672e 6170 7065 6e64 2828     ring.append((
-000157b0: 6c6f 6e67 2c20 6c61 7429 290a 2020 2020  long, lat)).    
-000157c0: 2020 2020 2020 2020 2020 2020 686f 6c65              hole
-000157d0: 732e 6170 7065 6e64 2872 696e 6729 0a20  s.append(ring). 
-000157e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000157f0: 6e20 2865 7874 6572 696f 722c 2068 6f6c  n (exterior, hol
-00015800: 6573 290a 0a20 2020 2020 2020 2073 656c  es)..        sel
-00015810: 662e 656e 645f 6f66 5f64 6174 6120 3d20  f.end_of_data = 
-00015820: 5472 7565 0a20 2020 2020 2020 2072 6169  True.        rai
-00015830: 7365 2045 7272 6f72 2872 6561 736f 6e3d  se Error(reason=
-00015840: 6622 556e 6b6e 6f77 6e20 636f 6c75 6d6e  f"Unknown column
-00015850: 2074 7970 6520 7b63 6f6c 7479 7065 7d22   type {coltype}"
-00015860: 290a 0a20 2020 2064 6566 205f 6765 745f  )..    def _get_
-00015870: 6279 7465 2873 656c 6629 3a0a 2020 2020  byte(self):.    
-00015880: 2020 2020 6f66 6673 6574 203d 2073 656c      offset = sel
-00015890: 662e 5f6f 6666 7365 740a 2020 2020 2020  f._offset.      
-000158a0: 2020 7365 6c66 2e5f 6f66 6673 6574 202b    self._offset +
-000158b0: 3d20 310a 2020 2020 2020 2020 7265 7475  = 1.        retu
-000158c0: 726e 2073 656c 662e 5f62 7566 2829 5b6f  rn self._buf()[o
-000158d0: 6666 7365 745d 0a0a 2020 2020 6465 6620  ffset]..    def 
-000158e0: 5f67 6574 5f69 6e74 2873 656c 6629 3a0a  _get_int(self):.
-000158f0: 2020 2020 2020 2020 6f66 6673 6574 203d          offset =
-00015900: 2073 656c 662e 5f6f 6666 7365 740a 2020   self._offset.  
-00015910: 2020 2020 2020 7365 6c66 2e5f 6f66 6673        self._offs
-00015920: 6574 202b 3d20 340a 2020 2020 2020 2020  et += 4.        
-00015930: 7265 7475 726e 2073 7472 7563 742e 756e  return struct.un
-00015940: 7061 636b 5f66 726f 6d28 2221 6922 2c20  pack_from("!i", 
-00015950: 7365 6c66 2e5f 6275 6628 292c 206f 6666  self._buf(), off
-00015960: 7365 7429 5b30 5d0a 0a20 2020 2064 6566  set)[0]..    def
-00015970: 205f 6765 745f 6c6f 6e67 2873 656c 6629   _get_long(self)
-00015980: 3a0a 2020 2020 2020 2020 6f66 6673 6574  :.        offset
-00015990: 203d 2073 656c 662e 5f6f 6666 7365 740a   = self._offset.
-000159a0: 2020 2020 2020 2020 7365 6c66 2e5f 6f66          self._of
-000159b0: 6673 6574 202b 3d20 380a 2020 2020 2020  fset += 8.      
-000159c0: 2020 7265 7475 726e 2073 7472 7563 742e    return struct.
-000159d0: 756e 7061 636b 5f66 726f 6d28 2221 7122  unpack_from("!q"
-000159e0: 2c20 7365 6c66 2e5f 6275 6628 292c 206f  , self._buf(), o
-000159f0: 6666 7365 7429 5b30 5d0a 0a20 2020 2064  ffset)[0]..    d
-00015a00: 6566 205f 6765 745f 7479 7065 2873 656c  ef _get_type(sel
-00015a10: 662c 2063 6f64 6529 3a0a 2020 2020 2020  f, code):.      
-00015a20: 2020 6f66 6673 6574 203d 2073 656c 662e    offset = self.
-00015a30: 5f6f 6666 7365 740a 2020 2020 2020 2020  _offset.        
-00015a40: 7365 6c66 2e5f 6f66 6673 6574 202b 3d20  self._offset += 
-00015a50: 7374 7275 6374 2e63 616c 6373 697a 6528  struct.calcsize(
-00015a60: 636f 6465 290a 2020 2020 2020 2020 7265  code).        re
-00015a70: 7475 726e 2073 7472 7563 742e 756e 7061  turn struct.unpa
-00015a80: 636b 5f66 726f 6d28 636f 6465 2c20 7365  ck_from(code, se
-00015a90: 6c66 2e5f 6275 6628 292c 206f 6666 7365  lf._buf(), offse
-00015aa0: 7429 5b30 5d0a 0a20 2020 2064 6566 205f  t)[0]..    def _
-00015ab0: 6765 745f 6172 7261 7928 7365 6c66 2c20  get_array(self, 
-00015ac0: 6c65 7665 6c29 3a0a 2020 2020 2020 2020  level):.        
-00015ad0: 6172 7261 7920 3d20 5b5d 0a0a 2020 2020  array = []..    
-00015ae0: 2020 2020 6e75 6d5f 656c 656d 656e 7473      num_elements
-00015af0: 203d 2073 656c 662e 5f67 6574 5f69 6e74   = self._get_int
-00015b00: 2829 0a0a 2020 2020 2020 2020 616c 6c5f  ()..        all_
-00015b10: 6e75 6c6c 203d 2073 656c 662e 5f67 6574  null = self._get
-00015b20: 5f62 7974 6528 290a 0a20 2020 2020 2020  _byte()..       
-00015b30: 2069 6620 616c 6c5f 6e75 6c6c 2021 3d20   if all_null != 
-00015b40: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-00015b50: 6574 7572 6e20 5b5d 0a0a 2020 2020 2020  eturn []..      
-00015b60: 2020 666f 7220 5f20 696e 2072 616e 6765    for _ in range
-00015b70: 286e 756d 5f65 6c65 6d65 6e74 7329 3a0a  (num_elements):.
-00015b80: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00015b90: 6576 656c 203e 2030 3a0a 2020 2020 2020  evel > 0:.      
-00015ba0: 2020 2020 2020 2020 2020 6172 7261 792e            array.
-00015bb0: 6170 7065 6e64 2873 656c 662e 5f67 6574  append(self._get
-00015bc0: 5f61 7272 6179 286c 6576 656c 202d 2031  _array(level - 1
-00015bd0: 2929 0a20 2020 2020 2020 2020 2020 2065  )).            e
-00015be0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00015bf0: 2020 2020 2061 7272 6179 2e61 7070 656e       array.appen
-00015c00: 6428 7365 6c66 2e5f 6465 636f 6465 5f65  d(self._decode_e
-00015c10: 6e74 7279 2829 290a 0a20 2020 2020 2020  ntry())..       
-00015c20: 2072 6574 7572 6e20 6172 7261 790a 0a20   return array.. 
-00015c30: 2020 2064 6566 205f 636c 6f73 655f 7265     def _close_re
-00015c40: 7375 6c74 7365 7428 7365 6c66 293a 0a20  sultset(self):. 
-00015c50: 2020 2020 2020 2072 6571 203d 2070 726f         req = pro
-00015c60: 746f 2e52 6571 7565 7374 2829 0a20 2020  to.Request().   
-00015c70: 2020 2020 2072 6571 2e74 7970 6520 3d20       req.type = 
-00015c80: 7072 6f74 6f2e 5265 7175 6573 742e 5265  proto.Request.Re
-00015c90: 7175 6573 7454 7970 652e 5661 6c75 6528  questType.Value(
-00015ca0: 2243 4c4f 5345 5f52 4553 554c 545f 5345  "CLOSE_RESULT_SE
-00015cb0: 5422 290a 0a20 2020 2020 2020 205f 7365  T")..        _se
-00015cc0: 6e64 5f6d 7367 2873 656c 662e 636f 6e6e  nd_msg(self.conn
-00015cd0: 6563 7469 6f6e 2c20 7265 7129 0a0a 2020  ection, req)..  
-00015ce0: 2020 2020 2020 7273 7020 3d20 5f72 6563        rsp = _rec
-00015cf0: 765f 6d73 6728 7365 6c66 2e63 6f6e 6e65  v_msg(self.conne
-00015d00: 6374 696f 6e2c 2070 726f 746f 2e43 6f6e  ction, proto.Con
-00015d10: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
-00015d20: 6528 2929 0a0a 2020 2020 2020 2020 6966  e())..        if
-00015d30: 2072 7370 2e74 7970 6520 3d3d 2070 726f   rsp.type == pro
-00015d40: 746f 2e43 6f6e 6669 726d 6174 696f 6e52  to.ConfirmationR
-00015d50: 6573 706f 6e73 652e 5245 5350 4f4e 5345  esponse.RESPONSE
-00015d60: 5f57 4152 4e3a 0a20 2020 2020 2020 2020  _WARN:.         
-00015d70: 2020 2077 6172 6e28 7273 702e 7265 6173     warn(rsp.reas
-00015d80: 6f6e 290a 2020 2020 2020 2020 656c 6966  on).        elif
-00015d90: 206e 6f74 2072 7370 2e74 7970 6520 3d3d   not rsp.type ==
-00015da0: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
-00015db0: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
-00015dc0: 4f4e 5345 5f4f 4b3a 0a20 2020 2020 2020  ONSE_OK:.       
-00015dd0: 2020 2020 2072 6169 7365 205f 636f 6e76       raise _conv
-00015de0: 6572 745f 6578 6365 7074 696f 6e28 7273  ert_exception(rs
-00015df0: 7029 0a0a 2020 2020 6465 6620 5f67 6574  p)..    def _get
-00015e00: 5f74 7570 6c65 2873 656c 6629 3a0a 2020  _tuple(self):.  
-00015e10: 2020 2020 2020 6e75 6d5f 656c 656d 656e        num_elemen
-00015e20: 7473 203d 2073 656c 662e 5f67 6574 5f69  ts = self._get_i
-00015e30: 6e74 2829 0a20 2020 2020 2020 2072 6573  nt().        res
-00015e40: 7475 706c 6520 3d20 2829 0a20 2020 2020  tuple = ().     
-00015e50: 2020 2066 6f72 205f 2069 6e20 7261 6e67     for _ in rang
-00015e60: 6528 6e75 6d5f 656c 656d 656e 7473 293a  e(num_elements):
-00015e70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00015e80: 7475 706c 6520 2b3d 2028 7365 6c66 2e5f  tuple += (self._
-00015e90: 6465 636f 6465 5f65 6e74 7279 2829 2c29  decode_entry(),)
-00015ea0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00015eb0: 7265 7374 7570 6c65 0a0a 0a64 6566 2063  restuple...def c
-00015ec0: 6f6e 6e65 6374 2864 736e 3d4e 6f6e 652c  onnect(dsn=None,
-00015ed0: 2075 7365 723d 4e6f 6e65 2c20 7061 7373   user=None, pass
-00015ee0: 776f 7264 3d4e 6f6e 652c 2068 6f73 743d  word=None, host=
-00015ef0: 4e6f 6e65 2c20 6461 7461 6261 7365 3d4e  None, database=N
-00015f00: 6f6e 652c 2074 6c73 3d4e 6f6e 652c 2066  one, tls=None, f
-00015f10: 6f72 6365 3d4e 6f6e 652c 2068 616e 6473  orce=None, hands
-00015f20: 6861 6b65 3d22 6763 6d22 2c20 636f 6e66  hake="gcm", conf
-00015f30: 6967 6669 6c65 3d4e 6f6e 6529 3a0a 2020  igfile=None):.  
-00015f40: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-00015f50: 626c 653d 746f 6f2d 6d61 6e79 2d61 7267  ble=too-many-arg
-00015f60: 756d 656e 7473 0a20 2020 2022 2222 4372  uments.    """Cr
-00015f70: 6561 7465 2061 206e 6577 2064 6174 6162  eate a new datab
-00015f80: 6173 6520 636f 6e6e 6563 7469 6f6e 2e0a  ase connection..
-00015f90: 0a20 2020 2054 6865 2063 6f6e 6e65 6374  .    The connect
-00015fa0: 696f 6e20 7061 7261 6d65 7465 7273 2063  ion parameters c
-00015fb0: 616e 2062 6520 7370 6563 6966 6965 6420  an be specified 
-00015fc0: 6173 2070 6172 7420 6f66 2074 6865 2064  as part of the d
-00015fd0: 736e 2c0a 2020 2020 7573 696e 6720 6b65  sn,.    using ke
-00015fe0: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
-00015ff0: 6f72 2062 6f74 682e 2020 4966 2062 6f74  or both.  If bot
-00016000: 6820 6172 6520 7370 6563 6966 6965 642c  h are specified,
-00016010: 2074 6865 206b 6579 776f 7264 0a20 2020   the keyword.   
-00016020: 2070 6172 616d 6574 6572 206f 7665 7272   parameter overr
-00016030: 6964 6573 2074 6865 2076 616c 7565 2069  ides the value i
-00016040: 6e20 7468 6520 6473 6e2e 0a0a 2020 2020  n the dsn...    
-00016050: 5468 6520 4f63 6965 6e74 2044 534e 2069  The Ocient DSN i
-00016060: 7320 6f66 2074 6865 2066 6f72 6d61 743a  s of the format:
-00016070: 0a20 2020 2060 6f63 6965 6e74 3a2f 2f75  .    `ocient://u
-00016080: 7365 723a 7061 7373 776f 7264 405b 686f  ser:password@[ho
-00016090: 7374 5d5b 3a70 6f72 745d 5b2f 6461 7461  st][:port][/data
-000160a0: 6261 7365 5d5b 3f70 6172 616d 313d 7661  base][?param1=va
-000160b0: 6c75 6531 262e 2e2e 5d60 0a0a 2020 2020  lue1&...]`..    
-000160c0: 6075 7365 7260 2061 6e64 2060 7061 7373  `user` and `pass
-000160d0: 776f 7264 6020 6d75 7374 2062 6520 7375  word` must be su
-000160e0: 7070 6c69 6564 2e20 2060 686f 7374 6020  pplied.  `host` 
-000160f0: 6465 6661 756c 7473 2074 6f20 6c6f 6361  defaults to loca
-00016100: 6c68 6f73 742c 0a20 2020 2070 6f72 7420  lhost,.    port 
-00016110: 6465 6661 756c 7473 2074 6f20 3430 3530  defaults to 4050
-00016120: 2c20 6461 7461 6261 7365 2064 6566 6175  , database defau
-00016130: 6c74 7320 746f 2060 7379 7374 656d 6020  lts to `system` 
-00016140: 616e 6420 6074 6c73 6020 6465 6661 756c  and `tls` defaul
-00016150: 7473 0a20 2020 2074 6f20 6075 6e76 6572  ts.    to `unver
-00016160: 6966 6965 6460 2e0a 0a20 2020 204d 756c  ified`...    Mul
-00016170: 7469 706c 6520 686f 7374 7320 6d61 7920  tiple hosts may 
-00016180: 6265 2073 7065 6369 6669 6564 2c20 7365  be specified, se
-00016190: 7061 7261 7465 6420 6279 2061 2063 6f6d  parated by a com
-000161a0: 6d61 2c20 696e 2077 6869 6368 2063 6173  ma, in which cas
-000161b0: 6520 7468 650a 2020 2020 686f 7374 7320  e the.    hosts 
-000161c0: 7769 6c6c 2062 6520 7472 6965 6420 696e  will be tried in
-000161d0: 206f 7264 6572 2020 5468 7573 2061 6e20   order  Thus an 
-000161e0: 6578 616d 706c 6520 4453 4e20 6d69 6768  example DSN migh
-000161f0: 7420 6265 0a20 2020 2060 6f63 6965 6e74  t be.    `ocient
-00016200: 3a2f 2f73 6f6d 656f 6e65 3a73 6f6d 6570  ://someone:somep
-00016210: 6173 7377 6f72 6440 686f 7374 312c 686f  assword@host1,ho
-00016220: 7374 323a 3430 3531 2f6d 7964 6260 0a0a  st2:4051/mydb`..
-00016230: 2020 2020 636f 6e66 6967 6669 6c65 2073      configfile s
-00016240: 7065 6369 6669 6573 2074 6865 206e 616d  pecifies the nam
-00016250: 6520 6f66 2061 2063 6f6e 6669 6775 7261  e of a configura
-00016260: 7469 6f6e 2066 696c 6520 696e 2049 4e49  tion file in INI
-00016270: 2066 6f72 6d61 742e 2053 6565 0a20 2020   format. See.   
-00016280: 2074 6865 2043 6f6e 6e65 6374 696f 6e20   the Connection 
-00016290: 636c 6173 7320 666f 7220 6d6f 7265 2064  class for more d
-000162a0: 6574 6169 6c65 6420 646f 6375 6d65 6e74  etailed document
-000162b0: 6174 696f 6e2e 0a0a 2020 2020 4375 7272  ation...    Curr
-000162c0: 656e 746c 7920 7375 7070 6f72 7465 6420  ently supported 
-000162d0: 7061 7261 6d65 7465 7273 2061 7265 3a0a  parameters are:.
-000162e0: 0a20 2020 202d 2074 6c73 3a20 5768 6963  .    - tls: Whic
-000162f0: 6820 6361 6e20 6861 7665 2074 6865 2076  h can have the v
-00016300: 616c 7565 7320 226f 6666 222c 2022 756e  alues "off", "un
-00016310: 7665 7269 6669 6564 222c 206f 7220 226f  verified", or "o
-00016320: 6e22 2069 6e20 7468 6520 6473 6e2c 0a20  n" in the dsn,. 
-00016330: 2020 2020 2020 2020 6f72 2043 6f6e 6e65          or Conne
-00016340: 6374 696f 6e2e 544c 535f 4e4f 4e45 2c20  ction.TLS_NONE, 
-00016350: 436f 6e6e 6563 7469 6f6e 2e54 4c53 5f55  Connection.TLS_U
-00016360: 4e56 4552 4946 4945 442c 206f 720a 2020  NVERIFIED, or.  
-00016370: 2020 2020 2020 2043 6f6e 6e65 6374 696f         Connectio
-00016380: 6e2e 544c 535f 4f4e 2061 7320 6120 6b65  n.TLS_ON as a ke
-00016390: 7977 6f72 6420 7061 7261 6d65 7465 722e  yword parameter.
-000163a0: 0a20 2020 202d 2068 616e 6473 6861 6b65  .    - handshake
-000163b0: 3a20 2243 4243 222c 2022 4743 4d22 2c20  : "CBC", "GCM", 
-000163c0: 6f72 2022 5353 4f22 2e20 2247 434d 2220  or "SSO". "GCM" 
-000163d0: 2847 616c 6f69 7320 436f 756e 7465 7220  (Galois Counter 
-000163e0: 4d6f 6465 2920 7368 6f75 6c64 2062 6520  Mode) should be 
-000163f0: 7573 6564 206f 7665 7220 2243 4243 2220  used over "CBC" 
-00016400: 2843 6970 6865 7220 426c 6f63 6b20 4368  (Cipher Block Ch
-00016410: 6169 6e69 6e67 2920 666f 7220 7061 7373  aining) for pass
-00016420: 776f 7264 2065 6e63 7279 7074 696f 6e2e  word encryption.
-00016430: 2022 5353 4f22 2066 6f72 2073 696e 676c   "SSO" for singl
-00016440: 6520 7369 676e 206f 6e2e 0a20 2020 202d  e sign on..    -
-00016450: 2066 6f72 6365 3a20 666f 7263 6520 7468   force: force th
-00016460: 6520 636f 6e6e 6563 7469 6f6e 2074 6f20  e connection to 
-00016470: 7265 6d61 696e 206f 6e20 7468 6973 2068  remain on this h
-00016480: 6f73 740a 2020 2020 2222 220a 2020 2020  ost.    """.    
-00016490: 6966 2069 7369 6e73 7461 6e63 6528 6861  if isinstance(ha
-000164a0: 6e64 7368 616b 652c 2073 7472 293a 0a20  ndshake, str):. 
-000164b0: 2020 2020 2020 2069 6620 6861 6e64 7368         if handsh
-000164c0: 616b 652e 6c6f 7765 7228 2920 3d3d 2022  ake.lower() == "
-000164d0: 6763 6d22 3a0a 2020 2020 2020 2020 2020  gcm":.          
-000164e0: 2020 6861 6e64 7368 616b 6520 3d20 436f    handshake = Co
-000164f0: 6e6e 6563 7469 6f6e 2e48 414e 4453 4841  nnection.HANDSHA
-00016500: 4b45 5f47 434d 0a20 2020 2020 2020 2065  KE_GCM.        e
-00016510: 6c69 6620 6861 6e64 7368 616b 652e 6c6f  lif handshake.lo
-00016520: 7765 7228 2920 3d3d 2022 6362 6322 3a0a  wer() == "cbc":.
-00016530: 2020 2020 2020 2020 2020 2020 6861 6e64              hand
-00016540: 7368 616b 6520 3d20 436f 6e6e 6563 7469  shake = Connecti
-00016550: 6f6e 2e48 414e 4453 4841 4b45 5f43 4243  on.HANDSHAKE_CBC
-00016560: 0a20 2020 2020 2020 2065 6c69 6620 6861  .        elif ha
-00016570: 6e64 7368 616b 652e 6c6f 7765 7228 2920  ndshake.lower() 
-00016580: 3d3d 2022 7373 6f22 3a0a 2020 2020 2020  == "sso":.      
-00016590: 2020 2020 2020 6861 6e64 7368 616b 6520        handshake 
-000165a0: 3d20 436f 6e6e 6563 7469 6f6e 2e48 414e  = Connection.HAN
-000165b0: 4453 4841 4b45 5f53 534f 0a20 2020 2020  DSHAKE_SSO.     
-000165c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000165d0: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
-000165e0: 6d65 4572 726f 7228 6622 556e 6b6e 6f77  meError(f"Unknow
-000165f0: 6e20 4861 6e64 7368 616b 6520 6d65 7468  n Handshake meth
-00016600: 6f64 207b 6861 6e64 7368 616b 657d 2229  od {handshake}")
-00016610: 0a0a 2020 2020 6966 2069 7369 6e73 7461  ..    if isinsta
-00016620: 6e63 6528 746c 732c 2073 7472 293a 0a20  nce(tls, str):. 
-00016630: 2020 2020 2020 2069 6620 746c 732e 6c6f         if tls.lo
-00016640: 7765 7228 2920 3d3d 2022 6f6e 223a 0a20  wer() == "on":. 
-00016650: 2020 2020 2020 2020 2020 2074 6c73 203d             tls =
-00016660: 2043 6f6e 6e65 6374 696f 6e2e 544c 535f   Connection.TLS_
-00016670: 4f4e 0a20 2020 2020 2020 2065 6c69 6620  ON.        elif 
-00016680: 746c 732e 6c6f 7765 7228 2920 3d3d 2022  tls.lower() == "
-00016690: 756e 7665 7269 6669 6564 223a 0a20 2020  unverified":.   
-000166a0: 2020 2020 2020 2020 2074 6c73 203d 2043           tls = C
-000166b0: 6f6e 6e65 6374 696f 6e2e 544c 535f 554e  onnection.TLS_UN
-000166c0: 5645 5249 4649 4544 0a20 2020 2020 2020  VERIFIED.       
-000166d0: 2065 6c69 6620 746c 732e 6c6f 7765 7228   elif tls.lower(
-000166e0: 2920 3d3d 2022 6f66 6622 3a0a 2020 2020  ) == "off":.    
-000166f0: 2020 2020 2020 2020 746c 7320 3d20 436f          tls = Co
-00016700: 6e6e 6563 7469 6f6e 2e54 4c53 5f4e 4f4e  nnection.TLS_NON
-00016710: 450a 2020 2020 2020 2020 656c 7365 3a0a  E.        else:.
-00016720: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00016730: 6520 5275 6e74 696d 6545 7272 6f72 2866  e RuntimeError(f
-00016740: 2255 6e6b 6e6f 776e 2054 4c53 206d 6f64  "Unknown TLS mod
-00016750: 6520 7b74 6c73 7d22 290a 0a20 2020 2070  e {tls}")..    p
-00016760: 6172 616d 7320 3d20 7b0a 2020 2020 2020  arams = {.      
-00016770: 2020 2275 7365 7222 3a20 7573 6572 2c0a    "user": user,.
-00016780: 2020 2020 2020 2020 2270 6173 7377 6f72          "passwor
-00016790: 6422 3a20 222a 2a2a 2a2a 222c 0a20 2020  d": "*****",.   
-000167a0: 2020 2020 2022 686f 7374 223a 2068 6f73       "host": hos
-000167b0: 742c 0a20 2020 2020 2020 2022 6461 7461  t,.        "data
-000167c0: 6261 7365 223a 2064 6174 6162 6173 652c  base": database,
-000167d0: 0a20 2020 2020 2020 2022 746c 7322 3a20  .        "tls": 
-000167e0: 746c 732c 0a20 2020 2020 2020 2022 6861  tls,.        "ha
-000167f0: 6e64 7368 616b 6522 3a20 6861 6e64 7368  ndshake": handsh
-00016800: 616b 652c 0a20 2020 207d 0a0a 2020 2020  ake,.    }..    
-00016810: 6c6f 6767 6572 2e64 6562 7567 2866 2243  logger.debug(f"C
-00016820: 6f6e 6e65 6374 207b 7061 7261 6d73 7d22  onnect {params}"
-00016830: 290a 0a20 2020 2072 6574 7572 6e20 436f  )..    return Co
-00016840: 6e6e 6563 7469 6f6e 2864 736e 2c20 7573  nnection(dsn, us
-00016850: 6572 2c20 7061 7373 776f 7264 2c20 686f  er, password, ho
-00016860: 7374 2c20 6461 7461 6261 7365 2c20 746c  st, database, tl
-00016870: 732c 2068 616e 6473 6861 6b65 2c20 666f  s, handshake, fo
-00016880: 7263 652c 2063 6f6e 6669 6766 696c 6529  rce, configfile)
-00016890: 0a0a 0a64 6566 205f 6375 7374 6f6d 5f74  ...def _custom_t
-000168a0: 7970 655f 746f 5f6a 736f 6e28 6f62 6a29  ype_to_json(obj)
-000168b0: 3a0a 2020 2020 2222 2248 656c 7065 7220  :.    """Helper 
-000168c0: 6675 6e63 7469 6f6e 2074 6f20 636f 6e76  function to conv
-000168d0: 6572 7420 7479 7065 7320 7265 7475 726e  ert types return
-000168e0: 6564 2066 726f 6d20 7175 6572 6965 7320  ed from queries 
-000168f0: 746f 0a20 2020 204a 534f 4e20 7661 6c75  to.    JSON valu
-00016900: 6573 2e20 2054 7970 6963 616c 6c79 2069  es.  Typically i
-00016910: 6e76 6f6b 6564 2070 6173 7365 6420 6173  nvoked passed as
-00016920: 2074 6865 2060 6465 6661 756c 7460 2070   the `default` p
-00016930: 6172 616d 6574 6572 0a20 2020 2074 6f20  arameter.    to 
-00016940: 6a73 6f6e 2e64 756d 7073 2061 7320 696e  json.dumps as in
-00016950: 3a0a 0a20 2020 2060 6a73 6f6e 2e64 756d  :..    `json.dum
-00016960: 7073 2873 6f6d 655f 726f 7773 2c20 6465  ps(some_rows, de
-00016970: 6661 756c 743d 5f63 7573 746f 6d5f 7479  fault=_custom_ty
-00016980: 7065 5f74 6f5f 6a73 6f6e 2960 0a20 2020  pe_to_json)`.   
-00016990: 2022 2222 0a20 2020 2069 6620 6973 696e   """.    if isin
-000169a0: 7374 616e 6365 286f 626a 2c20 6465 6369  stance(obj, deci
-000169b0: 6d61 6c2e 4465 6369 6d61 6c29 3a0a 2020  mal.Decimal):.  
-000169c0: 2020 2020 2020 7265 7475 726e 2073 7472        return str
-000169d0: 286f 626a 290a 0a20 2020 2069 6620 6973  (obj)..    if is
-000169e0: 696e 7374 616e 6365 286f 626a 2c20 6461  instance(obj, da
-000169f0: 7465 7469 6d65 2e64 6174 6574 696d 6529  tetime.datetime)
-00016a00: 206f 7220 6973 696e 7374 616e 6365 286f   or isinstance(o
-00016a10: 626a 2c20 6461 7465 7469 6d65 2e64 6174  bj, datetime.dat
-00016a20: 6529 206f 7220 6973 696e 7374 616e 6365  e) or isinstance
-00016a30: 286f 626a 2c20 6461 7465 7469 6d65 2e74  (obj, datetime.t
-00016a40: 696d 6529 3a0a 2020 2020 2020 2020 7265  ime):.        re
-00016a50: 7475 726e 206f 626a 2e69 736f 666f 726d  turn obj.isoform
-00016a60: 6174 2829 0a0a 2020 2020 6966 2069 7369  at()..    if isi
-00016a70: 6e73 7461 6e63 6528 6f62 6a2c 2062 7974  nstance(obj, byt
-00016a80: 6573 293a 0a20 2020 2020 2020 2072 6574  es):.        ret
-00016a90: 7572 6e20 6c69 7374 286f 626a 290a 0a20  urn list(obj).. 
-00016aa0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00016ab0: 286f 626a 2c20 7575 6964 2e55 5549 4429  (obj, uuid.UUID)
-00016ac0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00016ad0: 2073 7472 286f 626a 290a 0a20 2020 2069   str(obj)..    i
-00016ae0: 6620 6973 696e 7374 616e 6365 286f 626a  f isinstance(obj
-00016af0: 2c20 6970 6164 6472 6573 732e 4950 7634  , ipaddress.IPv4
-00016b00: 4164 6472 6573 7329 206f 7220 6973 696e  Address) or isin
-00016b10: 7374 616e 6365 286f 626a 2c20 6970 6164  stance(obj, ipad
-00016b20: 6472 6573 732e 4950 7636 4164 6472 6573  dress.IPv6Addres
-00016b30: 7329 3a0a 2020 2020 2020 2020 7265 7475  s):.        retu
-00016b40: 726e 2073 7472 286f 626a 290a 0a20 2020  rn str(obj)..   
-00016b50: 2070 7269 6e74 2866 2274 7970 655f 746f   print(f"type_to
-00016b60: 5f73 7472 696e 6720 676f 7420 6361 6c6c  _string got call
-00016b70: 6564 2066 6f72 2074 7970 657b 7479 7065  ed for type{type
-00016b80: 286f 626a 297d 2229 0a20 2020 2072 6574  (obj)}").    ret
-00016b90: 7572 6e20 6622 706c 6163 6568 6f6c 6465  urn f"placeholde
-00016ba0: 7220 666f 7220 7b74 7970 6528 6f62 6a29  r for {type(obj)
-00016bb0: 7d22 0a0a 0a64 6566 2061 7267 7061 7273  }"...def argpars
-00016bc0: 6572 2829 3a0a 2020 2020 6672 6f6d 2061  er():.    from a
-00016bd0: 7267 7061 7273 6520 696d 706f 7274 2041  rgparse import A
-00016be0: 7267 756d 656e 7450 6172 7365 722c 2046  rgumentParser, F
-00016bf0: 696c 6554 7970 652c 2052 6177 4465 7363  ileType, RawDesc
-00016c00: 7269 7074 696f 6e48 656c 7046 6f72 6d61  riptionHelpForma
-00016c10: 7474 6572 0a0a 2020 2020 636f 6e66 6967  tter..    config
-00016c20: 6669 6c65 203d 2070 6174 686c 6962 2e50  file = pathlib.P
-00016c30: 6174 682e 686f 6d65 2829 202f 2022 2e70  ath.home() / ".p
-00016c40: 796f 6369 656e 7422 0a0a 2020 2020 7061  yocient"..    pa
-00016c50: 7273 6572 203d 2041 7267 756d 656e 7450  rser = ArgumentP
-00016c60: 6172 7365 7228 0a20 2020 2020 2020 2064  arser(.        d
-00016c70: 6573 6372 6970 7469 6f6e 3d66 2222 224f  escription=f"""O
-00016c80: 6369 656e 7420 5079 7468 6f6e 2063 6c69  cient Python cli
-00016c90: 656e 7420 7b76 6572 7369 6f6e 7d2e 0a49  ent {version}..I
-00016ca0: 6e20 7468 6520 7369 6d70 6c65 7374 2063  n the simplest c
-00016cb0: 6173 652c 2072 756e 2077 6974 6820 6120  ase, run with a 
-00016cc0: 4461 7461 2053 6f75 7263 6520 4e61 6d65  Data Source Name
-00016cd0: 2028 6473 6e29 2061 6e64 2061 0a71 7565   (dsn) and a.que
-00016ce0: 7279 2e20 2046 6f72 2065 7861 6d70 6c65  ry.  For example
-00016cf0: 3a0a 2020 7079 6f63 6965 6e74 206f 6369  :.  pyocient oci
-00016d00: 656e 743a 2f2f 7573 6572 3a70 6173 7377  ent://user:passw
-00016d10: 6f72 6440 6d79 686f 7374 3a34 3035 302f  ord@myhost:4050/
-00016d20: 6d79 6462 2022 7365 6c65 6374 202a 2066  mydb "select * f
-00016d30: 726f 6d20 6d79 7461 626c 6522 0a0a 4d75  rom mytable"..Mu
-00016d40: 6c74 6970 6c65 2071 7565 7279 2073 7472  ltiple query str
-00016d50: 696e 6773 206d 6179 2062 6520 7072 6f76  ings may be prov
-00016d60: 6964 6564 0a0a 4453 4e27 7320 6172 6520  ided..DSN's are 
-00016d70: 6f66 2074 6865 2066 6f72 6d3a 0a20 206f  of the form:.  o
-00016d80: 6369 656e 743a 2f2f 7573 6572 3a70 6173  cient://user:pas
-00016d90: 7377 6f72 6440 5b68 6f73 745d 5b3a 706f  sword@[host][:po
-00016da0: 7274 5d5b 2f64 6174 6162 6173 655d 5b3f  rt][/database][?
-00016db0: 7061 7261 6d31 3d76 616c 7565 3126 2e2e  param1=value1&..
-00016dc0: 2e5d 0a0a 5375 7070 6f72 7465 6420 7061  .]..Supported pa
-00016dd0: 7261 6d65 7465 7220 6172 653a 0a0a 2d20  rameter are:..- 
-00016de0: 746c 733a 2057 6869 6368 2063 616e 2068  tls: Which can h
-00016df0: 6176 6520 7468 6520 7661 6c75 6573 2022  ave the values "
-00016e00: 6f66 6622 2c20 2275 6e76 6572 6966 6965  off", "unverifie
-00016e10: 6422 2c20 6f72 2022 6f6e 220a 0a2d 2066  d", or "on"..- f
-00016e20: 6f72 6365 3a20 7472 7565 206f 7220 6661  orce: true or fa
-00016e30: 6c73 6520 746f 2066 6f72 6365 2074 6865  lse to force the
-00016e40: 2063 6f6e 6e65 6374 696f 6e20 746f 2073   connection to s
-00016e50: 7461 7920 6f6e 2074 6869 7320 7365 7276  tay on this serv
-00016e60: 6572 0a0a 2d20 6861 6e64 7368 616b 653a  er..- handshake:
-00016e70: 2057 6869 6368 2063 616e 2068 6176 6520   Which can have 
-00016e80: 7468 6520 7661 6c75 6520 2263 6263 220a  the value "cbc".
-00016e90: 0a4d 756c 7469 706c 6520 686f 7374 7320  .Multiple hosts 
-00016ea0: 6d61 7920 6265 2073 7065 6369 6669 6564  may be specified
-00016eb0: 2c20 7365 7061 7261 7465 6420 6279 2061  , separated by a
-00016ec0: 2063 6f6d 6d61 2c20 696e 2077 6869 6368   comma, in which
-00016ed0: 2063 6173 6520 7468 650a 686f 7374 7320   case the.hosts 
-00016ee0: 7769 6c6c 2062 6520 7472 6965 6420 696e  will be tried in
-00016ef0: 206f 7264 6572 2020 5468 7573 2061 6e20   order  Thus an 
-00016f00: 6578 616d 706c 6520 4453 4e20 6d69 6768  example DSN migh
-00016f10: 7420 6265 0a60 6f63 6965 6e74 3a2f 2f73  t be.`ocient://s
-00016f20: 6f6d 656f 6e65 3a73 6f6d 6570 6173 7377  omeone:somepassw
-00016f30: 6f72 6440 686f 7374 312c 686f 7374 323a  ord@host1,host2:
-00016f40: 3430 3531 2f6d 7964 6260 0a0a 5768 656e  4051/mydb`..When
-00016f50: 2072 756e 6e69 6e67 2069 6e20 7468 6520   running in the 
-00016f60: 636f 6d6d 616e 6420 6c69 6e65 2069 6e74  command line int
-00016f70: 6572 6661 6365 2c20 7468 6520 666f 6c6c  erface, the foll
-00016f80: 6f77 696e 6720 6578 7472 6120 636f 6d6d  owing extra comm
-00016f90: 616e 6473 0a61 7265 2073 7570 706f 7274  ands.are support
-00016fa0: 6564 3a0a 0a2d 2063 6f6e 6e65 6374 2074  ed:..- connect t
-00016fb0: 6f20 276f 6369 656e 743a 2f2f 2e2e 2e2e  o 'ocient://....
-00016fc0: 2720 7573 6572 2073 6f6d 6575 7365 7220  ' user someuser 
-00016fd0: 7573 696e 6720 736f 6d65 7061 7373 776f  using somepasswo
-00016fe0: 7264 3b0a 0a20 2020 2077 6865 6e20 7468  rd;..    when th
-00016ff0: 6520 4453 4e20 666f 6c6c 6f77 7320 7468  e DSN follows th
-00017000: 6520 6e6f 726d 616c 2070 796f 6369 656e  e normal pyocien
-00017010: 7420 4453 4e20 666f 726d 6174 2c20 6275  t DSN format, bu
-00017020: 7420 7468 6520 7573 6572 6964 2061 6e64  t the userid and
-00017030: 2070 6173 7377 6f72 6420 6d61 7920 6265   password may be
-00017040: 2070 6173 7365 640a 2020 2020 7573 696e   passed.    usin
-00017050: 6720 7468 6520 5553 4552 2061 6e64 2055  g the USER and U
-00017060: 5349 4e47 206b 6579 776f 7264 7320 2873  SING keywords (s
-00017070: 696d 696c 6172 2074 6f20 7468 6520 4f63  imilar to the Oc
-00017080: 6965 6e74 204a 4442 4320 6472 6976 6572  ient JDBC driver
-00017090: 292e 2020 5468 6520 4453 4e20 6d75 7374  ).  The DSN must
-000170a0: 2062 6520 7175 6f74 6564 2e0a 0a2d 2073   be quoted...- s
-000170b0: 6f75 7263 6520 2766 696c 6527 3b0a 0a20  ource 'file';.. 
-000170c0: 2020 2045 7865 6375 7465 2074 6865 2073     Execute the s
-000170d0: 7461 7465 6d65 6e74 7320 6672 6f6d 2074  tatements from t
-000170e0: 6865 2073 7065 6369 6669 6564 2066 696c  he specified fil
-000170f0: 652e 2020 5468 6520 6669 6c65 206e 616d  e.  The file nam
-00017100: 6520 6d75 7374 2062 6520 7175 6f74 6564  e must be quoted
-00017110: 2e0a 0a2d 2073 6574 2066 6f72 6d61 7420  ...- set format 
-00017120: 7461 626c 653b 0a0a 2020 2020 5365 7420  table;..    Set 
-00017130: 7468 6520 6f75 7470 7574 2066 6f72 6d61  the output forma
-00017140: 7420 0a0a 2d20 7175 6974 3b0a 0a22 2222  t ..- quit;.."""
-00017150: 2c0a 2020 2020 2020 2020 666f 726d 6174  ,.        format
-00017160: 7465 725f 636c 6173 733d 5261 7744 6573  ter_class=RawDes
-00017170: 6372 6970 7469 6f6e 4865 6c70 466f 726d  criptionHelpForm
-00017180: 6174 7465 722c 0a20 2020 2029 0a0a 2020  atter,.    )..  
-00017190: 2020 2320 466c 6167 7320 7468 6174 2061    # Flags that a
-000171a0: 7070 6c79 2074 6f20 626f 7468 2065 7865  pply to both exe
-000171b0: 6375 7469 6f6e 206d 6f64 6573 0a20 2020  cution modes.   
-000171c0: 206f 7574 6772 6f75 7020 3d20 7061 7273   outgroup = pars
-000171d0: 6572 2e61 6464 5f6d 7574 7561 6c6c 795f  er.add_mutually_
-000171e0: 6578 636c 7573 6976 655f 6772 6f75 7028  exclusive_group(
-000171f0: 290a 2020 2020 6f75 7467 726f 7570 2e61  ).    outgroup.a
-00017200: 6464 5f61 7267 756d 656e 7428 222d 6f22  dd_argument("-o"
-00017210: 2c20 222d 2d6f 7574 6669 6c65 222c 2074  , "--outfile", t
-00017220: 7970 653d 4669 6c65 5479 7065 2822 7722  ype=FileType("w"
-00017230: 292c 2064 6566 6175 6c74 3d22 2d22 2c20  ), default="-", 
-00017240: 6865 6c70 3d22 4f75 7470 7574 2066 696c  help="Output fil
-00017250: 6522 290a 2020 2020 6f75 7467 726f 7570  e").    outgroup
-00017260: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
-00017270: 6e22 2c20 222d 2d6e 6f6f 7574 222c 2061  n", "--noout", a
-00017280: 6374 696f 6e3d 2273 746f 7265 5f63 6f6e  ction="store_con
-00017290: 7374 222c 2063 6f6e 7374 3d4e 6f6e 652c  st", const=None,
-000172a0: 2064 6573 743d 226f 7574 6669 6c65 222c   dest="outfile",
-000172b0: 2068 656c 703d 2244 6f20 6e6f 7420 6f75   help="Do not ou
-000172c0: 7470 7574 2072 6573 756c 7473 2229 0a20  tput results"). 
-000172d0: 2020 2063 6f6e 6669 6767 726f 7570 203d     configgroup =
-000172e0: 2070 6172 7365 722e 6164 645f 6d75 7475   parser.add_mutu
-000172f0: 616c 6c79 5f65 7863 6c75 7369 7665 5f67  ally_exclusive_g
-00017300: 726f 7570 2829 0a20 2020 2063 6f6e 6669  roup().    confi
-00017310: 6767 726f 7570 2e61 6464 5f61 7267 756d  ggroup.add_argum
-00017320: 656e 7428 222d 6322 2c20 222d 2d63 6f6e  ent("-c", "--con
-00017330: 6669 6766 696c 6522 2c20 7479 7065 3d73  figfile", type=s
-00017340: 7472 2c20 6465 6661 756c 743d 7374 7228  tr, default=str(
-00017350: 636f 6e66 6967 6669 6c65 292c 2068 656c  configfile), hel
-00017360: 703d 2243 6f6e 6669 6775 7261 7469 6f6e  p="Configuration
-00017370: 2066 696c 6522 290a 2020 2020 636f 6e66   file").    conf
-00017380: 6967 6772 6f75 702e 6164 645f 6172 6775  iggroup.add_argu
-00017390: 6d65 6e74 2822 2d2d 6e6f 636f 6e66 6967  ment("--noconfig
-000173a0: 222c 2061 6374 696f 6e3d 2273 746f 7265  ", action="store
-000173b0: 5f63 6f6e 7374 222c 2063 6f6e 7374 3d4e  _const", const=N
-000173c0: 6f6e 652c 2064 6573 743d 2263 6f6e 6669  one, dest="confi
-000173d0: 6766 696c 6522 2c20 6865 6c70 3d22 4e6f  gfile", help="No
-000173e0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-000173f0: 696c 6522 290a 2020 2020 7061 7273 6572  ile").    parser
-00017400: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
-00017410: 6922 2c20 222d 2d69 6e66 696c 6522 2c20  i", "--infile", 
-00017420: 7479 7065 3d46 696c 6554 7970 6528 2272  type=FileType("r
-00017430: 2229 2c20 6465 6661 756c 743d 4e6f 6e65  "), default=None
-00017440: 2c20 6865 6c70 3d22 496e 7075 7420 6669  , help="Input fi
-00017450: 6c65 2063 6f6e 7461 696e 696e 6720 5351  le containing SQ
-00017460: 4c20 7374 6174 656d 656e 7473 2229 0a20  L statements"). 
-00017470: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
-00017480: 6775 6d65 6e74 2822 2d6c 222c 2022 2d2d  gument("-l", "--
-00017490: 6c6f 676c 6576 656c 222c 2074 7970 653d  loglevel", type=
-000174a0: 7374 722c 2064 6566 6175 6c74 3d22 6372  str, default="cr
-000174b0: 6974 6963 616c 222c 2063 686f 6963 6573  itical", choices
-000174c0: 3d5b 2263 7269 7469 6361 6c22 2c20 2265  =["critical", "e
-000174d0: 7272 6f72 222c 2022 7761 726e 696e 6722  rror", "warning"
-000174e0: 2c20 2269 6e66 6f22 2c20 2264 6562 7567  , "info", "debug
-000174f0: 225d 2c20 6865 6c70 3d22 4c6f 6767 696e  "], help="Loggin
-00017500: 6720 6c65 7665 6c2c 2064 6566 6175 6c74  g level, default
-00017510: 7320 746f 2063 7269 7469 6361 6c22 290a  s to critical").
-00017520: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
-00017530: 7267 756d 656e 7428 222d 2d6c 6f67 6669  rgument("--logfi
-00017540: 6c65 222c 2074 7970 653d 4669 6c65 5479  le", type=FileTy
-00017550: 7065 2822 6122 292c 2064 6566 6175 6c74  pe("a"), default
-00017560: 3d73 7973 2e73 7464 6f75 742c 2068 656c  =sys.stdout, hel
-00017570: 703d 224c 6f67 2066 696c 6522 290a 2020  p="Log file").  
-00017580: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-00017590: 756d 656e 7428 222d 7422 2c20 222d 2d74  ument("-t", "--t
-000175a0: 696d 6522 2c20 6163 7469 6f6e 3d22 7374  ime", action="st
-000175b0: 6f72 655f 7472 7565 222c 2068 656c 703d  ore_true", help=
-000175c0: 224f 7574 7075 7420 7175 6572 7920 7469  "Output query ti
-000175d0: 6d65 2229 0a20 2020 2070 6172 7365 722e  me").    parser.
-000175e0: 6164 645f 6172 6775 6d65 6e74 2822 6473  add_argument("ds
-000175f0: 6e22 2c20 6e61 7267 733d 223f 222c 2068  n", nargs="?", h
-00017600: 656c 703d 2244 534e 206f 6620 7468 6520  elp="DSN of the 
-00017610: 666f 726d 206f 6369 656e 743a 2f2f 7573  form ocient://us
-00017620: 6572 3a70 6173 7377 6f72 6440 5b68 6f73  er:password@[hos
-00017630: 745d 5b3a 706f 7274 5d5b 2f64 6174 6162  t][:port][/datab
-00017640: 6173 655d 5b3f 7061 7261 6d31 3d76 616c  ase][?param1=val
-00017650: 7565 3126 2e2e 2e5d 2229 0a20 2020 2070  ue1&...]").    p
-00017660: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-00017670: 6e74 2822 7371 6c22 2c20 6e61 7267 733d  nt("sql", nargs=
-00017680: 223f 222c 2068 656c 703d 2253 514c 2073  "?", help="SQL s
-00017690: 7461 7465 6d65 6e74 2229 0a20 2020 2070  tatement").    p
-000176a0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-000176b0: 6e74 2822 2d2d 666f 726d 6174 222c 2022  nt("--format", "
-000176c0: 2d66 222c 2074 7970 653d 7374 722c 2063  -f", type=str, c
-000176d0: 686f 6963 6573 3d5b 226a 736f 6e22 2c20  hoices=["json", 
-000176e0: 2274 6162 6c65 225d 2c20 6465 6661 756c  "table"], defaul
-000176f0: 743d 226a 736f 6e22 2c20 6865 6c70 3d22  t="json", help="
-00017700: 4f75 7470 7574 2066 6f72 6d61 742c 2064  Output format, d
-00017710: 6566 6175 6c74 7320 746f 206a 736f 6e22  efaults to json"
-00017720: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
-00017730: 5f61 7267 756d 656e 7428 222d 2d6e 6f63  _argument("--noc
-00017740: 6f6c 6f72 222c 2061 6374 696f 6e3d 2273  olor", action="s
-00017750: 746f 7265 5f74 7275 6522 2c20 6865 6c70  tore_true", help
-00017760: 3d22 5768 656e 2075 7369 6e67 2070 796f  ="When using pyo
-00017770: 6369 656e 7420 696e 7465 7261 6374 6976  cient interactiv
-00017780: 656c 792c 2064 6f20 6e6f 7420 636f 6c6f  ely, do not colo
-00017790: 7222 290a 0a20 2020 2072 6574 7572 6e20  r")..    return 
-000177a0: 7061 7273 6572 0a0a 0a64 6566 206d 6169  parser...def mai
-000177b0: 6e28 293a 0a20 2020 2069 6d70 6f72 7420  n():.    import 
-000177c0: 6a73 6f6e 0a20 2020 2066 726f 6d20 7461  json.    from ta
-000177d0: 6275 6c61 7465 2069 6d70 6f72 7420 7461  bulate import ta
-000177e0: 6275 6c61 7465 0a20 2020 2066 726f 6d20  bulate.    from 
-000177f0: 7079 676d 656e 7473 2e6c 6578 6572 732e  pygments.lexers.
-00017800: 7371 6c20 696d 706f 7274 2053 716c 4c65  sql import SqlLe
-00017810: 7865 720a 2020 2020 6672 6f6d 2070 7967  xer.    from pyg
-00017820: 6d65 6e74 732e 746f 6b65 6e20 696d 706f  ments.token impo
-00017830: 7274 2054 6f6b 656e 0a0a 2020 2020 6172  rt Token..    ar
-00017840: 6773 203d 2061 7267 7061 7273 6572 2829  gs = argparser()
-00017850: 2e70 6172 7365 5f61 7267 7328 7379 732e  .parse_args(sys.
-00017860: 6172 6776 5b31 3a5d 290a 0a20 2020 206c  argv[1:])..    l
-00017870: 6f67 5f6c 6576 656c 203d 2067 6574 6174  og_level = getat
-00017880: 7472 286c 6f67 6769 6e67 2c20 6172 6773  tr(logging, args
-00017890: 2e6c 6f67 6c65 7665 6c2e 7570 7065 7228  .loglevel.upper(
-000178a0: 292c 204e 6f6e 6529 0a20 2020 2069 6620  ), None).    if 
-000178b0: 6e6f 7420 6973 696e 7374 616e 6365 286c  not isinstance(l
-000178c0: 6f67 5f6c 6576 656c 2c20 696e 7429 3a0a  og_level, int):.
-000178d0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-000178e0: 6c75 6545 7272 6f72 2822 496e 7661 6c69  lueError("Invali
-000178f0: 6420 6c6f 6720 6c65 7665 6c3a 2025 7322  d log level: %s"
-00017900: 2025 2061 7267 732e 6c6f 676c 6576 656c   % args.loglevel
-00017910: 290a 0a20 2020 206c 6f67 6769 6e67 2e62  )..    logging.b
-00017920: 6173 6963 436f 6e66 6967 286c 6576 656c  asicConfig(level
-00017930: 3d6c 6f67 5f6c 6576 656c 2c20 7374 7265  =log_level, stre
-00017940: 616d 3d61 7267 732e 6c6f 6766 696c 652c  am=args.logfile,
-00017950: 2066 6f72 6d61 743d 225b 2528 6173 6374   format="[%(asct
-00017960: 696d 6529 735d 5b25 286c 6576 656c 6e61  ime)s][%(levelna
-00017970: 6d65 2973 5d20 2528 6d65 7373 6167 6529  me)s] %(message)
-00017980: 7322 290a 0a20 2020 2073 716c 5f73 746d  s")..    sql_stm
-00017990: 7420 3d20 2222 0a20 2020 206c 6578 6572  t = "".    lexer
-000179a0: 203d 2053 716c 4c65 7865 7228 290a 0a20   = SqlLexer().. 
-000179b0: 2020 2064 6566 205f 756e 7175 6f74 6528     def _unquote(
-000179c0: 696e 7075 7429 3a0a 2020 2020 2020 2020  input):.        
-000179d0: 2222 220a 2020 2020 2020 2020 556e 7175  """.        Unqu
-000179e0: 6f74 6520 6120 7374 7269 6e67 2c20 7769  ote a string, wi
-000179f0: 7468 2065 6974 6865 7220 7369 6e67 6c65  th either single
-00017a00: 206f 7220 646f 7562 6c65 2071 756f 7465   or double quote
-00017a10: 730a 2020 2020 2020 2020 2222 220a 2020  s.        """.  
-00017a20: 2020 2020 2020 6966 2069 6e70 7574 5b30        if input[0
-00017a30: 5d20 3d3d 2027 2227 2061 6e64 2069 6e70  ] == '"' and inp
-00017a40: 7574 5b2d 315d 203d 3d20 2722 273a 0a20  ut[-1] == '"':. 
-00017a50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00017a60: 6e20 696e 7075 745b 313a 2d31 5d0a 2020  n input[1:-1].  
-00017a70: 2020 2020 2020 6966 2069 6e70 7574 5b30        if input[0
-00017a80: 5d20 3d3d 2022 2722 2061 6e64 2069 6e70  ] == "'" and inp
-00017a90: 7574 5b2d 315d 203d 3d20 2227 223a 0a20  ut[-1] == "'":. 
-00017aa0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00017ab0: 6e20 696e 7075 745b 313a 2d31 5d0a 2020  n input[1:-1].  
-00017ac0: 2020 2020 2020 7265 7475 726e 2069 6e70        return inp
-00017ad0: 7574 0a0a 2020 2020 6465 6620 5f64 6f5f  ut..    def _do_
-00017ae0: 6c69 6e65 2861 7267 732c 2063 6f6e 6e65  line(args, conne
-00017af0: 6374 696f 6e2c 2074 6578 742c 2073 716c  ction, text, sql
-00017b00: 5f73 746d 742c 2071 7565 7279 5f66 6e29  _stmt, query_fn)
-00017b10: 3a0a 2020 2020 2020 2020 6e65 775f 636f  :.        new_co
-00017b20: 6e6e 6563 7469 6f6e 203d 2063 6f6e 6e65  nnection = conne
-00017b30: 6374 696f 6e0a 2020 2020 2020 2020 666f  ction.        fo
-00017b40: 7220 2874 6f6b 656e 5f74 7970 652c 2074  r (token_type, t
-00017b50: 6f6b 656e 5f76 616c 2920 696e 206c 6578  oken_val) in lex
-00017b60: 6572 2e67 6574 5f74 6f6b 656e 7328 7465  er.get_tokens(te
-00017b70: 7874 293a 0a20 2020 2020 2020 2020 2020  xt):.           
-00017b80: 2069 6620 746f 6b65 6e5f 7479 7065 203d   if token_type =
-00017b90: 3d20 546f 6b65 6e2e 5075 6e63 7475 6174  = Token.Punctuat
-00017ba0: 696f 6e20 616e 6420 746f 6b65 6e5f 7661  ion and token_va
-00017bb0: 6c20 3d3d 2022 3b22 3a0a 2020 2020 2020  l == ";":.      
-00017bc0: 2020 2020 2020 2020 2020 6e65 775f 636f            new_co
-00017bd0: 6e6e 6563 7469 6f6e 203d 2071 7565 7279  nnection = query
-00017be0: 5f66 6e28 6172 6773 2c20 6e65 775f 636f  _fn(args, new_co
-00017bf0: 6e6e 6563 7469 6f6e 2c20 7371 6c5f 7374  nnection, sql_st
-00017c00: 6d74 290a 2020 2020 2020 2020 2020 2020  mt).            
-00017c10: 2020 2020 7371 6c5f 7374 6d74 203d 2022      sql_stmt = "
-00017c20: 220a 2020 2020 2020 2020 2020 2020 656c  ".            el
-00017c30: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00017c40: 2020 2020 7371 6c5f 7374 6d74 202b 3d20      sql_stmt += 
-00017c50: 746f 6b65 6e5f 7661 6c0a 0a20 2020 2020  token_val..     
-00017c60: 2020 2072 6574 7572 6e20 2873 716c 5f73     return (sql_s
-00017c70: 746d 742c 206e 6577 5f63 6f6e 6e65 6374  tmt, new_connect
-00017c80: 696f 6e29 0a0a 2020 2020 6465 6620 5f64  ion)..    def _d
-00017c90: 6f5f 7175 6572 7928 6172 6773 2c20 636f  o_query(args, co
-00017ca0: 6e6e 6563 7469 6f6e 2c20 7175 6572 7929  nnection, query)
-00017cb0: 3a0a 2020 2020 2020 2020 2320 4669 7273  :.        # Firs
-00017cc0: 742c 2073 6565 2069 6620 7468 6973 2069  t, see if this i
-00017cd0: 7320 736f 6d65 7468 696e 6720 7765 2073  s something we s
-00017ce0: 686f 756c 6420 6861 6e64 6c65 2068 6572  hould handle her
-00017cf0: 6520 696e 2074 6865 2043 4c49 0a20 2020  e in the CLI.   
-00017d00: 2020 2020 2074 6f6b 656e 7320 3d20 5b74       tokens = [t
-00017d10: 6f6b 656e 2066 6f72 2028 746f 6b65 6e5f  oken for (token_
-00017d20: 7479 7065 2c20 746f 6b65 6e29 2069 6e20  type, token) in 
-00017d30: 6c65 7865 722e 6765 745f 746f 6b65 6e73  lexer.get_tokens
-00017d40: 2871 7565 7279 2920 6966 2074 6f6b 656e  (query) if token
-00017d50: 5f74 7970 6520 696e 2028 546f 6b65 6e2e  _type in (Token.
-00017d60: 4b65 7977 6f72 642c 2054 6f6b 656e 2e4e  Keyword, Token.N
-00017d70: 616d 652c 2054 6f6b 656e 2e4c 6974 6572  ame, Token.Liter
-00017d80: 616c 2e53 7472 696e 672e 5379 6d62 6f6c  al.String.Symbol
-00017d90: 2c20 546f 6b65 6e2e 4c69 7465 7261 6c2e  , Token.Literal.
-00017da0: 5374 7269 6e67 2e53 696e 676c 6529 5d0a  String.Single)].
-00017db0: 0a20 2020 2020 2020 2023 2063 6f6e 6e65  .        # conne
-00017dc0: 6374 2074 6f20 7374 6174 656d 656e 740a  ct to statement.
-00017dd0: 2020 2020 2020 2020 6966 206c 656e 2874          if len(t
-00017de0: 6f6b 656e 7329 203e 2031 2061 6e64 2074  okens) > 1 and t
-00017df0: 6f6b 656e 735b 305d 2e6c 6f77 6572 2829  okens[0].lower()
-00017e00: 203d 3d20 2263 6f6e 6e65 6374 2220 616e   == "connect" an
-00017e10: 6420 746f 6b65 6e73 5b31 5d2e 6c6f 7765  d tokens[1].lowe
-00017e20: 7228 2920 3d3d 2022 746f 223a 0a20 2020  r() == "to":.   
-00017e30: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00017e40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00017e50: 206c 656e 2874 6f6b 656e 7329 203d 3d20   len(tokens) == 
-00017e60: 373a 0a20 2020 2020 2020 2020 2020 2020  7:.             
-00017e70: 2020 2020 2020 2069 6620 746f 6b65 6e73         if tokens
-00017e80: 5b33 5d2e 6c6f 7765 7228 2920 213d 2022  [3].lower() != "
-00017e90: 7573 6572 2220 6f72 2074 6f6b 656e 735b  user" or tokens[
-00017ea0: 355d 2e6c 6f77 6572 2829 2021 3d20 2275  5].lower() != "u
-00017eb0: 7369 6e67 223a 0a20 2020 2020 2020 2020  sing":.         
-00017ec0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00017ed0: 7269 6e74 2866 2249 6e76 616c 6964 2055  rint(f"Invalid U
-00017ee0: 5345 5220 6f72 2055 5349 4e47 206b 6579  SER or USING key
-00017ef0: 776f 7264 7320 6f6e 2043 4f4e 4e45 4354  words on CONNECT
-00017f00: 2054 4f22 290a 2020 2020 2020 2020 2020   TO").          
-00017f10: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00017f20: 7475 726e 2063 6f6e 6e65 6374 696f 6e0a  turn connection.
-00017f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f40: 2020 2020 6473 6e20 3d20 5f75 6e71 756f      dsn = _unquo
-00017f50: 7465 2874 6f6b 656e 735b 325d 290a 2020  te(tokens[2]).  
-00017f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f70: 2020 7573 6572 203d 205f 756e 7175 6f74    user = _unquot
-00017f80: 6528 746f 6b65 6e73 5b34 5d29 0a20 2020  e(tokens[4]).   
-00017f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fa0: 2070 6173 7377 6f72 6420 3d20 5f75 6e71   password = _unq
-00017fb0: 756f 7465 2874 6f6b 656e 735b 365d 290a  uote(tokens[6]).
-00017fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fd0: 2020 2020 7265 7475 726e 2063 6f6e 6e65      return conne
-00017fe0: 6374 2864 736e 2c20 7573 6572 3d75 7365  ct(dsn, user=use
-00017ff0: 722c 2070 6173 7377 6f72 643d 7061 7373  r, password=pass
-00018000: 776f 7264 2c20 636f 6e66 6967 6669 6c65  word, configfile
-00018010: 3d61 7267 732e 636f 6e66 6967 6669 6c65  =args.configfile
-00018020: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00018030: 2020 656c 6966 206c 656e 2874 6f6b 656e    elif len(token
-00018040: 7329 203d 3d20 333a 0a20 2020 2020 2020  s) == 3:.       
-00018050: 2020 2020 2020 2020 2020 2020 2064 736e               dsn
-00018060: 203d 205f 756e 7175 6f74 6528 746f 6b65   = _unquote(toke
-00018070: 6e73 5b32 5d29 0a20 2020 2020 2020 2020  ns[2]).         
-00018080: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00018090: 6e20 636f 6e6e 6563 7428 6473 6e2c 2063  n connect(dsn, c
-000180a0: 6f6e 6669 6766 696c 653d 6172 6773 2e63  onfigfile=args.c
-000180b0: 6f6e 6669 6766 696c 6529 0a20 2020 2020  onfigfile).     
-000180c0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-000180d0: 2866 2249 6e76 616c 6964 2043 4f4e 4e45  (f"Invalid CONNE
-000180e0: 4354 2054 4f20 7374 6174 656d 656e 7420  CT TO statement 
-000180f0: 7b6c 656e 2874 6f6b 656e 7329 7d20 7b74  {len(tokens)} {t
-00018100: 6f6b 656e 737d 2229 0a20 2020 2020 2020  okens}").       
-00018110: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00018120: 636f 6e6e 6563 7469 6f6e 0a20 2020 2020  connection.     
-00018130: 2020 2020 2020 2065 7863 6570 7420 5351         except SQ
-00018140: 4c45 7863 6570 7469 6f6e 2061 7320 653a  LException as e:
-00018150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018160: 2070 7269 6e74 2865 290a 2020 2020 2020   print(e).      
-00018170: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00018180: 2063 6f6e 6e65 6374 696f 6e0a 0a20 2020   connection..   
-00018190: 2020 2020 2023 2073 6574 2066 6f72 6d61       # set forma
-000181a0: 740a 2020 2020 2020 2020 6966 206c 656e  t.        if len
-000181b0: 2874 6f6b 656e 7329 203e 2031 2061 6e64  (tokens) > 1 and
-000181c0: 2074 6f6b 656e 735b 305d 2e6c 6f77 6572   tokens[0].lower
-000181d0: 2829 203d 3d20 2273 6574 2220 616e 6420  () == "set" and 
-000181e0: 746f 6b65 6e73 5b31 5d2e 6c6f 7765 7228  tokens[1].lower(
-000181f0: 2920 3d3d 2022 666f 726d 6174 223a 0a20  ) == "format":. 
-00018200: 2020 2020 2020 2020 2020 206e 6577 5f66             new_f
-00018210: 6f72 6d61 7420 3d20 746f 6b65 6e73 5b32  ormat = tokens[2
-00018220: 5d2e 6c6f 7765 7228 290a 2020 2020 2020  ].lower().      
-00018230: 2020 2020 2020 6966 206e 6577 5f66 6f72        if new_for
-00018240: 6d61 7420 696e 205b 226a 736f 6e22 2c20  mat in ["json", 
-00018250: 2274 6162 6c65 225d 3a0a 2020 2020 2020  "table"]:.      
-00018260: 2020 2020 2020 2020 2020 6172 6773 2e66            args.f
-00018270: 6f72 6d61 7420 3d20 6e65 775f 666f 726d  ormat = new_form
-00018280: 6174 0a20 2020 2020 2020 2020 2020 2020  at.             
-00018290: 2020 2070 7269 6e74 2822 4f4b 2229 0a20     print("OK"). 
-000182a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000182b0: 6574 7572 6e20 636f 6e6e 6563 7469 6f6e  eturn connection
-000182c0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000182d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000182e0: 2020 2070 7269 6e74 2866 2249 6e76 616c     print(f"Inval
-000182f0: 6964 206f 7574 7075 7420 666f 726d 6174  id output format
-00018300: 207b 6e65 775f 666f 726d 6174 7d22 290a   {new_format}").
-00018310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018320: 7265 7475 726e 2063 6f6e 6e65 6374 696f  return connectio
-00018330: 6e0a 0a20 2020 2020 2020 2023 2073 6f75  n..        # sou
-00018340: 7263 650a 2020 2020 2020 2020 6966 206c  rce.        if l
-00018350: 656e 2874 6f6b 656e 7329 203e 2030 2061  en(tokens) > 0 a
-00018360: 6e64 2074 6f6b 656e 735b 305d 2e6c 6f77  nd tokens[0].low
-00018370: 6572 2829 203d 3d20 2273 6f75 7263 6522  er() == "source"
-00018380: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00018390: 206c 656e 2874 6f6b 656e 7329 2021 3d20   len(tokens) != 
-000183a0: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
-000183b0: 2020 2070 7269 6e74 2822 496e 7661 6c69     print("Invali
-000183c0: 6420 534f 5552 4345 2073 7461 7465 6d65  d SOURCE stateme
-000183d0: 6e74 2229 0a20 2020 2020 2020 2020 2020  nt").           
-000183e0: 2020 2020 2072 6574 7572 6e20 636f 6e6e       return conn
-000183f0: 6563 7469 6f6e 0a0a 2020 2020 2020 2020  ection..        
-00018400: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00018410: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-00018420: 656e 285f 756e 7175 6f74 6528 746f 6b65  en(_unquote(toke
-00018430: 6e73 5b31 5d29 2c20 6d6f 6465 3d22 7222  ns[1]), mode="r"
-00018440: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-00018450: 2020 2020 2020 2020 2020 2020 2873 716c              (sql
-00018460: 5f73 746d 742c 2063 6f6e 6e65 6374 696f  _stmt, connectio
-00018470: 6e29 203d 205f 646f 5f6c 696e 6528 6172  n) = _do_line(ar
-00018480: 6773 2c20 636f 6e6e 6563 7469 6f6e 2c20  gs, connection, 
-00018490: 662e 7265 6164 2829 2c20 2222 2c20 5f64  f.read(), "", _d
-000184a0: 6f5f 7175 6572 7929 0a20 2020 2020 2020  o_query).       
-000184b0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-000184c0: 7371 6c5f 7374 6d74 2e73 7472 6970 2829  sql_stmt.strip()
-000184d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000184e0: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
-000184f0: 6e20 3d20 5f64 6f5f 7175 6572 7928 6172  n = _do_query(ar
-00018500: 6773 2c20 636f 6e6e 6563 7469 6f6e 2c20  gs, connection, 
-00018510: 7371 6c5f 7374 6d74 290a 2020 2020 2020  sql_stmt).      
-00018520: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00018530: 2063 6f6e 6e65 6374 696f 6e0a 2020 2020   connection.    
-00018540: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00018550: 7863 6570 7469 6f6e 2061 7320 653a 0a20  xception as e:. 
-00018560: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00018570: 7269 6e74 2865 290a 2020 2020 2020 2020  rint(e).        
-00018580: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00018590: 6f6e 6e65 6374 696f 6e0a 0a20 2020 2020  onnection..     
-000185a0: 2020 2023 2071 7569 740a 2020 2020 2020     # quit.      
-000185b0: 2020 6966 206c 656e 2874 6f6b 656e 7329    if len(tokens)
-000185c0: 203e 2030 2061 6e64 2074 6f6b 656e 735b   > 0 and tokens[
-000185d0: 305d 2e6c 6f77 6572 2829 203d 3d20 2271  0].lower() == "q
-000185e0: 7569 7422 3a0a 2020 2020 2020 2020 2020  uit":.          
-000185f0: 2020 7379 732e 6578 6974 2830 290a 0a20    sys.exit(0).. 
-00018600: 2020 2020 2020 2069 6620 636f 6e6e 6563         if connec
-00018610: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-00018620: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00018630: 6622 4e6f 2061 6374 6976 6520 636f 6e6e  f"No active conn
-00018640: 6563 7469 6f6e 2229 0a20 2020 2020 2020  ection").       
-00018650: 2020 2020 2072 6574 7572 6e20 636f 6e6e       return conn
-00018660: 6563 7469 6f6e 0a0a 2020 2020 2020 2020  ection..        
-00018670: 2320 4f4b 2c20 6966 2077 6520 6661 6c6c  # OK, if we fall
-00018680: 2074 6872 6f75 6768 2074 6f20 6865 7265   through to here
-00018690: 2c20 6861 7665 2074 6865 206e 6f72 6d61  , have the norma
-000186a0: 6c20 6c69 6272 6172 7920 6861 6e64 6c65  l library handle
-000186b0: 2069 740a 2020 2020 2020 2020 6966 2061   it.        if a
-000186c0: 7267 732e 7469 6d65 3a0a 2020 2020 2020  rgs.time:.      
-000186d0: 2020 2020 2020 7374 6172 7474 696d 6520        starttime 
-000186e0: 3d20 7469 6d65 5f6e 7328 290a 0a20 2020  = time_ns()..   
-000186f0: 2020 2020 2063 7572 736f 7220 3d20 636f       cursor = co
-00018700: 6e6e 6563 7469 6f6e 2e63 7572 736f 7228  nnection.cursor(
-00018710: 290a 0a20 2020 2020 2020 2074 7279 3a0a  )..        try:.
-00018720: 2020 2020 2020 2020 2020 2020 6375 7273              curs
-00018730: 6f72 2e65 7865 6375 7465 2871 7565 7279  or.execute(query
-00018740: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00018750: 6620 6375 7273 6f72 2e64 6573 6372 6970  f cursor.descrip
-00018760: 7469 6f6e 2061 6e64 206e 6f74 2063 7572  tion and not cur
-00018770: 736f 722e 6578 706c 6169 6e5f 7265 7375  sor.explain_resu
-00018780: 6c74 3a0a 2020 2020 2020 2020 2020 2020  lt:.            
-00018790: 2020 2020 7265 7375 6c74 203d 2063 7572      result = cur
-000187a0: 736f 722e 6665 7463 6861 6c6c 2829 0a20  sor.fetchall(). 
-000187b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000187c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000187d0: 2072 6573 756c 7420 3d20 6375 7273 6f72   result = cursor
-000187e0: 2e63 6f6e 6e65 6374 696f 6e0a 2020 2020  .connection.    
-000187f0: 2020 2020 6578 6365 7074 2053 514c 4578      except SQLEx
-00018800: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
-00018810: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00018820: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
-00018830: 6574 7572 6e20 6375 7273 6f72 2e63 6f6e  eturn cursor.con
-00018840: 6e65 6374 696f 6e0a 2020 2020 2020 2020  nection.        
-00018850: 6578 6365 7074 204b 6579 626f 6172 6449  except KeyboardI
-00018860: 6e74 6572 7275 7074 3a0a 2020 2020 2020  nterrupt:.      
-00018870: 2020 2020 2020 7072 696e 7428 224f 7065        print("Ope
-00018880: 7261 7469 6f6e 2069 6e74 6572 7275 7074  ration interrupt
-00018890: 6564 2e22 290a 2020 2020 2020 2020 2020  ed.").          
-000188a0: 2020 6375 725f 636f 6e6e 203d 2063 7572    cur_conn = cur
-000188b0: 736f 722e 636f 6e6e 6563 7469 6f6e 0a20  sor.connection. 
-000188c0: 2020 2020 2020 2020 2020 2063 7572 5f63             cur_c
-000188d0: 6f6e 6e2e 636c 6f73 6528 290a 2020 2020  onn.close().    
-000188e0: 2020 2020 2020 2020 7265 7475 726e 2043          return C
-000188f0: 6f6e 6e65 6374 696f 6e28 0a20 2020 2020  onnection(.     
-00018900: 2020 2020 2020 2020 2020 2075 7365 723d             user=
-00018910: 6375 725f 636f 6e6e 2e75 7365 722c 0a20  cur_conn.user,. 
-00018920: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00018930: 6173 7377 6f72 643d 6375 725f 636f 6e6e  assword=cur_conn
-00018940: 2e70 6173 7377 6f72 642c 0a20 2020 2020  .password,.     
-00018950: 2020 2020 2020 2020 2020 2068 6f73 743d             host=
-00018960: 222c 222e 6a6f 696e 2863 7572 5f63 6f6e  ",".join(cur_con
-00018970: 6e2e 686f 7374 7329 2c0a 2020 2020 2020  n.hosts),.      
-00018980: 2020 2020 2020 2020 2020 6461 7461 6261            databa
-00018990: 7365 3d63 7572 5f63 6f6e 6e2e 6461 7461  se=cur_conn.data
-000189a0: 6261 7365 2c0a 2020 2020 2020 2020 2020  base,.          
-000189b0: 2020 2020 2020 746c 733d 6375 725f 636f        tls=cur_co
-000189c0: 6e6e 2e74 6c73 2c0a 2020 2020 2020 2020  nn.tls,.        
-000189d0: 2020 2020 2020 2020 6861 6e64 7368 616b          handshak
-000189e0: 653d 6375 725f 636f 6e6e 2e68 616e 6473  e=cur_conn.hands
-000189f0: 6861 6b65 2c0a 2020 2020 2020 2020 2020  hake,.          
-00018a00: 2020 2020 2020 666f 7263 653d 6375 725f        force=cur_
-00018a10: 636f 6e6e 2e66 6f72 6365 2c0a 2020 2020  conn.force,.    
-00018a20: 2020 2020 2020 2020 2020 2020 7365 7373              sess
-00018a30: 696f 6e3d 6375 725f 636f 6e6e 2e73 6573  ion=cur_conn.ses
-00018a40: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
-00018a50: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
-00018a60: 6172 6773 2e74 696d 653a 0a20 2020 2020  args.time:.     
-00018a70: 2020 2020 2020 2065 6e64 7469 6d65 203d         endtime =
-00018a80: 2074 696d 655f 6e73 2829 0a0a 2020 2020   time_ns()..    
-00018a90: 2020 2020 6966 2063 7572 736f 722e 6465      if cursor.de
-00018aa0: 7363 7269 7074 696f 6e20 6973 204e 6f6e  scription is Non
-00018ab0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-00018ac0: 7269 6e74 2822 4f4b 2229 0a0a 2020 2020  rint("OK")..    
-00018ad0: 2020 2020 656c 6966 2061 7267 732e 6f75      elif args.ou
-00018ae0: 7466 696c 6520 6973 206e 6f74 204e 6f6e  tfile is not Non
-00018af0: 653a 0a0a 2020 2020 2020 2020 2020 2020  e:..            
-00018b00: 6966 2063 7572 736f 722e 6578 706c 6169  if cursor.explai
-00018b10: 6e5f 7265 7375 6c74 3a0a 2020 2020 2020  n_result:.      
-00018b20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00018b30: 203d 205b 7b22 6578 706c 6169 6e22 3a20   = [{"explain": 
-00018b40: 6a73 6f6e 2e6c 6f61 6473 2863 7572 736f  json.loads(curso
-00018b50: 722e 6578 706c 6169 6e5f 7265 7375 6c74  r.explain_result
-00018b60: 297d 5d0a 0a20 2020 2020 2020 2020 2020  )}]..           
-00018b70: 2020 2020 2070 7269 6e74 286a 736f 6e2e       print(json.
-00018b80: 6475 6d70 7328 7265 7375 6c74 2c20 696e  dumps(result, in
-00018b90: 6465 6e74 3d34 2c20 6465 6661 756c 743d  dent=4, default=
-00018ba0: 5f63 7573 746f 6d5f 7479 7065 5f74 6f5f  _custom_type_to_
-00018bb0: 6a73 6f6e 292c 2066 696c 653d 6172 6773  json), file=args
-00018bc0: 2e6f 7574 6669 6c65 290a 2020 2020 2020  .outfile).      
-00018bd0: 2020 2020 2020 656c 6966 2072 6573 756c        elif resul
-00018be0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00018bf0: 2020 2069 6620 6172 6773 2e66 6f72 6d61     if args.forma
-00018c00: 7420 3d3d 2022 6a73 6f6e 223a 0a20 2020  t == "json":.   
-00018c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c20: 2072 6573 756c 7420 3d20 5b72 6f77 2e5f   result = [row._
-00018c30: 6173 6469 6374 2829 2066 6f72 2072 6f77  asdict() for row
-00018c40: 2069 6e20 7265 7375 6c74 5d0a 0a20 2020   in result]..   
-00018c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c60: 2070 7269 6e74 286a 736f 6e2e 6475 6d70   print(json.dump
-00018c70: 7328 7265 7375 6c74 2c20 696e 6465 6e74  s(result, indent
-00018c80: 3d34 2c20 6465 6661 756c 743d 5f63 7573  =4, default=_cus
-00018c90: 746f 6d5f 7479 7065 5f74 6f5f 6a73 6f6e  tom_type_to_json
-00018ca0: 292c 2066 696c 653d 6172 6773 2e6f 7574  ), file=args.out
-00018cb0: 6669 6c65 290a 2020 2020 2020 2020 2020  file).          
-00018cc0: 2020 2020 2020 656c 6966 2061 7267 732e        elif args.
-00018cd0: 666f 726d 6174 203d 3d20 2274 6162 6c65  format == "table
-00018ce0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00018cf0: 2020 2020 2020 2070 7269 6e74 2874 6162         print(tab
-00018d00: 756c 6174 6528 7265 7375 6c74 2c20 6865  ulate(result, he
-00018d10: 6164 6572 733d 5b63 5b30 5d20 666f 7220  aders=[c[0] for 
-00018d20: 6320 696e 2063 7572 736f 722e 6465 7363  c in cursor.desc
-00018d30: 7269 7074 696f 6e5d 2c20 7461 626c 6566  ription], tablef
-00018d40: 6d74 3d22 7073 716c 2229 2c20 6669 6c65  mt="psql"), file
-00018d50: 3d61 7267 732e 6f75 7466 696c 6529 0a0a  =args.outfile)..
-00018d60: 2020 2020 2020 2020 6966 2061 7267 732e          if args.
-00018d70: 7469 6d65 3a0a 2020 2020 2020 2020 2020  time:.          
-00018d80: 2020 656e 6474 696d 6520 3d20 7469 6d65    endtime = time
-00018d90: 5f6e 7328 290a 2020 2020 2020 2020 2020  _ns().          
-00018da0: 2020 7072 696e 7428 6622 4578 6563 7574    print(f"Execut
-00018db0: 696f 6e20 7469 6d65 3a20 7b28 656e 6474  ion time: {(endt
-00018dc0: 696d 6520 2d20 7374 6172 7474 696d 6529  ime - starttime)
-00018dd0: 2f31 3030 3030 3030 3030 303a 2e33 667d  /1000000000:.3f}
-00018de0: 2073 6563 6f6e 6473 2229 0a20 2020 2020   seconds").     
-00018df0: 2020 2023 2049 6620 7765 2064 6f6e 2774     # If we don't
-00018e00: 2072 6574 7572 6e20 7468 6973 2063 6f6e   return this con
-00018e10: 6e65 6374 696f 6e2c 2074 6865 6e20 7765  nection, then we
-00018e20: 2065 6e64 2075 7020 7573 696e 6720 7468   end up using th
-00018e30: 6520 6f6c 6420 636f 6e6e 6563 7469 6f6e  e old connection
-00018e40: 2077 6869 6368 2077 6520 636f 756c 6420   which we could 
-00018e50: 6861 7665 2062 6565 6e20 7265 6469 7265  have been redire
-00018e60: 6374 6564 0a20 2020 2020 2020 2072 6574  cted.        ret
-00018e70: 7572 6e20 6375 7273 6f72 2e63 6f6e 6e65  urn cursor.conne
-00018e80: 6374 696f 6e0a 0a20 2020 2064 6566 205f  ction..    def _
-00018e90: 646f 5f72 6570 6c28 6172 6773 2c20 636f  do_repl(args, co
-00018ea0: 6e6e 6563 7469 6f6e 293a 0a20 2020 2020  nnection):.     
-00018eb0: 2020 2066 726f 6d20 7072 6f6d 7074 5f74     from prompt_t
-00018ec0: 6f6f 6c6b 6974 2069 6d70 6f72 7420 5072  oolkit import Pr
-00018ed0: 6f6d 7074 5365 7373 696f 6e0a 2020 2020  omptSession.    
-00018ee0: 2020 2020 6672 6f6d 2070 726f 6d70 745f      from prompt_
-00018ef0: 746f 6f6c 6b69 742e 6c65 7865 7273 2069  toolkit.lexers i
-00018f00: 6d70 6f72 7420 5079 676d 656e 7473 4c65  mport PygmentsLe
-00018f10: 7865 720a 2020 2020 2020 2020 6672 6f6d  xer.        from
-00018f20: 2070 726f 6d70 745f 746f 6f6c 6b69 742e   prompt_toolkit.
-00018f30: 6869 7374 6f72 7920 696d 706f 7274 2046  history import F
-00018f40: 696c 6548 6973 746f 7279 0a20 2020 2020  ileHistory.     
-00018f50: 2020 2066 726f 6d20 7061 7468 6c69 6220     from pathlib 
-00018f60: 696d 706f 7274 2050 6174 680a 0a20 2020  import Path..   
-00018f70: 2020 2020 2073 716c 5f73 746d 7420 3d20       sql_stmt = 
-00018f80: 2222 0a0a 2020 2020 2020 2020 6966 2061  ""..        if a
-00018f90: 7267 732e 6e6f 636f 6c6f 723a 0a20 2020  rgs.nocolor:.   
-00018fa0: 2020 2020 2020 2020 2073 6573 7369 6f6e           session
-00018fb0: 203d 2050 726f 6d70 7453 6573 7369 6f6e   = PromptSession
-00018fc0: 2868 6973 746f 7279 3d46 696c 6548 6973  (history=FileHis
-00018fd0: 746f 7279 2873 7472 2850 6174 682e 686f  tory(str(Path.ho
-00018fe0: 6d65 2829 202f 2022 2e70 796f 6369 656e  me() / ".pyocien
-00018ff0: 745f 6869 7374 6f72 7922 2929 290a 2020  t_history"))).  
-00019000: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00019010: 2020 2020 2020 2020 7365 7373 696f 6e20          session 
-00019020: 3d20 5072 6f6d 7074 5365 7373 696f 6e28  = PromptSession(
-00019030: 6c65 7865 723d 5079 676d 656e 7473 4c65  lexer=PygmentsLe
-00019040: 7865 7228 5371 6c4c 6578 6572 292c 2068  xer(SqlLexer), h
-00019050: 6973 746f 7279 3d46 696c 6548 6973 746f  istory=FileHisto
-00019060: 7279 2873 7472 2850 6174 682e 686f 6d65  ry(str(Path.home
-00019070: 2829 202f 2022 2e70 796f 6369 656e 745f  () / ".pyocient_
-00019080: 6869 7374 6f72 7922 2929 290a 0a20 2020  history")))..   
-00019090: 2020 2020 2069 6620 636f 6e6e 6563 7469       if connecti
-000190a0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-000190b0: 6375 7273 6f72 203d 2063 6f6e 6e65 6374  cursor = connect
-000190c0: 696f 6e2e 6375 7273 6f72 2829 0a20 2020  ion.cursor().   
-000190d0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-000190e0: 224f 6369 656e 7420 4461 7461 6261 7365  "Ocient Database
-000190f0: e284 a222 290a 2020 2020 2020 2020 2020  ...").          
-00019100: 2020 7072 696e 7428 6622 5379 7374 656d    print(f"System
-00019110: 2056 6572 7369 6f6e 3a20 7b63 7572 736f   Version: {curso
-00019120: 722e 6765 7453 7973 7465 6d56 6572 7369  r.getSystemVersi
-00019130: 6f6e 2829 7d2c 2043 6c69 656e 7420 5665  on()}, Client Ve
-00019140: 7273 696f 6e20 7b76 6572 7369 6f6e 7d22  rsion {version}"
-00019150: 290a 2020 2020 2020 2020 656f 6620 3d20  ).        eof = 
-00019160: 4661 6c73 650a 2020 2020 2020 2020 7465  False.        te
-00019170: 7874 203d 2022 220a 2020 2020 2020 2020  xt = "".        
-00019180: 7768 696c 6520 6e6f 7420 656f 663a 0a20  while not eof:. 
-00019190: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-000191a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191b0: 7465 7874 203d 2073 6573 7369 6f6e 2e70  text = session.p
-000191c0: 726f 6d70 7428 223e 2022 290a 2020 2020  rompt("> ").    
-000191d0: 2020 2020 2020 2020 6578 6365 7074 204b          except K
-000191e0: 6579 626f 6172 6449 6e74 6572 7275 7074  eyboardInterrupt
-000191f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019200: 2020 7371 6c5f 7374 6d74 203d 2022 220a    sql_stmt = "".
-00019210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019220: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-00019230: 2020 2020 2065 7863 6570 7420 454f 4645       except EOFE
-00019240: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
-00019250: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-00019260: 2020 2020 2020 2020 2873 716c 5f73 746d          (sql_stm
-00019270: 742c 2063 6f6e 6e65 6374 696f 6e29 203d  t, connection) =
-00019280: 205f 646f 5f6c 696e 6528 6172 6773 2c20   _do_line(args, 
-00019290: 636f 6e6e 6563 7469 6f6e 2c20 7465 7874  connection, text
-000192a0: 2c20 7371 6c5f 7374 6d74 2c20 5f64 6f5f  , sql_stmt, _do_
-000192b0: 7175 6572 7929 0a0a 2020 2020 2020 2020  query)..        
-000192c0: 6966 206c 656e 2873 716c 5f73 746d 742e  if len(sql_stmt.
-000192d0: 7374 7269 7028 2929 3a0a 2020 2020 2020  strip()):.      
-000192e0: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
-000192f0: 203d 205f 646f 5f71 7565 7279 2861 7267   = _do_query(arg
-00019300: 732c 2063 6f6e 6e65 6374 696f 6e2c 2073  s, connection, s
-00019310: 716c 5f73 746d 7429 0a0a 2020 2020 2020  ql_stmt)..      
-00019320: 2020 7072 696e 7428 2247 6f6f 6442 7965    print("GoodBye
-00019330: 2122 290a 0a20 2020 2074 7279 3a0a 2020  !")..    try:.  
-00019340: 2020 2020 2020 6966 2061 7267 732e 6473        if args.ds
-00019350: 6e3a 0a20 2020 2020 2020 2020 2020 2063  n:.            c
-00019360: 6f6e 6e65 6374 696f 6e20 3d20 636f 6e6e  onnection = conn
-00019370: 6563 7428 6172 6773 2e64 736e 2c20 636f  ect(args.dsn, co
-00019380: 6e66 6967 6669 6c65 3d61 7267 732e 636f  nfigfile=args.co
-00019390: 6e66 6967 6669 6c65 290a 2020 2020 2020  nfigfile).      
-000193a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000193b0: 2020 2020 636f 6e6e 6563 7469 6f6e 203d      connection =
-000193c0: 204e 6f6e 650a 0a20 2020 2020 2020 2069   None..        i
-000193d0: 6620 6172 6773 2e73 716c 3a0a 2020 2020  f args.sql:.    
-000193e0: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
-000193f0: 6f6e 203d 205f 646f 5f71 7565 7279 2861  on = _do_query(a
-00019400: 7267 732c 2063 6f6e 6e65 6374 696f 6e2c  rgs, connection,
-00019410: 2061 7267 732e 7371 6c29 0a20 2020 2020   args.sql).     
-00019420: 2020 2065 6c69 6620 6172 6773 2e69 6e66     elif args.inf
-00019430: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
-00019440: 2028 7371 6c5f 7374 6d74 2c20 636f 6e6e   (sql_stmt, conn
-00019450: 6563 7469 6f6e 2920 3d20 5f64 6f5f 6c69  ection) = _do_li
-00019460: 6e65 2861 7267 732c 2063 6f6e 6e65 6374  ne(args, connect
-00019470: 696f 6e2c 2061 7267 732e 696e 6669 6c65  ion, args.infile
-00019480: 2e72 6561 6428 292c 2073 716c 5f73 746d  .read(), sql_stm
-00019490: 742c 205f 646f 5f71 7565 7279 290a 2020  t, _do_query).  
-000194a0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-000194b0: 2873 716c 5f73 746d 742e 7374 7269 7028  (sql_stmt.strip(
-000194c0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-000194d0: 2020 2020 636f 6e6e 6563 7469 6f6e 203d      connection =
-000194e0: 205f 646f 5f71 7565 7279 2861 7267 732c   _do_query(args,
-000194f0: 2063 6f6e 6e65 6374 696f 6e2c 2073 716c   connection, sql
-00019500: 5f73 746d 7429 0a20 2020 2020 2020 2065  _stmt).        e
-00019510: 6c69 6620 7379 732e 7374 6469 6e2e 6973  lif sys.stdin.is
-00019520: 6174 7479 2829 3a0a 2020 2020 2020 2020  atty():.        
-00019530: 2020 2020 5f64 6f5f 7265 706c 2861 7267      _do_repl(arg
-00019540: 732c 2063 6f6e 6e65 6374 696f 6e29 0a20  s, connection). 
-00019550: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00019560: 2020 2020 2020 2020 2028 7371 6c5f 7374           (sql_st
-00019570: 6d74 2c20 636f 6e6e 6563 7469 6f6e 2920  mt, connection) 
-00019580: 3d20 5f64 6f5f 6c69 6e65 2861 7267 732c  = _do_line(args,
-00019590: 2063 6f6e 6e65 6374 696f 6e2c 2073 7973   connection, sys
-000195a0: 2e73 7464 696e 2e72 6561 6428 292c 2073  .stdin.read(), s
-000195b0: 716c 5f73 746d 742c 205f 646f 5f71 7565  ql_stmt, _do_que
-000195c0: 7279 290a 0a20 2020 2065 7863 6570 7420  ry)..    except 
-000195d0: 5351 4c45 7863 6570 7469 6f6e 2061 7320  SQLException as 
-000195e0: 6578 633a 0a20 2020 2020 2020 2070 7269  exc:.        pri
-000195f0: 6e74 2866 2245 7272 6f72 3a20 7b65 7863  nt(f"Error: {exc
-00019600: 2e72 6561 736f 6e7d 222c 2066 696c 653d  .reason}", file=
-00019610: 7379 732e 7374 6465 7272 290a 0a0a 6966  sys.stderr)...if
-00019620: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
-00019630: 6d61 696e 5f5f 223a 0a20 2020 206d 6169  main__":.    mai
-00019640: 6e28 290a                                n().
+00010f60: 2066 6f72 6365 3d73 656c 662e 636f 6e6e   force=self.conn
+00010f70: 6563 7469 6f6e 2e66 6f72 6365 2c0a 2020  ection.force,.  
+00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f90: 2020 7365 7373 696f 6e3d 7365 6c66 2e63    session=self.c
+00010fa0: 6f6e 6e65 6374 696f 6e2e 7365 7373 696f  onnection.sessio
+00010fb0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+00010fc0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+00010fd0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00010fe0: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00010ff0: 0a0a 2020 2020 2020 2020 6966 2072 7370  ..        if rsp
+00011000: 2e72 6573 706f 6e73 652e 7479 7065 203d  .response.type =
+00011010: 3d20 7072 6f74 6f2e 436f 6e66 6972 6d61  = proto.Confirma
+00011020: 7469 6f6e 5265 7370 6f6e 7365 2e52 4553  tionResponse.RES
+00011030: 504f 4e53 455f 5741 524e 3a0a 2020 2020  PONSE_WARN:.    
+00011040: 2020 2020 2020 2020 7761 726e 2872 7370          warn(rsp
+00011050: 2e72 6573 706f 6e73 652e 7265 6173 6f6e  .response.reason
+00011060: 290a 2020 2020 2020 2020 656c 6966 206e  ).        elif n
+00011070: 6f74 2072 7370 2e72 6573 706f 6e73 652e  ot rsp.response.
+00011080: 7479 7065 203d 3d20 7072 6f74 6f2e 436f  type == proto.Co
+00011090: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
+000110a0: 7365 2e52 4553 504f 4e53 455f 4f4b 3a0a  se.RESPONSE_OK:.
+000110b0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+000110c0: 7370 2e72 6573 706f 6e73 652e 7665 6e64  sp.response.vend
+000110d0: 6f72 5f63 6f64 6520 3d3d 2053 4553 5349  or_code == SESSI
+000110e0: 4f4e 5f45 5850 4952 4544 5f43 4f44 453a  ON_EXPIRED_CODE:
+000110f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011100: 2023 204e 6565 6420 746f 2072 6566 7265   # Need to refre
+00011110: 7368 2074 6865 2073 6573 7369 6f6e 0a20  sh the session. 
+00011120: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011130: 656c 662e 636f 6e6e 6563 7469 6f6e 2e72  elf.connection.r
+00011140: 6566 7265 7368 2829 0a20 2020 2020 2020  efresh().       
+00011150: 2020 2020 2020 2020 2023 2061 6e64 2074           # and t
+00011160: 7279 2061 6761 696e 0a20 2020 2020 2020  ry again.       
+00011170: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
+00011180: 7865 6375 7465 5f6c 6973 7428 6f70 6572  xecute_list(oper
+00011190: 6174 696f 6e3d 6f70 6572 6174 696f 6e29  ation=operation)
+000111a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000111b0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+000111c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000111d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000111e0: 5f63 6f6e 7665 7274 5f65 7863 6570 7469  _convert_excepti
+000111f0: 6f6e 2872 7370 2e72 6573 706f 6e73 6529  on(rsp.response)
+00011200: 0a0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+00011210: 6573 6372 6970 7469 6f6e 203d 205b 5d0a  escription = [].
+00011220: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
+00011230: 6661 6374 6f72 792e 7072 6f63 6573 7328  factory.process(
+00011240: 7273 7029 0a20 2020 2020 2020 2069 6620  rsp).        if 
+00011250: 6e6f 7420 726f 7773 3a0a 2020 2020 2020  not rows:.      
+00011260: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00011270: 7265 7375 6c74 203d 205b 5d0a 2020 2020  result = [].    
+00011280: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
+00011290: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+000112a0: 2074 6865 2063 6f6c 756d 6e20 6465 7363   the column desc
+000112b0: 7269 7074 696f 6e73 0a20 2020 2020 2020  riptions.       
+000112c0: 2072 6f77 203d 2072 6f77 735b 305d 0a20   row = rows[0]. 
+000112d0: 2020 2020 2020 2066 6f72 2066 6965 6c64         for field
+000112e0: 2069 6e20 726f 772e 5f66 6965 6c64 733a   in row._fields:
+000112f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00011300: 662e 6465 7363 7269 7074 696f 6e2e 6170  f.description.ap
+00011310: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
+00011320: 2020 2020 2020 2866 6965 6c64 2c20 5479        (field, Ty
+00011330: 7065 436f 6465 732e 636c 735f 746f 5f74  peCodes.cls_to_t
+00011340: 7970 6528 726f 772e 5f66 6965 6c64 5f74  ype(row._field_t
+00011350: 7970 6573 5b66 6965 6c64 5d29 2c20 4e6f  ypes[field]), No
+00011360: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20  ne, None, None, 
+00011370: 4e6f 6e65 2c20 4e6f 6e65 2920 2023 2064  None, None)  # d
+00011380: 6973 706c 6179 5f73 697a 6520 2023 2069  isplay_size  # i
+00011390: 6e74 6572 6e61 6c5f 7369 7a65 2020 2320  nternal_size  # 
+000113a0: 7072 6563 6973 696f 6e20 2023 2073 6361  precision  # sca
+000113b0: 6c65 2020 2320 6e75 6c6c 5f6f 6b0a 2020  le  # null_ok.  
+000113c0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000113d0: 2020 2020 2023 2061 6e64 2073 6574 2074       # and set t
+000113e0: 6865 2072 6573 756c 7473 0a20 2020 2020  he results.     
+000113f0: 2020 2073 656c 662e 6c69 7374 5f72 6573     self.list_res
+00011400: 756c 7420 3d20 726f 7773 0a0a 2020 2020  ult = rows..    
+00011410: 6465 6620 5f67 6574 5f72 6573 756c 745f  def _get_result_
+00011420: 6d65 7461 6461 7461 2873 656c 6629 3a0a  metadata(self):.
+00011430: 2020 2020 2020 2020 2222 2249 6e74 6572          """Inter
+00011440: 6e61 6c20 726f 7574 696e 6520 746f 2067  nal routine to g
+00011450: 6574 206d 6574 6164 6174 6120 666f 7220  et metadata for 
+00011460: 6120 7265 7375 6c74 2073 6574 2222 220a  a result set""".
+00011470: 2020 2020 2020 2020 2320 7079 6c69 6e74          # pylint
+00011480: 3a20 6469 7361 626c 653d 6e6f 2d6d 656d  : disable=no-mem
+00011490: 6265 720a 2020 2020 2020 2020 7265 7120  ber.        req 
+000114a0: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
+000114b0: 290a 2020 2020 2020 2020 7265 712e 7479  ).        req.ty
+000114c0: 7065 203d 2072 6571 2e46 4554 4348 5f4d  pe = req.FETCH_M
+000114d0: 4554 4144 4154 410a 0a20 2020 2020 2020  ETADATA..       
+000114e0: 205f 7365 6e64 5f6d 7367 2873 656c 662e   _send_msg(self.
+000114f0: 636f 6e6e 6563 7469 6f6e 2c20 7265 7129  connection, req)
+00011500: 0a0a 2020 2020 2020 2020 7273 7020 3d20  ..        rsp = 
+00011510: 5f72 6563 765f 6d73 6728 7365 6c66 2e63  _recv_msg(self.c
+00011520: 6f6e 6e65 6374 696f 6e2c 2070 726f 746f  onnection, proto
+00011530: 2e46 6574 6368 4d65 7461 6461 7461 5265  .FetchMetadataRe
+00011540: 7370 6f6e 7365 2829 290a 2020 2020 2020  sponse()).      
+00011550: 2020 6966 2072 7370 2e72 6573 706f 6e73    if rsp.respons
+00011560: 652e 7479 7065 203d 3d20 7072 6f74 6f2e  e.type == proto.
+00011570: 436f 6e66 6972 6d61 7469 6f6e 5265 7370  ConfirmationResp
+00011580: 6f6e 7365 2e52 4553 504f 4e53 455f 5741  onse.RESPONSE_WA
+00011590: 524e 3a0a 2020 2020 2020 2020 2020 2020  RN:.            
+000115a0: 7761 726e 2872 7370 2e72 6573 706f 6e73  warn(rsp.respons
+000115b0: 652e 7265 6173 6f6e 290a 2020 2020 2020  e.reason).      
+000115c0: 2020 656c 6966 206e 6f74 2072 7370 2e72    elif not rsp.r
+000115d0: 6573 706f 6e73 652e 7479 7065 203d 3d20  esponse.type == 
+000115e0: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
+000115f0: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
+00011600: 4e53 455f 4f4b 3a0a 2020 2020 2020 2020  NSE_OK:.        
+00011610: 2020 2020 7261 6973 6520 5f63 6f6e 7665      raise _conve
+00011620: 7274 5f65 7863 6570 7469 6f6e 2872 7370  rt_exception(rsp
+00011630: 2e72 6573 706f 6e73 6529 0a0a 2020 2020  .response)..    
+00011640: 2020 2020 636f 6c73 203d 207b 7d0a 2020      cols = {}.  
+00011650: 2020 2020 2020 666f 7220 286b 6579 2c20        for (key, 
+00011660: 7661 6c75 6529 2069 6e20 7273 702e 636f  value) in rsp.co
+00011670: 6c73 3270 6f73 2e69 7465 6d73 2829 3a0a  ls2pos.items():.
+00011680: 2020 2020 2020 2020 2020 2020 636f 6c73              cols
+00011690: 5b76 616c 7565 5d20 3d20 6b65 790a 0a20  [value] = key.. 
+000116a0: 2020 2020 2020 2073 656c 662e 6465 7363         self.desc
+000116b0: 7269 7074 696f 6e20 3d20 5b5d 0a20 2020  ription = [].   
+000116c0: 2020 2020 2063 6f6c 6e61 6d65 7320 3d20       colnames = 
+000116d0: 5b5d 0a20 2020 2020 2020 2066 6f72 2069  [].        for i
+000116e0: 2069 6e20 7261 6e67 6528 6c65 6e28 636f   in range(len(co
+000116f0: 6c73 2929 3a20 2023 2070 796c 696e 743a  ls)):  # pylint:
+00011700: 2064 6973 6162 6c65 3d63 6f6e 7369 6465   disable=conside
+00011710: 722d 7573 696e 672d 656e 756d 6572 6174  r-using-enumerat
+00011720: 650a 2020 2020 2020 2020 2020 2020 6e61  e.            na
+00011730: 6d65 203d 2063 6f6c 735b 695d 0a20 2020  me = cols[i].   
+00011740: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
+00011750: 7475 706c 6520 6973 2064 6566 696e 6564  tuple is defined
+00011760: 2069 6e20 5045 5020 3234 390a 2020 2020   in PEP 249.    
+00011770: 2020 2020 2020 2020 7365 6c66 2e64 6573          self.des
+00011780: 6372 6970 7469 6f6e 2e61 7070 656e 6428  cription.append(
+00011790: 286e 616d 652c 2054 7970 6543 6f64 6573  (name, TypeCodes
+000117a0: 2e74 6f5f 7479 7065 2872 7370 2e63 6f6c  .to_type(rsp.col
+000117b0: 7332 5479 7065 735b 6e61 6d65 5d29 2c20  s2Types[name]), 
+000117c0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
+000117d0: 2c20 4e6f 6e65 2c20 4e6f 6e65 2929 2020  , None, None))  
+000117e0: 2320 6469 7370 6c61 795f 7369 7a65 2020  # display_size  
+000117f0: 2320 696e 7465 726e 616c 5f73 697a 6520  # internal_size 
+00011800: 2023 2070 7265 6369 7369 6f6e 2020 2320   # precision  # 
+00011810: 7363 616c 6520 2023 206e 756c 6c5f 6f6b  scale  # null_ok
+00011820: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+00011830: 6e61 6d65 732e 6170 7065 6e64 286e 616d  names.append(nam
+00011840: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+00011850: 7265 7375 6c74 7365 745f 7475 706c 6520  resultset_tuple 
+00011860: 3d20 6e61 6d65 6474 7570 6c65 2822 526f  = namedtuple("Ro
+00011870: 7722 2c20 636f 6c6e 616d 6573 2c20 7265  w", colnames, re
+00011880: 6e61 6d65 3d54 7275 6529 0a0a 2020 2020  name=True)..    
+00011890: 6465 6620 5f65 7865 6375 7465 5f75 7064  def _execute_upd
+000118a0: 6174 6528 7365 6c66 2c20 6f70 6572 6174  ate(self, operat
+000118b0: 696f 6e29 3a0a 2020 2020 2020 2020 2222  ion):.        ""
+000118c0: 2245 7865 6375 7465 2061 6e20 7570 6461  "Execute an upda
+000118d0: 7465 2073 7461 7465 6d65 6e74 2222 220a  te statement""".
+000118e0: 2020 2020 2020 2020 2320 7079 6c69 6e74          # pylint
+000118f0: 3a20 6469 7361 626c 653d 6e6f 2d6d 656d  : disable=no-mem
+00011900: 6265 720a 2020 2020 2020 2020 2320 5768  ber.        # Wh
+00011910: 696c 6520 7765 2061 7265 2072 6564 6972  ile we are redir
+00011920: 6563 7469 6e67 2e2e 2e0a 0a20 2020 2020  ecting.....     
+00011930: 2020 2023 2054 6865 7265 2069 7320 6e6f     # There is no
+00011940: 2072 6573 756c 7473 6574 2064 6174 6120   resultset data 
+00011950: 6672 6f6d 2061 6e20 7570 6461 7465 0a20  from an update. 
+00011960: 2020 2020 2020 2073 656c 662e 656e 645f         self.end_
+00011970: 6f66 5f64 6174 6120 3d20 5472 7565 0a0a  of_data = True..
+00011980: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
+00011990: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+000119a0: 7265 7120 3d20 7072 6f74 6f2e 5265 7175  req = proto.Requ
+000119b0: 6573 7428 290a 2020 2020 2020 2020 2020  est().          
+000119c0: 2020 7265 712e 7479 7065 203d 2072 6571    req.type = req
+000119d0: 2e45 5845 4355 5445 5f55 5044 4154 450a  .EXECUTE_UPDATE.
+000119e0: 2020 2020 2020 2020 2020 2020 7265 712e              req.
+000119f0: 6578 6563 7574 655f 7570 6461 7465 2e73  execute_update.s
+00011a00: 716c 203d 206f 7065 7261 7469 6f6e 0a20  ql = operation. 
+00011a10: 2020 2020 2020 2020 2020 2072 6571 2e65             req.e
+00011a20: 7865 6375 7465 5f75 7064 6174 652e 666f  xecute_update.fo
+00011a30: 7263 6520 3d20 7365 6c66 2e63 6f6e 6e65  rce = self.conne
+00011a40: 6374 696f 6e2e 666f 7263 650a 0a20 2020  ction.force..   
+00011a50: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00011a60: 2020 2020 2020 2020 2020 2020 2020 5f73                _s
+00011a70: 656e 645f 6d73 6728 7365 6c66 2e63 6f6e  end_msg(self.con
+00011a80: 6e65 6374 696f 6e2c 2072 6571 290a 0a20  nection, req).. 
+00011a90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00011aa0: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
+00011ab0: 656c 662e 636f 6e6e 6563 7469 6f6e 2c20  elf.connection, 
+00011ac0: 7072 6f74 6f2e 4578 6563 7574 6555 7064  proto.ExecuteUpd
+00011ad0: 6174 6552 6573 706f 6e73 6528 2929 0a20  ateResponse()). 
+00011ae0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00011af0: 7420 494f 4572 726f 723a 0a20 2020 2020  t IOError:.     
+00011b00: 2020 2020 2020 2020 2020 2023 2072 656d             # rem
+00011b10: 616b 6520 6f75 7220 636f 6e6e 6563 7469  ake our connecti
+00011b20: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+00011b30: 2020 2073 656c 662e 636f 6e6e 6563 7469     self.connecti
+00011b40: 6f6e 203d 2043 6f6e 6e65 6374 696f 6e28  on = Connection(
+00011b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011b60: 2020 2020 2075 7365 723d 7365 6c66 2e63       user=self.c
+00011b70: 6f6e 6e65 6374 696f 6e2e 7573 6572 2c0a  onnection.user,.
+00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b90: 2020 2020 7061 7373 776f 7264 3d73 656c      password=sel
+00011ba0: 662e 636f 6e6e 6563 7469 6f6e 2e70 6173  f.connection.pas
+00011bb0: 7377 6f72 642c 0a20 2020 2020 2020 2020  sword,.         
+00011bc0: 2020 2020 2020 2020 2020 2068 6f73 743d             host=
+00011bd0: 6622 7b27 2c27 2e6a 6f69 6e28 7365 6c66  f"{','.join(self
+00011be0: 2e63 6f6e 6e65 6374 696f 6e2e 686f 7374  .connection.host
+00011bf0: 7329 7d3a 7b73 656c 662e 636f 6e6e 6563  s)}:{self.connec
+00011c00: 7469 6f6e 2e70 6f72 747d 222c 0a20 2020  tion.port}",.   
+00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c20: 2064 6174 6162 6173 653d 7365 6c66 2e63   database=self.c
+00011c30: 6f6e 6e65 6374 696f 6e2e 6461 7461 6261  onnection.databa
+00011c40: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00011c50: 2020 2020 2020 2020 746c 733d 7365 6c66          tls=self
+00011c60: 2e63 6f6e 6e65 6374 696f 6e2e 746c 732c  .connection.tls,
+00011c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011c80: 2020 2020 2068 616e 6473 6861 6b65 3d73       handshake=s
+00011c90: 656c 662e 636f 6e6e 6563 7469 6f6e 2e68  elf.connection.h
+00011ca0: 616e 6473 6861 6b65 2c0a 2020 2020 2020  andshake,.      
+00011cb0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00011cc0: 7263 653d 7365 6c66 2e63 6f6e 6e65 6374  rce=self.connect
+00011cd0: 696f 6e2e 666f 7263 652c 0a20 2020 2020  ion.force,.     
+00011ce0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011cf0: 6573 7369 6f6e 3d73 656c 662e 636f 6e6e  ession=self.conn
+00011d00: 6563 7469 6f6e 2e73 6573 7369 6f6e 2c0a  ection.session,.
+00011d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d20: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00011d30: 2020 2063 6f6e 7469 6e75 650a 0a20 2020     continue..   
+00011d40: 2020 2020 2020 2020 2069 6620 7273 702e           if rsp.
+00011d50: 7265 7370 6f6e 7365 2e74 7970 6520 3d3d  response.type ==
+00011d60: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
+00011d70: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
+00011d80: 4f4e 5345 5f57 4152 4e3a 0a20 2020 2020  ONSE_WARN:.     
+00011d90: 2020 2020 2020 2020 2020 2077 6172 6e28             warn(
+00011da0: 7273 702e 7265 7370 6f6e 7365 2e72 6561  rsp.response.rea
+00011db0: 736f 6e29 0a20 2020 2020 2020 2020 2020  son).           
+00011dc0: 2065 6c69 6620 6e6f 7420 7273 702e 7265   elif not rsp.re
+00011dd0: 7370 6f6e 7365 2e74 7970 6520 3d3d 2070  sponse.type == p
+00011de0: 726f 746f 2e43 6f6e 6669 726d 6174 696f  roto.Confirmatio
+00011df0: 6e52 6573 706f 6e73 652e 5245 5350 4f4e  nResponse.RESPON
+00011e00: 5345 5f4f 4b3a 0a20 2020 2020 2020 2020  SE_OK:.         
+00011e10: 2020 2020 2020 2069 6620 7273 702e 7265         if rsp.re
+00011e20: 7370 6f6e 7365 2e76 656e 646f 725f 636f  sponse.vendor_co
+00011e30: 6465 203d 3d20 5345 5353 494f 4e5f 4558  de == SESSION_EX
+00011e40: 5049 5245 445f 434f 4445 3a0a 2020 2020  PIRED_CODE:.    
+00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e60: 2320 4e65 6564 2074 6f20 7265 6672 6573  # Need to refres
+00011e70: 6820 7468 6520 7365 7373 696f 6e0a 2020  h the session.  
+00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e90: 2020 7365 6c66 2e63 6f6e 6e65 6374 696f    self.connectio
+00011ea0: 6e2e 7265 6672 6573 6828 290a 2020 2020  n.refresh().    
+00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ec0: 2320 616e 6420 7472 7920 6167 6169 6e0a  # and try again.
+00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ee0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+00011ef0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00011f00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00011f10: 2020 2020 2020 2072 6169 7365 205f 636f         raise _co
+00011f20: 6e76 6572 745f 6578 6365 7074 696f 6e28  nvert_exception(
+00011f30: 7273 702e 7265 7370 6f6e 7365 290a 0a20  rsp.response).. 
+00011f40: 2020 2020 2020 2020 2020 2023 2073 6565             # see
+00011f50: 2069 6620 7765 2061 7265 2062 6569 6e67   if we are being
+00011f60: 2074 6f6c 6420 746f 2072 6564 6972 6563   told to redirec
+00011f70: 740a 2020 2020 2020 2020 2020 2020 6966  t.            if
+00011f80: 206e 6f74 2072 7370 2e72 6564 6972 6563   not rsp.redirec
+00011f90: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00011fa0: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
+00011fb0: 2020 2020 2020 2320 7265 6d61 6b65 206f        # remake o
+00011fc0: 7572 2063 6f6e 6e65 6374 696f 6e0a 2020  ur connection.  
+00011fd0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00011fe0: 6f6e 6e65 6374 696f 6e20 3d20 7365 6c66  onnection = self
+00011ff0: 2e63 6f6e 6e65 6374 696f 6e2e 7265 6469  .connection.redi
+00012000: 7265 6374 2872 7370 2e72 6564 6972 6563  rect(rsp.redirec
+00012010: 7448 6f73 742c 2072 7370 2e72 6564 6972  tHost, rsp.redir
+00012020: 6563 7450 6f72 7429 0a0a 2020 2020 6465  ectPort)..    de
+00012030: 6620 5f65 7865 6375 7465 5f66 6f72 6365  f _execute_force
+00012040: 2873 656c 662c 206f 7065 7261 7469 6f6e  (self, operation
+00012050: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00012060: 2020 2069 6620 6f70 6572 6174 696f 6e2e     if operation.
+00012070: 7374 7269 7028 292e 7570 7065 7228 2920  strip().upper() 
+00012080: 3d3d 2022 464f 5243 4520 5245 4449 5245  == "FORCE REDIRE
+00012090: 4354 223a 0a20 2020 2020 2020 2020 2020  CT":.           
+000120a0: 2023 2053 6574 7320 7468 6520 6e65 7874   # Sets the next
+000120b0: 2063 6f6d 6d61 6e64 2074 6861 7420 6973   command that is
+000120c0: 2065 7865 6375 7465 2071 7565 7279 2074   execute query t
+000120d0: 6f20 7265 6469 7265 6374 0a20 2020 2020  o redirect.     
+000120e0: 2020 2020 2020 2073 656c 662e 636f 6e6e         self.conn
+000120f0: 6563 7469 6f6e 2e66 6f72 6365 5f6e 6578  ection.force_nex
+00012100: 745f 7265 6469 7265 6374 203d 2054 7275  t_redirect = Tru
+00012110: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+00012120: 6c66 2e65 6e64 5f6f 665f 6461 7461 203d  lf.end_of_data =
+00012130: 2054 7275 650a 2020 2020 2020 2020 656c   True.        el
+00012140: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00012150: 2320 466f 7263 6520 6578 7465 726e 616c  # Force external
+00012160: 2063 6f6d 6d61 6e64 0a20 2020 2020 2020   command.       
+00012170: 2020 2020 2073 656c 662e 5f65 7865 6375       self._execu
+00012180: 7465 5f66 6f72 6365 5f65 7874 6572 6e61  te_force_externa
+00012190: 6c28 6f70 6572 6174 696f 6e29 0a0a 2020  l(operation)..  
+000121a0: 2020 6465 6620 5f65 7865 6375 7465 5f66    def _execute_f
+000121b0: 6f72 6365 5f65 7874 6572 6e61 6c28 7365  orce_external(se
+000121c0: 6c66 2c20 6f70 6572 6174 696f 6e29 202d  lf, operation) -
+000121d0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+000121e0: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+000121f0: 653d 6e6f 2d6d 656d 6265 720a 2020 2020  e=no-member.    
+00012200: 2020 2020 2320 5768 696c 6520 7765 2061      # While we a
+00012210: 7265 2072 6564 6972 6563 7469 6e67 2e2e  re redirecting..
+00012220: 2e0a 2020 2020 2020 2020 6661 6374 6f72  ..        factor
+00012230: 7920 3d20 5f4f 4349 454e 545f 5245 5155  y = _OCIENT_REQU
+00012240: 4553 545f 4641 4354 4f52 4945 535b 2246  EST_FACTORIES["F
+00012250: 4f52 4345 225d 0a20 2020 2020 2020 2072  ORCE"].        r
+00012260: 6571 203d 2066 6163 746f 7279 2e72 6571  eq = factory.req
+00012270: 7565 7374 286f 7065 7261 7469 6f6e 3d6f  uest(operation=o
+00012280: 7065 7261 7469 6f6e 290a 0a20 2020 2020  peration)..     
+00012290: 2020 205f 7365 6e64 5f6d 7367 2873 656c     _send_msg(sel
+000122a0: 662e 636f 6e6e 6563 7469 6f6e 2c20 7265  f.connection, re
+000122b0: 7129 0a0a 2020 2020 2020 2020 7273 7020  q)..        rsp 
+000122c0: 3d20 5f72 6563 765f 6d73 6728 7365 6c66  = _recv_msg(self
+000122d0: 2e63 6f6e 6e65 6374 696f 6e2c 2070 726f  .connection, pro
+000122e0: 746f 2e43 6f6e 6669 726d 6174 696f 6e52  to.ConfirmationR
+000122f0: 6573 706f 6e73 6528 2929 0a0a 2020 2020  esponse())..    
+00012300: 2020 2020 6966 2072 7370 2e74 7970 6520      if rsp.type 
+00012310: 3d3d 2070 726f 746f 2e43 6f6e 6669 726d  == proto.Confirm
+00012320: 6174 696f 6e52 6573 706f 6e73 652e 5245  ationResponse.RE
+00012330: 5350 4f4e 5345 5f57 4152 4e3a 0a20 2020  SPONSE_WARN:.   
+00012340: 2020 2020 2020 2020 2077 6172 6e28 7273           warn(rs
+00012350: 702e 7265 6173 6f6e 290a 2020 2020 2020  p.reason).      
+00012360: 2020 656c 6966 206e 6f74 2072 7370 2e74    elif not rsp.t
+00012370: 7970 6520 3d3d 2070 726f 746f 2e43 6f6e  ype == proto.Con
+00012380: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
+00012390: 652e 5245 5350 4f4e 5345 5f4f 4b3a 0a20  e.RESPONSE_OK:. 
+000123a0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000123b0: 205f 636f 6e76 6572 745f 6578 6365 7074   _convert_except
+000123c0: 696f 6e28 7273 7029 0a0a 2020 2020 6465  ion(rsp)..    de
+000123d0: 6620 5f65 7865 6375 7465 5f73 6574 2873  f _execute_set(s
+000123e0: 656c 662c 2070 6172 616d 7329 202d 3e20  elf, params) -> 
+000123f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
+00012400: 206c 656e 2870 6172 616d 7329 2021 3d20   len(params) != 
+00012410: 323a 0a20 2020 2020 2020 2020 2020 2072  2:.            r
+00012420: 6169 7365 2050 726f 6772 616d 6d69 6e67  aise Programming
+00012430: 4572 726f 7228 7265 6173 6f6e 3d22 5379  Error(reason="Sy
+00012440: 6e74 6178 2065 7272 6f72 2229 0a0a 2020  ntax error")..  
+00012450: 2020 2020 2020 2320 5468 6572 6520 6973        # There is
+00012460: 206e 6f20 7265 7375 6c74 7365 7420 6461   no resultset da
+00012470: 7461 2066 726f 6d20 616e 2075 7064 6174  ta from an updat
+00012480: 650a 2020 2020 2020 2020 7365 6c66 2e65  e.        self.e
+00012490: 6e64 5f6f 665f 6461 7461 203d 2054 7275  nd_of_data = Tru
+000124a0: 650a 0a20 2020 2020 2020 206f 7020 3d20  e..        op = 
+000124b0: 7061 7261 6d73 5b30 5d2e 7570 7065 7228  params[0].upper(
+000124c0: 290a 2020 2020 2020 2020 7661 6c20 3d20  ).        val = 
+000124d0: 7061 7261 6d73 5b31 5d2e 7374 7269 7028  params[1].strip(
+000124e0: 290a 0a20 2020 2020 2020 2069 6620 6f70  )..        if op
+000124f0: 203d 3d20 2253 4348 454d 4122 3a0a 2020   == "SCHEMA":.  
+00012500: 2020 2020 2020 2020 2020 6661 6374 6f72            factor
+00012510: 7920 3d20 5f4f 4349 454e 545f 5245 5155  y = _OCIENT_REQU
+00012520: 4553 545f 4641 4354 4f52 4945 535b 2253  EST_FACTORIES["S
+00012530: 4554 2053 4348 454d 4122 5d0a 2020 2020  ET SCHEMA"].    
+00012540: 2020 2020 2020 2020 7265 7120 3d20 6661          req = fa
+00012550: 6374 6f72 792e 7265 7175 6573 7428 7661  ctory.request(va
+00012560: 6c29 0a20 2020 2020 2020 2065 6c73 653a  l).        else:
+00012570: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00012580: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012590: 2020 7661 6c20 3d20 696e 7428 7661 6c29    val = int(val)
+000125a0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+000125b0: 6570 7420 5661 6c75 6545 7272 6f72 3a0a  ept ValueError:.
+000125c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125d0: 7261 6973 6520 5072 6f67 7261 6d6d 696e  raise Programmin
+000125e0: 6745 7272 6f72 2872 6561 736f 6e3d 2253  gError(reason="S
+000125f0: 796e 7461 7820 6572 726f 7220 696e 2053  yntax error in S
+00012600: 4554 2e20 5661 6c75 6520 6d75 7374 2062  ET. Value must b
+00012610: 6520 6e75 6d65 7269 6322 290a 0a20 2020  e numeric")..   
+00012620: 2020 2020 2020 2020 2066 6163 746f 7279           factory
+00012630: 203d 205f 4f43 4945 4e54 5f52 4551 5545   = _OCIENT_REQUE
+00012640: 5354 5f46 4143 544f 5249 4553 5b22 5345  ST_FACTORIES["SE
+00012650: 5422 5d0a 2020 2020 2020 2020 2020 2020  T"].            
+00012660: 7265 7120 3d20 6661 6374 6f72 792e 7265  req = factory.re
+00012670: 7175 6573 7428 6f70 2c20 7661 6c29 0a0a  quest(op, val)..
+00012680: 2020 2020 2020 2020 5f73 656e 645f 6d73          _send_ms
+00012690: 6728 7365 6c66 2e63 6f6e 6e65 6374 696f  g(self.connectio
+000126a0: 6e2c 2072 6571 290a 0a20 2020 2020 2020  n, req)..       
+000126b0: 2072 7370 203d 205f 7265 6376 5f6d 7367   rsp = _recv_msg
+000126c0: 2873 656c 662e 636f 6e6e 6563 7469 6f6e  (self.connection
+000126d0: 2c20 6661 6374 6f72 792e 7265 7370 6f6e  , factory.respon
+000126e0: 7365 2829 290a 0a20 2020 2020 2020 2069  se())..        i
+000126f0: 6620 7273 702e 7479 7065 203d 3d20 7072  f rsp.type == pr
+00012700: 6f74 6f2e 436f 6e66 6972 6d61 7469 6f6e  oto.Confirmation
+00012710: 5265 7370 6f6e 7365 2e52 4553 504f 4e53  Response.RESPONS
+00012720: 455f 5741 524e 3a0a 2020 2020 2020 2020  E_WARN:.        
+00012730: 2020 2020 7761 726e 2872 7370 2e72 6561      warn(rsp.rea
+00012740: 736f 6e29 0a20 2020 2020 2020 2065 6c69  son).        eli
+00012750: 6620 6e6f 7420 7273 702e 7479 7065 203d  f not rsp.type =
+00012760: 3d20 7072 6f74 6f2e 436f 6e66 6972 6d61  = proto.Confirma
+00012770: 7469 6f6e 5265 7370 6f6e 7365 2e52 4553  tionResponse.RES
+00012780: 504f 4e53 455f 4f4b 3a0a 2020 2020 2020  PONSE_OK:.      
+00012790: 2020 2020 2020 6966 2072 7370 2e72 6573        if rsp.res
+000127a0: 706f 6e73 652e 7665 6e64 6f72 5f63 6f64  ponse.vendor_cod
+000127b0: 6520 3d3d 2053 4553 5349 4f4e 5f45 5850  e == SESSION_EXP
+000127c0: 4952 4544 5f43 4f44 453a 0a20 2020 2020  IRED_CODE:.     
+000127d0: 2020 2020 2020 2020 2020 2023 204e 6565             # Nee
+000127e0: 6420 746f 2072 6566 7265 7368 2074 6865  d to refresh the
+000127f0: 2073 6573 7369 6f6e 0a20 2020 2020 2020   session.       
+00012800: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00012810: 6e6e 6563 7469 6f6e 2e72 6566 7265 7368  nnection.refresh
+00012820: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00012830: 2020 2023 2061 6e64 2074 7279 2061 6761     # and try aga
+00012840: 696e 0a20 2020 2020 2020 2020 2020 2020  in.             
+00012850: 2020 2073 656c 662e 5f65 7865 6375 7465     self._execute
+00012860: 5f73 6574 2870 6172 616d 7329 0a20 2020  _set(params).   
+00012870: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00012880: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
+00012890: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000128a0: 2020 2020 2020 7261 6973 6520 5f63 6f6e        raise _con
+000128b0: 7665 7274 5f65 7863 6570 7469 6f6e 2872  vert_exception(r
+000128c0: 7370 290a 0a20 2020 2064 6566 205f 6578  sp)..    def _ex
+000128d0: 6563 7574 655f 6765 745f 7363 6865 6d61  ecute_get_schema
+000128e0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+000128f0: 2020 2020 2020 2020 6661 6374 6f72 7920          factory 
+00012900: 3d20 5f4f 4349 454e 545f 5245 5155 4553  = _OCIENT_REQUES
+00012910: 545f 4641 4354 4f52 4945 535b 2247 4554  T_FACTORIES["GET
+00012920: 2053 4348 454d 4122 5d0a 2020 2020 2020   SCHEMA"].      
+00012930: 2020 7265 7120 3d20 6661 6374 6f72 792e    req = factory.
+00012940: 7265 7175 6573 7428 290a 0a20 2020 2020  request()..     
+00012950: 2020 205f 7365 6e64 5f6d 7367 2873 656c     _send_msg(sel
+00012960: 662e 636f 6e6e 6563 7469 6f6e 2c20 7265  f.connection, re
+00012970: 7129 0a0a 2020 2020 2020 2020 7273 7020  q)..        rsp 
+00012980: 3d20 5f72 6563 765f 6d73 6728 7365 6c66  = _recv_msg(self
+00012990: 2e63 6f6e 6e65 6374 696f 6e2c 2066 6163  .connection, fac
+000129a0: 746f 7279 2e72 6573 706f 6e73 6528 2929  tory.response())
+000129b0: 0a0a 2020 2020 2020 2020 6966 2072 7370  ..        if rsp
+000129c0: 2e72 6573 706f 6e73 652e 7479 7065 203d  .response.type =
+000129d0: 3d20 7072 6f74 6f2e 436f 6e66 6972 6d61  = proto.Confirma
+000129e0: 7469 6f6e 5265 7370 6f6e 7365 2e52 4553  tionResponse.RES
+000129f0: 504f 4e53 455f 5741 524e 3a0a 2020 2020  PONSE_WARN:.    
+00012a00: 2020 2020 2020 2020 7761 726e 2872 7370          warn(rsp
+00012a10: 2e72 6573 706f 6e73 652e 7265 6173 6f6e  .response.reason
+00012a20: 290a 2020 2020 2020 2020 656c 6966 206e  ).        elif n
+00012a30: 6f74 2072 7370 2e72 6573 706f 6e73 652e  ot rsp.response.
+00012a40: 7479 7065 203d 3d20 7072 6f74 6f2e 436f  type == proto.Co
+00012a50: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
+00012a60: 7365 2e52 4553 504f 4e53 455f 4f4b 3a0a  se.RESPONSE_OK:.
+00012a70: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00012a80: 7370 2e72 6573 706f 6e73 652e 7665 6e64  sp.response.vend
+00012a90: 6f72 5f63 6f64 6520 3d3d 2053 4553 5349  or_code == SESSI
+00012aa0: 4f4e 5f45 5850 4952 4544 5f43 4f44 453a  ON_EXPIRED_CODE:
+00012ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ac0: 2023 204e 6565 6420 746f 2072 6566 7265   # Need to refre
+00012ad0: 7368 2074 6865 2073 6573 7369 6f6e 0a20  sh the session. 
+00012ae0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012af0: 656c 662e 636f 6e6e 6563 7469 6f6e 2e72  elf.connection.r
+00012b00: 6566 7265 7368 2829 0a20 2020 2020 2020  efresh().       
+00012b10: 2020 2020 2020 2020 2023 2061 6e64 2074           # and t
+00012b20: 7279 2061 6761 696e 0a20 2020 2020 2020  ry again.       
+00012b30: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
+00012b40: 7865 6375 7465 5f67 6574 5f73 6368 656d  xecute_get_schem
+00012b50: 6128 290a 2020 2020 2020 2020 2020 2020  a().            
+00012b60: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00012b70: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00012b80: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00012b90: 7365 205f 636f 6e76 6572 745f 6578 6365  se _convert_exce
+00012ba0: 7074 696f 6e28 7273 702e 7265 7370 6f6e  ption(rsp.respon
+00012bb0: 7365 290a 0a20 2020 2020 2020 2073 656c  se)..        sel
+00012bc0: 662e 6465 7363 7269 7074 696f 6e20 3d20  f.description = 
+00012bd0: 5b28 2273 6368 656d 6122 2c20 5479 7065  [("schema", Type
+00012be0: 436f 6465 732e 4348 4152 2c20 4e6f 6e65  Codes.CHAR, None
+00012bf0: 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f  , None, None, No
+00012c00: 6e65 2c20 4e6f 6e65 295d 2020 2320 6469  ne, None)]  # di
+00012c10: 7370 6c61 795f 7369 7a65 2020 2320 696e  splay_size  # in
+00012c20: 7465 726e 616c 5f73 697a 6520 2023 2070  ternal_size  # p
+00012c30: 7265 6369 7369 6f6e 2020 2320 7363 616c  recision  # scal
+00012c40: 6520 2023 206e 756c 6c5f 6f6b 0a0a 2020  e  # null_ok..  
+00012c50: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00012c60: 7265 7375 6c74 203d 205b 0a20 2020 2020  result = [.     
+00012c70: 2020 2020 2020 206e 616d 6564 7475 706c         namedtupl
+00012c80: 6528 2252 6f77 222c 2028 2273 6368 656d  e("Row", ("schem
+00012c90: 6122 2929 280a 2020 2020 2020 2020 2020  a"))(.          
+00012ca0: 2020 2020 2020 7273 702e 7363 6865 6d61        rsp.schema
+00012cb0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00012cc0: 2020 2020 2020 2020 5d0a 0a20 2020 2023          ]..    #
+00012cd0: 2049 6620 7765 206e 6565 6420 746f 2069   If we need to i
+00012ce0: 6d70 6c65 6d65 6e74 206d 6f72 6520 6f66  mplement more of
+00012cf0: 2074 6865 7365 2073 6f72 7473 206f 6620   these sorts of 
+00012d00: 6375 7374 6f6d 2063 6f6d 6d61 6e64 732c  custom commands,
+00012d10: 2063 6f6e 7369 6465 720a 2020 2020 2320   consider.    # 
+00012d20: 6d61 6b69 6e67 2061 2066 6163 746f 7279  making a factory
+00012d30: 2066 6f72 2074 6865 2064 6573 6372 6970   for the descrip
+00012d40: 7469 6f6e 2061 6e64 2072 6573 756c 7473  tion and results
+00012d50: 2e0a 2020 2020 6465 6620 5f65 7865 6375  ..    def _execu
+00012d60: 7465 5f67 6574 5f73 6572 7665 725f 7365  te_get_server_se
+00012d70: 7373 696f 6e5f 6964 2873 656c 6629 202d  ssion_id(self) -
+00012d80: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00012d90: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
+00012da0: 203d 205b 2822 7365 7276 6572 5f73 6573   = [("server_ses
+00012db0: 7369 6f6e 5f69 6422 2c20 5479 7065 436f  sion_id", TypeCo
+00012dc0: 6465 732e 4348 4152 2c20 4e6f 6e65 2c20  des.CHAR, None, 
+00012dd0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
+00012de0: 2c20 4e6f 6e65 295d 2020 2320 6469 7370  , None)]  # disp
+00012df0: 6c61 795f 7369 7a65 2020 2320 696e 7465  lay_size  # inte
+00012e00: 726e 616c 5f73 697a 6520 2023 2070 7265  rnal_size  # pre
+00012e10: 6369 7369 6f6e 2020 2320 7363 616c 6520  cision  # scale 
+00012e20: 2023 206e 756c 6c5f 6f6b 0a20 2020 2020   # null_ok.     
+00012e30: 2020 2073 656c 662e 6c69 7374 5f72 6573     self.list_res
+00012e40: 756c 7420 3d20 5b0a 2020 2020 2020 2020  ult = [.        
+00012e50: 2020 2020 6e61 6d65 6474 7570 6c65 2822      namedtuple("
+00012e60: 526f 7722 2c20 2822 7365 7276 6572 5f73  Row", ("server_s
+00012e70: 6573 7369 6f6e 5f69 6422 2929 280a 2020  ession_id"))(.  
+00012e80: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012e90: 6c66 2e63 6f6e 6e65 6374 696f 6e2e 7365  lf.connection.se
+00012ea0: 7276 6572 5365 7373 696f 6e49 642c 0a20  rverSessionId,. 
+00012eb0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00012ec0: 2020 2020 205d 0a0a 2020 2020 6465 6620       ]..    def 
+00012ed0: 5f65 7865 6375 7465 5f67 6574 2873 656c  _execute_get(sel
+00012ee0: 662c 2070 6172 616d 7329 202d 3e20 4e6f  f, params) -> No
+00012ef0: 6e65 3a0a 2020 2020 2020 2020 6966 206c  ne:.        if l
+00012f00: 656e 2870 6172 616d 7329 203d 3d20 3120  en(params) == 1 
+00012f10: 616e 6420 7061 7261 6d73 5b30 5d2e 7570  and params[0].up
+00012f20: 7065 7228 2920 3d3d 2022 5343 4845 4d41  per() == "SCHEMA
+00012f30: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
+00012f40: 656c 662e 5f65 7865 6375 7465 5f67 6574  elf._execute_get
+00012f50: 5f73 6368 656d 6128 290a 2020 2020 2020  _schema().      
+00012f60: 2020 656c 6966 206c 656e 2870 6172 616d    elif len(param
+00012f70: 7329 203d 3d20 3320 616e 6420 7061 7261  s) == 3 and para
+00012f80: 6d73 5b30 5d2e 7570 7065 7228 2920 3d3d  ms[0].upper() ==
+00012f90: 2022 5345 5256 4552 2220 616e 6420 7061   "SERVER" and pa
+00012fa0: 7261 6d73 5b31 5d2e 7570 7065 7228 2920  rams[1].upper() 
+00012fb0: 3d3d 2022 5345 5353 494f 4e22 2061 6e64  == "SESSION" and
+00012fc0: 2070 6172 616d 735b 325d 2e75 7070 6572   params[2].upper
+00012fd0: 2829 203d 3d20 2249 4422 3a0a 2020 2020  () == "ID":.    
+00012fe0: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
+00012ff0: 6563 7574 655f 6765 745f 7365 7276 6572  ecute_get_server
+00013000: 5f73 6573 7369 6f6e 5f69 6428 290a 2020  _session_id().  
+00013010: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00013020: 2020 2020 2020 2020 7261 6973 6520 5072          raise Pr
+00013030: 6f67 7261 6d6d 696e 6745 7272 6f72 2872  ogrammingError(r
+00013040: 6561 736f 6e3d 2253 796e 7461 7820 6572  eason="Syntax er
+00013050: 726f 7222 290a 0a20 2020 2064 6566 205f  ror")..    def _
+00013060: 6578 6563 7574 655f 636c 6561 7228 7365  execute_clear(se
+00013070: 6c66 2c20 7061 7261 6d73 2920 2d3e 204e  lf, params) -> N
+00013080: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
+00013090: 6c65 6e28 7061 7261 6d73 2920 213d 2031  len(params) != 1
+000130a0: 206f 7220 7061 7261 6d73 5b30 5d2e 7570   or params[0].up
+000130b0: 7065 7228 2920 213d 2022 4341 4348 4522  per() != "CACHE"
+000130c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+000130d0: 6973 6520 5072 6f67 7261 6d6d 696e 6745  ise ProgrammingE
+000130e0: 7272 6f72 2872 6561 736f 6e3d 2253 796e  rror(reason="Syn
+000130f0: 7461 7820 6572 726f 7222 290a 0a20 2020  tax error")..   
+00013100: 2020 2020 2023 2054 6865 7265 2069 7320       # There is 
+00013110: 6e6f 2072 6573 756c 7473 6574 2064 6174  no resultset dat
+00013120: 6120 6672 6f6d 2061 6e20 7570 6461 7465  a from an update
+00013130: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
+00013140: 645f 6f66 5f64 6174 6120 3d20 5472 7565  d_of_data = True
+00013150: 0a0a 2020 2020 2020 2020 6661 6374 6f72  ..        factor
+00013160: 7920 3d20 5f4f 4349 454e 545f 5245 5155  y = _OCIENT_REQU
+00013170: 4553 545f 4641 4354 4f52 4945 535b 2243  EST_FACTORIES["C
+00013180: 4c45 4152 2043 4143 4845 225d 0a20 2020  LEAR CACHE"].   
+00013190: 2020 2020 2072 6571 203d 2066 6163 746f       req = facto
+000131a0: 7279 2e72 6571 7565 7374 2829 0a0a 2020  ry.request()..  
+000131b0: 2020 2020 2020 5f73 656e 645f 6d73 6728        _send_msg(
+000131c0: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2c  self.connection,
+000131d0: 2072 6571 290a 0a20 2020 2020 2020 2072   req)..        r
+000131e0: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
+000131f0: 656c 662e 636f 6e6e 6563 7469 6f6e 2c20  elf.connection, 
+00013200: 6661 6374 6f72 792e 7265 7370 6f6e 7365  factory.response
+00013210: 2829 290a 0a20 2020 2020 2020 2069 6620  ())..        if 
+00013220: 7273 702e 7479 7065 203d 3d20 7072 6f74  rsp.type == prot
+00013230: 6f2e 436f 6e66 6972 6d61 7469 6f6e 5265  o.ConfirmationRe
+00013240: 7370 6f6e 7365 2e52 4553 504f 4e53 455f  sponse.RESPONSE_
+00013250: 5741 524e 3a0a 2020 2020 2020 2020 2020  WARN:.          
+00013260: 2020 7761 726e 2872 7370 2e72 6561 736f    warn(rsp.reaso
+00013270: 6e29 0a20 2020 2020 2020 2065 6c69 6620  n).        elif 
+00013280: 6e6f 7420 7273 702e 7479 7065 203d 3d20  not rsp.type == 
+00013290: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
+000132a0: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
+000132b0: 4e53 455f 4f4b 3a0a 2020 2020 2020 2020  NSE_OK:.        
+000132c0: 2020 2020 6966 2072 7370 2e76 656e 646f      if rsp.vendo
+000132d0: 725f 636f 6465 203d 3d20 5345 5353 494f  r_code == SESSIO
+000132e0: 4e5f 4558 5049 5245 445f 434f 4445 3a0a  N_EXPIRED_CODE:.
+000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013300: 2320 4e65 6564 2074 6f20 7265 6672 6573  # Need to refres
+00013310: 6820 7468 6520 7365 7373 696f 6e0a 2020  h the session.  
+00013320: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00013330: 6c66 2e63 6f6e 6e65 6374 696f 6e2e 7265  lf.connection.re
+00013340: 6672 6573 6828 290a 2020 2020 2020 2020  fresh().        
+00013350: 2020 2020 2020 2020 2320 616e 6420 7472          # and tr
+00013360: 7920 6167 6169 6e0a 2020 2020 2020 2020  y again.        
+00013370: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
+00013380: 6563 7574 655f 636c 6561 7228 7061 7261  ecute_clear(para
+00013390: 6d73 290a 2020 2020 2020 2020 2020 2020  ms).            
+000133a0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+000133b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000133c0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+000133d0: 7365 205f 636f 6e76 6572 745f 6578 6365  se _convert_exce
+000133e0: 7074 696f 6e28 7273 7029 0a0a 2020 2020  ption(rsp)..    
+000133f0: 6465 6620 5f65 7865 6375 7465 5f63 616e  def _execute_can
+00013400: 6365 6c6b 696c 6c28 7365 6c66 2c20 6f70  celkill(self, op
+00013410: 2c20 6964 2920 2d3e 204e 6f6e 653a 0a20  , id) -> None:. 
+00013420: 2020 2020 2020 2069 6620 6c65 6e28 6964         if len(id
+00013430: 2920 213d 2031 3a0a 2020 2020 2020 2020  ) != 1:.        
+00013440: 2020 2020 7261 6973 6520 5072 6f67 7261      raise Progra
+00013450: 6d6d 696e 6745 7272 6f72 2872 6561 736f  mmingError(reaso
+00013460: 6e3d 2253 796e 7461 7820 6572 726f 7222  n="Syntax error"
+00013470: 290a 0a20 2020 2020 2020 2023 2054 6865  )..        # The
+00013480: 7265 2069 7320 6e6f 2072 6573 756c 7473  re is no results
+00013490: 6574 2064 6174 6120 6672 6f6d 2061 6e20  et data from an 
+000134a0: 7570 6461 7465 0a20 2020 2020 2020 2073  update.        s
+000134b0: 656c 662e 656e 645f 6f66 5f64 6174 6120  elf.end_of_data 
+000134c0: 3d20 5472 7565 0a0a 2020 2020 2020 2020  = True..        
+000134d0: 6661 6374 6f72 7920 3d20 5f4f 4349 454e  factory = _OCIEN
+000134e0: 545f 5245 5155 4553 545f 4641 4354 4f52  T_REQUEST_FACTOR
+000134f0: 4945 535b 6f70 5d0a 2020 2020 2020 2020  IES[op].        
+00013500: 7265 7120 3d20 6661 6374 6f72 792e 7265  req = factory.re
+00013510: 7175 6573 7428 6964 5b30 5d29 0a0a 2020  quest(id[0])..  
+00013520: 2020 2020 2020 5f73 656e 645f 6d73 6728        _send_msg(
+00013530: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2c  self.connection,
+00013540: 2072 6571 290a 0a20 2020 2020 2020 2072   req)..        r
+00013550: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
+00013560: 656c 662e 636f 6e6e 6563 7469 6f6e 2c20  elf.connection, 
+00013570: 6661 6374 6f72 792e 7265 7370 6f6e 7365  factory.response
+00013580: 2829 290a 0a20 2020 2020 2020 2069 6620  ())..        if 
+00013590: 7273 702e 7265 7370 6f6e 7365 2e74 7970  rsp.response.typ
+000135a0: 6520 3d3d 2070 726f 746f 2e43 6f6e 6669  e == proto.Confi
+000135b0: 726d 6174 696f 6e52 6573 706f 6e73 652e  rmationResponse.
+000135c0: 5245 5350 4f4e 5345 5f57 4152 4e3a 0a20  RESPONSE_WARN:. 
+000135d0: 2020 2020 2020 2020 2020 2077 6172 6e28             warn(
+000135e0: 7273 702e 7265 7370 6f6e 7365 2e72 6561  rsp.response.rea
+000135f0: 736f 6e29 0a20 2020 2020 2020 2065 6c69  son).        eli
+00013600: 6620 6e6f 7420 7273 702e 7265 7370 6f6e  f not rsp.respon
+00013610: 7365 2e74 7970 6520 3d3d 2070 726f 746f  se.type == proto
+00013620: 2e43 6f6e 6669 726d 6174 696f 6e52 6573  .ConfirmationRes
+00013630: 706f 6e73 652e 5245 5350 4f4e 5345 5f4f  ponse.RESPONSE_O
+00013640: 4b3a 0a20 2020 2020 2020 2020 2020 2069  K:.            i
+00013650: 6620 7273 702e 7265 7370 6f6e 7365 2e76  f rsp.response.v
+00013660: 656e 646f 725f 636f 6465 203d 3d20 5345  endor_code == SE
+00013670: 5353 494f 4e5f 4558 5049 5245 445f 434f  SSION_EXPIRED_CO
+00013680: 4445 3a0a 2020 2020 2020 2020 2020 2020  DE:.            
+00013690: 2020 2020 2320 4e65 6564 2074 6f20 7265      # Need to re
+000136a0: 6672 6573 6820 7468 6520 7365 7373 696f  fresh the sessio
+000136b0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+000136c0: 2020 7365 6c66 2e63 6f6e 6e65 6374 696f    self.connectio
+000136d0: 6e2e 7265 6672 6573 6828 290a 2020 2020  n.refresh().    
+000136e0: 2020 2020 2020 2020 2020 2020 2320 616e              # an
+000136f0: 6420 7472 7920 6167 6169 6e0a 2020 2020  d try again.    
+00013700: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013710: 2e5f 6578 6563 7574 655f 6361 6e63 656c  ._execute_cancel
+00013720: 6b69 6c6c 286f 702c 2069 6429 0a20 2020  kill(op, id).   
+00013730: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00013740: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
+00013750: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00013760: 2020 2020 2020 7261 6973 6520 5f63 6f6e        raise _con
+00013770: 7665 7274 5f65 7863 6570 7469 6f6e 2872  vert_exception(r
+00013780: 7370 2e72 6573 706f 6e73 6529 0a0a 2020  sp.response)..  
+00013790: 2020 2320 544f 444f 3a20 7265 706c 6163    # TODO: replac
+000137a0: 6520 7468 6520 6f74 6865 7220 6d65 7461  e the other meta
+000137b0: 6461 7461 2063 616c 6c0a 2020 2020 6465  data call.    de
+000137c0: 6620 5f65 7865 6375 7465 5f73 7973 7465  f _execute_syste
+000137d0: 6d6d 6574 6164 6174 6128 7365 6c66 2c20  mmetadata(self, 
+000137e0: 6f70 2c20 7363 6865 6d61 3d4e 6f6e 652c  op, schema=None,
+000137f0: 2074 6162 6c65 3d4e 6f6e 652c 2063 6f6c   table=None, col
+00013800: 756d 6e3d 4e6f 6e65 2c20 7669 6577 3d4e  umn=None, view=N
+00013810: 6f6e 6529 3a0a 2020 2020 2020 2020 6661  one):.        fa
+00013820: 6374 6f72 7920 3d20 5f4f 4349 454e 545f  ctory = _OCIENT_
+00013830: 5245 5155 4553 545f 4641 4354 4f52 4945  REQUEST_FACTORIE
+00013840: 535b 2247 4554 2053 5953 5445 4d20 4d45  S["GET SYSTEM ME
+00013850: 5441 4441 5441 225d 0a20 2020 2020 2020  TADATA"].       
+00013860: 2072 6571 203d 2066 6163 746f 7279 2e72   req = factory.r
+00013870: 6571 7565 7374 286f 702c 2073 6368 656d  equest(op, schem
+00013880: 612c 2074 6162 6c65 2c20 636f 6c75 6d6e  a, table, column
+00013890: 2c20 7669 6577 290a 0a20 2020 2020 2020  , view)..       
+000138a0: 205f 7365 6e64 5f6d 7367 2873 656c 662e   _send_msg(self.
+000138b0: 636f 6e6e 6563 7469 6f6e 2c20 7265 7129  connection, req)
+000138c0: 0a0a 2020 2020 2020 2020 7273 7020 3d20  ..        rsp = 
+000138d0: 5f72 6563 765f 6d73 6728 7365 6c66 2e63  _recv_msg(self.c
+000138e0: 6f6e 6e65 6374 696f 6e2c 2066 6163 746f  onnection, facto
+000138f0: 7279 2e72 6573 706f 6e73 6528 2929 0a0a  ry.response())..
+00013900: 2020 2020 2020 2020 6966 2072 7370 2e72          if rsp.r
+00013910: 6573 706f 6e73 652e 7479 7065 203d 3d20  esponse.type == 
+00013920: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
+00013930: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
+00013940: 4e53 455f 5741 524e 3a0a 2020 2020 2020  NSE_WARN:.      
+00013950: 2020 2020 2020 7761 726e 2872 7370 2e72        warn(rsp.r
+00013960: 6573 706f 6e73 652e 7265 6173 6f6e 290a  esponse.reason).
+00013970: 2020 2020 2020 2020 656c 6966 206e 6f74          elif not
+00013980: 2072 7370 2e72 6573 706f 6e73 652e 7479   rsp.response.ty
+00013990: 7065 203d 3d20 7072 6f74 6f2e 436f 6e66  pe == proto.Conf
+000139a0: 6972 6d61 7469 6f6e 5265 7370 6f6e 7365  irmationResponse
+000139b0: 2e52 4553 504f 4e53 455f 4f4b 3a0a 2020  .RESPONSE_OK:.  
+000139c0: 2020 2020 2020 2020 2020 6966 2072 7370            if rsp
+000139d0: 2e72 6573 706f 6e73 652e 7665 6e64 6f72  .response.vendor
+000139e0: 5f63 6f64 6520 3d3d 2053 4553 5349 4f4e  _code == SESSION
+000139f0: 5f45 5850 4952 4544 5f43 4f44 453a 0a20  _EXPIRED_CODE:. 
+00013a00: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00013a10: 204e 6565 6420 746f 2072 6566 7265 7368   Need to refresh
+00013a20: 2074 6865 2073 6573 7369 6f6e 0a20 2020   the session.   
+00013a30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013a40: 662e 636f 6e6e 6563 7469 6f6e 2e72 6566  f.connection.ref
+00013a50: 7265 7368 2829 0a20 2020 2020 2020 2020  resh().         
+00013a60: 2020 2020 2020 2023 2061 6e64 2074 7279         # and try
+00013a70: 2061 6761 696e 0a20 2020 2020 2020 2020   again.         
+00013a80: 2020 2020 2020 2073 656c 662e 5f65 7865         self._exe
+00013a90: 6375 7465 5f73 7973 7465 6d6d 6574 6164  cute_systemmetad
+00013aa0: 6174 6128 6f70 2c20 7363 6865 6d61 3d73  ata(op, schema=s
+00013ab0: 6368 656d 612c 2074 6162 6c65 3d74 6162  chema, table=tab
+00013ac0: 6c65 2c20 636f 6c75 6d6e 3d63 6f6c 756d  le, column=colum
+00013ad0: 6e2c 2076 6965 773d 7669 6577 290a 2020  n, view=view).  
+00013ae0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00013af0: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+00013b00: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00013b10: 2020 2020 2020 2072 6169 7365 205f 636f         raise _co
+00013b20: 6e76 6572 745f 6578 6365 7074 696f 6e28  nvert_exception(
+00013b30: 7273 702e 7265 7370 6f6e 7365 290a 0a20  rsp.response).. 
+00013b40: 2020 2020 2020 2069 6620 7273 702e 4861         if rsp.Ha
+00013b50: 7346 6965 6c64 2822 7265 7375 6c74 5f73  sField("result_s
+00013b60: 6574 5f76 616c 2229 3a0a 2020 2020 2020  et_val"):.      
+00013b70: 2020 2020 2020 7365 6c66 2e5f 6765 745f        self._get_
+00013b80: 7265 7375 6c74 5f6d 6574 6164 6174 6128  result_metadata(
+00013b90: 290a 0a20 2020 2020 2020 2020 2020 2066  )..            f
+00013ba0: 6f72 2062 6c6f 6220 696e 2072 7370 2e72  or blob in rsp.r
+00013bb0: 6573 756c 745f 7365 745f 7661 6c2e 626c  esult_set_val.bl
+00013bc0: 6f62 733a 0a20 2020 2020 2020 2020 2020  obs:.           
+00013bd0: 2020 2020 2073 656c 662e 5f62 7566 6665       self._buffe
+00013be0: 7273 2e61 7070 656e 6428 626c 6f62 290a  rs.append(blob).
+00013bf0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013c00: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
+00013c10: 2069 6620 7273 702e 4861 7346 6965 6c64   if rsp.HasField
+00013c20: 2822 7374 7269 6e67 5f76 616c 2229 3a0a  ("string_val"):.
+00013c30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013c40: 726e 2072 7370 2e73 7472 696e 675f 7661  rn rsp.string_va
+00013c50: 6c0a 0a20 2020 2020 2020 2072 6574 7572  l..        retur
+00013c60: 6e20 7273 702e 696e 745f 7661 6c0a 0a20  n rsp.int_val.. 
+00013c70: 2020 2064 6566 205f 6765 745f 6d6f 7265     def _get_more
+00013c80: 5f64 6174 6128 7365 6c66 293a 0a20 2020  _data(self):.   
+00013c90: 2020 2020 2022 2222 496e 7465 726e 616c       """Internal
+00013ca0: 2072 6f75 7469 6e65 2074 6f20 6765 7420   routine to get 
+00013cb0: 6d6f 7265 2064 6174 6120 6672 6f6d 2061  more data from a
+00013cc0: 2071 7565 7279 2222 220a 2020 2020 2020   query""".      
+00013cd0: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
+00013ce0: 626c 653d 6e6f 2d6d 656d 6265 720a 2020  ble=no-member.  
+00013cf0: 2020 2020 2020 7265 7120 3d20 7072 6f74        req = prot
+00013d00: 6f2e 5265 7175 6573 7428 290a 2020 2020  o.Request().    
+00013d10: 2020 2020 7265 712e 7479 7065 203d 2072      req.type = r
+00013d20: 6571 2e46 4554 4348 5f44 4154 410a 2020  eq.FETCH_DATA.  
+00013d30: 2020 2020 2020 7265 712e 6665 7463 685f        req.fetch_
+00013d40: 6461 7461 2e66 6574 6368 5f73 697a 6520  data.fetch_size 
+00013d50: 3d20 7365 6c66 2e61 7272 6179 7369 7a65  = self.arraysize
+00013d60: 0a20 2020 2020 2020 205f 7365 6e64 5f6d  .        _send_m
+00013d70: 7367 2873 656c 662e 636f 6e6e 6563 7469  sg(self.connecti
+00013d80: 6f6e 2c20 7265 7129 0a0a 2020 2020 2020  on, req)..      
+00013d90: 2020 7273 7020 3d20 5f72 6563 765f 6d73    rsp = _recv_ms
+00013da0: 6728 7365 6c66 2e63 6f6e 6e65 6374 696f  g(self.connectio
+00013db0: 6e2c 2070 726f 746f 2e46 6574 6368 4461  n, proto.FetchDa
+00013dc0: 7461 5265 7370 6f6e 7365 2829 290a 0a20  taResponse()).. 
+00013dd0: 2020 2020 2020 2069 6620 7273 702e 7265         if rsp.re
+00013de0: 7370 6f6e 7365 2e74 7970 6520 3d3d 2070  sponse.type == p
+00013df0: 726f 746f 2e43 6f6e 6669 726d 6174 696f  roto.Confirmatio
+00013e00: 6e52 6573 706f 6e73 652e 5245 5350 4f4e  nResponse.RESPON
+00013e10: 5345 5f45 5252 4f52 3a0a 2020 2020 2020  SE_ERROR:.      
+00013e20: 2020 2020 2020 7261 6973 6520 5f63 6f6e        raise _con
+00013e30: 7665 7274 5f65 7863 6570 7469 6f6e 2872  vert_exception(r
+00013e40: 7370 2e72 6573 706f 6e73 6529 0a0a 2020  sp.response)..  
+00013e50: 2020 2020 2020 666f 7220 626c 6f62 2069        for blob i
+00013e60: 6e20 7273 702e 7265 7375 6c74 5f73 6574  n rsp.result_set
+00013e70: 2e62 6c6f 6273 3a0a 2020 2020 2020 2020  .blobs:.        
+00013e80: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00013e90: 5f62 7566 6665 7273 3a0a 2020 2020 2020  _buffers:.      
+00013ea0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00013eb0: 6f66 6673 6574 203d 2030 0a20 2020 2020  offset = 0.     
+00013ec0: 2020 2020 2020 2073 656c 662e 5f62 7566         self._buf
+00013ed0: 6665 7273 2e61 7070 656e 6428 626c 6f62  fers.append(blob
+00013ee0: 290a 0a20 2020 2064 6566 2066 6574 6368  )..    def fetch
+00013ef0: 6d61 6e79 2873 656c 662c 2073 697a 653d  many(self, size=
+00013f00: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
+00013f10: 2222 4665 7463 6820 7468 6520 6e65 7874  ""Fetch the next
+00013f20: 2073 6574 206f 6620 726f 7773 206f 6620   set of rows of 
+00013f30: 6120 7175 6572 7920 7265 7375 6c74 2c20  a query result, 
+00013f40: 7265 7475 726e 696e 6720 6120 7365 7175  returning a sequ
+00013f50: 656e 6365 206f 660a 2020 2020 2020 2020  ence of.        
+00013f60: 7365 7175 656e 6365 7320 2865 2e67 2e20  sequences (e.g. 
+00013f70: 6120 6c69 7374 206f 6620 7475 706c 6573  a list of tuples
+00013f80: 292e 2041 6e20 656d 7074 7920 7365 7175  ). An empty sequ
+00013f90: 656e 6365 2069 7320 7265 7475 726e 6564  ence is returned
+00013fa0: 2077 6865 6e20 6e6f 0a20 2020 2020 2020   when no.       
+00013fb0: 206d 6f72 6520 726f 7773 2061 7265 2061   more rows are a
+00013fc0: 7661 696c 6162 6c65 2e0a 0a20 2020 2020  vailable...     
+00013fd0: 2020 2054 6865 206e 756d 6265 7220 6f66     The number of
+00013fe0: 2072 6f77 7320 746f 2066 6574 6368 2070   rows to fetch p
+00013ff0: 6572 2063 616c 6c20 6973 2073 7065 6369  er call is speci
+00014000: 6669 6564 2062 7920 7468 6520 7061 7261  fied by the para
+00014010: 6d65 7465 722e 2049 6620 6974 0a20 2020  meter. If it.   
+00014020: 2020 2020 2069 7320 6e6f 7420 6769 7665       is not give
+00014030: 6e2c 2074 6865 2063 7572 736f 7227 7320  n, the cursor's 
+00014040: 6172 7261 7973 697a 6520 6465 7465 726d  arraysize determ
+00014050: 696e 6573 2074 6865 206e 756d 6265 7220  ines the number 
+00014060: 6f66 2072 6f77 7320 746f 2062 650a 2020  of rows to be.  
+00014070: 2020 2020 2020 6665 7463 6865 642e 2054        fetched. T
+00014080: 6865 206d 6574 686f 6420 7769 6c6c 2074  he method will t
+00014090: 7279 2074 6f20 6665 7463 6820 6173 206d  ry to fetch as m
+000140a0: 616e 7920 726f 7773 2061 7320 696e 6469  any rows as indi
+000140b0: 6361 7465 6420 6279 2074 6865 2073 697a  cated by the siz
+000140c0: 650a 2020 2020 2020 2020 7061 7261 6d65  e.        parame
+000140d0: 7465 722e 2049 6620 7468 6973 2069 7320  ter. If this is 
+000140e0: 6e6f 7420 706f 7373 6962 6c65 2064 7565  not possible due
+000140f0: 2074 6f20 7468 6520 7370 6563 6966 6965   to the specifie
+00014100: 6420 6e75 6d62 6572 206f 6620 726f 7773  d number of rows
+00014110: 206e 6f74 0a20 2020 2020 2020 2062 6569   not.        bei
+00014120: 6e67 2061 7661 696c 6162 6c65 2c20 6665  ng available, fe
+00014130: 7765 7220 726f 7773 206d 6179 2062 6520  wer rows may be 
+00014140: 7265 7475 726e 6564 2e0a 2020 2020 2020  returned..      
+00014150: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00014160: 2073 697a 6520 6973 204e 6f6e 653a 0a20   size is None:. 
+00014170: 2020 2020 2020 2020 2020 2073 697a 6520             size 
+00014180: 3d20 7365 6c66 2e61 7272 6179 7369 7a65  = self.arraysize
+00014190: 0a0a 2020 2020 2020 2020 726f 7773 203d  ..        rows =
+000141a0: 205b 5d0a 2020 2020 2020 2020 7768 696c   [].        whil
+000141b0: 6520 7369 7a65 203e 2030 3a0a 2020 2020  e size > 0:.    
+000141c0: 2020 2020 2020 2020 615f 726f 7720 3d20          a_row = 
+000141d0: 7365 6c66 2e66 6574 6368 6f6e 6528 290a  self.fetchone().
+000141e0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+000141f0: 5f72 6f77 2069 7320 4e6f 6e65 3a0a 2020  _row is None:.  
+00014200: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00014210: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00014220: 726f 7773 2e61 7070 656e 6428 615f 726f  rows.append(a_ro
+00014230: 7729 0a20 2020 2020 2020 2020 2020 2073  w).            s
+00014240: 697a 6520 2d3d 2031 0a20 2020 2020 2020  ize -= 1.       
+00014250: 2072 6574 7572 6e20 726f 7773 0a0a 2020   return rows..  
+00014260: 2020 6465 6620 6665 7463 6861 6c6c 2873    def fetchall(s
+00014270: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00014280: 2246 6574 6368 2061 6c6c 2028 7265 6d61  "Fetch all (rema
+00014290: 696e 696e 6729 2072 6f77 7320 6f66 2061  ining) rows of a
+000142a0: 2071 7565 7279 2072 6573 756c 742c 2072   query result, r
+000142b0: 6574 7572 6e69 6e67 2074 6865 6d20 6173  eturning them as
+000142c0: 2061 0a20 2020 2020 2020 2073 6571 7565   a.        seque
+000142d0: 6e63 6520 6f66 2073 6571 7565 6e63 6573  nce of sequences
+000142e0: 2028 652e 672e 2061 206c 6973 7420 6f66   (e.g. a list of
+000142f0: 2074 7570 6c65 7329 2e20 4e6f 7465 2074   tuples). Note t
+00014300: 6861 7420 7468 6520 6375 7273 6f72 2773  hat the cursor's
+00014310: 0a20 2020 2020 2020 2061 7272 6179 7369  .        arraysi
+00014320: 7a65 2061 7474 7269 6275 7465 2063 616e  ze attribute can
+00014330: 2061 6666 6563 7420 7468 6520 7065 7266   affect the perf
+00014340: 6f72 6d61 6e63 6520 6f66 2074 6869 7320  ormance of this 
+00014350: 6f70 6572 6174 696f 6e2e 0a20 2020 2020  operation..     
+00014360: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00014370: 6574 7572 6e20 7365 6c66 2e66 6574 6368  eturn self.fetch
+00014380: 6d61 6e79 2873 697a 653d 7379 732e 6d61  many(size=sys.ma
+00014390: 7873 697a 6529 0a0a 2020 2020 6465 6620  xsize)..    def 
+000143a0: 5f5f 6e65 7874 5f5f 2873 656c 6629 3a0a  __next__(self):.
+000143b0: 2020 2020 2020 2020 615f 726f 7720 3d20          a_row = 
+000143c0: 7365 6c66 2e66 6574 6368 6f6e 6528 290a  self.fetchone().
+000143d0: 2020 2020 2020 2020 6966 2061 5f72 6f77          if a_row
+000143e0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+000143f0: 2020 2020 2020 7261 6973 6520 5374 6f70        raise Stop
+00014400: 4974 6572 6174 696f 6e0a 2020 2020 2020  Iteration.      
+00014410: 2020 7265 7475 726e 2061 5f72 6f77 0a0a    return a_row..
+00014420: 2020 2020 6465 6620 5f5f 6974 6572 5f5f      def __iter__
+00014430: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00014440: 7265 7475 726e 2073 656c 660a 0a20 2020  return self..   
+00014450: 2064 6566 2066 6574 6368 7661 6c28 7365   def fetchval(se
+00014460: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00014470: 5468 6520 6665 7463 6876 616c 2829 2063  The fetchval() c
+00014480: 6f6e 7665 6e69 656e 6365 206d 6574 686f  onvenience metho
+00014490: 6420 7265 7475 726e 7320 7468 6520 6669  d returns the fi
+000144a0: 7273 7420 636f 6c75 6d6e 206f 6620 7468  rst column of th
+000144b0: 650a 2020 2020 2020 2020 6669 7273 7420  e.        first 
+000144c0: 726f 7720 6966 2074 6865 7265 2061 7265  row if there are
+000144d0: 2072 6573 756c 7473 2c20 6f74 6865 7277   results, otherw
+000144e0: 6973 6520 6974 2072 6574 7572 6e73 204e  ise it returns N
+000144f0: 6f6e 652e 0a20 2020 2020 2020 2022 2222  one..        """
+00014500: 0a20 2020 2020 2020 2061 726f 7720 3d20  .        arow = 
+00014510: 7365 6c66 2e66 6574 6368 6f6e 6528 290a  self.fetchone().
+00014520: 2020 2020 2020 2020 6966 2061 726f 773a          if arow:
+00014530: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00014540: 7572 6e20 6172 6f77 5b30 5d0a 2020 2020  urn arow[0].    
+00014550: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00014560: 0a20 2020 2064 6566 2066 6574 6368 6f6e  .    def fetchon
+00014570: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00014580: 2022 2222 4665 7463 6820 7468 6520 6e65   """Fetch the ne
+00014590: 7874 2072 6f77 206f 6620 6120 7175 6572  xt row of a quer
+000145a0: 7920 7265 7375 6c74 2073 6574 2c20 7265  y result set, re
+000145b0: 7475 726e 696e 6720 6120 7369 6e67 6c65  turning a single
+000145c0: 2073 6571 7565 6e63 652c 0a20 2020 2020   sequence,.     
+000145d0: 2020 206f 7220 4e6f 6e65 2077 6865 6e20     or None when 
+000145e0: 6e6f 206d 6f72 6520 6461 7461 2069 7320  no more data is 
+000145f0: 6176 6169 6c61 626c 652e 0a20 2020 2020  available..     
+00014600: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
+00014610: 2049 6620 7468 6572 6520 7761 7320 6e65   If there was ne
+00014620: 7665 7220 6120 7175 6572 7920 6578 6563  ver a query exec
+00014630: 7574 6564 2c20 7468 726f 7720 616e 2065  uted, throw an e
+00014640: 7272 6f72 0a20 2020 2020 2020 2069 6620  rror.        if 
+00014650: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
+00014660: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00014670: 2020 2020 2020 7261 6973 6520 5072 6f67        raise Prog
+00014680: 7261 6d6d 696e 6745 7272 6f72 2822 4e6f  rammingError("No
+00014690: 2072 6573 756c 7420 7365 7420 6176 6169   result set avai
+000146a0: 6c61 626c 6522 290a 0a20 2020 2020 2020  lable")..       
+000146b0: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+000146c0: 6c65 203d 2074 6f6f 2d6d 616e 792d 6272  le = too-many-br
+000146d0: 616e 6368 6573 0a20 2020 2020 2020 2069  anches.        i
+000146e0: 6620 7365 6c66 2e65 6e64 5f6f 665f 6461  f self.end_of_da
+000146f0: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
+00014700: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+00014710: 2020 2020 2023 2073 7065 6369 616c 2063       # special c
+00014720: 6173 6520 6578 706c 6169 6e2e 0a20 2020  ase explain..   
+00014730: 2020 2020 2069 6620 7365 6c66 2e65 7870       if self.exp
+00014740: 6c61 696e 5f72 6573 756c 7420 6973 206e  lain_result is n
+00014750: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00014760: 2020 2020 2072 6574 203d 2073 656c 662e       ret = self.
+00014770: 6578 706c 6169 6e5f 7265 7375 6c74 0a20  explain_result. 
+00014780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014790: 656e 645f 6f66 5f64 6174 6120 3d20 5472  end_of_data = Tr
+000147a0: 7565 0a20 2020 2020 2020 2020 2020 2072  ue.            r
+000147b0: 6574 7572 6e20 5b72 6574 5d0a 0a20 2020  eturn [ret]..   
+000147c0: 2020 2020 2069 6620 7365 6c66 2e6c 6973       if self.lis
+000147d0: 745f 7265 7375 6c74 2069 7320 6e6f 7420  t_result is not 
+000147e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000147f0: 2020 6966 2073 656c 662e 5f6f 6666 7365    if self._offse
+00014800: 7420 3e3d 206c 656e 2873 656c 662e 6c69  t >= len(self.li
+00014810: 7374 5f72 6573 756c 7429 3a0a 2020 2020  st_result):.    
+00014820: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014830: 2e65 6e64 5f6f 665f 6461 7461 203d 2054  .end_of_data = T
+00014840: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+00014850: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00014860: 2020 2020 2020 2020 2020 2020 615f 726f              a_ro
+00014870: 7720 3d20 7365 6c66 2e6c 6973 745f 7265  w = self.list_re
+00014880: 7375 6c74 5b73 656c 662e 5f6f 6666 7365  sult[self._offse
+00014890: 745d 0a20 2020 2020 2020 2020 2020 2073  t].            s
+000148a0: 656c 662e 5f6f 6666 7365 7420 2b3d 2031  elf._offset += 1
+000148b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000148c0: 7572 6e20 615f 726f 770a 0a20 2020 2020  urn a_row..     
+000148d0: 2020 2069 6620 7365 6c66 2e72 6f77 636f     if self.rowco
+000148e0: 756e 7420 3c20 303a 0a20 2020 2020 2020  unt < 0:.       
+000148f0: 2020 2020 2073 656c 662e 726f 7763 6f75       self.rowcou
+00014900: 6e74 203d 2030 0a0a 2020 2020 2020 2020  nt = 0..        
+00014910: 7768 696c 6520 6e6f 7420 7365 6c66 2e5f  while not self._
+00014920: 6275 6666 6572 733a 0a20 2020 2020 2020  buffers:.       
+00014930: 2020 2020 2073 656c 662e 5f67 6574 5f6d       self._get_m
+00014940: 6f72 655f 6461 7461 2829 0a20 2020 2020  ore_data().     
+00014950: 2020 2020 2020 2077 6869 6c65 2073 656c         while sel
+00014960: 662e 5f62 7566 6665 7273 2061 6e64 2073  f._buffers and s
+00014970: 656c 662e 5f62 7566 2829 203d 3d20 6222  elf._buf() == b"
+00014980: 5c30 5c30 5c30 5c30 223a 0a20 2020 2020  \0\0\0\0":.     
+00014990: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000149a0: 5f62 7566 6665 7273 2e70 6f70 2830 290a  _buffers.pop(0).
+000149b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000149c0: 6e6f 7420 7365 6c66 2e5f 6275 6666 6572  not self._buffer
+000149d0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000149e0: 2020 2023 206e 6f20 6461 7461 2079 6574     # no data yet
+000149f0: 2e2e 2e77 6169 7420 736f 2077 6520 646f  ...wait so we do
+00014a00: 6e27 7420 6861 6d6d 6572 2074 6865 2068  n't hammer the h
+00014a10: 6f73 7420 6265 666f 7265 2061 736b 696e  ost before askin
+00014a20: 6720 666f 7220 6d6f 7265 0a20 2020 2020  g for more.     
+00014a30: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
+00014a40: 2830 2e32 3529 0a0a 2020 2020 2020 2020  (0.25)..        
+00014a50: 6966 2073 656c 662e 5f6f 6666 7365 7420  if self._offset 
+00014a60: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00014a70: 2020 7365 6c66 2e5f 6765 745f 6e75 6d5f    self._get_num_
+00014a80: 726f 7773 2829 0a0a 2020 2020 2020 2020  rows()..        
+00014a90: 726f 775f 6c65 6e67 7468 203d 2073 656c  row_length = sel
+00014aa0: 662e 5f67 6574 5f69 6e74 2829 202d 2034  f._get_int() - 4
+00014ab0: 2020 2320 726f 775f 6c65 6e67 7468 2069    # row_length i
+00014ac0: 6e63 6c75 6465 7320 7468 6520 3420 6279  ncludes the 4 by
+00014ad0: 7465 7320 7765 206a 7573 7420 636f 6e73  tes we just cons
+00014ae0: 756d 6564 0a20 2020 2020 2020 2065 6e64  umed.        end
+00014af0: 5f6f 6666 7365 7420 3d20 7365 6c66 2e5f  _offset = self._
+00014b00: 6f66 6673 6574 202b 2072 6f77 5f6c 656e  offset + row_len
+00014b10: 6774 680a 0a20 2020 2020 2020 2069 6620  gth..        if 
+00014b20: 7365 6c66 2e5f 6279 7465 735f 7265 6d61  self._bytes_rema
+00014b30: 696e 696e 6728 2920 3d3d 2031 2061 6e64  ining() == 1 and
+00014b40: 2073 656c 662e 5f62 7566 2829 5b73 656c   self._buf()[sel
+00014b50: 662e 5f6f 6666 7365 745d 203d 3d20 5479  f._offset] == Ty
+00014b60: 7065 436f 6465 732e 4445 4d3a 0a20 2020  peCodes.DEM:.   
+00014b70: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
+00014b80: 7763 6f75 6e74 202d 3d20 310a 2020 2020  wcount -= 1.    
+00014b90: 2020 2020 2020 2020 7365 6c66 2e5f 6275          self._bu
+00014ba0: 6666 6572 732e 706f 7028 3029 0a20 2020  ffers.pop(0).   
+00014bb0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00014bc0: 6c6f 7365 5f72 6573 756c 7473 6574 2829  lose_resultset()
+00014bd0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00014be0: 7572 6e20 7365 6c66 2e5f 7072 6f63 6573  urn self._proces
+00014bf0: 735f 7065 6e64 696e 6728 290a 0a20 2020  s_pending()..   
+00014c00: 2020 2020 2061 5f72 6f77 203d 205b 5d0a       a_row = [].
+00014c10: 2020 2020 2020 2020 7768 696c 6520 7365          while se
+00014c20: 6c66 2e5f 6f66 6673 6574 203c 2065 6e64  lf._offset < end
+00014c30: 5f6f 6666 7365 743a 0a20 2020 2020 2020  _offset:.       
+00014c40: 2020 2020 2061 5f72 6f77 2e61 7070 656e       a_row.appen
+00014c50: 6428 7365 6c66 2e5f 6465 636f 6465 5f65  d(self._decode_e
+00014c60: 6e74 7279 2829 290a 0a20 2020 2020 2020  ntry())..       
+00014c70: 2069 6620 7365 6c66 2e5f 6f66 6673 6574   if self._offset
+00014c80: 203e 3d20 6c65 6e28 7365 6c66 2e5f 6275   >= len(self._bu
+00014c90: 6628 2929 3a0a 2020 2020 2020 2020 2020  f()):.          
+00014ca0: 2020 7365 6c66 2e5f 6275 6666 6572 732e    self._buffers.
+00014cb0: 706f 7028 3029 0a20 2020 2020 2020 2020  pop(0).         
+00014cc0: 2020 2073 656c 662e 5f6f 6666 7365 7420     self._offset 
+00014cd0: 3d20 300a 2020 2020 2020 2020 7365 6c66  = 0.        self
+00014ce0: 2e72 6f77 6e75 6d62 6572 202b 3d20 310a  .rownumber += 1.
+00014cf0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00014d00: 656c 662e 7265 7375 6c74 7365 745f 7475  elf.resultset_tu
+00014d10: 706c 652e 5f6d 616b 6528 615f 726f 7729  ple._make(a_row)
+00014d20: 0a0a 2020 2020 6465 6620 5f70 726f 6365  ..    def _proce
+00014d30: 7373 5f70 656e 6469 6e67 2873 656c 6629  ss_pending(self)
+00014d40: 3a0a 2020 2020 2020 2020 2320 6966 2077  :.        # if w
+00014d50: 6520 6861 7665 2061 6e79 2070 656e 6469  e have any pendi
+00014d60: 6e67 2071 7565 7269 6573 2074 6f20 6578  ng queries to ex
+00014d70: 6563 7574 652c 206b 6963 6b20 6f6e 6520  ecute, kick one 
+00014d80: 6f66 6620 6e6f 770a 2020 2020 2020 2020  off now.        
+00014d90: 6966 2073 656c 662e 5f70 656e 6469 6e67  if self._pending
+00014da0: 5f6f 7073 3a0a 2020 2020 2020 2020 2020  _ops:.          
+00014db0: 2020 7365 6c66 2e5f 6275 6666 6572 7320    self._buffers 
+00014dc0: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+00014dd0: 2073 656c 662e 5f6f 6666 7365 7420 3d20   self._offset = 
+00014de0: 300a 2020 2020 2020 2020 2020 2020 7365  0.            se
+00014df0: 6c66 2e5f 6578 6563 7574 655f 696e 7465  lf._execute_inte
+00014e00: 726e 616c 2873 656c 662e 5f70 656e 6469  rnal(self._pendi
+00014e10: 6e67 5f6f 7073 2e70 6f70 2830 2929 0a20  ng_ops.pop(0)). 
+00014e20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00014e30: 6e20 7365 6c66 2e66 6574 6368 6f6e 6528  n self.fetchone(
+00014e40: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00014e50: 656e 645f 6f66 5f64 6174 6120 3d20 5472  end_of_data = Tr
+00014e60: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+00014e70: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
+00014e80: 5f62 7566 2873 656c 6629 3a0a 2020 2020  _buf(self):.    
+00014e90: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00014ea0: 5f62 7566 6665 7273 5b30 5d0a 0a20 2020  _buffers[0]..   
+00014eb0: 2064 6566 205f 6279 7465 735f 7265 6d61   def _bytes_rema
+00014ec0: 696e 696e 6728 7365 6c66 293a 0a20 2020  ining(self):.   
+00014ed0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00014ee0: 2e5f 6275 6666 6572 733a 0a20 2020 2020  ._buffers:.     
+00014ef0: 2020 2020 2020 2072 6574 7572 6e20 300a         return 0.
+00014f00: 2020 2020 2020 2020 7265 7475 726e 206c          return l
+00014f10: 656e 2873 656c 662e 5f62 7566 6665 7273  en(self._buffers
+00014f20: 5b30 5d29 202d 2073 656c 662e 5f6f 6666  [0]) - self._off
+00014f30: 7365 740a 0a20 2020 2064 6566 205f 6765  set..    def _ge
+00014f40: 745f 6e75 6d5f 726f 7773 2873 656c 6629  t_num_rows(self)
+00014f50: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00014f60: 662e 5f62 7974 6573 5f72 656d 6169 6e69  f._bytes_remaini
+00014f70: 6e67 2829 203e 3d20 343a 0a20 2020 2020  ng() >= 4:.     
+00014f80: 2020 2020 2020 2073 656c 662e 726f 7763         self.rowc
+00014f90: 6f75 6e74 202b 3d20 7365 6c66 2e5f 6765  ount += self._ge
+00014fa0: 745f 696e 7428 290a 0a20 2020 2064 6566  t_int()..    def
+00014fb0: 205f 6465 636f 6465 5f65 6e74 7279 2873   _decode_entry(s
+00014fc0: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
+00014fd0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+00014fe0: 746f 6f2d 6d61 6e79 2d6c 6f63 616c 732c  too-many-locals,
+00014ff0: 746f 6f2d 6d61 6e79 2d72 6574 7572 6e2d  too-many-return-
+00015000: 7374 6174 656d 656e 7473 2c74 6f6f 2d6d  statements,too-m
+00015010: 616e 792d 6272 616e 6368 6573 2c74 6f6f  any-branches,too
+00015020: 2d6d 616e 792d 7374 6174 656d 656e 7473  -many-statements
+00015030: 0a20 2020 2020 2020 2063 6f6c 7479 7065  .        coltype
+00015040: 203d 2073 656c 662e 5f67 6574 5f62 7974   = self._get_byt
+00015050: 6528 290a 0a20 2020 2020 2020 2023 2069  e()..        # i
+00015060: 6620 7468 6973 2069 7320 7468 6520 6561  f this is the ea
+00015070: 7379 2063 6f6e 7665 7273 696f 6e2c 206a  sy conversion, j
+00015080: 7573 7420 646f 2069 740a 2020 2020 2020  ust do it.      
+00015090: 2020 6966 2063 6f6c 7479 7065 2069 6e20    if coltype in 
+000150a0: 5f74 7970 655f 6d61 703a 0a20 2020 2020  _type_map:.     
+000150b0: 2020 2020 2020 2074 6d20 3d20 5f74 7970         tm = _typ
+000150c0: 655f 6d61 705b 636f 6c74 7970 655d 0a20  e_map[coltype]. 
+000150d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000150e0: 6e20 7365 6c66 2e5f 6765 745f 7479 7065  n self._get_type
+000150f0: 2874 6d5b 305d 2c20 746d 5b31 5d29 0a0a  (tm[0], tm[1])..
+00015100: 2020 2020 2020 2020 6966 2063 6f6c 7479          if colty
+00015110: 7065 203d 3d20 5479 7065 436f 6465 732e  pe == TypeCodes.
+00015120: 5354 5249 4e47 3a0a 2020 2020 2020 2020  STRING:.        
+00015130: 2020 2020 7374 726c 656e 203d 2073 656c      strlen = sel
+00015140: 662e 5f67 6574 5f69 6e74 2829 0a20 2020  f._get_int().   
+00015150: 2020 2020 2020 2020 206f 6666 7365 7420           offset 
+00015160: 3d20 7365 6c66 2e5f 6f66 6673 6574 0a20  = self._offset. 
+00015170: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015180: 5f6f 6666 7365 7420 2b3d 2073 7472 6c65  _offset += strle
+00015190: 6e0a 2020 2020 2020 2020 2020 2020 7265  n.            re
+000151a0: 7475 726e 2073 656c 662e 5f62 7566 2829  turn self._buf()
+000151b0: 5b6f 6666 7365 7420 3a20 6f66 6673 6574  [offset : offset
+000151c0: 202b 2073 7472 6c65 6e5d 2e64 6563 6f64   + strlen].decod
+000151d0: 6528 2275 7466 2d38 222c 2065 7272 6f72  e("utf-8", error
+000151e0: 733d 2272 6570 6c61 6365 2229 0a0a 2020  s="replace")..  
+000151f0: 2020 2020 2020 6966 2063 6f6c 7479 7065        if coltype
+00015200: 203d 3d20 5479 7065 436f 6465 732e 5449   == TypeCodes.TI
+00015210: 4d45 5354 414d 503a 0a20 2020 2020 2020  MESTAMP:.       
+00015220: 2020 2020 2072 6574 7572 6e20 6461 7465       return date
+00015230: 7469 6d65 2e64 6174 6574 696d 652e 7574  time.datetime.ut
+00015240: 6366 726f 6d74 696d 6573 7461 6d70 2873  cfromtimestamp(s
+00015250: 656c 662e 5f67 6574 5f6c 6f6e 6728 2929  elf._get_long())
+00015260: 0a0a 2020 2020 2020 2020 6966 2063 6f6c  ..        if col
+00015270: 7479 7065 203d 3d20 5479 7065 436f 6465  type == TypeCode
+00015280: 732e 4e55 4c4c 3a0a 2020 2020 2020 2020  s.NULL:.        
+00015290: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+000152a0: 0a20 2020 2020 2020 2069 6620 636f 6c74  .        if colt
+000152b0: 7970 6520 3d3d 2054 7970 6543 6f64 6573  ype == TypeCodes
+000152c0: 2e42 5954 453a 0a20 2020 2020 2020 2020  .BYTE:.         
+000152d0: 2020 2072 6574 7572 6e20 696e 742e 6672     return int.fr
+000152e0: 6f6d 5f62 7974 6573 2873 656c 662e 5f67  om_bytes(self._g
+000152f0: 6574 5f74 7970 6528 312c 205f 756e 7061  et_type(1, _unpa
+00015300: 636b 5f63 6861 7229 2c20 2262 6967 222c  ck_char), "big",
+00015310: 2073 6967 6e65 643d 5472 7565 290a 0a20   signed=True).. 
+00015320: 2020 2020 2020 2069 6620 636f 6c74 7970         if coltyp
+00015330: 6520 3d3d 2054 7970 6543 6f64 6573 2e54  e == TypeCodes.T
+00015340: 494d 453a 0a20 2020 2020 2020 2020 2020  IME:.           
+00015350: 2073 6563 6f6e 6473 203d 2073 656c 662e   seconds = self.
+00015360: 5f67 6574 5f6c 6f6e 6728 290a 2020 2020  _get_long().    
+00015370: 2020 2020 2020 2020 7365 636f 6e64 203d          second =
+00015380: 2069 6e74 2873 6563 6f6e 6473 2025 2036   int(seconds % 6
+00015390: 3029 0a20 2020 2020 2020 2020 2020 206d  0).            m
+000153a0: 696e 7574 6573 203d 2073 6563 6f6e 6473  inutes = seconds
+000153b0: 202f 2036 300a 2020 2020 2020 2020 2020   / 60.          
+000153c0: 2020 6d69 6e75 7465 203d 2069 6e74 286d    minute = int(m
+000153d0: 696e 7574 6573 2025 2036 3029 0a20 2020  inutes % 60).   
+000153e0: 2020 2020 2020 2020 2068 6f75 7273 203d           hours =
+000153f0: 206d 696e 7574 6573 202f 2036 300a 2020   minutes / 60.  
+00015400: 2020 2020 2020 2020 2020 686f 7572 203d            hour =
+00015410: 2069 6e74 2868 6f75 7273 2025 2032 3429   int(hours % 24)
+00015420: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00015430: 7572 6e20 6461 7465 7469 6d65 2e74 696d  urn datetime.tim
+00015440: 6528 686f 7572 2c20 6d69 6e75 7465 2c20  e(hour, minute, 
+00015450: 7365 636f 6e64 290a 0a20 2020 2020 2020  second)..       
+00015460: 2069 6620 636f 6c74 7970 6520 3d3d 2054   if coltype == T
+00015470: 7970 6543 6f64 6573 2e42 494e 4152 593a  ypeCodes.BINARY:
+00015480: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00015490: 6c65 6e20 3d20 7365 6c66 2e5f 6765 745f  len = self._get_
+000154a0: 696e 7428 290a 2020 2020 2020 2020 2020  int().          
+000154b0: 2020 6f66 6673 6574 203d 2073 656c 662e    offset = self.
+000154c0: 5f6f 6666 7365 740a 2020 2020 2020 2020  _offset.        
+000154d0: 2020 2020 7365 6c66 2e5f 6f66 6673 6574      self._offset
+000154e0: 202b 3d20 7374 726c 656e 0a20 2020 2020   += strlen.     
+000154f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00015500: 6c66 2e5f 6275 6628 295b 6f66 6673 6574  lf._buf()[offset
+00015510: 203a 206f 6666 7365 7420 2b20 7374 726c   : offset + strl
+00015520: 656e 5d0a 0a20 2020 2020 2020 2069 6620  en]..        if 
+00015530: 636f 6c74 7970 6520 3d3d 2054 7970 6543  coltype == TypeC
+00015540: 6f64 6573 2e44 4543 494d 414c 3a0a 2020  odes.DECIMAL:.  
+00015550: 2020 2020 2020 2020 2020 7072 6563 6973            precis
+00015560: 696f 6e20 3d20 7365 6c66 2e5f 6765 745f  ion = self._get_
+00015570: 6279 7465 2829 0a20 2020 2020 2020 2020  byte().         
+00015580: 2020 2073 6361 6c65 203d 2073 656c 662e     scale = self.
+00015590: 5f67 6574 5f62 7974 6528 290a 0a20 2020  _get_byte()..   
+000155a0: 2020 2020 2020 2020 2069 6620 7072 6563           if prec
+000155b0: 6973 696f 6e20 2520 3220 3d3d 2030 3a0a  ision % 2 == 0:.
+000155c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155d0: 7374 726c 656e 203d 2069 6e74 2828 7072  strlen = int((pr
+000155e0: 6563 6973 696f 6e20 2f20 3229 202b 2031  ecision / 2) + 1
+000155f0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00015600: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00015610: 2020 2020 7374 726c 656e 203d 2069 6e74      strlen = int
+00015620: 2828 7072 6563 6973 696f 6e20 2b20 3129  ((precision + 1)
+00015630: 202f 2032 290a 0a20 2020 2020 2020 2020   / 2)..         
+00015640: 2020 2064 6174 6120 3d20 7365 6c66 2e5f     data = self._
+00015650: 6275 6628 295b 7365 6c66 2e5f 6f66 6673  buf()[self._offs
+00015660: 6574 203a 2028 7365 6c66 2e5f 6f66 6673  et : (self._offs
+00015670: 6574 202b 2073 7472 6c65 6e20 2d20 3129  et + strlen - 1)
+00015680: 5d0a 2020 2020 2020 2020 2020 2020 6469  ].            di
+00015690: 6769 7473 203d 205b 5d0a 2020 2020 2020  gits = [].      
+000156a0: 2020 2020 2020 666f 7220 6279 7465 2069        for byte i
+000156b0: 6e20 6461 7461 3a0a 2020 2020 2020 2020  n data:.        
+000156c0: 2020 2020 2020 2020 6469 6769 7473 2e61          digits.a
+000156d0: 7070 656e 6428 2862 7974 6520 2620 3078  ppend((byte & 0x
+000156e0: 4630 2920 3e3e 2034 290a 2020 2020 2020  F0) >> 4).      
+000156f0: 2020 2020 2020 2020 2020 6469 6769 7473            digits
+00015700: 2e61 7070 656e 6428 6279 7465 2026 2030  .append(byte & 0
+00015710: 7830 4629 0a0a 2020 2020 2020 2020 2020  x0F)..          
+00015720: 2020 7369 676e 203d 2073 656c 662e 5f62    sign = self._b
+00015730: 7566 2829 5b73 656c 662e 5f6f 6666 7365  uf()[self._offse
+00015740: 7420 2b20 7374 726c 656e 202d 2031 5d0a  t + strlen - 1].
+00015750: 0a20 2020 2020 2020 2020 2020 2064 6967  .            dig
+00015760: 6974 732e 6170 7065 6e64 2873 6967 6e20  its.append(sign 
+00015770: 3e3e 2034 290a 2020 2020 2020 2020 2020  >> 4).          
+00015780: 2020 7369 676e 203d 2073 6967 6e20 2620    sign = sign & 
+00015790: 3078 3046 0a0a 2020 2020 2020 2020 2020  0x0F..          
+000157a0: 2020 6966 2073 6967 6e20 3d3d 2031 323a    if sign == 12:
+000157b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000157c0: 2073 6967 6e20 3d20 300a 2020 2020 2020   sign = 0.      
+000157d0: 2020 2020 2020 656c 6966 2073 6967 6e20        elif sign 
+000157e0: 3d3d 2031 333a 0a20 2020 2020 2020 2020  == 13:.         
+000157f0: 2020 2020 2020 2073 6967 6e20 3d20 310a         sign = 1.
+00015800: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00015810: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015820: 2020 7261 6973 6520 4572 726f 7228 7265    raise Error(re
+00015830: 6173 6f6e 3d66 2255 6e6b 6e6f 776e 2064  ason=f"Unknown d
+00015840: 6563 696d 616c 2073 6967 6e20 7661 6c75  ecimal sign valu
+00015850: 6520 7b73 6967 6e7d 2229 0a0a 2020 2020  e {sign}")..    
+00015860: 2020 2020 2020 2020 7365 6c66 2e5f 6f66          self._of
+00015870: 6673 6574 202b 3d20 7374 726c 656e 0a20  fset += strlen. 
+00015880: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00015890: 6e20 6465 6369 6d61 6c2e 4465 6369 6d61  n decimal.Decima
+000158a0: 6c28 2873 6967 6e2c 2064 6967 6974 732c  l((sign, digits,
+000158b0: 202d 7363 616c 6529 290a 0a20 2020 2020   -scale))..     
+000158c0: 2020 2069 6620 636f 6c74 7970 6520 3d3d     if coltype ==
+000158d0: 2054 7970 6543 6f64 6573 2e41 5252 4159   TypeCodes.ARRAY
+000158e0: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+000158f0: 7374 6564 5f6c 6576 656c 203d 2030 0a0a  sted_level = 0..
+00015900: 2020 2020 2020 2020 2020 2020 6172 7261              arra
+00015910: 7974 7970 6520 3d20 7365 6c66 2e5f 6765  ytype = self._ge
+00015920: 745f 6279 7465 2829 0a0a 2020 2020 2020  t_byte()..      
+00015930: 2020 2020 2020 7768 696c 6520 6172 7261        while arra
+00015940: 7974 7970 6520 3d3d 2054 7970 6543 6f64  ytype == TypeCod
+00015950: 6573 2e41 5252 4159 3a0a 2020 2020 2020  es.ARRAY:.      
+00015960: 2020 2020 2020 2020 2020 6172 7261 7974            arrayt
+00015970: 7970 6520 3d20 7365 6c66 2e5f 6765 745f  ype = self._get_
+00015980: 6279 7465 2829 0a20 2020 2020 2020 2020  byte().         
+00015990: 2020 2020 2020 206e 6573 7465 645f 6c65         nested_le
+000159a0: 7665 6c20 2b3d 2031 0a0a 2020 2020 2020  vel += 1..      
+000159b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000159c0: 662e 5f67 6574 5f61 7272 6179 286e 6573  f._get_array(nes
+000159d0: 7465 645f 6c65 7665 6c29 0a0a 2020 2020  ted_level)..    
+000159e0: 2020 2020 6966 2063 6f6c 7479 7065 203d      if coltype =
+000159f0: 3d20 5479 7065 436f 6465 732e 5555 4944  = TypeCodes.UUID
+00015a00: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00015a10: 6c66 2e5f 6f66 6673 6574 202b 3d20 3136  lf._offset += 16
+00015a20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00015a30: 7572 6e20 7575 6964 2e55 5549 4428 6279  urn uuid.UUID(by
+00015a40: 7465 733d 7365 6c66 2e5f 6275 6628 295b  tes=self._buf()[
+00015a50: 7365 6c66 2e5f 6f66 6673 6574 202d 2031  self._offset - 1
+00015a60: 3620 3a20 7365 6c66 2e5f 6f66 6673 6574  6 : self._offset
+00015a70: 5d29 0a0a 2020 2020 2020 2020 6966 2063  ])..        if c
+00015a80: 6f6c 7479 7065 203d 3d20 5479 7065 436f  oltype == TypeCo
+00015a90: 6465 732e 5354 5f50 4f49 4e54 3a0a 2020  des.ST_POINT:.  
+00015aa0: 2020 2020 2020 2020 2020 6c6f 6e67 203d            long =
+00015ab0: 2073 656c 662e 5f67 6574 5f64 6f75 626c   self._get_doubl
+00015ac0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00015ad0: 6c61 7420 3d20 7365 6c66 2e5f 6765 745f  lat = self._get_
+00015ae0: 646f 7562 6c65 2829 0a20 2020 2020 2020  double().       
+00015af0: 2020 2020 2072 6574 7572 6e20 5f53 5450       return _STP
+00015b00: 6f69 6e74 286c 6f6e 672c 206c 6174 290a  oint(long, lat).
+00015b10: 0a20 2020 2020 2020 2069 6620 636f 6c74  .        if colt
+00015b20: 7970 6520 3d3d 2054 7970 6543 6f64 6573  ype == TypeCodes
+00015b30: 2e44 4154 453a 0a20 2020 2020 2020 2020  .DATE:.         
+00015b40: 2020 2064 203d 2064 6174 6574 696d 652e     d = datetime.
+00015b50: 6461 7465 7469 6d65 2e75 7463 6672 6f6d  datetime.utcfrom
+00015b60: 7469 6d65 7374 616d 7028 7365 6c66 2e5f  timestamp(self._
+00015b70: 6765 745f 6c6f 6e67 2829 202f 2031 3030  get_long() / 100
+00015b80: 302e 3029 0a20 2020 2020 2020 2020 2020  0.0).           
+00015b90: 2072 6574 7572 6e20 6461 7465 7469 6d65   return datetime
+00015ba0: 2e64 6174 6528 642e 7965 6172 2c20 642e  .date(d.year, d.
+00015bb0: 6d6f 6e74 682c 2064 2e64 6179 290a 0a20  month, d.day).. 
+00015bc0: 2020 2020 2020 2069 6620 636f 6c74 7970         if coltyp
+00015bd0: 6520 3d3d 2054 7970 6543 6f64 6573 2e49  e == TypeCodes.I
+00015be0: 503a 0a20 2020 2020 2020 2020 2020 206f  P:.            o
+00015bf0: 6666 203d 2073 656c 662e 5f6f 6666 7365  ff = self._offse
+00015c00: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
+00015c10: 6c66 2e5f 6f66 6673 6574 202b 3d20 3136  lf._offset += 16
+00015c20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00015c30: 7572 6e20 6970 6164 6472 6573 732e 6970  urn ipaddress.ip
+00015c40: 5f61 6464 7265 7373 2873 656c 662e 5f62  _address(self._b
+00015c50: 7566 2829 5b6f 6666 203a 206f 6666 202b  uf()[off : off +
+00015c60: 2031 365d 290a 0a20 2020 2020 2020 2069   16])..        i
+00015c70: 6620 636f 6c74 7970 6520 3d3d 2054 7970  f coltype == Typ
+00015c80: 6543 6f64 6573 2e49 5056 343a 0a20 2020  eCodes.IPV4:.   
+00015c90: 2020 2020 2020 2020 206f 6666 203d 2073           off = s
+00015ca0: 656c 662e 5f6f 6666 7365 740a 2020 2020  elf._offset.    
+00015cb0: 2020 2020 2020 2020 7365 6c66 2e5f 6f66          self._of
+00015cc0: 6673 6574 202b 3d20 340a 2020 2020 2020  fset += 4.      
+00015cd0: 2020 2020 2020 7265 7475 726e 2069 7061        return ipa
+00015ce0: 6464 7265 7373 2e69 705f 6164 6472 6573  ddress.ip_addres
+00015cf0: 7328 7365 6c66 2e5f 6275 6628 295b 6f66  s(self._buf()[of
+00015d00: 6620 3a20 6f66 6620 2b20 345d 290a 0a20  f : off + 4]).. 
+00015d10: 2020 2020 2020 2069 6620 636f 6c74 7970         if coltyp
+00015d20: 6520 3d3d 2054 7970 6543 6f64 6573 2e54  e == TypeCodes.T
+00015d30: 494d 4553 5441 4d50 5f4e 414e 4f53 3a0a  IMESTAMP_NANOS:.
+00015d40: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+00015d50: 7374 616d 7020 3d20 7365 6c66 2e5f 6765  stamp = self._ge
+00015d60: 745f 6c6f 6e67 2829 202f 2031 3030 3030  t_long() / 10000
+00015d70: 3030 3030 302e 300a 2020 2020 2020 2020  00000.0.        
+00015d80: 2020 2020 7265 7475 726e 2064 6174 6574      return datet
+00015d90: 696d 652e 6461 7465 7469 6d65 2e75 7463  ime.datetime.utc
+00015da0: 6672 6f6d 7469 6d65 7374 616d 7028 7469  fromtimestamp(ti
+00015db0: 6d65 7374 616d 7029 0a0a 2020 2020 2020  mestamp)..      
+00015dc0: 2020 6966 2063 6f6c 7479 7065 203d 3d20    if coltype == 
+00015dd0: 5479 7065 436f 6465 732e 5449 4d45 5f4e  TypeCodes.TIME_N
+00015de0: 414e 4f53 3a0a 2020 2020 2020 2020 2020  ANOS:.          
+00015df0: 2020 6e61 6e6f 7320 3d20 7365 6c66 2e5f    nanos = self._
+00015e00: 6765 745f 6c6f 6e67 2829 0a20 2020 2020  get_long().     
+00015e10: 2020 2020 2020 206d 6963 726f 7320 3d20         micros = 
+00015e20: 696e 7428 286e 616e 6f73 202f 2031 3030  int((nanos / 100
+00015e30: 3029 2025 2031 3030 3030 3030 290a 2020  0) % 1000000).  
+00015e40: 2020 2020 2020 2020 2020 7365 636f 6e64            second
+00015e50: 7320 3d20 6e61 6e6f 7320 2f20 3130 3030  s = nanos / 1000
+00015e60: 3030 3030 3030 0a20 2020 2020 2020 2020  000000.         
+00015e70: 2020 2073 6563 6f6e 6420 3d20 696e 7428     second = int(
+00015e80: 7365 636f 6e64 7320 2520 3630 290a 2020  seconds % 60).  
+00015e90: 2020 2020 2020 2020 2020 6d69 6e75 7465            minute
+00015ea0: 7320 3d20 7365 636f 6e64 7320 2f20 3630  s = seconds / 60
+00015eb0: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
+00015ec0: 7574 6520 3d20 696e 7428 6d69 6e75 7465  ute = int(minute
+00015ed0: 7320 2520 3630 290a 2020 2020 2020 2020  s % 60).        
+00015ee0: 2020 2020 686f 7572 7320 3d20 6d69 6e75      hours = minu
+00015ef0: 7465 7320 2f20 3630 0a20 2020 2020 2020  tes / 60.       
+00015f00: 2020 2020 2068 6f75 7220 3d20 696e 7428       hour = int(
+00015f10: 686f 7572 7320 2520 3234 290a 0a20 2020  hours % 24)..   
+00015f20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00015f30: 6461 7465 7469 6d65 2e74 696d 6528 686f  datetime.time(ho
+00015f40: 7572 2c20 6d69 6e75 7465 2c20 7365 636f  ur, minute, seco
+00015f50: 6e64 2c20 6d69 6372 6f73 290a 0a20 2020  nd, micros)..   
+00015f60: 2020 2020 2069 6620 636f 6c74 7970 6520       if coltype 
+00015f70: 3d3d 2054 7970 6543 6f64 6573 2e54 5550  == TypeCodes.TUP
+00015f80: 4c45 3a0a 2020 2020 2020 2020 2020 2020  LE:.            
+00015f90: 7265 7475 726e 2073 656c 662e 5f67 6574  return self._get
+00015fa0: 5f74 7570 6c65 2829 0a0a 2020 2020 2020  _tuple()..      
+00015fb0: 2020 6966 2063 6f6c 7479 7065 203d 3d20    if coltype == 
+00015fc0: 5479 7065 436f 6465 732e 5354 5f4c 494e  TypeCodes.ST_LIN
+00015fd0: 4553 5452 494e 473a 0a20 2020 2020 2020  ESTRING:.       
+00015fe0: 2020 2020 2070 6f69 6e74 7320 3d20 5b5d       points = []
+00015ff0: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+00016000: 5f65 6c65 6d65 6e74 7320 3d20 7365 6c66  _elements = self
+00016010: 2e5f 6765 745f 696e 7428 290a 2020 2020  ._get_int().    
+00016020: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00016030: 2072 616e 6765 286e 756d 5f65 6c65 6d65   range(num_eleme
+00016040: 6e74 7329 3a0a 2020 2020 2020 2020 2020  nts):.          
+00016050: 2020 2020 2020 6c6f 6e67 203d 2073 656c        long = sel
+00016060: 662e 5f67 6574 5f64 6f75 626c 6528 290a  f._get_double().
+00016070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016080: 6c61 7420 3d20 7365 6c66 2e5f 6765 745f  lat = self._get_
+00016090: 646f 7562 6c65 2829 0a20 2020 2020 2020  double().       
+000160a0: 2020 2020 2020 2020 2070 6f69 6e74 732e           points.
+000160b0: 6170 7065 6e64 285f 5354 506f 696e 7428  append(_STPoint(
+000160c0: 6c6f 6e67 2c20 6c61 7429 290a 2020 2020  long, lat)).    
+000160d0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000160e0: 5354 4c69 6e65 7374 7269 6e67 2870 6f69  STLinestring(poi
+000160f0: 6e74 7329 0a0a 2020 2020 2020 2020 6966  nts)..        if
+00016100: 2063 6f6c 7479 7065 203d 3d20 5479 7065   coltype == Type
+00016110: 436f 6465 732e 5354 5f50 4f4c 5947 4f4e  Codes.ST_POLYGON
+00016120: 3a0a 2020 2020 2020 2020 2020 2020 6578  :.            ex
+00016130: 7465 7269 6f72 203d 205b 5d0a 2020 2020  terior = [].    
+00016140: 2020 2020 2020 2020 6e75 6d5f 656c 656d          num_elem
+00016150: 656e 7473 203d 2073 656c 662e 5f67 6574  ents = self._get
+00016160: 5f69 6e74 2829 0a20 2020 2020 2020 2020  _int().         
+00016170: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00016180: 6528 6e75 6d5f 656c 656d 656e 7473 293a  e(num_elements):
+00016190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000161a0: 206c 6f6e 6720 3d20 7365 6c66 2e5f 6765   long = self._ge
+000161b0: 745f 646f 7562 6c65 2829 0a20 2020 2020  t_double().     
+000161c0: 2020 2020 2020 2020 2020 206c 6174 203d             lat =
+000161d0: 2073 656c 662e 5f67 6574 5f64 6f75 626c   self._get_doubl
+000161e0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+000161f0: 2020 2020 6578 7465 7269 6f72 2e61 7070      exterior.app
+00016200: 656e 6428 5f53 5450 6f69 6e74 286c 6f6e  end(_STPoint(lon
+00016210: 672c 206c 6174 2929 0a20 2020 2020 2020  g, lat)).       
+00016220: 2020 2020 2068 6f6c 6573 203d 205b 5d0a       holes = [].
+00016230: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
+00016240: 7269 6e67 7320 3d20 7365 6c66 2e5f 6765  rings = self._ge
+00016250: 745f 696e 7428 290a 2020 2020 2020 2020  t_int().        
+00016260: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00016270: 6765 286e 756d 5f72 696e 6773 293a 0a20  ge(num_rings):. 
+00016280: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00016290: 756d 5f65 6c65 6d65 6e74 7320 3d20 7365  um_elements = se
+000162a0: 6c66 2e5f 6765 745f 696e 7428 290a 2020  lf._get_int().  
+000162b0: 2020 2020 2020 2020 2020 2020 2020 7269                ri
+000162c0: 6e67 203d 205b 5d0a 2020 2020 2020 2020  ng = [].        
+000162d0: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
+000162e0: 2072 616e 6765 286e 756d 5f65 6c65 6d65   range(num_eleme
+000162f0: 6e74 7329 3a0a 2020 2020 2020 2020 2020  nts):.          
+00016300: 2020 2020 2020 2020 2020 6c6f 6e67 203d            long =
+00016310: 2073 656c 662e 5f67 6574 5f64 6f75 626c   self._get_doubl
+00016320: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00016330: 2020 2020 2020 2020 6c61 7420 3d20 7365          lat = se
+00016340: 6c66 2e5f 6765 745f 646f 7562 6c65 2829  lf._get_double()
+00016350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016360: 2020 2020 2072 696e 672e 6170 7065 6e64       ring.append
+00016370: 285f 5354 506f 696e 7428 6c6f 6e67 2c20  (_STPoint(long, 
+00016380: 6c61 7429 290a 2020 2020 2020 2020 2020  lat)).          
+00016390: 2020 2020 2020 686f 6c65 732e 6170 7065        holes.appe
+000163a0: 6e64 2872 696e 6729 0a20 2020 2020 2020  nd(ring).       
+000163b0: 2020 2020 2072 6574 7572 6e20 5f53 5450       return _STP
+000163c0: 6f6c 7967 6f6e 2865 7874 6572 696f 722c  olygon(exterior,
+000163d0: 2068 6f6c 6573 290a 0a20 2020 2020 2020   holes)..       
+000163e0: 2073 656c 662e 656e 645f 6f66 5f64 6174   self.end_of_dat
+000163f0: 6120 3d20 5472 7565 0a20 2020 2020 2020  a = True.       
+00016400: 2072 6169 7365 2045 7272 6f72 2872 6561   raise Error(rea
+00016410: 736f 6e3d 6622 556e 6b6e 6f77 6e20 636f  son=f"Unknown co
+00016420: 6c75 6d6e 2074 7970 6520 7b63 6f6c 7479  lumn type {colty
+00016430: 7065 7d22 290a 0a20 2020 2064 6566 205f  pe}")..    def _
+00016440: 6765 745f 6279 7465 2873 656c 6629 3a0a  get_byte(self):.
+00016450: 2020 2020 2020 2020 6f66 6673 6574 203d          offset =
+00016460: 2073 656c 662e 5f6f 6666 7365 740a 2020   self._offset.  
+00016470: 2020 2020 2020 7365 6c66 2e5f 6f66 6673        self._offs
+00016480: 6574 202b 3d20 310a 2020 2020 2020 2020  et += 1.        
+00016490: 7265 7475 726e 2073 656c 662e 5f62 7566  return self._buf
+000164a0: 2829 5b6f 6666 7365 745d 0a0a 2020 2020  ()[offset]..    
+000164b0: 6465 6620 5f67 6574 5f69 6e74 2873 656c  def _get_int(sel
+000164c0: 6629 3a0a 2020 2020 2020 2020 6f66 6673  f):.        offs
+000164d0: 6574 203d 2073 656c 662e 5f6f 6666 7365  et = self._offse
+000164e0: 740a 2020 2020 2020 2020 7365 6c66 2e5f  t.        self._
+000164f0: 6f66 6673 6574 202b 3d20 340a 2020 2020  offset += 4.    
+00016500: 2020 2020 7265 7475 726e 205f 756e 7061      return _unpa
+00016510: 636b 5f69 6e74 2873 656c 662e 5f62 7566  ck_int(self._buf
+00016520: 2829 2c20 6f66 6673 6574 295b 305d 0a0a  (), offset)[0]..
+00016530: 2020 2020 6465 6620 5f67 6574 5f6c 6f6e      def _get_lon
+00016540: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
+00016550: 206f 6666 7365 7420 3d20 7365 6c66 2e5f   offset = self._
+00016560: 6f66 6673 6574 0a20 2020 2020 2020 2073  offset.        s
+00016570: 656c 662e 5f6f 6666 7365 7420 2b3d 2038  elf._offset += 8
+00016580: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00016590: 5f75 6e70 6163 6b5f 6c6f 6e67 2873 656c  _unpack_long(sel
+000165a0: 662e 5f62 7566 2829 2c20 6f66 6673 6574  f._buf(), offset
+000165b0: 295b 305d 0a0a 2020 2020 6465 6620 5f67  )[0]..    def _g
+000165c0: 6574 5f64 6f75 626c 6528 7365 6c66 293a  et_double(self):
+000165d0: 0a20 2020 2020 2020 206f 6666 7365 7420  .        offset 
+000165e0: 3d20 7365 6c66 2e5f 6f66 6673 6574 0a20  = self._offset. 
+000165f0: 2020 2020 2020 2073 656c 662e 5f6f 6666         self._off
+00016600: 7365 7420 2b3d 2038 0a20 2020 2020 2020  set += 8.       
+00016610: 2072 6574 7572 6e20 5f75 6e70 6163 6b5f   return _unpack_
+00016620: 646f 7562 6c65 2873 656c 662e 5f62 7566  double(self._buf
+00016630: 2829 2c20 6f66 6673 6574 295b 305d 0a0a  (), offset)[0]..
+00016640: 2020 2020 6465 6620 5f67 6574 5f74 7970      def _get_typ
+00016650: 6528 7365 6c66 2c20 6461 7461 6c65 6e2c  e(self, datalen,
+00016660: 2075 6e70 6163 6b65 7229 3a0a 2020 2020   unpacker):.    
+00016670: 2020 2020 6f66 6673 6574 203d 2073 656c      offset = sel
+00016680: 662e 5f6f 6666 7365 740a 2020 2020 2020  f._offset.      
+00016690: 2020 7365 6c66 2e5f 6f66 6673 6574 202b    self._offset +
+000166a0: 3d20 6461 7461 6c65 6e0a 2020 2020 2020  = datalen.      
+000166b0: 2020 7265 7475 726e 2075 6e70 6163 6b65    return unpacke
+000166c0: 7228 7365 6c66 2e5f 6275 6628 292c 206f  r(self._buf(), o
+000166d0: 6666 7365 7429 5b30 5d0a 0a20 2020 2064  ffset)[0]..    d
+000166e0: 6566 205f 6765 745f 6172 7261 7928 7365  ef _get_array(se
+000166f0: 6c66 2c20 6c65 7665 6c29 3a0a 2020 2020  lf, level):.    
+00016700: 2020 2020 6172 7261 7920 3d20 5b5d 0a0a      array = []..
+00016710: 2020 2020 2020 2020 6e75 6d5f 656c 656d          num_elem
+00016720: 656e 7473 203d 2073 656c 662e 5f67 6574  ents = self._get
+00016730: 5f69 6e74 2829 0a0a 2020 2020 2020 2020  _int()..        
+00016740: 616c 6c5f 6e75 6c6c 203d 2073 656c 662e  all_null = self.
+00016750: 5f67 6574 5f62 7974 6528 290a 0a20 2020  _get_byte()..   
+00016760: 2020 2020 2069 6620 616c 6c5f 6e75 6c6c       if all_null
+00016770: 2021 3d20 303a 0a20 2020 2020 2020 2020   != 0:.         
+00016780: 2020 2072 6574 7572 6e20 5b5d 0a0a 2020     return []..  
+00016790: 2020 2020 2020 666f 7220 5f20 696e 2072        for _ in r
+000167a0: 616e 6765 286e 756d 5f65 6c65 6d65 6e74  ange(num_element
+000167b0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+000167c0: 6966 206c 6576 656c 203e 2030 3a0a 2020  if level > 0:.  
+000167d0: 2020 2020 2020 2020 2020 2020 2020 6172                ar
+000167e0: 7261 792e 6170 7065 6e64 2873 656c 662e  ray.append(self.
+000167f0: 5f67 6574 5f61 7272 6179 286c 6576 656c  _get_array(level
+00016800: 202d 2031 2929 0a20 2020 2020 2020 2020   - 1)).         
+00016810: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00016820: 2020 2020 2020 2020 2061 7272 6179 2e61           array.a
+00016830: 7070 656e 6428 7365 6c66 2e5f 6465 636f  ppend(self._deco
+00016840: 6465 5f65 6e74 7279 2829 290a 0a20 2020  de_entry())..   
+00016850: 2020 2020 2072 6574 7572 6e20 6172 7261       return arra
+00016860: 790a 0a20 2020 2064 6566 205f 636c 6f73  y..    def _clos
+00016870: 655f 7265 7375 6c74 7365 7428 7365 6c66  e_resultset(self
+00016880: 293a 0a20 2020 2020 2020 2072 6571 203d  ):.        req =
+00016890: 2070 726f 746f 2e52 6571 7565 7374 2829   proto.Request()
+000168a0: 0a20 2020 2020 2020 2072 6571 2e74 7970  .        req.typ
+000168b0: 6520 3d20 7072 6f74 6f2e 5265 7175 6573  e = proto.Reques
+000168c0: 742e 5265 7175 6573 7454 7970 652e 5661  t.RequestType.Va
+000168d0: 6c75 6528 2243 4c4f 5345 5f52 4553 554c  lue("CLOSE_RESUL
+000168e0: 545f 5345 5422 290a 0a20 2020 2020 2020  T_SET")..       
+000168f0: 205f 7365 6e64 5f6d 7367 2873 656c 662e   _send_msg(self.
+00016900: 636f 6e6e 6563 7469 6f6e 2c20 7265 7129  connection, req)
+00016910: 0a0a 2020 2020 2020 2020 7273 7020 3d20  ..        rsp = 
+00016920: 5f72 6563 765f 6d73 6728 7365 6c66 2e63  _recv_msg(self.c
+00016930: 6f6e 6e65 6374 696f 6e2c 2070 726f 746f  onnection, proto
+00016940: 2e43 6f6e 6669 726d 6174 696f 6e52 6573  .ConfirmationRes
+00016950: 706f 6e73 6528 2929 0a0a 2020 2020 2020  ponse())..      
+00016960: 2020 6966 2072 7370 2e74 7970 6520 3d3d    if rsp.type ==
+00016970: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
+00016980: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
+00016990: 4f4e 5345 5f57 4152 4e3a 0a20 2020 2020  ONSE_WARN:.     
+000169a0: 2020 2020 2020 2077 6172 6e28 7273 702e         warn(rsp.
+000169b0: 7265 6173 6f6e 290a 2020 2020 2020 2020  reason).        
+000169c0: 656c 6966 206e 6f74 2072 7370 2e74 7970  elif not rsp.typ
+000169d0: 6520 3d3d 2070 726f 746f 2e43 6f6e 6669  e == proto.Confi
+000169e0: 726d 6174 696f 6e52 6573 706f 6e73 652e  rmationResponse.
+000169f0: 5245 5350 4f4e 5345 5f4f 4b3a 0a20 2020  RESPONSE_OK:.   
+00016a00: 2020 2020 2020 2020 2072 6169 7365 205f           raise _
+00016a10: 636f 6e76 6572 745f 6578 6365 7074 696f  convert_exceptio
+00016a20: 6e28 7273 7029 0a0a 2020 2020 6465 6620  n(rsp)..    def 
+00016a30: 5f67 6574 5f74 7570 6c65 2873 656c 6629  _get_tuple(self)
+00016a40: 3a0a 2020 2020 2020 2020 6e75 6d5f 656c  :.        num_el
+00016a50: 656d 656e 7473 203d 2073 656c 662e 5f67  ements = self._g
+00016a60: 6574 5f69 6e74 2829 0a20 2020 2020 2020  et_int().       
+00016a70: 2072 6573 7475 706c 6520 3d20 2829 0a20   restuple = (). 
+00016a80: 2020 2020 2020 2066 6f72 205f 2069 6e20         for _ in 
+00016a90: 7261 6e67 6528 6e75 6d5f 656c 656d 656e  range(num_elemen
+00016aa0: 7473 293a 0a20 2020 2020 2020 2020 2020  ts):.           
+00016ab0: 2072 6573 7475 706c 6520 2b3d 2028 7365   restuple += (se
+00016ac0: 6c66 2e5f 6465 636f 6465 5f65 6e74 7279  lf._decode_entry
+00016ad0: 2829 2c29 0a20 2020 2020 2020 2072 6574  (),).        ret
+00016ae0: 7572 6e20 7265 7374 7570 6c65 0a0a 0a64  urn restuple...d
+00016af0: 6566 2063 6f6e 6e65 6374 2864 736e 3d4e  ef connect(dsn=N
+00016b00: 6f6e 652c 2075 7365 723d 4e6f 6e65 2c20  one, user=None, 
+00016b10: 7061 7373 776f 7264 3d4e 6f6e 652c 2068  password=None, h
+00016b20: 6f73 743d 4e6f 6e65 2c20 6461 7461 6261  ost=None, databa
+00016b30: 7365 3d4e 6f6e 652c 2074 6c73 3d4e 6f6e  se=None, tls=Non
+00016b40: 652c 2066 6f72 6365 3d4e 6f6e 652c 2068  e, force=None, h
+00016b50: 616e 6473 6861 6b65 3d22 6763 6d22 2c20  andshake="gcm", 
+00016b60: 636f 6e66 6967 6669 6c65 3d4e 6f6e 6529  configfile=None)
+00016b70: 3a0a 2020 2020 2320 7079 6c69 6e74 3a20  :.    # pylint: 
+00016b80: 6469 7361 626c 653d 746f 6f2d 6d61 6e79  disable=too-many
+00016b90: 2d61 7267 756d 656e 7473 0a20 2020 2022  -arguments.    "
+00016ba0: 2222 4372 6561 7465 2061 206e 6577 2064  ""Create a new d
+00016bb0: 6174 6162 6173 6520 636f 6e6e 6563 7469  atabase connecti
+00016bc0: 6f6e 2e0a 0a20 2020 2054 6865 2063 6f6e  on...    The con
+00016bd0: 6e65 6374 696f 6e20 7061 7261 6d65 7465  nection paramete
+00016be0: 7273 2063 616e 2062 6520 7370 6563 6966  rs can be specif
+00016bf0: 6965 6420 6173 2070 6172 7420 6f66 2074  ied as part of t
+00016c00: 6865 2064 736e 2c0a 2020 2020 7573 696e  he dsn,.    usin
+00016c10: 6720 6b65 7977 6f72 6420 6172 6775 6d65  g keyword argume
+00016c20: 6e74 7320 6f72 2062 6f74 682e 2020 4966  nts or both.  If
+00016c30: 2062 6f74 6820 6172 6520 7370 6563 6966   both are specif
+00016c40: 6965 642c 2074 6865 206b 6579 776f 7264  ied, the keyword
+00016c50: 0a20 2020 2070 6172 616d 6574 6572 206f  .    parameter o
+00016c60: 7665 7272 6964 6573 2074 6865 2076 616c  verrides the val
+00016c70: 7565 2069 6e20 7468 6520 6473 6e2e 0a0a  ue in the dsn...
+00016c80: 2020 2020 5468 6520 4f63 6965 6e74 2044      The Ocient D
+00016c90: 534e 2069 7320 6f66 2074 6865 2066 6f72  SN is of the for
+00016ca0: 6d61 743a 0a20 2020 2060 6f63 6965 6e74  mat:.    `ocient
+00016cb0: 3a2f 2f75 7365 723a 7061 7373 776f 7264  ://user:password
+00016cc0: 405b 686f 7374 5d5b 3a70 6f72 745d 5b2f  @[host][:port][/
+00016cd0: 6461 7461 6261 7365 5d5b 3f70 6172 616d  database][?param
+00016ce0: 313d 7661 6c75 6531 262e 2e2e 5d60 0a0a  1=value1&...]`..
+00016cf0: 2020 2020 6075 7365 7260 2061 6e64 2060      `user` and `
+00016d00: 7061 7373 776f 7264 6020 6d75 7374 2062  password` must b
+00016d10: 6520 7375 7070 6c69 6564 2e20 2060 686f  e supplied.  `ho
+00016d20: 7374 6020 6465 6661 756c 7473 2074 6f20  st` defaults to 
+00016d30: 6c6f 6361 6c68 6f73 742c 0a20 2020 2070  localhost,.    p
+00016d40: 6f72 7420 6465 6661 756c 7473 2074 6f20  ort defaults to 
+00016d50: 3430 3530 2c20 6461 7461 6261 7365 2064  4050, database d
+00016d60: 6566 6175 6c74 7320 746f 2060 7379 7374  efaults to `syst
+00016d70: 656d 6020 616e 6420 6074 6c73 6020 6465  em` and `tls` de
+00016d80: 6661 756c 7473 0a20 2020 2074 6f20 6075  faults.    to `u
+00016d90: 6e76 6572 6966 6965 6460 2e0a 0a20 2020  nverified`...   
+00016da0: 204d 756c 7469 706c 6520 686f 7374 7320   Multiple hosts 
+00016db0: 6d61 7920 6265 2073 7065 6369 6669 6564  may be specified
+00016dc0: 2c20 7365 7061 7261 7465 6420 6279 2061  , separated by a
+00016dd0: 2063 6f6d 6d61 2c20 696e 2077 6869 6368   comma, in which
+00016de0: 2063 6173 6520 7468 650a 2020 2020 686f   case the.    ho
+00016df0: 7374 7320 7769 6c6c 2062 6520 7472 6965  sts will be trie
+00016e00: 6420 696e 206f 7264 6572 2020 5468 7573  d in order  Thus
+00016e10: 2061 6e20 6578 616d 706c 6520 4453 4e20   an example DSN 
+00016e20: 6d69 6768 7420 6265 0a20 2020 2060 6f63  might be.    `oc
+00016e30: 6965 6e74 3a2f 2f73 6f6d 656f 6e65 3a73  ient://someone:s
+00016e40: 6f6d 6570 6173 7377 6f72 6440 686f 7374  omepassword@host
+00016e50: 312c 686f 7374 323a 3430 3531 2f6d 7964  1,host2:4051/myd
+00016e60: 6260 0a0a 2020 2020 636f 6e66 6967 6669  b`..    configfi
+00016e70: 6c65 2073 7065 6369 6669 6573 2074 6865  le specifies the
+00016e80: 206e 616d 6520 6f66 2061 2063 6f6e 6669   name of a confi
+00016e90: 6775 7261 7469 6f6e 2066 696c 6520 696e  guration file in
+00016ea0: 2049 4e49 2066 6f72 6d61 742e 2053 6565   INI format. See
+00016eb0: 0a20 2020 2074 6865 2043 6f6e 6e65 6374  .    the Connect
+00016ec0: 696f 6e20 636c 6173 7320 666f 7220 6d6f  ion class for mo
+00016ed0: 7265 2064 6574 6169 6c65 6420 646f 6375  re detailed docu
+00016ee0: 6d65 6e74 6174 696f 6e2e 0a0a 2020 2020  mentation...    
+00016ef0: 4375 7272 656e 746c 7920 7375 7070 6f72  Currently suppor
+00016f00: 7465 6420 7061 7261 6d65 7465 7273 2061  ted parameters a
+00016f10: 7265 3a0a 0a20 2020 202d 2074 6c73 3a20  re:..    - tls: 
+00016f20: 5768 6963 6820 6361 6e20 6861 7665 2074  Which can have t
+00016f30: 6865 2076 616c 7565 7320 226f 6666 222c  he values "off",
+00016f40: 2022 756e 7665 7269 6669 6564 222c 206f   "unverified", o
+00016f50: 7220 226f 6e22 2069 6e20 7468 6520 6473  r "on" in the ds
+00016f60: 6e2c 0a20 2020 2020 2020 2020 6f72 2043  n,.         or C
+00016f70: 6f6e 6e65 6374 696f 6e2e 544c 535f 4e4f  onnection.TLS_NO
+00016f80: 4e45 2c20 436f 6e6e 6563 7469 6f6e 2e54  NE, Connection.T
+00016f90: 4c53 5f55 4e56 4552 4946 4945 442c 206f  LS_UNVERIFIED, o
+00016fa0: 720a 2020 2020 2020 2020 2043 6f6e 6e65  r.         Conne
+00016fb0: 6374 696f 6e2e 544c 535f 4f4e 2061 7320  ction.TLS_ON as 
+00016fc0: 6120 6b65 7977 6f72 6420 7061 7261 6d65  a keyword parame
+00016fd0: 7465 722e 0a20 2020 202d 2068 616e 6473  ter..    - hands
+00016fe0: 6861 6b65 3a20 2243 4243 222c 2022 4743  hake: "CBC", "GC
+00016ff0: 4d22 2c20 6f72 2022 5353 4f22 2e20 2247  M", or "SSO". "G
+00017000: 434d 2220 2847 616c 6f69 7320 436f 756e  CM" (Galois Coun
+00017010: 7465 7220 4d6f 6465 2920 7368 6f75 6c64  ter Mode) should
+00017020: 2062 6520 7573 6564 206f 7665 7220 2243   be used over "C
+00017030: 4243 2220 2843 6970 6865 7220 426c 6f63  BC" (Cipher Bloc
+00017040: 6b20 4368 6169 6e69 6e67 2920 666f 7220  k Chaining) for 
+00017050: 7061 7373 776f 7264 2065 6e63 7279 7074  password encrypt
+00017060: 696f 6e2e 2022 5353 4f22 2066 6f72 2073  ion. "SSO" for s
+00017070: 696e 676c 6520 7369 676e 206f 6e2e 0a20  ingle sign on.. 
+00017080: 2020 202d 2066 6f72 6365 3a20 666f 7263     - force: forc
+00017090: 6520 7468 6520 636f 6e6e 6563 7469 6f6e  e the connection
+000170a0: 2074 6f20 7265 6d61 696e 206f 6e20 7468   to remain on th
+000170b0: 6973 2068 6f73 740a 2020 2020 2222 220a  is host.    """.
+000170c0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000170d0: 6528 6861 6e64 7368 616b 652c 2073 7472  e(handshake, str
+000170e0: 293a 0a20 2020 2020 2020 2069 6620 6861  ):.        if ha
+000170f0: 6e64 7368 616b 652e 6c6f 7765 7228 2920  ndshake.lower() 
+00017100: 3d3d 2022 6763 6d22 3a0a 2020 2020 2020  == "gcm":.      
+00017110: 2020 2020 2020 6861 6e64 7368 616b 6520        handshake 
+00017120: 3d20 436f 6e6e 6563 7469 6f6e 2e48 414e  = Connection.HAN
+00017130: 4453 4841 4b45 5f47 434d 0a20 2020 2020  DSHAKE_GCM.     
+00017140: 2020 2065 6c69 6620 6861 6e64 7368 616b     elif handshak
+00017150: 652e 6c6f 7765 7228 2920 3d3d 2022 6362  e.lower() == "cb
+00017160: 6322 3a0a 2020 2020 2020 2020 2020 2020  c":.            
+00017170: 6861 6e64 7368 616b 6520 3d20 436f 6e6e  handshake = Conn
+00017180: 6563 7469 6f6e 2e48 414e 4453 4841 4b45  ection.HANDSHAKE
+00017190: 5f43 4243 0a20 2020 2020 2020 2065 6c69  _CBC.        eli
+000171a0: 6620 6861 6e64 7368 616b 652e 6c6f 7765  f handshake.lowe
+000171b0: 7228 2920 3d3d 2022 7373 6f22 3a0a 2020  r() == "sso":.  
+000171c0: 2020 2020 2020 2020 2020 6861 6e64 7368            handsh
+000171d0: 616b 6520 3d20 436f 6e6e 6563 7469 6f6e  ake = Connection
+000171e0: 2e48 414e 4453 4841 4b45 5f53 534f 0a20  .HANDSHAKE_SSO. 
+000171f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00017200: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
+00017210: 756e 7469 6d65 4572 726f 7228 6622 556e  untimeError(f"Un
+00017220: 6b6e 6f77 6e20 4861 6e64 7368 616b 6520  known Handshake 
+00017230: 6d65 7468 6f64 207b 6861 6e64 7368 616b  method {handshak
+00017240: 657d 2229 0a0a 2020 2020 6966 2069 7369  e}")..    if isi
+00017250: 6e73 7461 6e63 6528 746c 732c 2073 7472  nstance(tls, str
+00017260: 293a 0a20 2020 2020 2020 2069 6620 746c  ):.        if tl
+00017270: 732e 6c6f 7765 7228 2920 3d3d 2022 6f6e  s.lower() == "on
+00017280: 223a 0a20 2020 2020 2020 2020 2020 2074  ":.            t
+00017290: 6c73 203d 2043 6f6e 6e65 6374 696f 6e2e  ls = Connection.
+000172a0: 544c 535f 4f4e 0a20 2020 2020 2020 2065  TLS_ON.        e
+000172b0: 6c69 6620 746c 732e 6c6f 7765 7228 2920  lif tls.lower() 
+000172c0: 3d3d 2022 756e 7665 7269 6669 6564 223a  == "unverified":
+000172d0: 0a20 2020 2020 2020 2020 2020 2074 6c73  .            tls
+000172e0: 203d 2043 6f6e 6e65 6374 696f 6e2e 544c   = Connection.TL
+000172f0: 535f 554e 5645 5249 4649 4544 0a20 2020  S_UNVERIFIED.   
+00017300: 2020 2020 2065 6c69 6620 746c 732e 6c6f       elif tls.lo
+00017310: 7765 7228 2920 3d3d 2022 6f66 6622 3a0a  wer() == "off":.
+00017320: 2020 2020 2020 2020 2020 2020 746c 7320              tls 
+00017330: 3d20 436f 6e6e 6563 7469 6f6e 2e54 4c53  = Connection.TLS
+00017340: 5f4e 4f4e 450a 2020 2020 2020 2020 656c  _NONE.        el
+00017350: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00017360: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
+00017370: 6f72 2866 2255 6e6b 6e6f 776e 2054 4c53  or(f"Unknown TLS
+00017380: 206d 6f64 6520 7b74 6c73 7d22 290a 0a20   mode {tls}").. 
+00017390: 2020 2070 6172 616d 7320 3d20 7b0a 2020     params = {.  
+000173a0: 2020 2020 2020 2275 7365 7222 3a20 7573        "user": us
+000173b0: 6572 2c0a 2020 2020 2020 2020 2270 6173  er,.        "pas
+000173c0: 7377 6f72 6422 3a20 222a 2a2a 2a2a 222c  sword": "*****",
+000173d0: 0a20 2020 2020 2020 2022 686f 7374 223a  .        "host":
+000173e0: 2068 6f73 742c 0a20 2020 2020 2020 2022   host,.        "
+000173f0: 6461 7461 6261 7365 223a 2064 6174 6162  database": datab
+00017400: 6173 652c 0a20 2020 2020 2020 2022 746c  ase,.        "tl
+00017410: 7322 3a20 746c 732c 0a20 2020 2020 2020  s": tls,.       
+00017420: 2022 6861 6e64 7368 616b 6522 3a20 6861   "handshake": ha
+00017430: 6e64 7368 616b 652c 0a20 2020 207d 0a0a  ndshake,.    }..
+00017440: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00017450: 2866 2243 6f6e 6e65 6374 207b 7061 7261  (f"Connect {para
+00017460: 6d73 7d22 290a 0a20 2020 2072 6574 7572  ms}")..    retur
+00017470: 6e20 436f 6e6e 6563 7469 6f6e 2864 736e  n Connection(dsn
+00017480: 2c20 7573 6572 2c20 7061 7373 776f 7264  , user, password
+00017490: 2c20 686f 7374 2c20 6461 7461 6261 7365  , host, database
+000174a0: 2c20 746c 732c 2068 616e 6473 6861 6b65  , tls, handshake
+000174b0: 2c20 666f 7263 652c 2063 6f6e 6669 6766  , force, configf
+000174c0: 696c 6529 0a0a 0a64 6566 205f 6375 7374  ile)...def _cust
+000174d0: 6f6d 5f74 7970 655f 746f 5f6a 736f 6e28  om_type_to_json(
+000174e0: 6f62 6a29 3a0a 2020 2020 2222 2248 656c  obj):.    """Hel
+000174f0: 7065 7220 6675 6e63 7469 6f6e 2074 6f20  per function to 
+00017500: 636f 6e76 6572 7420 7479 7065 7320 7265  convert types re
+00017510: 7475 726e 6564 2066 726f 6d20 7175 6572  turned from quer
+00017520: 6965 7320 746f 0a20 2020 204a 534f 4e20  ies to.    JSON 
+00017530: 7661 6c75 6573 2e20 2054 7970 6963 616c  values.  Typical
+00017540: 6c79 2069 6e76 6f6b 6564 2070 6173 7365  ly invoked passe
+00017550: 6420 6173 2074 6865 2060 6465 6661 756c  d as the `defaul
+00017560: 7460 2070 6172 616d 6574 6572 0a20 2020  t` parameter.   
+00017570: 2074 6f20 6a73 6f6e 2e64 756d 7073 2061   to json.dumps a
+00017580: 7320 696e 3a0a 0a20 2020 2060 6a73 6f6e  s in:..    `json
+00017590: 2e64 756d 7073 2873 6f6d 655f 726f 7773  .dumps(some_rows
+000175a0: 2c20 6465 6661 756c 743d 5f63 7573 746f  , default=_custo
+000175b0: 6d5f 7479 7065 5f74 6f5f 6a73 6f6e 2960  m_type_to_json)`
+000175c0: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
+000175d0: 6973 696e 7374 616e 6365 286f 626a 2c20  isinstance(obj, 
+000175e0: 6465 6369 6d61 6c2e 4465 6369 6d61 6c29  decimal.Decimal)
+000175f0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00017600: 2073 7472 286f 626a 290a 0a20 2020 2069   str(obj)..    i
+00017610: 6620 6973 696e 7374 616e 6365 286f 626a  f isinstance(obj
+00017620: 2c20 2864 6174 6574 696d 652e 6461 7465  , (datetime.date
+00017630: 7469 6d65 2c20 6461 7465 7469 6d65 2e64  time, datetime.d
+00017640: 6174 652c 2064 6174 6574 696d 652e 7469  ate, datetime.ti
+00017650: 6d65 2929 3a0a 2020 2020 2020 2020 7265  me)):.        re
+00017660: 7475 726e 206f 626a 2e69 736f 666f 726d  turn obj.isoform
+00017670: 6174 2829 0a0a 2020 2020 6966 2069 7369  at()..    if isi
+00017680: 6e73 7461 6e63 6528 6f62 6a2c 2062 7974  nstance(obj, byt
+00017690: 6573 293a 0a20 2020 2020 2020 2072 6574  es):.        ret
+000176a0: 7572 6e20 6c69 7374 286f 626a 290a 0a20  urn list(obj).. 
+000176b0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+000176c0: 286f 626a 2c20 2875 7569 642e 5555 4944  (obj, (uuid.UUID
+000176d0: 2c20 6970 6164 6472 6573 732e 4950 7634  , ipaddress.IPv4
+000176e0: 4164 6472 6573 732c 2069 7061 6464 7265  Address, ipaddre
+000176f0: 7373 2e49 5076 3641 6464 7265 7373 2929  ss.IPv6Address))
+00017700: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00017710: 2073 7472 286f 626a 290a 0a20 2020 2069   str(obj)..    i
+00017720: 6620 6973 696e 7374 616e 6365 286f 626a  f isinstance(obj
+00017730: 2c20 285f 5354 506f 696e 742c 205f 5354  , (_STPoint, _ST
+00017740: 4c69 6e65 7374 7269 6e67 2c20 5f53 5450  Linestring, _STP
+00017750: 6f6c 7967 6f6e 2929 3a0a 2020 2020 2020  olygon)):.      
+00017760: 2020 2320 544f 444f 2047 656f 4a53 4f4e    # TODO GeoJSON
+00017770: 3f3f 0a20 2020 2020 2020 2072 6574 7572  ??.        retur
+00017780: 6e20 7374 7228 6f62 6a29 0a0a 2020 2020  n str(obj)..    
+00017790: 7072 696e 7428 6622 7479 7065 5f74 6f5f  print(f"type_to_
+000177a0: 7374 7269 6e67 2067 6f74 2063 616c 6c65  string got calle
+000177b0: 6420 666f 7220 7479 7065 207b 7479 7065  d for type {type
+000177c0: 286f 626a 297d 2229 0a20 2020 2072 6574  (obj)}").    ret
+000177d0: 7572 6e20 6622 706c 6163 6568 6f6c 6465  urn f"placeholde
+000177e0: 7220 666f 7220 7b74 7970 6528 6f62 6a29  r for {type(obj)
+000177f0: 7d22 0a0a 0a64 6566 2061 7267 7061 7273  }"...def argpars
+00017800: 6572 2829 3a0a 2020 2020 6672 6f6d 2061  er():.    from a
+00017810: 7267 7061 7273 6520 696d 706f 7274 2041  rgparse import A
+00017820: 7267 756d 656e 7450 6172 7365 722c 2046  rgumentParser, F
+00017830: 696c 6554 7970 652c 2052 6177 4465 7363  ileType, RawDesc
+00017840: 7269 7074 696f 6e48 656c 7046 6f72 6d61  riptionHelpForma
+00017850: 7474 6572 0a0a 2020 2020 636f 6e66 6967  tter..    config
+00017860: 6669 6c65 203d 2070 6174 686c 6962 2e50  file = pathlib.P
+00017870: 6174 682e 686f 6d65 2829 202f 2022 2e70  ath.home() / ".p
+00017880: 796f 6369 656e 7422 0a0a 2020 2020 7061  yocient"..    pa
+00017890: 7273 6572 203d 2041 7267 756d 656e 7450  rser = ArgumentP
+000178a0: 6172 7365 7228 0a20 2020 2020 2020 2064  arser(.        d
+000178b0: 6573 6372 6970 7469 6f6e 3d66 2222 224f  escription=f"""O
+000178c0: 6369 656e 7420 5079 7468 6f6e 2063 6c69  cient Python cli
+000178d0: 656e 7420 7b76 6572 7369 6f6e 7d2e 0a49  ent {version}..I
+000178e0: 6e20 7468 6520 7369 6d70 6c65 7374 2063  n the simplest c
+000178f0: 6173 652c 2072 756e 2077 6974 6820 6120  ase, run with a 
+00017900: 4461 7461 2053 6f75 7263 6520 4e61 6d65  Data Source Name
+00017910: 2028 6473 6e29 2061 6e64 2061 0a71 7565   (dsn) and a.que
+00017920: 7279 2e20 2046 6f72 2065 7861 6d70 6c65  ry.  For example
+00017930: 3a0a 2020 7079 6f63 6965 6e74 206f 6369  :.  pyocient oci
+00017940: 656e 743a 2f2f 7573 6572 3a70 6173 7377  ent://user:passw
+00017950: 6f72 6440 6d79 686f 7374 3a34 3035 302f  ord@myhost:4050/
+00017960: 6d79 6462 2022 7365 6c65 6374 202a 2066  mydb "select * f
+00017970: 726f 6d20 6d79 7461 626c 6522 0a0a 4d75  rom mytable"..Mu
+00017980: 6c74 6970 6c65 2071 7565 7279 2073 7472  ltiple query str
+00017990: 696e 6773 206d 6179 2062 6520 7072 6f76  ings may be prov
+000179a0: 6964 6564 0a0a 4453 4e27 7320 6172 6520  ided..DSN's are 
+000179b0: 6f66 2074 6865 2066 6f72 6d3a 0a20 206f  of the form:.  o
+000179c0: 6369 656e 743a 2f2f 7573 6572 3a70 6173  cient://user:pas
+000179d0: 7377 6f72 6440 5b68 6f73 745d 5b3a 706f  sword@[host][:po
+000179e0: 7274 5d5b 2f64 6174 6162 6173 655d 5b3f  rt][/database][?
+000179f0: 7061 7261 6d31 3d76 616c 7565 3126 2e2e  param1=value1&..
+00017a00: 2e5d 0a0a 5375 7070 6f72 7465 6420 7061  .]..Supported pa
+00017a10: 7261 6d65 7465 7220 6172 653a 0a0a 2d20  rameter are:..- 
+00017a20: 746c 733a 2057 6869 6368 2063 616e 2068  tls: Which can h
+00017a30: 6176 6520 7468 6520 7661 6c75 6573 2022  ave the values "
+00017a40: 6f66 6622 2c20 2275 6e76 6572 6966 6965  off", "unverifie
+00017a50: 6422 2c20 6f72 2022 6f6e 220a 0a2d 2066  d", or "on"..- f
+00017a60: 6f72 6365 3a20 7472 7565 206f 7220 6661  orce: true or fa
+00017a70: 6c73 6520 746f 2066 6f72 6365 2074 6865  lse to force the
+00017a80: 2063 6f6e 6e65 6374 696f 6e20 746f 2073   connection to s
+00017a90: 7461 7920 6f6e 2074 6869 7320 7365 7276  tay on this serv
+00017aa0: 6572 0a0a 2d20 6861 6e64 7368 616b 653a  er..- handshake:
+00017ab0: 2057 6869 6368 2063 616e 2068 6176 6520   Which can have 
+00017ac0: 7468 6520 7661 6c75 6520 2263 6263 220a  the value "cbc".
+00017ad0: 0a4d 756c 7469 706c 6520 686f 7374 7320  .Multiple hosts 
+00017ae0: 6d61 7920 6265 2073 7065 6369 6669 6564  may be specified
+00017af0: 2c20 7365 7061 7261 7465 6420 6279 2061  , separated by a
+00017b00: 2063 6f6d 6d61 2c20 696e 2077 6869 6368   comma, in which
+00017b10: 2063 6173 6520 7468 650a 686f 7374 7320   case the.hosts 
+00017b20: 7769 6c6c 2062 6520 7472 6965 6420 696e  will be tried in
+00017b30: 206f 7264 6572 2020 5468 7573 2061 6e20   order  Thus an 
+00017b40: 6578 616d 706c 6520 4453 4e20 6d69 6768  example DSN migh
+00017b50: 7420 6265 0a60 6f63 6965 6e74 3a2f 2f73  t be.`ocient://s
+00017b60: 6f6d 656f 6e65 3a73 6f6d 6570 6173 7377  omeone:somepassw
+00017b70: 6f72 6440 686f 7374 312c 686f 7374 323a  ord@host1,host2:
+00017b80: 3430 3531 2f6d 7964 6260 0a0a 5768 656e  4051/mydb`..When
+00017b90: 2072 756e 6e69 6e67 2069 6e20 7468 6520   running in the 
+00017ba0: 636f 6d6d 616e 6420 6c69 6e65 2069 6e74  command line int
+00017bb0: 6572 6661 6365 2c20 7468 6520 666f 6c6c  erface, the foll
+00017bc0: 6f77 696e 6720 6578 7472 6120 636f 6d6d  owing extra comm
+00017bd0: 616e 6473 0a61 7265 2073 7570 706f 7274  ands.are support
+00017be0: 6564 3a0a 0a2d 2063 6f6e 6e65 6374 2074  ed:..- connect t
+00017bf0: 6f20 276f 6369 656e 743a 2f2f 2e2e 2e2e  o 'ocient://....
+00017c00: 2720 7573 6572 2073 6f6d 6575 7365 7220  ' user someuser 
+00017c10: 7573 696e 6720 736f 6d65 7061 7373 776f  using somepasswo
+00017c20: 7264 3b0a 0a20 2020 2077 6865 6e20 7468  rd;..    when th
+00017c30: 6520 4453 4e20 666f 6c6c 6f77 7320 7468  e DSN follows th
+00017c40: 6520 6e6f 726d 616c 2070 796f 6369 656e  e normal pyocien
+00017c50: 7420 4453 4e20 666f 726d 6174 2c20 6275  t DSN format, bu
+00017c60: 7420 7468 6520 7573 6572 6964 2061 6e64  t the userid and
+00017c70: 2070 6173 7377 6f72 6420 6d61 7920 6265   password may be
+00017c80: 2070 6173 7365 640a 2020 2020 7573 696e   passed.    usin
+00017c90: 6720 7468 6520 5553 4552 2061 6e64 2055  g the USER and U
+00017ca0: 5349 4e47 206b 6579 776f 7264 7320 2873  SING keywords (s
+00017cb0: 696d 696c 6172 2074 6f20 7468 6520 4f63  imilar to the Oc
+00017cc0: 6965 6e74 204a 4442 4320 6472 6976 6572  ient JDBC driver
+00017cd0: 292e 2020 5468 6520 4453 4e20 6d75 7374  ).  The DSN must
+00017ce0: 2062 6520 7175 6f74 6564 2e0a 0a2d 2073   be quoted...- s
+00017cf0: 6f75 7263 6520 2766 696c 6527 3b0a 0a20  ource 'file';.. 
+00017d00: 2020 2045 7865 6375 7465 2074 6865 2073     Execute the s
+00017d10: 7461 7465 6d65 6e74 7320 6672 6f6d 2074  tatements from t
+00017d20: 6865 2073 7065 6369 6669 6564 2066 696c  he specified fil
+00017d30: 652e 2020 5468 6520 6669 6c65 206e 616d  e.  The file nam
+00017d40: 6520 6d75 7374 2062 6520 7175 6f74 6564  e must be quoted
+00017d50: 2e0a 0a2d 2073 6574 2066 6f72 6d61 7420  ...- set format 
+00017d60: 7461 626c 653b 0a0a 2020 2020 5365 7420  table;..    Set 
+00017d70: 7468 6520 6f75 7470 7574 2066 6f72 6d61  the output forma
+00017d80: 7420 0a0a 2d20 7175 6974 3b0a 0a22 2222  t ..- quit;.."""
+00017d90: 2c0a 2020 2020 2020 2020 666f 726d 6174  ,.        format
+00017da0: 7465 725f 636c 6173 733d 5261 7744 6573  ter_class=RawDes
+00017db0: 6372 6970 7469 6f6e 4865 6c70 466f 726d  criptionHelpForm
+00017dc0: 6174 7465 722c 0a20 2020 2029 0a0a 2020  atter,.    )..  
+00017dd0: 2020 2320 466c 6167 7320 7468 6174 2061    # Flags that a
+00017de0: 7070 6c79 2074 6f20 626f 7468 2065 7865  pply to both exe
+00017df0: 6375 7469 6f6e 206d 6f64 6573 0a20 2020  cution modes.   
+00017e00: 206f 7574 6772 6f75 7020 3d20 7061 7273   outgroup = pars
+00017e10: 6572 2e61 6464 5f6d 7574 7561 6c6c 795f  er.add_mutually_
+00017e20: 6578 636c 7573 6976 655f 6772 6f75 7028  exclusive_group(
+00017e30: 290a 2020 2020 6f75 7467 726f 7570 2e61  ).    outgroup.a
+00017e40: 6464 5f61 7267 756d 656e 7428 222d 6f22  dd_argument("-o"
+00017e50: 2c20 222d 2d6f 7574 6669 6c65 222c 2074  , "--outfile", t
+00017e60: 7970 653d 4669 6c65 5479 7065 2822 7722  ype=FileType("w"
+00017e70: 292c 2064 6566 6175 6c74 3d22 2d22 2c20  ), default="-", 
+00017e80: 6865 6c70 3d22 4f75 7470 7574 2066 696c  help="Output fil
+00017e90: 6522 290a 2020 2020 6f75 7467 726f 7570  e").    outgroup
+00017ea0: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
+00017eb0: 6e22 2c20 222d 2d6e 6f6f 7574 222c 2061  n", "--noout", a
+00017ec0: 6374 696f 6e3d 2273 746f 7265 5f63 6f6e  ction="store_con
+00017ed0: 7374 222c 2063 6f6e 7374 3d4e 6f6e 652c  st", const=None,
+00017ee0: 2064 6573 743d 226f 7574 6669 6c65 222c   dest="outfile",
+00017ef0: 2068 656c 703d 2244 6f20 6e6f 7420 6f75   help="Do not ou
+00017f00: 7470 7574 2072 6573 756c 7473 2229 0a20  tput results"). 
+00017f10: 2020 2063 6f6e 6669 6767 726f 7570 203d     configgroup =
+00017f20: 2070 6172 7365 722e 6164 645f 6d75 7475   parser.add_mutu
+00017f30: 616c 6c79 5f65 7863 6c75 7369 7665 5f67  ally_exclusive_g
+00017f40: 726f 7570 2829 0a20 2020 2063 6f6e 6669  roup().    confi
+00017f50: 6767 726f 7570 2e61 6464 5f61 7267 756d  ggroup.add_argum
+00017f60: 656e 7428 222d 6322 2c20 222d 2d63 6f6e  ent("-c", "--con
+00017f70: 6669 6766 696c 6522 2c20 7479 7065 3d73  figfile", type=s
+00017f80: 7472 2c20 6465 6661 756c 743d 7374 7228  tr, default=str(
+00017f90: 636f 6e66 6967 6669 6c65 292c 2068 656c  configfile), hel
+00017fa0: 703d 2243 6f6e 6669 6775 7261 7469 6f6e  p="Configuration
+00017fb0: 2066 696c 6522 290a 2020 2020 636f 6e66   file").    conf
+00017fc0: 6967 6772 6f75 702e 6164 645f 6172 6775  iggroup.add_argu
+00017fd0: 6d65 6e74 2822 2d2d 6e6f 636f 6e66 6967  ment("--noconfig
+00017fe0: 222c 2061 6374 696f 6e3d 2273 746f 7265  ", action="store
+00017ff0: 5f63 6f6e 7374 222c 2063 6f6e 7374 3d4e  _const", const=N
+00018000: 6f6e 652c 2064 6573 743d 2263 6f6e 6669  one, dest="confi
+00018010: 6766 696c 6522 2c20 6865 6c70 3d22 4e6f  gfile", help="No
+00018020: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+00018030: 696c 6522 290a 2020 2020 7061 7273 6572  ile").    parser
+00018040: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
+00018050: 6922 2c20 222d 2d69 6e66 696c 6522 2c20  i", "--infile", 
+00018060: 7479 7065 3d46 696c 6554 7970 6528 2272  type=FileType("r
+00018070: 2229 2c20 6465 6661 756c 743d 4e6f 6e65  "), default=None
+00018080: 2c20 6865 6c70 3d22 496e 7075 7420 6669  , help="Input fi
+00018090: 6c65 2063 6f6e 7461 696e 696e 6720 5351  le containing SQ
+000180a0: 4c20 7374 6174 656d 656e 7473 2229 0a20  L statements"). 
+000180b0: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+000180c0: 6775 6d65 6e74 2822 2d6c 222c 2022 2d2d  gument("-l", "--
+000180d0: 6c6f 676c 6576 656c 222c 2074 7970 653d  loglevel", type=
+000180e0: 7374 722c 2064 6566 6175 6c74 3d22 6372  str, default="cr
+000180f0: 6974 6963 616c 222c 2063 686f 6963 6573  itical", choices
+00018100: 3d5b 2263 7269 7469 6361 6c22 2c20 2265  =["critical", "e
+00018110: 7272 6f72 222c 2022 7761 726e 696e 6722  rror", "warning"
+00018120: 2c20 2269 6e66 6f22 2c20 2264 6562 7567  , "info", "debug
+00018130: 225d 2c20 6865 6c70 3d22 4c6f 6767 696e  "], help="Loggin
+00018140: 6720 6c65 7665 6c2c 2064 6566 6175 6c74  g level, default
+00018150: 7320 746f 2063 7269 7469 6361 6c22 290a  s to critical").
+00018160: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
+00018170: 7267 756d 656e 7428 222d 2d6c 6f67 6669  rgument("--logfi
+00018180: 6c65 222c 2074 7970 653d 4669 6c65 5479  le", type=FileTy
+00018190: 7065 2822 6122 292c 2064 6566 6175 6c74  pe("a"), default
+000181a0: 3d73 7973 2e73 7464 6f75 742c 2068 656c  =sys.stdout, hel
+000181b0: 703d 224c 6f67 2066 696c 6522 290a 2020  p="Log file").  
+000181c0: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+000181d0: 756d 656e 7428 222d 7422 2c20 222d 2d74  ument("-t", "--t
+000181e0: 696d 6522 2c20 6163 7469 6f6e 3d22 7374  ime", action="st
+000181f0: 6f72 655f 7472 7565 222c 2068 656c 703d  ore_true", help=
+00018200: 224f 7574 7075 7420 7175 6572 7920 7469  "Output query ti
+00018210: 6d65 2229 0a20 2020 2070 6172 7365 722e  me").    parser.
+00018220: 6164 645f 6172 6775 6d65 6e74 2822 6473  add_argument("ds
+00018230: 6e22 2c20 6e61 7267 733d 223f 222c 2068  n", nargs="?", h
+00018240: 656c 703d 2244 534e 206f 6620 7468 6520  elp="DSN of the 
+00018250: 666f 726d 206f 6369 656e 743a 2f2f 7573  form ocient://us
+00018260: 6572 3a70 6173 7377 6f72 6440 5b68 6f73  er:password@[hos
+00018270: 745d 5b3a 706f 7274 5d5b 2f64 6174 6162  t][:port][/datab
+00018280: 6173 655d 5b3f 7061 7261 6d31 3d76 616c  ase][?param1=val
+00018290: 7565 3126 2e2e 2e5d 2229 0a20 2020 2070  ue1&...]").    p
+000182a0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+000182b0: 6e74 2822 7371 6c22 2c20 6e61 7267 733d  nt("sql", nargs=
+000182c0: 223f 222c 2068 656c 703d 2253 514c 2073  "?", help="SQL s
+000182d0: 7461 7465 6d65 6e74 2229 0a20 2020 2070  tatement").    p
+000182e0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+000182f0: 6e74 2822 2d2d 666f 726d 6174 222c 2022  nt("--format", "
+00018300: 2d66 222c 2074 7970 653d 7374 722c 2063  -f", type=str, c
+00018310: 686f 6963 6573 3d5b 226a 736f 6e22 2c20  hoices=["json", 
+00018320: 2274 6162 6c65 222c 2022 6373 7622 5d2c  "table", "csv"],
+00018330: 2064 6566 6175 6c74 3d22 6a73 6f6e 222c   default="json",
+00018340: 2068 656c 703d 224f 7574 7075 7420 666f   help="Output fo
+00018350: 726d 6174 2c20 6465 6661 756c 7473 2074  rmat, defaults t
+00018360: 6f20 6a73 6f6e 2229 0a20 2020 2070 6172  o json").    par
+00018370: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
+00018380: 2822 2d2d 6e6f 636f 6c6f 7222 2c20 6163  ("--nocolor", ac
+00018390: 7469 6f6e 3d22 7374 6f72 655f 7472 7565  tion="store_true
+000183a0: 222c 2068 656c 703d 2257 6865 6e20 7573  ", help="When us
+000183b0: 696e 6720 7079 6f63 6965 6e74 2069 6e74  ing pyocient int
+000183c0: 6572 6163 7469 7665 6c79 2c20 646f 206e  eractively, do n
+000183d0: 6f74 2063 6f6c 6f72 2229 0a0a 2020 2020  ot color")..    
+000183e0: 7265 7475 726e 2070 6172 7365 720a 0a0a  return parser...
+000183f0: 6465 6620 6d61 696e 2829 3a0a 2020 2020  def main():.    
+00018400: 696d 706f 7274 206a 736f 6e0a 2020 2020  import json.    
+00018410: 696d 706f 7274 2063 7376 0a20 2020 2066  import csv.    f
+00018420: 726f 6d20 7461 6275 6c61 7465 2069 6d70  rom tabulate imp
+00018430: 6f72 7420 7461 6275 6c61 7465 0a20 2020  ort tabulate.   
+00018440: 2066 726f 6d20 7079 676d 656e 7473 2e6c   from pygments.l
+00018450: 6578 6572 732e 7371 6c20 696d 706f 7274  exers.sql import
+00018460: 2053 716c 4c65 7865 720a 2020 2020 6672   SqlLexer.    fr
+00018470: 6f6d 2070 7967 6d65 6e74 732e 746f 6b65  om pygments.toke
+00018480: 6e20 696d 706f 7274 2054 6f6b 656e 0a0a  n import Token..
+00018490: 2020 2020 6172 6773 203d 2061 7267 7061      args = argpa
+000184a0: 7273 6572 2829 2e70 6172 7365 5f61 7267  rser().parse_arg
+000184b0: 7328 7379 732e 6172 6776 5b31 3a5d 290a  s(sys.argv[1:]).
+000184c0: 0a20 2020 206c 6f67 5f6c 6576 656c 203d  .    log_level =
+000184d0: 2067 6574 6174 7472 286c 6f67 6769 6e67   getattr(logging
+000184e0: 2c20 6172 6773 2e6c 6f67 6c65 7665 6c2e  , args.loglevel.
+000184f0: 7570 7065 7228 292c 204e 6f6e 6529 0a20  upper(), None). 
+00018500: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+00018510: 616e 6365 286c 6f67 5f6c 6576 656c 2c20  ance(log_level, 
+00018520: 696e 7429 3a0a 2020 2020 2020 2020 7261  int):.        ra
+00018530: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00018540: 496e 7661 6c69 6420 6c6f 6720 6c65 7665  Invalid log leve
+00018550: 6c3a 2025 7322 2025 2061 7267 732e 6c6f  l: %s" % args.lo
+00018560: 676c 6576 656c 290a 0a20 2020 206c 6f67  glevel)..    log
+00018570: 6769 6e67 2e62 6173 6963 436f 6e66 6967  ging.basicConfig
+00018580: 286c 6576 656c 3d6c 6f67 5f6c 6576 656c  (level=log_level
+00018590: 2c20 7374 7265 616d 3d61 7267 732e 6c6f  , stream=args.lo
+000185a0: 6766 696c 652c 2066 6f72 6d61 743d 225b  gfile, format="[
+000185b0: 2528 6173 6374 696d 6529 735d 5b25 286c  %(asctime)s][%(l
+000185c0: 6576 656c 6e61 6d65 2973 5d20 2528 6d65  evelname)s] %(me
+000185d0: 7373 6167 6529 7322 290a 0a20 2020 2073  ssage)s")..    s
+000185e0: 716c 5f73 746d 7420 3d20 2222 0a20 2020  ql_stmt = "".   
+000185f0: 206c 6578 6572 203d 2053 716c 4c65 7865   lexer = SqlLexe
+00018600: 7228 290a 0a20 2020 2064 6566 205f 756e  r()..    def _un
+00018610: 7175 6f74 6528 696e 7075 7429 3a0a 2020  quote(input):.  
+00018620: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00018630: 2020 556e 7175 6f74 6520 6120 7374 7269    Unquote a stri
+00018640: 6e67 2c20 7769 7468 2065 6974 6865 7220  ng, with either 
+00018650: 7369 6e67 6c65 206f 7220 646f 7562 6c65  single or double
+00018660: 2071 756f 7465 730a 2020 2020 2020 2020   quotes.        
+00018670: 2222 220a 2020 2020 2020 2020 6966 2069  """.        if i
+00018680: 6e70 7574 5b30 5d20 3d3d 2027 2227 2061  nput[0] == '"' a
+00018690: 6e64 2069 6e70 7574 5b2d 315d 203d 3d20  nd input[-1] == 
+000186a0: 2722 273a 0a20 2020 2020 2020 2020 2020  '"':.           
+000186b0: 2072 6574 7572 6e20 696e 7075 745b 313a   return input[1:
+000186c0: 2d31 5d0a 2020 2020 2020 2020 6966 2069  -1].        if i
+000186d0: 6e70 7574 5b30 5d20 3d3d 2022 2722 2061  nput[0] == "'" a
+000186e0: 6e64 2069 6e70 7574 5b2d 315d 203d 3d20  nd input[-1] == 
+000186f0: 2227 223a 0a20 2020 2020 2020 2020 2020  "'":.           
+00018700: 2072 6574 7572 6e20 696e 7075 745b 313a   return input[1:
+00018710: 2d31 5d0a 2020 2020 2020 2020 7265 7475  -1].        retu
+00018720: 726e 2069 6e70 7574 0a0a 2020 2020 6465  rn input..    de
+00018730: 6620 5f64 6f5f 6c69 6e65 2861 7267 732c  f _do_line(args,
+00018740: 2063 6f6e 6e65 6374 696f 6e2c 2074 6578   connection, tex
+00018750: 742c 2073 716c 5f73 746d 742c 2071 7565  t, sql_stmt, que
+00018760: 7279 5f66 6e29 3a0a 2020 2020 2020 2020  ry_fn):.        
+00018770: 6e65 775f 636f 6e6e 6563 7469 6f6e 203d  new_connection =
+00018780: 2063 6f6e 6e65 6374 696f 6e0a 2020 2020   connection.    
+00018790: 2020 2020 666f 7220 2874 6f6b 656e 5f74      for (token_t
+000187a0: 7970 652c 2074 6f6b 656e 5f76 616c 2920  ype, token_val) 
+000187b0: 696e 206c 6578 6572 2e67 6574 5f74 6f6b  in lexer.get_tok
+000187c0: 656e 7328 7465 7874 293a 0a20 2020 2020  ens(text):.     
+000187d0: 2020 2020 2020 2069 6620 746f 6b65 6e5f         if token_
+000187e0: 7479 7065 203d 3d20 546f 6b65 6e2e 5075  type == Token.Pu
+000187f0: 6e63 7475 6174 696f 6e20 616e 6420 746f  nctuation and to
+00018800: 6b65 6e5f 7661 6c20 3d3d 2022 3b22 3a0a  ken_val == ";":.
+00018810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018820: 6e65 775f 636f 6e6e 6563 7469 6f6e 203d  new_connection =
+00018830: 2071 7565 7279 5f66 6e28 6172 6773 2c20   query_fn(args, 
+00018840: 6e65 775f 636f 6e6e 6563 7469 6f6e 2c20  new_connection, 
+00018850: 7371 6c5f 7374 6d74 290a 2020 2020 2020  sql_stmt).      
+00018860: 2020 2020 2020 2020 2020 7371 6c5f 7374            sql_st
+00018870: 6d74 203d 2022 220a 2020 2020 2020 2020  mt = "".        
+00018880: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00018890: 2020 2020 2020 2020 2020 7371 6c5f 7374            sql_st
+000188a0: 6d74 202b 3d20 746f 6b65 6e5f 7661 6c0a  mt += token_val.
+000188b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000188c0: 2873 716c 5f73 746d 742c 206e 6577 5f63  (sql_stmt, new_c
+000188d0: 6f6e 6e65 6374 696f 6e29 0a0a 2020 2020  onnection)..    
+000188e0: 6465 6620 5f64 6f5f 7175 6572 7928 6172  def _do_query(ar
+000188f0: 6773 2c20 636f 6e6e 6563 7469 6f6e 2c20  gs, connection, 
+00018900: 7175 6572 7929 3a0a 2020 2020 2020 2020  query):.        
+00018910: 2320 4669 7273 742c 2073 6565 2069 6620  # First, see if 
+00018920: 7468 6973 2069 7320 736f 6d65 7468 696e  this is somethin
+00018930: 6720 7765 2073 686f 756c 6420 6861 6e64  g we should hand
+00018940: 6c65 2068 6572 6520 696e 2074 6865 2043  le here in the C
+00018950: 4c49 0a20 2020 2020 2020 2074 6f6b 656e  LI.        token
+00018960: 7320 3d20 5b74 6f6b 656e 2066 6f72 2028  s = [token for (
+00018970: 746f 6b65 6e5f 7479 7065 2c20 746f 6b65  token_type, toke
+00018980: 6e29 2069 6e20 6c65 7865 722e 6765 745f  n) in lexer.get_
+00018990: 746f 6b65 6e73 2871 7565 7279 2920 6966  tokens(query) if
+000189a0: 2074 6f6b 656e 5f74 7970 6520 696e 2028   token_type in (
+000189b0: 546f 6b65 6e2e 4b65 7977 6f72 642c 2054  Token.Keyword, T
+000189c0: 6f6b 656e 2e4e 616d 652c 2054 6f6b 656e  oken.Name, Token
+000189d0: 2e4c 6974 6572 616c 2e53 7472 696e 672e  .Literal.String.
+000189e0: 5379 6d62 6f6c 2c20 546f 6b65 6e2e 4c69  Symbol, Token.Li
+000189f0: 7465 7261 6c2e 5374 7269 6e67 2e53 696e  teral.String.Sin
+00018a00: 676c 6529 5d0a 0a20 2020 2020 2020 2023  gle)]..        #
+00018a10: 2063 6f6e 6e65 6374 2074 6f20 7374 6174   connect to stat
+00018a20: 656d 656e 740a 2020 2020 2020 2020 6966  ement.        if
+00018a30: 206c 656e 2874 6f6b 656e 7329 203e 2031   len(tokens) > 1
+00018a40: 2061 6e64 2074 6f6b 656e 735b 305d 2e6c   and tokens[0].l
+00018a50: 6f77 6572 2829 203d 3d20 2263 6f6e 6e65  ower() == "conne
+00018a60: 6374 2220 616e 6420 746f 6b65 6e73 5b31  ct" and tokens[1
+00018a70: 5d2e 6c6f 7765 7228 2920 3d3d 2022 746f  ].lower() == "to
+00018a80: 223a 0a20 2020 2020 2020 2020 2020 2074  ":.            t
+00018a90: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00018aa0: 2020 2020 6966 206c 656e 2874 6f6b 656e      if len(token
+00018ab0: 7329 203d 3d20 373a 0a20 2020 2020 2020  s) == 7:.       
+00018ac0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00018ad0: 746f 6b65 6e73 5b33 5d2e 6c6f 7765 7228  tokens[3].lower(
+00018ae0: 2920 213d 2022 7573 6572 2220 6f72 2074  ) != "user" or t
+00018af0: 6f6b 656e 735b 355d 2e6c 6f77 6572 2829  okens[5].lower()
+00018b00: 2021 3d20 2275 7369 6e67 223a 0a20 2020   != "using":.   
+00018b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b20: 2020 2020 2070 7269 6e74 2866 2249 6e76       print(f"Inv
+00018b30: 616c 6964 2055 5345 5220 6f72 2055 5349  alid USER or USI
+00018b40: 4e47 206b 6579 776f 7264 7320 6f6e 2043  NG keywords on C
+00018b50: 4f4e 4e45 4354 2054 4f22 290a 2020 2020  ONNECT TO").    
+00018b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b70: 2020 2020 7265 7475 726e 2063 6f6e 6e65      return conne
+00018b80: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
+00018b90: 2020 2020 2020 2020 2020 6473 6e20 3d20            dsn = 
+00018ba0: 5f75 6e71 756f 7465 2874 6f6b 656e 735b  _unquote(tokens[
+00018bb0: 325d 290a 2020 2020 2020 2020 2020 2020  2]).            
+00018bc0: 2020 2020 2020 2020 7573 6572 203d 205f          user = _
+00018bd0: 756e 7175 6f74 6528 746f 6b65 6e73 5b34  unquote(tokens[4
+00018be0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00018bf0: 2020 2020 2020 2070 6173 7377 6f72 6420         password 
+00018c00: 3d20 5f75 6e71 756f 7465 2874 6f6b 656e  = _unquote(token
+00018c10: 735b 365d 290a 2020 2020 2020 2020 2020  s[6]).          
+00018c20: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00018c30: 2063 6f6e 6e65 6374 2864 736e 2c20 7573   connect(dsn, us
+00018c40: 6572 3d75 7365 722c 2070 6173 7377 6f72  er=user, passwor
+00018c50: 643d 7061 7373 776f 7264 2c20 636f 6e66  d=password, conf
+00018c60: 6967 6669 6c65 3d61 7267 732e 636f 6e66  igfile=args.conf
+00018c70: 6967 6669 6c65 290a 2020 2020 2020 2020  igfile).        
+00018c80: 2020 2020 2020 2020 656c 6966 206c 656e          elif len
+00018c90: 2874 6f6b 656e 7329 203d 3d20 333a 0a20  (tokens) == 3:. 
+00018ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cb0: 2020 2064 736e 203d 205f 756e 7175 6f74     dsn = _unquot
+00018cc0: 6528 746f 6b65 6e73 5b32 5d29 0a20 2020  e(tokens[2]).   
+00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ce0: 2072 6574 7572 6e20 636f 6e6e 6563 7428   return connect(
+00018cf0: 6473 6e2c 2063 6f6e 6669 6766 696c 653d  dsn, configfile=
+00018d00: 6172 6773 2e63 6f6e 6669 6766 696c 6529  args.configfile)
+00018d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018d20: 2070 7269 6e74 2866 2249 6e76 616c 6964   print(f"Invalid
+00018d30: 2043 4f4e 4e45 4354 2054 4f20 7374 6174   CONNECT TO stat
+00018d40: 656d 656e 7420 7b6c 656e 2874 6f6b 656e  ement {len(token
+00018d50: 7329 7d20 7b74 6f6b 656e 737d 2229 0a20  s)} {tokens}"). 
+00018d60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00018d70: 6574 7572 6e20 636f 6e6e 6563 7469 6f6e  eturn connection
+00018d80: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00018d90: 6570 7420 5351 4c45 7863 6570 7469 6f6e  ept SQLException
+00018da0: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+00018db0: 2020 2020 2020 2070 7269 6e74 2865 290a         print(e).
+00018dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018dd0: 7265 7475 726e 2063 6f6e 6e65 6374 696f  return connectio
+00018de0: 6e0a 0a20 2020 2020 2020 2023 2073 6574  n..        # set
+00018df0: 2066 6f72 6d61 740a 2020 2020 2020 2020   format.        
+00018e00: 6966 206c 656e 2874 6f6b 656e 7329 203e  if len(tokens) >
+00018e10: 2031 2061 6e64 2074 6f6b 656e 735b 305d   1 and tokens[0]
+00018e20: 2e6c 6f77 6572 2829 203d 3d20 2273 6574  .lower() == "set
+00018e30: 2220 616e 6420 746f 6b65 6e73 5b31 5d2e  " and tokens[1].
+00018e40: 6c6f 7765 7228 2920 3d3d 2022 666f 726d  lower() == "form
+00018e50: 6174 223a 0a20 2020 2020 2020 2020 2020  at":.           
+00018e60: 206e 6577 5f66 6f72 6d61 7420 3d20 746f   new_format = to
+00018e70: 6b65 6e73 5b32 5d2e 6c6f 7765 7228 290a  kens[2].lower().
+00018e80: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00018e90: 6577 5f66 6f72 6d61 7420 696e 205b 226a  ew_format in ["j
+00018ea0: 736f 6e22 2c20 2274 6162 6c65 222c 2022  son", "table", "
+00018eb0: 6373 7622 5d3a 0a20 2020 2020 2020 2020  csv"]:.         
+00018ec0: 2020 2020 2020 2061 7267 732e 666f 726d         args.form
+00018ed0: 6174 203d 206e 6577 5f66 6f72 6d61 740a  at = new_format.
+00018ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ef0: 7072 696e 7428 224f 4b22 290a 2020 2020  print("OK").    
+00018f00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00018f10: 726e 2063 6f6e 6e65 6374 696f 6e0a 2020  rn connection.  
+00018f20: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00018f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f40: 7072 696e 7428 6622 496e 7661 6c69 6420  print(f"Invalid 
+00018f50: 6f75 7470 7574 2066 6f72 6d61 7420 7b6e  output format {n
+00018f60: 6577 5f66 6f72 6d61 747d 2229 0a20 2020  ew_format}").   
+00018f70: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00018f80: 7572 6e20 636f 6e6e 6563 7469 6f6e 0a0a  urn connection..
+00018f90: 2020 2020 2020 2020 2320 736f 7572 6365          # source
+00018fa0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00018fb0: 746f 6b65 6e73 2920 3e20 3020 616e 6420  tokens) > 0 and 
+00018fc0: 746f 6b65 6e73 5b30 5d2e 6c6f 7765 7228  tokens[0].lower(
+00018fd0: 2920 3d3d 2022 736f 7572 6365 223a 0a20  ) == "source":. 
+00018fe0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00018ff0: 6e28 746f 6b65 6e73 2920 213d 2032 3a0a  n(tokens) != 2:.
+00019000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019010: 7072 696e 7428 2249 6e76 616c 6964 2053  print("Invalid S
+00019020: 4f55 5243 4520 7374 6174 656d 656e 7422  OURCE statement"
+00019030: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00019040: 2020 7265 7475 726e 2063 6f6e 6e65 6374    return connect
+00019050: 696f 6e0a 0a20 2020 2020 2020 2020 2020  ion..           
+00019060: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00019070: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+00019080: 5f75 6e71 756f 7465 2874 6f6b 656e 735b  _unquote(tokens[
+00019090: 315d 292c 206d 6f64 653d 2272 2229 2061  1]), mode="r") a
+000190a0: 7320 663a 0a20 2020 2020 2020 2020 2020  s f:.           
+000190b0: 2020 2020 2020 2020 2028 7371 6c5f 7374           (sql_st
+000190c0: 6d74 2c20 636f 6e6e 6563 7469 6f6e 2920  mt, connection) 
+000190d0: 3d20 5f64 6f5f 6c69 6e65 2861 7267 732c  = _do_line(args,
+000190e0: 2063 6f6e 6e65 6374 696f 6e2c 2066 2e72   connection, f.r
+000190f0: 6561 6428 292c 2022 222c 205f 646f 5f71  ead(), "", _do_q
+00019100: 7565 7279 290a 2020 2020 2020 2020 2020  uery).          
+00019110: 2020 2020 2020 6966 206c 656e 2873 716c        if len(sql
+00019120: 5f73 746d 742e 7374 7269 7028 2929 3a0a  _stmt.strip()):.
+00019130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019140: 2020 2020 636f 6e6e 6563 7469 6f6e 203d      connection =
+00019150: 205f 646f 5f71 7565 7279 2861 7267 732c   _do_query(args,
+00019160: 2063 6f6e 6e65 6374 696f 6e2c 2073 716c   connection, sql
+00019170: 5f73 746d 7429 0a20 2020 2020 2020 2020  _stmt).         
+00019180: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
+00019190: 6e6e 6563 7469 6f6e 0a20 2020 2020 2020  nnection.       
+000191a0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+000191b0: 7074 696f 6e20 6173 2065 3a0a 2020 2020  ption as e:.    
+000191c0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000191d0: 7428 6529 0a20 2020 2020 2020 2020 2020  t(e).           
+000191e0: 2020 2020 2072 6574 7572 6e20 636f 6e6e       return conn
+000191f0: 6563 7469 6f6e 0a0a 2020 2020 2020 2020  ection..        
+00019200: 2320 7175 6974 0a20 2020 2020 2020 2069  # quit.        i
+00019210: 6620 6c65 6e28 746f 6b65 6e73 2920 3e20  f len(tokens) > 
+00019220: 3020 616e 6420 746f 6b65 6e73 5b30 5d2e  0 and tokens[0].
+00019230: 6c6f 7765 7228 2920 3d3d 2022 7175 6974  lower() == "quit
+00019240: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
+00019250: 7973 2e65 7869 7428 3029 0a0a 2020 2020  ys.exit(0)..    
+00019260: 2020 2020 6966 2063 6f6e 6e65 6374 696f      if connectio
+00019270: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+00019280: 2020 2020 2020 2070 7269 6e74 2866 224e         print(f"N
+00019290: 6f20 6163 7469 7665 2063 6f6e 6e65 6374  o active connect
+000192a0: 696f 6e22 290a 2020 2020 2020 2020 2020  ion").          
+000192b0: 2020 7265 7475 726e 2063 6f6e 6e65 6374    return connect
+000192c0: 696f 6e0a 0a20 2020 2020 2020 2023 204f  ion..        # O
+000192d0: 4b2c 2069 6620 7765 2066 616c 6c20 7468  K, if we fall th
+000192e0: 726f 7567 6820 746f 2068 6572 652c 2068  rough to here, h
+000192f0: 6176 6520 7468 6520 6e6f 726d 616c 206c  ave the normal l
+00019300: 6962 7261 7279 2068 616e 646c 6520 6974  ibrary handle it
+00019310: 0a20 2020 2020 2020 2069 6620 6172 6773  .        if args
+00019320: 2e74 696d 653a 0a20 2020 2020 2020 2020  .time:.         
+00019330: 2020 2073 7461 7274 7469 6d65 203d 2074     starttime = t
+00019340: 696d 655f 6e73 2829 0a0a 2020 2020 2020  ime_ns()..      
+00019350: 2020 6375 7273 6f72 203d 2063 6f6e 6e65    cursor = conne
+00019360: 6374 696f 6e2e 6375 7273 6f72 2829 0a0a  ction.cursor()..
+00019370: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00019380: 2020 2020 2020 2020 2063 7572 736f 722e           cursor.
+00019390: 6578 6563 7574 6528 7175 6572 7929 0a0a  execute(query)..
+000193a0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+000193b0: 7572 736f 722e 6465 7363 7269 7074 696f  ursor.descriptio
+000193c0: 6e20 616e 6420 6e6f 7420 6375 7273 6f72  n and not cursor
+000193d0: 2e65 7870 6c61 696e 5f72 6573 756c 743a  .explain_result:
+000193e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000193f0: 2072 6573 756c 7420 3d20 6375 7273 6f72   result = cursor
+00019400: 2e66 6574 6368 616c 6c28 290a 2020 2020  .fetchall().    
+00019410: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00019420: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00019430: 7375 6c74 203d 2063 7572 736f 722e 636f  sult = cursor.co
+00019440: 6e6e 6563 7469 6f6e 0a20 2020 2020 2020  nnection.       
+00019450: 2065 7863 6570 7420 5351 4c45 7863 6570   except SQLExcep
+00019460: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+00019470: 2020 2020 2020 2070 7269 6e74 2865 290a         print(e).
+00019480: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00019490: 726e 2063 7572 736f 722e 636f 6e6e 6563  rn cursor.connec
+000194a0: 7469 6f6e 0a20 2020 2020 2020 2065 7863  tion.        exc
+000194b0: 6570 7420 4b65 7962 6f61 7264 496e 7465  ept KeyboardInte
+000194c0: 7272 7570 743a 0a20 2020 2020 2020 2020  rrupt:.         
+000194d0: 2020 2070 7269 6e74 2822 4f70 6572 6174     print("Operat
+000194e0: 696f 6e20 696e 7465 7272 7570 7465 642e  ion interrupted.
+000194f0: 2229 0a20 2020 2020 2020 2020 2020 2063  ").            c
+00019500: 7572 5f63 6f6e 6e20 3d20 6375 7273 6f72  ur_conn = cursor
+00019510: 2e63 6f6e 6e65 6374 696f 6e0a 2020 2020  .connection.    
+00019520: 2020 2020 2020 2020 6375 725f 636f 6e6e          cur_conn
+00019530: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+00019540: 2020 2020 2072 6574 7572 6e20 436f 6e6e       return Conn
+00019550: 6563 7469 6f6e 280a 2020 2020 2020 2020  ection(.        
+00019560: 2020 2020 2020 2020 7573 6572 3d63 7572          user=cur
+00019570: 5f63 6f6e 6e2e 7573 6572 2c0a 2020 2020  _conn.user,.    
+00019580: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00019590: 776f 7264 3d63 7572 5f63 6f6e 6e2e 7061  word=cur_conn.pa
+000195a0: 7373 776f 7264 2c0a 2020 2020 2020 2020  ssword,.        
+000195b0: 2020 2020 2020 2020 686f 7374 3d22 2c22          host=","
+000195c0: 2e6a 6f69 6e28 6375 725f 636f 6e6e 2e68  .join(cur_conn.h
+000195d0: 6f73 7473 292c 0a20 2020 2020 2020 2020  osts),.         
+000195e0: 2020 2020 2020 2064 6174 6162 6173 653d         database=
+000195f0: 6375 725f 636f 6e6e 2e64 6174 6162 6173  cur_conn.databas
+00019600: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00019610: 2020 2074 6c73 3d63 7572 5f63 6f6e 6e2e     tls=cur_conn.
+00019620: 746c 732c 0a20 2020 2020 2020 2020 2020  tls,.           
+00019630: 2020 2020 2068 616e 6473 6861 6b65 3d63       handshake=c
+00019640: 7572 5f63 6f6e 6e2e 6861 6e64 7368 616b  ur_conn.handshak
+00019650: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00019660: 2020 2066 6f72 6365 3d63 7572 5f63 6f6e     force=cur_con
+00019670: 6e2e 666f 7263 652c 0a20 2020 2020 2020  n.force,.       
+00019680: 2020 2020 2020 2020 2073 6573 7369 6f6e           session
+00019690: 3d63 7572 5f63 6f6e 6e2e 7365 7373 696f  =cur_conn.sessio
+000196a0: 6e2c 0a20 2020 2020 2020 2020 2020 2029  n,.            )
+000196b0: 0a0a 2020 2020 2020 2020 6966 2061 7267  ..        if arg
+000196c0: 732e 7469 6d65 3a0a 2020 2020 2020 2020  s.time:.        
+000196d0: 2020 2020 656e 6474 696d 6520 3d20 7469      endtime = ti
+000196e0: 6d65 5f6e 7328 290a 0a20 2020 2020 2020  me_ns()..       
+000196f0: 2069 6620 6375 7273 6f72 2e64 6573 6372   if cursor.descr
+00019700: 6970 7469 6f6e 2069 7320 4e6f 6e65 3a0a  iption is None:.
+00019710: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00019720: 7428 224f 4b22 290a 0a20 2020 2020 2020  t("OK")..       
+00019730: 2065 6c69 6620 6172 6773 2e6f 7574 6669   elif args.outfi
+00019740: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  le is not None:.
+00019750: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00019760: 6375 7273 6f72 2e65 7870 6c61 696e 5f72  cursor.explain_r
+00019770: 6573 756c 743a 0a20 2020 2020 2020 2020  esult:.         
+00019780: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00019790: 5b7b 2265 7870 6c61 696e 223a 206a 736f  [{"explain": jso
+000197a0: 6e2e 6c6f 6164 7328 6375 7273 6f72 2e65  n.loads(cursor.e
+000197b0: 7870 6c61 696e 5f72 6573 756c 7429 7d5d  xplain_result)}]
+000197c0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000197d0: 2020 7072 696e 7428 6a73 6f6e 2e64 756d    print(json.dum
+000197e0: 7073 2872 6573 756c 742c 2069 6e64 656e  ps(result, inden
+000197f0: 743d 342c 2064 6566 6175 6c74 3d5f 6375  t=4, default=_cu
+00019800: 7374 6f6d 5f74 7970 655f 746f 5f6a 736f  stom_type_to_jso
+00019810: 6e29 2c20 6669 6c65 3d61 7267 732e 6f75  n), file=args.ou
+00019820: 7466 696c 6529 0a20 2020 2020 2020 2020  tfile).         
+00019830: 2020 2065 6c69 6620 7265 7375 6c74 3a0a     elif result:.
+00019840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019850: 6966 2061 7267 732e 666f 726d 6174 203d  if args.format =
+00019860: 3d20 226a 736f 6e22 3a0a 2020 2020 2020  = "json":.      
+00019870: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00019880: 7375 6c74 203d 205b 726f 772e 5f61 7364  sult = [row._asd
+00019890: 6963 7428 2920 666f 7220 726f 7720 696e  ict() for row in
+000198a0: 2072 6573 756c 745d 0a0a 2020 2020 2020   result]..      
+000198b0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000198c0: 696e 7428 6a73 6f6e 2e64 756d 7073 2872  int(json.dumps(r
+000198d0: 6573 756c 742c 2069 6e64 656e 743d 342c  esult, indent=4,
+000198e0: 2064 6566 6175 6c74 3d5f 6375 7374 6f6d   default=_custom
+000198f0: 5f74 7970 655f 746f 5f6a 736f 6e29 2c20  _type_to_json), 
+00019900: 6669 6c65 3d61 7267 732e 6f75 7466 696c  file=args.outfil
+00019910: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00019920: 2020 2065 6c69 6620 6172 6773 2e66 6f72     elif args.for
+00019930: 6d61 7420 3d3d 2022 7461 626c 6522 3a0a  mat == "table":.
+00019940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019950: 2020 2020 7072 696e 7428 7461 6275 6c61      print(tabula
+00019960: 7465 2872 6573 756c 742c 2068 6561 6465  te(result, heade
+00019970: 7273 3d5b 635b 305d 2066 6f72 2063 2069  rs=[c[0] for c i
+00019980: 6e20 6375 7273 6f72 2e64 6573 6372 6970  n cursor.descrip
+00019990: 7469 6f6e 5d2c 2074 6162 6c65 666d 743d  tion], tablefmt=
+000199a0: 2270 7371 6c22 292c 2066 696c 653d 6172  "psql"), file=ar
+000199b0: 6773 2e6f 7574 6669 6c65 290a 2020 2020  gs.outfile).    
+000199c0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+000199d0: 2061 7267 732e 666f 726d 6174 203d 3d20   args.format == 
+000199e0: 2263 7376 223a 0a20 2020 2020 2020 2020  "csv":.         
+000199f0: 2020 2020 2020 2020 2020 2063 7376 2e77             csv.w
+00019a00: 7269 7465 7228 6172 6773 2e6f 7574 6669  riter(args.outfi
+00019a10: 6c65 2c20 7175 6f74 696e 673d 6373 762e  le, quoting=csv.
+00019a20: 5155 4f54 455f 414c 4c29 2e77 7269 7465  QUOTE_ALL).write
+00019a30: 726f 7728 5b63 5b30 5d20 666f 7220 6320  row([c[0] for c 
+00019a40: 696e 2063 7572 736f 722e 6465 7363 7269  in cursor.descri
+00019a50: 7074 696f 6e5d 290a 2020 2020 2020 2020  ption]).        
+00019a60: 2020 2020 2020 2020 2020 2020 7772 6974              writ
+00019a70: 6572 203d 2063 7376 2e77 7269 7465 7228  er = csv.writer(
+00019a80: 6172 6773 2e6f 7574 6669 6c65 290a 2020  args.outfile).  
+00019a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019aa0: 2020 666f 7220 726f 7720 696e 2072 6573    for row in res
+00019ab0: 756c 743a 0a20 2020 2020 2020 2020 2020  ult:.           
+00019ac0: 2020 2020 2020 2020 2020 2020 2077 7269               wri
+00019ad0: 7465 722e 7772 6974 6572 6f77 2872 6f77  ter.writerow(row
+00019ae0: 290a 0a20 2020 2020 2020 2069 6620 6172  )..        if ar
+00019af0: 6773 2e74 696d 653a 0a20 2020 2020 2020  gs.time:.       
+00019b00: 2020 2020 2065 6e64 7469 6d65 203d 2074       endtime = t
+00019b10: 696d 655f 6e73 2829 0a20 2020 2020 2020  ime_ns().       
+00019b20: 2020 2020 2070 7269 6e74 2866 2245 7865       print(f"Exe
+00019b30: 6375 7469 6f6e 2074 696d 653a 207b 2865  cution time: {(e
+00019b40: 6e64 7469 6d65 202d 2073 7461 7274 7469  ndtime - startti
+00019b50: 6d65 292f 3130 3030 3030 3030 3030 3a2e  me)/1000000000:.
+00019b60: 3366 7d20 7365 636f 6e64 7322 290a 2020  3f} seconds").  
+00019b70: 2020 2020 2020 2320 4966 2077 6520 646f        # If we do
+00019b80: 6e27 7420 7265 7475 726e 2074 6869 7320  n't return this 
+00019b90: 636f 6e6e 6563 7469 6f6e 2c20 7468 656e  connection, then
+00019ba0: 2077 6520 656e 6420 7570 2075 7369 6e67   we end up using
+00019bb0: 2074 6865 206f 6c64 2063 6f6e 6e65 6374   the old connect
+00019bc0: 696f 6e20 7768 6963 6820 7765 2063 6f75  ion which we cou
+00019bd0: 6c64 2068 6176 6520 6265 656e 2072 6564  ld have been red
+00019be0: 6972 6563 7465 640a 2020 2020 2020 2020  irected.        
+00019bf0: 7265 7475 726e 2063 7572 736f 722e 636f  return cursor.co
+00019c00: 6e6e 6563 7469 6f6e 0a0a 2020 2020 6465  nnection..    de
+00019c10: 6620 5f64 6f5f 7265 706c 2861 7267 732c  f _do_repl(args,
+00019c20: 2063 6f6e 6e65 6374 696f 6e29 3a0a 2020   connection):.  
+00019c30: 2020 2020 2020 6672 6f6d 2070 726f 6d70        from promp
+00019c40: 745f 746f 6f6c 6b69 7420 696d 706f 7274  t_toolkit import
+00019c50: 2050 726f 6d70 7453 6573 7369 6f6e 0a20   PromptSession. 
+00019c60: 2020 2020 2020 2066 726f 6d20 7072 6f6d         from prom
+00019c70: 7074 5f74 6f6f 6c6b 6974 2e6c 6578 6572  pt_toolkit.lexer
+00019c80: 7320 696d 706f 7274 2050 7967 6d65 6e74  s import Pygment
+00019c90: 734c 6578 6572 0a20 2020 2020 2020 2066  sLexer.        f
+00019ca0: 726f 6d20 7072 6f6d 7074 5f74 6f6f 6c6b  rom prompt_toolk
+00019cb0: 6974 2e68 6973 746f 7279 2069 6d70 6f72  it.history impor
+00019cc0: 7420 4669 6c65 4869 7374 6f72 790a 2020  t FileHistory.  
+00019cd0: 2020 2020 2020 6672 6f6d 2070 6174 686c        from pathl
+00019ce0: 6962 2069 6d70 6f72 7420 5061 7468 0a0a  ib import Path..
+00019cf0: 2020 2020 2020 2020 7371 6c5f 7374 6d74          sql_stmt
+00019d00: 203d 2022 220a 0a20 2020 2020 2020 2069   = ""..        i
+00019d10: 6620 6172 6773 2e6e 6f63 6f6c 6f72 3a0a  f args.nocolor:.
+00019d20: 2020 2020 2020 2020 2020 2020 7365 7373              sess
+00019d30: 696f 6e20 3d20 5072 6f6d 7074 5365 7373  ion = PromptSess
+00019d40: 696f 6e28 6869 7374 6f72 793d 4669 6c65  ion(history=File
+00019d50: 4869 7374 6f72 7928 7374 7228 5061 7468  History(str(Path
+00019d60: 2e68 6f6d 6528 2920 2f20 222e 7079 6f63  .home() / ".pyoc
+00019d70: 6965 6e74 5f68 6973 746f 7279 2229 2929  ient_history")))
+00019d80: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00019d90: 2020 2020 2020 2020 2020 2073 6573 7369             sessi
+00019da0: 6f6e 203d 2050 726f 6d70 7453 6573 7369  on = PromptSessi
+00019db0: 6f6e 286c 6578 6572 3d50 7967 6d65 6e74  on(lexer=Pygment
+00019dc0: 734c 6578 6572 2853 716c 4c65 7865 7229  sLexer(SqlLexer)
+00019dd0: 2c20 6869 7374 6f72 793d 4669 6c65 4869  , history=FileHi
+00019de0: 7374 6f72 7928 7374 7228 5061 7468 2e68  story(str(Path.h
+00019df0: 6f6d 6528 2920 2f20 222e 7079 6f63 6965  ome() / ".pyocie
+00019e00: 6e74 5f68 6973 746f 7279 2229 2929 0a0a  nt_history")))..
+00019e10: 2020 2020 2020 2020 6966 2063 6f6e 6e65          if conne
+00019e20: 6374 696f 6e3a 0a20 2020 2020 2020 2020  ction:.         
+00019e30: 2020 2063 7572 736f 7220 3d20 636f 6e6e     cursor = conn
+00019e40: 6563 7469 6f6e 2e63 7572 736f 7228 290a  ection.cursor().
+00019e50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00019e60: 7428 6622 4f63 6965 6e74 2044 6174 6162  t(f"Ocient Datab
+00019e70: 6173 65e2 84a2 2229 0a20 2020 2020 2020  ase...").       
+00019e80: 2020 2020 2070 7269 6e74 2866 2253 7973       print(f"Sys
+00019e90: 7465 6d20 5665 7273 696f 6e3a 207b 6375  tem Version: {cu
+00019ea0: 7273 6f72 2e67 6574 5379 7374 656d 5665  rsor.getSystemVe
+00019eb0: 7273 696f 6e28 297d 2c20 436c 6965 6e74  rsion()}, Client
+00019ec0: 2056 6572 7369 6f6e 207b 7665 7273 696f   Version {versio
+00019ed0: 6e7d 2229 0a20 2020 2020 2020 2065 6f66  n}").        eof
+00019ee0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00019ef0: 2074 6578 7420 3d20 2222 0a20 2020 2020   text = "".     
+00019f00: 2020 2077 6869 6c65 206e 6f74 2065 6f66     while not eof
+00019f10: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
+00019f20: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00019f30: 2020 2074 6578 7420 3d20 7365 7373 696f     text = sessio
+00019f40: 6e2e 7072 6f6d 7074 2822 3e20 2229 0a20  n.prompt("> "). 
+00019f50: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00019f60: 7420 4b65 7962 6f61 7264 496e 7465 7272  t KeyboardInterr
+00019f70: 7570 743a 0a20 2020 2020 2020 2020 2020  upt:.           
+00019f80: 2020 2020 2073 716c 5f73 746d 7420 3d20       sql_stmt = 
+00019f90: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
+00019fa0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+00019fb0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00019fc0: 4f46 4572 726f 723a 0a20 2020 2020 2020  OFError:.       
+00019fd0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+00019fe0: 2020 2020 2020 2020 2020 2028 7371 6c5f             (sql_
+00019ff0: 7374 6d74 2c20 636f 6e6e 6563 7469 6f6e  stmt, connection
+0001a000: 2920 3d20 5f64 6f5f 6c69 6e65 2861 7267  ) = _do_line(arg
+0001a010: 732c 2063 6f6e 6e65 6374 696f 6e2c 2074  s, connection, t
+0001a020: 6578 742c 2073 716c 5f73 746d 742c 205f  ext, sql_stmt, _
+0001a030: 646f 5f71 7565 7279 290a 0a20 2020 2020  do_query)..     
+0001a040: 2020 2069 6620 6c65 6e28 7371 6c5f 7374     if len(sql_st
+0001a050: 6d74 2e73 7472 6970 2829 293a 0a20 2020  mt.strip()):.   
+0001a060: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
+0001a070: 696f 6e20 3d20 5f64 6f5f 7175 6572 7928  ion = _do_query(
+0001a080: 6172 6773 2c20 636f 6e6e 6563 7469 6f6e  args, connection
+0001a090: 2c20 7371 6c5f 7374 6d74 290a 0a20 2020  , sql_stmt)..   
+0001a0a0: 2020 2020 2070 7269 6e74 2822 476f 6f64       print("Good
+0001a0b0: 4279 6521 2229 0a0a 2020 2020 7472 793a  Bye!")..    try:
+0001a0c0: 0a20 2020 2020 2020 2069 6620 6172 6773  .        if args
+0001a0d0: 2e64 736e 3a0a 2020 2020 2020 2020 2020  .dsn:.          
+0001a0e0: 2020 636f 6e6e 6563 7469 6f6e 203d 2063    connection = c
+0001a0f0: 6f6e 6e65 6374 2861 7267 732e 6473 6e2c  onnect(args.dsn,
+0001a100: 2063 6f6e 6669 6766 696c 653d 6172 6773   configfile=args
+0001a110: 2e63 6f6e 6669 6766 696c 6529 0a20 2020  .configfile).   
+0001a120: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001a130: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
+0001a140: 6e20 3d20 4e6f 6e65 0a0a 2020 2020 2020  n = None..      
+0001a150: 2020 6966 2061 7267 732e 7371 6c3a 0a20    if args.sql:. 
+0001a160: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
+0001a170: 6374 696f 6e20 3d20 5f64 6f5f 7175 6572  ction = _do_quer
+0001a180: 7928 6172 6773 2c20 636f 6e6e 6563 7469  y(args, connecti
+0001a190: 6f6e 2c20 6172 6773 2e73 716c 290a 2020  on, args.sql).  
+0001a1a0: 2020 2020 2020 656c 6966 2061 7267 732e        elif args.
+0001a1b0: 696e 6669 6c65 3a0a 2020 2020 2020 2020  infile:.        
+0001a1c0: 2020 2020 2873 716c 5f73 746d 742c 2063      (sql_stmt, c
+0001a1d0: 6f6e 6e65 6374 696f 6e29 203d 205f 646f  onnection) = _do
+0001a1e0: 5f6c 696e 6528 6172 6773 2c20 636f 6e6e  _line(args, conn
+0001a1f0: 6563 7469 6f6e 2c20 6172 6773 2e69 6e66  ection, args.inf
+0001a200: 696c 652e 7265 6164 2829 2c20 7371 6c5f  ile.read(), sql_
+0001a210: 7374 6d74 2c20 5f64 6f5f 7175 6572 7929  stmt, _do_query)
+0001a220: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001a230: 6c65 6e28 7371 6c5f 7374 6d74 2e73 7472  len(sql_stmt.str
+0001a240: 6970 2829 293a 0a20 2020 2020 2020 2020  ip()):.         
+0001a250: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
+0001a260: 6e20 3d20 5f64 6f5f 7175 6572 7928 6172  n = _do_query(ar
+0001a270: 6773 2c20 636f 6e6e 6563 7469 6f6e 2c20  gs, connection, 
+0001a280: 7371 6c5f 7374 6d74 290a 2020 2020 2020  sql_stmt).      
+0001a290: 2020 656c 6966 2073 7973 2e73 7464 696e    elif sys.stdin
+0001a2a0: 2e69 7361 7474 7928 293a 0a20 2020 2020  .isatty():.     
+0001a2b0: 2020 2020 2020 205f 646f 5f72 6570 6c28         _do_repl(
+0001a2c0: 6172 6773 2c20 636f 6e6e 6563 7469 6f6e  args, connection
+0001a2d0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0001a2e0: 2020 2020 2020 2020 2020 2020 2873 716c              (sql
+0001a2f0: 5f73 746d 742c 2063 6f6e 6e65 6374 696f  _stmt, connectio
+0001a300: 6e29 203d 205f 646f 5f6c 696e 6528 6172  n) = _do_line(ar
+0001a310: 6773 2c20 636f 6e6e 6563 7469 6f6e 2c20  gs, connection, 
+0001a320: 7379 732e 7374 6469 6e2e 7265 6164 2829  sys.stdin.read()
+0001a330: 2c20 7371 6c5f 7374 6d74 2c20 5f64 6f5f  , sql_stmt, _do_
+0001a340: 7175 6572 7929 0a0a 2020 2020 6578 6365  query)..    exce
+0001a350: 7074 2053 514c 4578 6365 7074 696f 6e20  pt SQLException 
+0001a360: 6173 2065 7863 3a0a 2020 2020 2020 2020  as exc:.        
+0001a370: 7072 696e 7428 6622 4572 726f 723a 207b  print(f"Error: {
+0001a380: 6578 632e 7265 6173 6f6e 7d22 2c20 6669  exc.reason}", fi
+0001a390: 6c65 3d73 7973 2e73 7464 6572 7229 0a0a  le=sys.stderr)..
+0001a3a0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
+0001a3b0: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
+0001a3c0: 6d61 696e 2829 0a                        main().
```

### Comparing `pyocient-1.0.7/setup.py` & `pyocient-1.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,74 +6,61 @@
 import pathlib
 import subprocess
 import os
 
 here = pathlib.Path(__file__).parent.absolute()
 
 # Get the long description from the README file
-long_description = (here / 'README.md').read_text(encoding='utf-8')
+long_description = (here / "README.md").read_text(encoding="utf-8")
 
-version={}
-with open(os.path.join(here, 'version.py')) as version_file:
+version = {}
+with open(os.path.join(here, "version.py")) as version_file:
     exec(version_file.read(), version)
-    version = version['__version__']
+    version = version["__version__"]
 
 setup(
-    name='pyocient',
-
+    name="pyocient",
     version=version,
-
-    description='Ocient Database Python API',
-
-    author='Ocient Inc', 
-    author_email='info@ocient.com',
-
+    description="Ocient Database Python API",
+    author="Ocient Inc",
+    author_email="info@ocient.com",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-
-    url='https://www.ocient.com/',
-
+    long_description_content_type="text/markdown",
+    url="https://www.ocient.com/",
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 3 - Alpha',
-
+        "Development Status :: 3 - Alpha",
         # Indicate who your project is intended for
-        'Topic :: Database',
-        'Topic :: Database :: Front-Ends',
-        'Topic :: Software Development',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Intended Audience :: Developers',
-
-        'License :: OSI Approved :: Apache Software License',
+        "Topic :: Database",
+        "Topic :: Database :: Front-Ends",
+        "Topic :: Software Development",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: Apache Software License",
     ],
-
-    keywords='database, sql, development',
-
+    keywords="database, sql, development",
     setup_requires=[
-        'wheel',
+        "wheel",
     ],
-
     install_requires=[
-        'dsnparse',
-        'prompt-toolkit',
-        'pygments',
-        'tabulate',
-        'cryptography<3.4',
-        'cffi<=1.14.6',
-        'google-auth<2.0dev', # because google-api-python-client doesn't provide an upper bound for this dep
-        'google-api-python-client',
+        "dsnparse",
+        "prompt-toolkit",
+        "pygments",
+        "tabulate",
+        "cryptography<=36.0",
+        "cffi<=1.15.0",
+        "google-auth<=2.6",  # because google-api-python-client doesn't provide an upper bound for this dep
+        "protobuf<=3.19.1",  # because google-api-python-client doesn't provide an upper bound for this dep
+        "google-api-python-client",
     ],
-
-    py_modules = ["pyocient", "version", "ClientWireProtocol_pb2"],
-
+    py_modules=["pyocient", "version", "ClientWireProtocol_pb2"],
     entry_points={
-        'console_scripts': [
-            'pyocient=pyocient:main',
+        "console_scripts": [
+            "pyocient=pyocient:main",
         ],
     },
-
-    python_requires='>=3.5, <4',
+    python_requires=">=3.5, <4",
 )
```

