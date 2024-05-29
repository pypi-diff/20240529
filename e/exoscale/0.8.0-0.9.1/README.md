# Comparing `tmp/exoscale-0.8.0.tar.gz` & `tmp/exoscale-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu May 11 14:44:45 2023, max compression
+gzip compressed data, last modified: Mon Apr 29 10:35:56 2024, max compression
```

## Comparing `exoscale-0.8.0.tar` & `exoscale-0.9.1.tar`

### file list

```diff
@@ -1,15 +1,9 @@
--rw-r--r--   0        0        0     8652 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/__init__.py
--rw-r--r--   0        0        0   526553 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/openapi.json
--rw-r--r--   0        0        0     4471 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/__init__.py
--rw-r--r--   0        0        0   112258 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/compute.py
--rw-r--r--   0        0        0     8501 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/dns.py
--rw-r--r--   0        0        0     4578 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/iam.py
--rw-r--r--   0        0        0     6915 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/polling.py
--rw-r--r--   0        0        0    24928 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/runstatus.py
--rw-r--r--   0        0        0    23936 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/storage.py
--rw-r--r--   0        0        0     8534 2023-05-11 14:44:45.000000 exoscale-0.8.0/exoscale/api/v2.py
--rw-r--r--   0        0        0       50 2023-05-11 14:44:45.000000 exoscale-0.8.0/.gitignore
--rw-r--r--   0        0        0      746 2023-05-11 14:44:45.000000 exoscale-0.8.0/LICENSE
--rw-r--r--   0        0        0      995 2023-05-11 14:44:45.000000 exoscale-0.8.0/README.md
--rw-r--r--   0        0        0     1474 2023-05-11 14:44:45.000000 exoscale-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2457 2023-05-11 14:44:45.000000 exoscale-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-04-29 10:35:56.000000 exoscale-0.9.1/exoscale/__init__.py
+-rw-r--r--   0        0        0   676635 2024-04-29 10:35:56.000000 exoscale-0.9.1/exoscale/openapi.json
+-rw-r--r--   0        0        0        0 2024-04-29 10:35:56.000000 exoscale-0.9.1/exoscale/api/__init__.py
+-rw-r--r--   0        0        0    10833 2024-04-29 10:35:56.000000 exoscale-0.9.1/exoscale/api/v2.py
+-rw-r--r--   0        0        0       72 2024-04-29 10:35:56.000000 exoscale-0.9.1/.gitignore
+-rw-r--r--   0        0        0      746 2024-04-29 10:35:56.000000 exoscale-0.9.1/LICENSE
+-rw-r--r--   0        0        0      643 2024-04-29 10:35:56.000000 exoscale-0.9.1/README.md
+-rw-r--r--   0        0        0     1337 2024-04-29 10:35:56.000000 exoscale-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1888 2024-04-29 10:35:56.000000 exoscale-0.9.1/PKG-INFO
```

### Comparing `exoscale-0.8.0/exoscale/openapi.json` & `exoscale-0.9.1/exoscale/openapi.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.924165824712876%*

 * *Differences: {"'components'": "{'schemas': {'dbaas-pg-pool-size': {'maximum': 10000}, 'private-network': "*

 * *                 "{'properties': {'labels': {'description': 'Resource labels'}}}, 'elastic-ip': "*

 * *                 "{'properties': {'labels': {'description': 'Resource labels'}}}, "*

 * *                 "'dbaas-pg-database-name': {'maxLength': 63}, 'dbaas-service-mysql': "*

 * *                 "{'properties': {'mysql-settings': {'$ref': "*

 * *                 "'#/components/schemas/json-schema-mysql', delete: ['type']}, 'zone' […]*

```diff
@@ -128,14 +128,167 @@
                         "maxLength": 255,
                         "minLength": 1,
                         "type": "string"
                     }
                 },
                 "type": "object"
             },
+            "block-storage-snapshot": {
+                "description": "Block storage snapshot",
+                "properties": {
+                    "block-storage-volume": {
+                        "$ref": "#/components/schemas/block-storage-volume-target",
+                        "description": "Referenced volume"
+                    },
+                    "created-at": {
+                        "description": "Snapshot creation date",
+                        "format": "date-time",
+                        "readOnly": true,
+                        "type": "string"
+                    },
+                    "id": {
+                        "description": "Snapshot ID",
+                        "format": "uuid",
+                        "readOnly": true,
+                        "type": "string"
+                    },
+                    "labels": {
+                        "$ref": "#/components/schemas/labels",
+                        "description": "Resource labels"
+                    },
+                    "name": {
+                        "description": "Snapshot name",
+                        "maxLength": 255,
+                        "minLength": 1,
+                        "type": "string"
+                    },
+                    "size": {
+                        "description": "Snapshot size",
+                        "exclusiveMinimum": false,
+                        "format": "int64",
+                        "minimum": 10,
+                        "type": "integer"
+                    },
+                    "state": {
+                        "description": "Snapshot state",
+                        "enum": [
+                            "allocated",
+                            "created",
+                            "creating",
+                            "destroyed",
+                            "destroying",
+                            "error",
+                            "partially-destroyed",
+                            "promoting"
+                        ],
+                        "readOnly": true,
+                        "type": "string"
+                    },
+                    "volume-size": {
+                        "description": "Original Volume size",
+                        "exclusiveMinimum": false,
+                        "format": "int64",
+                        "minimum": 0,
+                        "type": "integer"
+                    }
+                },
+                "type": "object"
+            },
+            "block-storage-snapshot-target": {
+                "description": "Target block storage snapshot",
+                "properties": {
+                    "id": {
+                        "description": "Block storage snapshot ID",
+                        "format": "uuid",
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
+            "block-storage-volume": {
+                "description": "Block storage volume",
+                "properties": {
+                    "block-storage-snapshots": {
+                        "description": "Volume snapshots, if any",
+                        "items": {
+                            "$ref": "#/components/schemas/block-storage-snapshot-target"
+                        },
+                        "type": "array"
+                    },
+                    "blocksize": {
+                        "description": "Volume block size",
+                        "exclusiveMinimum": false,
+                        "format": "int64",
+                        "minimum": 0,
+                        "readOnly": true,
+                        "type": "integer"
+                    },
+                    "created-at": {
+                        "description": "Volume creation date",
+                        "format": "date-time",
+                        "readOnly": true,
+                        "type": "string"
+                    },
+                    "id": {
+                        "description": "Volume ID",
+                        "format": "uuid",
+                        "readOnly": true,
+                        "type": "string"
+                    },
+                    "instance": {
+                        "$ref": "#/components/schemas/instance-target",
+                        "description": "Volume attached instance, if any"
+                    },
+                    "labels": {
+                        "$ref": "#/components/schemas/labels",
+                        "description": "Resource labels"
+                    },
+                    "name": {
+                        "description": "Volume name",
+                        "maxLength": 255,
+                        "minLength": 1,
+                        "type": "string"
+                    },
+                    "size": {
+                        "description": "Volume size",
+                        "exclusiveMinimum": false,
+                        "format": "int64",
+                        "minimum": 10,
+                        "type": "integer"
+                    },
+                    "state": {
+                        "description": "Volume state",
+                        "enum": [
+                            "attached",
+                            "attaching",
+                            "creating",
+                            "deleted",
+                            "deleting",
+                            "detached",
+                            "detaching",
+                            "error",
+                            "snapshotting"
+                        ],
+                        "readOnly": true,
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
+            "block-storage-volume-target": {
+                "description": "Target block storage volume",
+                "properties": {
+                    "id": {
+                        "description": "Block storage volume ID",
+                        "format": "uuid",
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
             "cdn-configuration": {
                 "description": "CDN configuration",
                 "properties": {
                     "bucket": {
                         "description": "CDN configuration bucket name",
                         "type": "string"
                     },
@@ -205,21 +358,26 @@
                         "exclusiveMinimum": false,
                         "format": "int64",
                         "minimum": 0,
                         "readOnly": true,
                         "type": "integer"
                     },
                     "recovery-mode": {
-                        "description": "Mechanism how backups can be restored. 'regular'\n                                            means a backup is restored as is so that the system\n                                            is restored to the state it was when the backup was generated.\n                                            'pitr' means point-in-time-recovery, which allows restoring\n                                            the system to any state since the first available full snapshot.",
+                        "description": "Mechanism how backups can be restored. 'regular'\n                                            means a backup is restored as is so that the system\n                                            is restored to the state it was when the backup was generated.\n                                            'pitr' means point-in-time-recovery, which allows restoring the system to any state since the first available full snapshot.",
                         "readOnly": true,
                         "type": "string"
                     }
                 },
                 "type": "object"
             },
+            "dbaas-database-name": {
+                "maxLength": 40,
+                "minLength": 1,
+                "type": "string"
+            },
             "dbaas-integration": {
                 "properties": {
                     "description": {
                         "description": "Description of the integration",
                         "type": "string"
                     },
                     "dest": {
@@ -446,14 +604,19 @@
                     "status": {
                         "description": "Migration status",
                         "type": "string"
                     }
                 },
                 "type": "object"
             },
+            "dbaas-mysql-database-name": {
+                "maxLength": 64,
+                "minLength": 1,
+                "type": "string"
+            },
             "dbaas-node-state": {
                 "description": "Automatic maintenance settings",
                 "properties": {
                     "name": {
                         "description": "Name of the service node",
                         "type": "string"
                     },
@@ -583,36 +746,46 @@
                         "description": "Enable to enforce index rules in a limited fashion for requests that use the _mget, _msearch, and _bulk APIs",
                         "type": "boolean"
                     }
                 },
                 "type": "object"
             },
             "dbaas-pg-database-name": {
-                "maxLength": 40,
+                "maxLength": 63,
                 "minLength": 1,
                 "type": "string"
             },
             "dbaas-pg-pool-name": {
                 "maxLength": 63,
                 "minLength": 1,
                 "type": "string"
             },
             "dbaas-pg-pool-size": {
                 "exclusiveMaximum": false,
                 "exclusiveMinimum": false,
                 "format": "int64",
-                "maximum": 1000,
+                "maximum": 10000,
                 "minimum": 1,
                 "type": "integer"
             },
             "dbaas-pg-pool-username": {
                 "maxLength": 64,
                 "minLength": 1,
                 "type": "string"
             },
+            "dbaas-pg-target-versions": {
+                "enum": [
+                    "12",
+                    "13",
+                    "14",
+                    "15",
+                    "16"
+                ],
+                "type": "string"
+            },
             "dbaas-plan": {
                 "description": "DBaaS plan",
                 "properties": {
                     "authorized": {
                         "description": "Requires authorization or publicly available",
                         "readOnly": true,
                         "type": "boolean"
@@ -787,14 +960,18 @@
                         "$ref": "#/components/schemas/dbaas-service-type-name",
                         "description": "Service type code"
                     },
                     "updated-at": {
                         "description": "Service last update timestamp (ISO 8601)",
                         "format": "date-time",
                         "type": "string"
+                    },
+                    "zone": {
+                        "description": "The zone where the service is running",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "name",
                     "plan",
                     "type"
                 ],
@@ -856,68 +1033,14 @@
                     "host",
                     "port",
                     "route",
                     "usage"
                 ],
                 "type": "object"
             },
-            "dbaas-service-connection-pools": {
-                "description": "PostgreSQL PGBouncer connection pools",
-                "properties": {
-                    "connection-uri": {
-                        "description": "Connection URI for the DB pool",
-                        "type": "string"
-                    },
-                    "database": {
-                        "description": "Service database name",
-                        "maxLength": 40,
-                        "minLength": 1,
-                        "type": "string"
-                    },
-                    "pool-mode": {
-                        "description": "PGBouncer pool mode",
-                        "enum": [
-                            "session",
-                            "statement",
-                            "transaction"
-                        ],
-                        "type": "string"
-                    },
-                    "pool-name": {
-                        "description": "Connection pool name",
-                        "maxLength": 60,
-                        "minLength": 1,
-                        "type": "string"
-                    },
-                    "pool-size": {
-                        "description": "Size of PGBouncer's PostgreSQL side connection pool",
-                        "exclusiveMaximum": false,
-                        "exclusiveMinimum": false,
-                        "format": "int64",
-                        "maximum": 1000,
-                        "minimum": 1,
-                        "type": "integer"
-                    },
-                    "username": {
-                        "description": "Pool username",
-                        "maxLength": 64,
-                        "minLength": 1,
-                        "type": "string"
-                    }
-                },
-                "required": [
-                    "connection-uri",
-                    "database",
-                    "pool-mode",
-                    "pool-name",
-                    "pool-size",
-                    "username"
-                ],
-                "type": "object"
-            },
             "dbaas-service-grafana": {
                 "properties": {
                     "backups": {
                         "description": "List of backups for the service",
                         "items": {
                             "$ref": "#/components/schemas/dbaas-service-backup"
                         },
@@ -992,16 +1115,16 @@
                         "description": "TODO UNIT disk space for data storage",
                         "exclusiveMinimum": false,
                         "format": "int64",
                         "minimum": 0,
                         "type": "integer"
                     },
                     "grafana-settings": {
-                        "description": "Grafana specific settings",
-                        "type": "object"
+                        "$ref": "#/components/schemas/json-schema-grafana",
+                        "description": "Grafana specific settings"
                     },
                     "integrations": {
                         "description": "Service integrations",
                         "items": {
                             "$ref": "#/components/schemas/dbaas-integration"
                         },
                         "type": "array"
@@ -1102,14 +1225,18 @@
                             "type": "object"
                         },
                         "type": "array"
                     },
                     "version": {
                         "description": "Grafana version",
                         "type": "string"
+                    },
+                    "zone": {
+                        "description": "The zone where the service is running",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "name",
                     "plan",
                     "type"
                 ],
@@ -1314,28 +1441,28 @@
                         "type": "array"
                     },
                     "kafka-connect-enabled": {
                         "description": "Whether Kafka Connect is enabled",
                         "type": "boolean"
                     },
                     "kafka-connect-settings": {
-                        "description": "Kafka Connect configuration values",
-                        "type": "object"
+                        "$ref": "#/components/schemas/json-schema-kafka-connect",
+                        "description": "Kafka Connect configuration values"
                     },
                     "kafka-rest-enabled": {
                         "description": "Whether Kafka REST is enabled",
                         "type": "boolean"
                     },
                     "kafka-rest-settings": {
-                        "description": "Kafka REST configuration",
-                        "type": "object"
+                        "$ref": "#/components/schemas/json-schema-kafka-rest",
+                        "description": "Kafka REST configuration"
                     },
                     "kafka-settings": {
-                        "description": "Kafka-specific settings",
-                        "type": "object"
+                        "$ref": "#/components/schemas/json-schema-kafka",
+                        "description": "Kafka-specific settings"
                     },
                     "maintenance": {
                         "$ref": "#/components/schemas/dbaas-service-maintenance",
                         "description": "Automatic maintenance settings"
                     },
                     "name": {
                         "$ref": "#/components/schemas/dbaas-service-name",
@@ -1381,16 +1508,16 @@
                         "type": "string"
                     },
                     "schema-registry-enabled": {
                         "description": "Whether Schema-Registry is enabled",
                         "type": "boolean"
                     },
                     "schema-registry-settings": {
-                        "description": "Schema Registry configuration",
-                        "type": "object"
+                        "$ref": "#/components/schemas/json-schema-schema-registry",
+                        "description": "Schema Registry configuration"
                     },
                     "state": {
                         "$ref": "#/components/schemas/enum-service-state",
                         "description": "State of the service"
                     },
                     "termination-protection": {
                         "description": "Service is protected against termination and powering off",
@@ -1440,14 +1567,18 @@
                             "type": "object"
                         },
                         "type": "array"
                     },
                     "version": {
                         "description": "Kafka version",
                         "type": "string"
+                    },
+                    "zone": {
+                        "description": "The zone where the service is running",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "name",
                     "plan",
                     "type"
                 ],
@@ -1624,14 +1755,21 @@
                         "type": "object"
                     },
                     "created-at": {
                         "description": "Service creation timestamp (ISO 8601)",
                         "format": "date-time",
                         "type": "string"
                     },
+                    "databases": {
+                        "description": "List of MySQL databases",
+                        "items": {
+                            "$ref": "#/components/schemas/dbaas-mysql-database-name"
+                        },
+                        "type": "array"
+                    },
                     "disk-size": {
                         "description": "TODO UNIT disk space for data storage",
                         "exclusiveMinimum": false,
                         "format": "int64",
                         "minimum": 0,
                         "type": "integer"
                     },
@@ -1650,16 +1788,16 @@
                         "type": "array"
                     },
                     "maintenance": {
                         "$ref": "#/components/schemas/dbaas-service-maintenance",
                         "description": "Automatic maintenance settings"
                     },
                     "mysql-settings": {
-                        "description": "MySQL-specific settings",
-                        "type": "object"
+                        "$ref": "#/components/schemas/json-schema-mysql",
+                        "description": "MySQL-specific settings"
                     },
                     "name": {
                         "$ref": "#/components/schemas/dbaas-service-name",
                         "description": "Service name"
                     },
                     "node-count": {
                         "description": "Number of service nodes in the active plan",
@@ -1745,14 +1883,18 @@
                             "type": "object"
                         },
                         "type": "array"
                     },
                     "version": {
                         "description": "MySQL version",
                         "type": "string"
+                    },
+                    "zone": {
+                        "description": "The zone where the service is running",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "name",
                     "plan",
                     "type"
                 ],
@@ -2043,16 +2185,16 @@
                                 "minimum": 5000,
                                 "type": "integer"
                             }
                         },
                         "type": "object"
                     },
                     "opensearch-settings": {
-                        "description": "OpenSearch-specific settings",
-                        "type": "object"
+                        "$ref": "#/components/schemas/json-schema-opensearch",
+                        "description": "OpenSearch-specific settings"
                     },
                     "plan": {
                         "description": "Subscription plan",
                         "type": "string"
                     },
                     "state": {
                         "$ref": "#/components/schemas/enum-service-state",
@@ -2096,14 +2238,18 @@
                             "type": "object"
                         },
                         "type": "array"
                     },
                     "version": {
                         "description": "OpenSearch version",
                         "type": "string"
+                    },
+                    "zone": {
+                        "description": "The zone where the service is running",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "name",
                     "plan",
                     "type"
                 ],
@@ -2221,15 +2367,15 @@
                         "items": {
                             "properties": {
                                 "connection-uri": {
                                     "description": "Connection URI for the DB pool",
                                     "type": "string"
                                 },
                                 "database": {
-                                    "$ref": "#/components/schemas/dbaas-pg-database-name",
+                                    "$ref": "#/components/schemas/dbaas-database-name",
                                     "description": "Service database name"
                                 },
                                 "mode": {
                                     "$ref": "#/components/schemas/enum-pg-pool-mode",
                                     "description": "PGBouncer pool mode"
                                 },
                                 "name": {
@@ -2261,15 +2407,15 @@
                         "description": "Service creation timestamp (ISO 8601)",
                         "format": "date-time",
                         "type": "string"
                     },
                     "databases": {
                         "description": "List of PostgreSQL databases",
                         "items": {
-                            "$ref": "#/components/schemas/dbaas-pg-database-name"
+                            "$ref": "#/components/schemas/dbaas-database-name"
                         },
                         "type": "array"
                     },
                     "disk-size": {
                         "description": "TODO UNIT disk space for data storage",
                         "exclusiveMinimum": false,
                         "format": "int64",
@@ -2337,24 +2483,24 @@
                         "description": "Service notifications",
                         "items": {
                             "$ref": "#/components/schemas/dbaas-service-notification"
                         },
                         "type": "array"
                     },
                     "pg-settings": {
-                        "description": "PostgreSQL-specific settings",
-                        "type": "object"
+                        "$ref": "#/components/schemas/json-schema-pg",
+                        "description": "PostgreSQL-specific settings"
                     },
                     "pgbouncer-settings": {
-                        "description": "PGBouncer connection pooling settings",
-                        "type": "object"
+                        "$ref": "#/components/schemas/json-schema-pgbouncer",
+                        "description": "PGBouncer connection pooling settings"
                     },
                     "pglookout-settings": {
-                        "description": "PGLookout settings",
-                        "type": "object"
+                        "$ref": "#/components/schemas/json-schema-pglookout",
+                        "description": "PGLookout settings"
                     },
                     "plan": {
                         "description": "Subscription plan",
                         "type": "string"
                     },
                     "shared-buffers-percentage": {
                         "description": "Percentage of total RAM that the database server uses for shared memory buffers. Valid range is 20-60 (float), which corresponds to 20% - 60%. This setting adjusts the shared_buffers configuration value.",
@@ -2374,16 +2520,16 @@
                         "description": "Synchronous replication type. Note that the service plan also needs to support synchronous replication."
                     },
                     "termination-protection": {
                         "description": "Service is protected against termination and powering off",
                         "type": "boolean"
                     },
                     "timescaledb-settings": {
-                        "description": "TimescaleDB extension configuration values",
-                        "type": "object"
+                        "$ref": "#/components/schemas/json-schema-timescaledb",
+                        "description": "TimescaleDB extension configuration values"
                     },
                     "type": {
                         "$ref": "#/components/schemas/dbaas-service-type-name",
                         "description": "Service type code"
                     },
                     "updated-at": {
                         "description": "Service last update timestamp (ISO 8601)",
@@ -2435,14 +2581,18 @@
                         "description": "Sets the maximum amount of memory to be used by a query operation (such as a sort or hash table) before writing to temporary disk files, in MB. Default is 1MB + 0.075% of total RAM (up to 32MB).",
                         "exclusiveMaximum": false,
                         "exclusiveMinimum": false,
                         "format": "int64",
                         "maximum": 1024,
                         "minimum": 1,
                         "type": "integer"
+                    },
+                    "zone": {
+                        "description": "The zone where the service is running",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "name",
                     "plan",
                     "type"
                 ],
@@ -2593,16 +2743,16 @@
                         "type": "array"
                     },
                     "plan": {
                         "description": "Subscription plan",
                         "type": "string"
                     },
                     "redis-settings": {
-                        "description": "Redis-specific settings",
-                        "type": "object"
+                        "$ref": "#/components/schemas/json-schema-redis",
+                        "description": "Redis-specific settings"
                     },
                     "state": {
                         "$ref": "#/components/schemas/enum-service-state",
                         "description": "State of the service"
                     },
                     "termination-protection": {
                         "description": "Service is protected against termination and powering off",
@@ -2671,14 +2821,18 @@
                             "type": "object"
                         },
                         "type": "array"
                     },
                     "version": {
                         "description": "Redis version",
                         "type": "string"
+                    },
+                    "zone": {
+                        "description": "The zone where the service is running",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "name",
                     "plan",
                     "type"
                 ],
@@ -2783,19 +2937,101 @@
                     },
                     "task-type": {
                         "type": "string"
                     }
                 },
                 "type": "object"
             },
+            "dbaas-user-kafka-secrets": {
+                "description": "Kafka User secrets",
+                "properties": {
+                    "access-cert": {
+                        "description": "Kafka certificate",
+                        "type": "string"
+                    },
+                    "access-cert-expiry": {
+                        "format": "date-time",
+                        "type": "string"
+                    },
+                    "access-key": {
+                        "description": "Kafka access key",
+                        "type": "string"
+                    },
+                    "password": {
+                        "description": "Kafka password",
+                        "type": "string"
+                    },
+                    "username": {
+                        "description": "Kafka username",
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
+            "dbaas-user-mysql-secrets": {
+                "description": "MySQL User secrets",
+                "properties": {
+                    "password": {
+                        "description": "MySQL password",
+                        "type": "string"
+                    },
+                    "username": {
+                        "description": "MySQL username",
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
+            "dbaas-user-opensearch-secrets": {
+                "description": "Opensearch User secrets",
+                "properties": {
+                    "password": {
+                        "description": "Opensearch password",
+                        "type": "string"
+                    },
+                    "username": {
+                        "description": "Opensearch username",
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
             "dbaas-user-password": {
                 "maxLength": 256,
                 "minLength": 8,
                 "type": "string"
             },
+            "dbaas-user-postgres-secrets": {
+                "description": "Postgres User secrets",
+                "properties": {
+                    "password": {
+                        "description": "Postgres password",
+                        "type": "string"
+                    },
+                    "username": {
+                        "description": "Postgres username",
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
+            "dbaas-user-redis-secrets": {
+                "description": "Redis User secrets",
+                "properties": {
+                    "password": {
+                        "description": "Redis password",
+                        "type": "string"
+                    },
+                    "username": {
+                        "description": "Redis username",
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
             "dbaas-user-username": {
                 "maxLength": 64,
                 "minLength": 1,
                 "type": "string"
             },
             "deploy-target": {
                 "description": "Deploy target",
@@ -2894,25 +3130,20 @@
                     "type": {
                         "description": "DNS domain record type",
                         "enum": [
                             "A",
                             "AAAA",
                             "ALIAS",
                             "CAA",
-                            "CDNSKEY",
-                            "CDS",
                             "CNAME",
-                            "DNSKEY",
-                            "DS",
                             "HINFO",
                             "MX",
                             "NAPTR",
                             "NS",
                             "POOL",
-                            "PTR",
                             "SOA",
                             "SPF",
                             "SRV",
                             "SSHFP",
                             "TXT",
                             "URL"
                         ],
@@ -2967,15 +3198,15 @@
                     "ip": {
                         "description": "Elastic IP address",
                         "readOnly": true,
                         "type": "string"
                     },
                     "labels": {
                         "$ref": "#/components/schemas/labels",
-                        "description": "Elastic IP labels"
+                        "description": "Resource labels"
                     }
                 },
                 "type": "object"
             },
             "elastic-ip-healthcheck": {
                 "description": "Elastic IP address healthcheck",
                 "properties": {
@@ -3071,16 +3302,16 @@
                     "replica"
                 ],
                 "type": "string"
             },
             "enum-integration-types": {
                 "enum": [
                     "datasource",
-                    "metrics",
-                    "read_replica"
+                    "logs",
+                    "metrics"
                 ],
                 "type": "string"
             },
             "enum-kafka-auth-method": {
                 "enum": [
                     "certificate",
                     "sasl"
@@ -3183,30 +3414,38 @@
                         "description": "Query string parameters (free form map)",
                         "type": "object"
                     },
                     "handler": {
                         "description": "Operation handler name",
                         "type": "string"
                     },
+                    "iam-api-key": {
+                        "$ref": "#/components/schemas/iam-api-key",
+                        "description": "Details about the IAM API Key"
+                    },
+                    "iam-role": {
+                        "$ref": "#/components/schemas/iam-role",
+                        "description": "Details about the IAM Role"
+                    },
                     "message": {
                         "description": "Operation message",
                         "type": "string"
                     },
                     "path-params": {
                         "description": "URI path parameters (free form map)",
                         "type": "object"
                     },
-                    "remote-addr": {
-                        "description": "Client IP address",
-                        "type": "string"
-                    },
                     "request-id": {
                         "description": "Operation unique identifier",
                         "type": "string"
                     },
+                    "source-ip": {
+                        "description": "Client IP address",
+                        "type": "string"
+                    },
                     "status": {
                         "description": "Operation HTTP status",
                         "exclusiveMinimum": true,
                         "format": "int64",
                         "minimum": 0,
                         "type": "integer"
                     },
@@ -3430,15 +3669,20 @@
                     "ipv6-address": {
                         "description": "Instance IPv6 address",
                         "readOnly": true,
                         "type": "string"
                     },
                     "labels": {
                         "$ref": "#/components/schemas/labels",
-                        "description": "Instance Labels"
+                        "description": "Resource labels"
+                    },
+                    "mac-address": {
+                        "description": "Instance MAC address",
+                        "readOnly": true,
+                        "type": "string"
                     },
                     "manager": {
                         "$ref": "#/components/schemas/manager",
                         "description": "Instance manager",
                         "readOnly": true
                     },
                     "name": {
@@ -3446,15 +3690,27 @@
                         "maxLength": 255,
                         "minLength": 1,
                         "type": "string"
                     },
                     "private-networks": {
                         "description": "Instance Private Networks",
                         "items": {
-                            "$ref": "#/components/schemas/private-network"
+                            "description": "Private Network",
+                            "properties": {
+                                "id": {
+                                    "description": "Private Network ID",
+                                    "format": "uuid",
+                                    "type": "string"
+                                },
+                                "mac-address": {
+                                    "description": "Private Network MAC address",
+                                    "type": "string"
+                                }
+                            },
+                            "type": "object"
                         },
                         "type": "array"
                     },
                     "public-ip": {
                         "description": "Instance public IPv4 address",
                         "format": "ipv4",
                         "readOnly": true,
@@ -3486,28 +3742,17 @@
                         "description": "Instance SSH Keys",
                         "items": {
                             "$ref": "#/components/schemas/ssh-key"
                         },
                         "type": "array"
                     },
                     "state": {
+                        "$ref": "#/components/schemas/instance-state",
                         "description": "Instance state",
-                        "enum": [
-                            "destroyed",
-                            "destroying",
-                            "error",
-                            "expunging",
-                            "migrating",
-                            "running",
-                            "starting",
-                            "stopped",
-                            "stopping"
-                        ],
-                        "readOnly": true,
-                        "type": "string"
+                        "readOnly": true
                     },
                     "template": {
                         "$ref": "#/components/schemas/template",
                         "description": "Instance Template"
                     },
                     "user-data": {
                         "description": "Instance Cloud-init user-data (base64 encoded)",
@@ -3654,15 +3899,16 @@
                         "description": "Instance Pool state",
                         "enum": [
                             "creating",
                             "destroying",
                             "running",
                             "scaling-down",
                             "scaling-up",
-                            "suspended"
+                            "suspended",
+                            "updating"
                         ],
                         "readOnly": true,
                         "type": "string"
                     },
                     "template": {
                         "$ref": "#/components/schemas/template",
                         "description": "Instances template"
@@ -3671,14 +3917,39 @@
                         "description": "Instances Cloud-init user-data",
                         "minLength": 1,
                         "type": "string"
                     }
                 },
                 "type": "object"
             },
+            "instance-state": {
+                "enum": [
+                    "destroyed",
+                    "destroying",
+                    "error",
+                    "expunging",
+                    "migrating",
+                    "running",
+                    "starting",
+                    "stopped",
+                    "stopping"
+                ],
+                "type": "string"
+            },
+            "instance-target": {
+                "description": "Target Instance",
+                "properties": {
+                    "id": {
+                        "description": "Instance ID",
+                        "format": "uuid",
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
             "instance-type": {
                 "description": "Compute instance type",
                 "properties": {
                     "authorized": {
                         "description": "Requires authorization or publicly available",
                         "readOnly": true,
                         "type": "boolean"
@@ -3753,14 +4024,2527 @@
                         },
                         "readOnly": true,
                         "type": "array"
                     }
                 },
                 "type": "object"
             },
+            "json-schema-grafana": {
+                "properties": {
+                    "alerting_enabled": {
+                        "example": true,
+                        "title": "Enable or disable Grafana legacy alerting functionality. This should not be enabled with unified_alerting_enabled.",
+                        "type": "boolean"
+                    },
+                    "alerting_error_or_timeout": {
+                        "enum": [
+                            "alerting",
+                            "keep_state"
+                        ],
+                        "example": "alerting",
+                        "title": "Default error or timeout setting for new alerting rules",
+                        "type": "string"
+                    },
+                    "alerting_max_annotations_to_keep": {
+                        "example": 0,
+                        "maximum": 1000000,
+                        "minimum": 0,
+                        "title": "Max number of alert annotations that Grafana stores. 0 (default) keeps all alert annotations.",
+                        "type": "integer"
+                    },
+                    "alerting_nodata_or_nullvalues": {
+                        "enum": [
+                            "alerting",
+                            "keep_state",
+                            "no_data",
+                            "ok"
+                        ],
+                        "example": "ok",
+                        "title": "Default value for 'no data or null values' for new alerting rules",
+                        "type": "string"
+                    },
+                    "allow_embedding": {
+                        "example": false,
+                        "title": "Allow embedding Grafana dashboards with iframe/frame/object/embed tags. Disabled by default to limit impact of clickjacking",
+                        "type": "boolean"
+                    },
+                    "auth_azuread": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "allow_sign_up": {
+                                "example": false,
+                                "title": "Automatically sign-up users on successful sign-in",
+                                "type": "boolean"
+                            },
+                            "allowed_domains": {
+                                "items": {
+                                    "example": "mycompany.com",
+                                    "maxLength": 255,
+                                    "title": "Allowed domain",
+                                    "type": "string"
+                                },
+                                "maxItems": 50,
+                                "title": "Allowed domains",
+                                "type": "array"
+                            },
+                            "allowed_groups": {
+                                "items": {
+                                    "example": "c0ffee15-c01d-0000-1111-012345abcdef",
+                                    "maxLength": 36,
+                                    "pattern": "^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$",
+                                    "title": "Group Object ID from Azure AD",
+                                    "type": "string"
+                                },
+                                "maxItems": 50,
+                                "title": "Require users to belong to one of given groups",
+                                "type": "array"
+                            },
+                            "auth_url": {
+                                "example": "https://login.microsoftonline.com/<AZURE_TENANT_ID>/oauth2/v2.0/authorize",
+                                "maxLength": 2048,
+                                "title": "Authorization URL",
+                                "type": "string"
+                            },
+                            "client_id": {
+                                "example": "b1ba0bf54a4c2c0a1c29",
+                                "maxLength": 1024,
+                                "pattern": "^[ -~]+$",
+                                "title": "Client ID from provider",
+                                "type": "string"
+                            },
+                            "client_secret": {
+                                "example": "bfa6gea4f129076761dcba8ce5e1e406bd83af7b",
+                                "maxLength": 1024,
+                                "pattern": "^[ -~]+$",
+                                "title": "Client secret from provider",
+                                "type": "string"
+                            },
+                            "token_url": {
+                                "example": "https://login.microsoftonline.com/<AZURE_TENANT_ID>/oauth2/v2.0/token",
+                                "maxLength": 2048,
+                                "title": "Token URL",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "client_id",
+                            "client_secret",
+                            "auth_url",
+                            "token_url"
+                        ],
+                        "title": "Azure AD OAuth integration",
+                        "type": "object"
+                    },
+                    "auth_basic_enabled": {
+                        "example": true,
+                        "title": "Enable or disable basic authentication form, used by Grafana built-in login",
+                        "type": "boolean"
+                    },
+                    "auth_generic_oauth": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "allow_sign_up": {
+                                "example": false,
+                                "title": "Automatically sign-up users on successful sign-in",
+                                "type": "boolean"
+                            },
+                            "allowed_domains": {
+                                "items": {
+                                    "example": "mycompany.com",
+                                    "maxLength": 255,
+                                    "title": "Allowed domain",
+                                    "type": "string"
+                                },
+                                "maxItems": 50,
+                                "title": "Allowed domains",
+                                "type": "array"
+                            },
+                            "allowed_organizations": {
+                                "items": {
+                                    "example": "myorg",
+                                    "maxLength": 256,
+                                    "pattern": "^[\\S]+$",
+                                    "title": "Allowed organization",
+                                    "type": "string"
+                                },
+                                "maxItems": 50,
+                                "title": "Require user to be member of one of the listed organizations",
+                                "type": "array"
+                            },
+                            "api_url": {
+                                "example": "https://yourprovider.com/api",
+                                "maxLength": 2048,
+                                "title": "API URL",
+                                "type": "string"
+                            },
+                            "auth_url": {
+                                "example": "https://yourprovider.com/oauth/authorize",
+                                "maxLength": 2048,
+                                "title": "Authorization URL",
+                                "type": "string"
+                            },
+                            "auto_login": {
+                                "example": false,
+                                "title": "Allow users to bypass the login screen and automatically log in",
+                                "type": "boolean"
+                            },
+                            "client_id": {
+                                "example": "b1ba0bf54a4c2c0a1c29",
+                                "maxLength": 1024,
+                                "pattern": "^[ -~]+$",
+                                "title": "Client ID from provider",
+                                "type": "string"
+                            },
+                            "client_secret": {
+                                "example": "bfa6gea4f129076761dcba8ce5e1e406bd83af7b",
+                                "maxLength": 1024,
+                                "pattern": "^[ -~]+$",
+                                "title": "Client secret from provider",
+                                "type": "string"
+                            },
+                            "name": {
+                                "example": "My authentication",
+                                "maxLength": 128,
+                                "pattern": "^[a-zA-Z0-9_\\- ]+$",
+                                "title": "Name of the OAuth integration",
+                                "type": "string"
+                            },
+                            "scopes": {
+                                "items": {
+                                    "example": "email",
+                                    "maxLength": 256,
+                                    "pattern": "^[\\S]+$",
+                                    "title": "OAuth scope",
+                                    "type": "string"
+                                },
+                                "maxItems": 50,
+                                "title": "OAuth scopes",
+                                "type": "array"
+                            },
+                            "token_url": {
+                                "example": "https://yourprovider.com/oauth/token",
+                                "maxLength": 2048,
+                                "title": "Token URL",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "api_url",
+                            "auth_url",
+                            "client_id",
+                            "client_secret",
+                            "token_url"
+                        ],
+                        "title": "Generic OAuth integration",
+                        "type": "object"
+                    },
+                    "auth_github": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "allow_sign_up": {
+                                "example": false,
+                                "title": "Automatically sign-up users on successful sign-in",
+                                "type": "boolean"
+                            },
+                            "allowed_organizations": {
+                                "items": {
+                                    "example": "aiven",
+                                    "maxLength": 256,
+                                    "pattern": "^[A-Za-z0-9-]+$",
+                                    "title": "Organization name",
+                                    "type": "string"
+                                },
+                                "maxItems": 50,
+                                "title": "Require users to belong to one of given organizations",
+                                "type": "array"
+                            },
+                            "client_id": {
+                                "example": "b1ba0bf54a4c2c0a1c29",
+                                "maxLength": 1024,
+                                "pattern": "^[ -~]+$",
+                                "title": "Client ID from provider",
+                                "type": "string"
+                            },
+                            "client_secret": {
+                                "example": "bfa6gea4f129076761dcba8ce5e1e406bd83af7b",
+                                "maxLength": 1024,
+                                "pattern": "^[ -~]+$",
+                                "title": "Client secret from provider",
+                                "type": "string"
+                            },
+                            "team_ids": {
+                                "items": {
+                                    "example": 150,
+                                    "maximum": 9223372036854776000,
+                                    "minimum": 1,
+                                    "title": "Team ID",
+                                    "type": "integer"
+                                },
+                                "maxItems": 50,
+                                "title": "Require users to belong to one of given team IDs",
+                                "type": "array"
+                            }
+                        },
+                        "required": [
+                            "client_id",
+                            "client_secret"
+                        ],
+                        "title": "Github Auth integration",
+                        "type": "object"
+                    },
+                    "auth_gitlab": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "allow_sign_up": {
+                                "example": false,
+                                "title": "Automatically sign-up users on successful sign-in",
+                                "type": "boolean"
+                            },
+                            "allowed_groups": {
+                                "items": {
+                                    "example": "aiven/developers",
+                                    "maxLength": 256,
+                                    "pattern": "^[a-z0-9-_/]+$",
+                                    "title": "Group or subgroup name",
+                                    "type": "string"
+                                },
+                                "maxItems": 50,
+                                "title": "Require users to belong to one of given groups",
+                                "type": "array"
+                            },
+                            "api_url": {
+                                "example": "https://gitlab.com/api/v4",
+                                "maxLength": 2048,
+                                "title": "API URL. This only needs to be set when using self hosted GitLab",
+                                "type": "string"
+                            },
+                            "auth_url": {
+                                "example": "https://gitlab.com/oauth/authorize",
+                                "maxLength": 2048,
+                                "title": "Authorization URL. This only needs to be set when using self hosted GitLab",
+                                "type": "string"
+                            },
+                            "client_id": {
+                                "example": "b1ba0bf54a4c2c0a1c29",
+                                "maxLength": 1024,
+                                "pattern": "^[ -~]+$",
+                                "title": "Client ID from provider",
+                                "type": "string"
+                            },
+                            "client_secret": {
+                                "example": "bfa6gea4f129076761dcba8ce5e1e406bd83af7b",
+                                "maxLength": 1024,
+                                "pattern": "^[ -~]+$",
+                                "title": "Client secret from provider",
+                                "type": "string"
+                            },
+                            "token_url": {
+                                "example": "https://gitlab.com/oauth/token",
+                                "maxLength": 2048,
+                                "title": "Token URL. This only needs to be set when using self hosted GitLab",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "client_id",
+                            "client_secret",
+                            "allowed_groups"
+                        ],
+                        "title": "GitLab Auth integration",
+                        "type": "object"
+                    },
+                    "auth_google": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "allow_sign_up": {
+                                "example": false,
+                                "title": "Automatically sign-up users on successful sign-in",
+                                "type": "boolean"
+                            },
+                            "allowed_domains": {
+                                "items": {
+                                    "example": "example.com",
+                                    "maxLength": 255,
+                                    "title": "Domain",
+                                    "type": "string"
+                                },
+                                "maxItems": 64,
+                                "title": "Domains allowed to sign-in to this Grafana",
+                                "type": "array"
+                            },
+                            "client_id": {
+                                "example": "b1ba0bf54a4c2c0a1c29",
+                                "maxLength": 1024,
+                                "pattern": "^[ -~]+$",
+                                "title": "Client ID from provider",
+                                "type": "string"
+                            },
+                            "client_secret": {
+                                "example": "bfa6gea4f129076761dcba8ce5e1e406bd83af7b",
+                                "maxLength": 1024,
+                                "pattern": "^[ -~]+$",
+                                "title": "Client secret from provider",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "client_id",
+                            "client_secret",
+                            "allowed_domains"
+                        ],
+                        "title": "Google Auth integration",
+                        "type": "object"
+                    },
+                    "cookie_samesite": {
+                        "enum": [
+                            "lax",
+                            "none",
+                            "strict"
+                        ],
+                        "example": "lax",
+                        "title": "Cookie SameSite attribute: 'strict' prevents sending cookie for cross-site requests, effectively disabling direct linking from other sites to Grafana. 'lax' is the default value.",
+                        "type": "string"
+                    },
+                    "dashboard_previews_enabled": {
+                        "description": "This feature is new in Grafana 9 and is quite resource intensive. It may cause low-end plans to work more slowly while the dashboard previews are rendering.",
+                        "example": false,
+                        "title": "Enable browsing of dashboards in grid (pictures) mode",
+                        "type": "boolean"
+                    },
+                    "dashboards_min_refresh_interval": {
+                        "description": "Signed sequence of decimal numbers, followed by a unit suffix (ms, s, m, h, d), e.g. 30s, 1h",
+                        "example": "5s",
+                        "maxLength": 16,
+                        "pattern": "^[0-9]+(ms|s|m|h|d)$",
+                        "title": "Minimum refresh interval",
+                        "type": "string"
+                    },
+                    "dashboards_versions_to_keep": {
+                        "example": 20,
+                        "maximum": 100,
+                        "minimum": 1,
+                        "title": "Dashboard versions to keep per dashboard",
+                        "type": "integer"
+                    },
+                    "dataproxy_send_user_header": {
+                        "example": false,
+                        "title": "Send 'X-Grafana-User' header to data source",
+                        "type": "boolean"
+                    },
+                    "dataproxy_timeout": {
+                        "example": 30,
+                        "maximum": 90,
+                        "minimum": 15,
+                        "title": "Timeout for data proxy requests in seconds",
+                        "type": "integer"
+                    },
+                    "date_formats": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "default_timezone": {
+                                "example": "Europe/Helsinki",
+                                "maxLength": 64,
+                                "pattern": "^([a-zA-Z_]+/){1,2}[a-zA-Z_-]+$|^(Etc/)?([Uu][Tt][Cc]|[Gg][Mm][Tt])([+-](\\d){1,2})?$|^([Ff][Aa][Cc][Tt][Oo][Rr][Yy])$|^([Bb][Rr][Oo][Ww][Ss][Ee][Rr])$",
+                                "title": "Default time zone for user preferences. Value 'browser' uses browser local time zone.",
+                                "type": "string"
+                            },
+                            "full_date": {
+                                "example": "YYYY MM DD",
+                                "maxLength": 128,
+                                "pattern": "^(([Hh]mm(ss)?|Mo|MM?M?M?|Do|DDDo|DD?D?D?|ddd?d?|do?|w[o|w]?|W[o|W]?|Qo?|N{1,5}|YYYYYY|YYYYY|YYYY|YY|y{2,4}|yo?|gg(ggg?)?|GG(GGG?)?|e|E|a|A|hh?|HH?|kk?|mm?|ss?|S{1,9}|x|X|zz?|ZZ?|LTS|LT|LL?L?L?|l{1,4}|[-+/T,;.: ]?)*)$",
+                                "title": "Moment.js style format string for cases where full date is shown",
+                                "type": "string"
+                            },
+                            "interval_day": {
+                                "example": "MM/DD",
+                                "maxLength": 128,
+                                "pattern": "^(([Hh]mm(ss)?|Mo|MM?M?M?|Do|DDDo|DD?D?D?|ddd?d?|do?|w[o|w]?|W[o|W]?|Qo?|N{1,5}|YYYYYY|YYYYY|YYYY|YY|y{2,4}|yo?|gg(ggg?)?|GG(GGG?)?|e|E|a|A|hh?|HH?|kk?|mm?|ss?|S{1,9}|x|X|zz?|ZZ?|LTS|LT|LL?L?L?|l{1,4}|[-+/T,;.: ]?)*)$",
+                                "title": "Moment.js style format string used when a time requiring day accuracy is shown",
+                                "type": "string"
+                            },
+                            "interval_hour": {
+                                "example": "MM/DD HH:mm",
+                                "maxLength": 128,
+                                "pattern": "^(([Hh]mm(ss)?|Mo|MM?M?M?|Do|DDDo|DD?D?D?|ddd?d?|do?|w[o|w]?|W[o|W]?|Qo?|N{1,5}|YYYYYY|YYYYY|YYYY|YY|y{2,4}|yo?|gg(ggg?)?|GG(GGG?)?|e|E|a|A|hh?|HH?|kk?|mm?|ss?|S{1,9}|x|X|zz?|ZZ?|LTS|LT|LL?L?L?|l{1,4}|[-+/T,;.: ]?)*)$",
+                                "title": "Moment.js style format string used when a time requiring hour accuracy is shown",
+                                "type": "string"
+                            },
+                            "interval_minute": {
+                                "example": "HH:mm",
+                                "maxLength": 128,
+                                "pattern": "^(([Hh]mm(ss)?|Mo|MM?M?M?|Do|DDDo|DD?D?D?|ddd?d?|do?|w[o|w]?|W[o|W]?|Qo?|N{1,5}|YYYYYY|YYYYY|YYYY|YY|y{2,4}|yo?|gg(ggg?)?|GG(GGG?)?|e|E|a|A|hh?|HH?|kk?|mm?|ss?|S{1,9}|x|X|zz?|ZZ?|LTS|LT|LL?L?L?|l{1,4}|[-+/T,;.: ]?)*)$",
+                                "title": "Moment.js style format string used when a time requiring minute accuracy is shown",
+                                "type": "string"
+                            },
+                            "interval_month": {
+                                "example": "YYYY-MM",
+                                "maxLength": 128,
+                                "pattern": "^(([Hh]mm(ss)?|Mo|MM?M?M?|Do|DDDo|DD?D?D?|ddd?d?|do?|w[o|w]?|W[o|W]?|Qo?|N{1,5}|YYYYYY|YYYYY|YYYY|YY|y{2,4}|yo?|gg(ggg?)?|GG(GGG?)?|e|E|a|A|hh?|HH?|kk?|mm?|ss?|S{1,9}|x|X|zz?|ZZ?|LTS|LT|LL?L?L?|l{1,4}|[-+/T,;.: ]?)*)$",
+                                "title": "Moment.js style format string used when a time requiring month accuracy is shown",
+                                "type": "string"
+                            },
+                            "interval_second": {
+                                "example": "HH:mm:ss",
+                                "maxLength": 128,
+                                "pattern": "^(([Hh]mm(ss)?|Mo|MM?M?M?|Do|DDDo|DD?D?D?|ddd?d?|do?|w[o|w]?|W[o|W]?|Qo?|N{1,5}|YYYYYY|YYYYY|YYYY|YY|y{2,4}|yo?|gg(ggg?)?|GG(GGG?)?|e|E|a|A|hh?|HH?|kk?|mm?|ss?|S{1,9}|x|X|zz?|ZZ?|LTS|LT|LL?L?L?|l{1,4}|[-+/T,;.: ]?)*)$",
+                                "title": "Moment.js style format string used when a time requiring second accuracy is shown",
+                                "type": "string"
+                            },
+                            "interval_year": {
+                                "example": "YYYY",
+                                "maxLength": 128,
+                                "pattern": "^(([Hh]mm(ss)?|Mo|MM?M?M?|Do|DDDo|DD?D?D?|ddd?d?|do?|w[o|w]?|W[o|W]?|Qo?|N{1,5}|YYYYYY|YYYYY|YYYY|YY|y{2,4}|yo?|gg(ggg?)?|GG(GGG?)?|e|E|a|A|hh?|HH?|kk?|mm?|ss?|S{1,9}|x|X|zz?|ZZ?|LTS|LT|LL?L?L?|l{1,4}|[-+/T,;.: ]?)*)$",
+                                "title": "Moment.js style format string used when a time requiring year accuracy is shown",
+                                "type": "string"
+                            }
+                        },
+                        "title": "Grafana date format specifications",
+                        "type": "object"
+                    },
+                    "disable_gravatar": {
+                        "example": false,
+                        "title": "Set to true to disable gravatar. Defaults to false (gravatar is enabled)",
+                        "type": "boolean"
+                    },
+                    "editors_can_admin": {
+                        "example": false,
+                        "title": "Editors can manage folders, teams and dashboards created by them",
+                        "type": "boolean"
+                    },
+                    "google_analytics_ua_id": {
+                        "example": "UA-123456-4",
+                        "maxLength": 64,
+                        "pattern": "^(G|UA|YT|MO)-[a-zA-Z0-9-]+$",
+                        "title": "Google Analytics ID",
+                        "type": "string"
+                    },
+                    "metrics_enabled": {
+                        "example": true,
+                        "title": "Enable Grafana /metrics endpoint",
+                        "type": "boolean"
+                    },
+                    "oauth_allow_insecure_email_lookup": {
+                        "example": false,
+                        "title": "Enforce user lookup based on email instead of the unique ID provided by the IdP",
+                        "type": "boolean"
+                    },
+                    "privatelink_access": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "grafana": {
+                                "example": true,
+                                "title": "Enable grafana",
+                                "type": "boolean"
+                            }
+                        },
+                        "title": "Allow access to selected service components through Privatelink",
+                        "type": "object"
+                    },
+                    "recovery_basebackup_name": {
+                        "example": "backup-20191112t091354293891z",
+                        "maxLength": 128,
+                        "pattern": "^[a-zA-Z0-9-_:.]+$",
+                        "title": "Name of the basebackup to restore in forked service",
+                        "type": "string"
+                    },
+                    "smtp_server": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "from_address": {
+                                "example": "yourgrafanauser@yourdomain.example.com",
+                                "maxLength": 319,
+                                "pattern": "^[A-Za-z0-9_\\-\\.+'&]+@(([\\da-zA-Z])([_\\w-]{0,62})\\.){0,127}(([\\da-zA-Z])[_\\w-]{0,61})?([\\da-zA-Z]\\.((xn\\-\\-[a-zA-Z\\d]+)|([a-zA-Z\\d]{2,})))$",
+                                "title": "Address used for sending emails",
+                                "type": "string"
+                            },
+                            "from_name": {
+                                "example": "Company Grafana",
+                                "maxLength": 128,
+                                "nullable": true,
+                                "pattern": "^[^\\x00-\\x1F]+$",
+                                "title": "Name used in outgoing emails, defaults to Grafana",
+                                "type": "string"
+                            },
+                            "host": {
+                                "example": "smtp.example.com",
+                                "maxLength": 255,
+                                "title": "Server hostname or IP",
+                                "type": "string"
+                            },
+                            "password": {
+                                "example": "ein0eemeev5eeth3Ahfu",
+                                "maxLength": 255,
+                                "nullable": true,
+                                "pattern": "^[^\\x00-\\x1F]+$",
+                                "title": "Password for SMTP authentication",
+                                "type": "string"
+                            },
+                            "port": {
+                                "example": 25,
+                                "maximum": 65535,
+                                "minimum": 1,
+                                "title": "SMTP server port",
+                                "type": "integer"
+                            },
+                            "skip_verify": {
+                                "example": "false",
+                                "title": "Skip verifying server certificate. Defaults to false",
+                                "type": "boolean"
+                            },
+                            "starttls_policy": {
+                                "enum": [
+                                    "MandatoryStartTLS",
+                                    "NoStartTLS",
+                                    "OpportunisticStartTLS"
+                                ],
+                                "example": "NoStartTLS",
+                                "title": "Either OpportunisticStartTLS, MandatoryStartTLS or NoStartTLS. Default is OpportunisticStartTLS.",
+                                "type": "string"
+                            },
+                            "username": {
+                                "example": "smtpuser",
+                                "maxLength": 255,
+                                "nullable": true,
+                                "pattern": "^[^\\x00-\\x1F]+$",
+                                "title": "Username for SMTP authentication",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "host",
+                            "port",
+                            "from_address"
+                        ],
+                        "title": "SMTP server settings",
+                        "type": "object"
+                    },
+                    "unified_alerting_enabled": {
+                        "example": true,
+                        "title": "Enable or disable Grafana unified alerting functionality. By default this is enabled and any legacy alerts will be migrated on upgrade to Grafana 9+. To stay on legacy alerting, set unified_alerting_enabled to false and alerting_enabled to true. See https://grafana.com/docs/grafana/latest/alerting/set-up/migrating-alerts/ for more details.",
+                        "type": "boolean"
+                    },
+                    "user_auto_assign_org": {
+                        "example": false,
+                        "title": "Auto-assign new users on signup to main organization. Defaults to false",
+                        "type": "boolean"
+                    },
+                    "user_auto_assign_org_role": {
+                        "enum": [
+                            "Admin",
+                            "Editor",
+                            "Viewer"
+                        ],
+                        "example": "Viewer",
+                        "title": "Set role for new signups. Defaults to Viewer",
+                        "type": "string"
+                    },
+                    "viewers_can_edit": {
+                        "example": false,
+                        "title": "Users with view-only permission can edit but not save dashboards",
+                        "type": "boolean"
+                    }
+                },
+                "title": "Grafana settings",
+                "type": "object"
+            },
+            "json-schema-kafka": {
+                "additionalProperties": false,
+                "default": {},
+                "properties": {
+                    "auto_create_topics_enable": {
+                        "description": "Enable auto creation of topics",
+                        "example": true,
+                        "title": "auto.create.topics.enable",
+                        "type": "boolean"
+                    },
+                    "compression_type": {
+                        "description": "Specify the final compression type for a given topic. This configuration accepts the standard compression codecs ('gzip', 'snappy', 'lz4', 'zstd'). It additionally accepts 'uncompressed' which is equivalent to no compression; and 'producer' which means retain the original compression codec set by the producer.",
+                        "enum": [
+                            "gzip",
+                            "lz4",
+                            "producer",
+                            "snappy",
+                            "uncompressed",
+                            "zstd"
+                        ],
+                        "title": "compression.type",
+                        "type": "string"
+                    },
+                    "connections_max_idle_ms": {
+                        "description": "Idle connections timeout: the server socket processor threads close the connections that idle for longer than this.",
+                        "example": 540000,
+                        "maximum": 3600000,
+                        "minimum": 1000,
+                        "title": "connections.max.idle.ms",
+                        "type": "integer"
+                    },
+                    "default_replication_factor": {
+                        "description": "Replication factor for autocreated topics",
+                        "maximum": 10,
+                        "minimum": 1,
+                        "title": "default.replication.factor",
+                        "type": "integer"
+                    },
+                    "group_initial_rebalance_delay_ms": {
+                        "description": "The amount of time, in milliseconds, the group coordinator will wait for more consumers to join a new group before performing the first rebalance. A longer delay means potentially fewer rebalances, but increases the time until processing begins. The default value for this is 3 seconds. During development and testing it might be desirable to set this to 0 in order to not delay test execution time.",
+                        "example": 3000,
+                        "maximum": 300000,
+                        "minimum": 0,
+                        "title": "group.initial.rebalance.delay.ms",
+                        "type": "integer"
+                    },
+                    "group_max_session_timeout_ms": {
+                        "description": "The maximum allowed session timeout for registered consumers. Longer timeouts give consumers more time to process messages in between heartbeats at the cost of a longer time to detect failures.",
+                        "example": 1800000,
+                        "maximum": 1800000,
+                        "minimum": 0,
+                        "title": "group.max.session.timeout.ms",
+                        "type": "integer"
+                    },
+                    "group_min_session_timeout_ms": {
+                        "description": "The minimum allowed session timeout for registered consumers. Longer timeouts give consumers more time to process messages in between heartbeats at the cost of a longer time to detect failures.",
+                        "example": 6000,
+                        "maximum": 60000,
+                        "minimum": 0,
+                        "title": "group.min.session.timeout.ms",
+                        "type": "integer"
+                    },
+                    "log-cleanup-and-compaction": {
+                        "properties": {
+                            "log_cleaner_delete_retention_ms": {
+                                "description": "How long are delete records retained?",
+                                "example": 86400000,
+                                "maximum": 315569260000,
+                                "minimum": 0,
+                                "title": "log.cleaner.delete.retention.ms",
+                                "type": "integer"
+                            },
+                            "log_cleaner_max_compaction_lag_ms": {
+                                "description": "The maximum amount of time message will remain uncompacted. Only applicable for logs that are being compacted",
+                                "maximum": 9223372036854776000,
+                                "minimum": 30000,
+                                "title": "log.cleaner.max.compaction.lag.ms",
+                                "type": "integer"
+                            },
+                            "log_cleaner_min_cleanable_ratio": {
+                                "description": "Controls log compactor frequency. Larger value means more frequent compactions but also more space wasted for logs. Consider setting log.cleaner.max.compaction.lag.ms to enforce compactions sooner, instead of setting a very high value for this option.",
+                                "example": 0.5,
+                                "maximum": 0.9,
+                                "minimum": 0.2,
+                                "title": "log.cleaner.min.cleanable.ratio",
+                                "type": "number"
+                            },
+                            "log_cleaner_min_compaction_lag_ms": {
+                                "description": "The minimum time a message will remain uncompacted in the log. Only applicable for logs that are being compacted.",
+                                "maximum": 9223372036854776000,
+                                "minimum": 0,
+                                "title": "log.cleaner.min.compaction.lag.ms",
+                                "type": "integer"
+                            },
+                            "log_cleanup_policy": {
+                                "description": "The default cleanup policy for segments beyond the retention window",
+                                "enum": [
+                                    "compact",
+                                    "compact,delete",
+                                    "delete"
+                                ],
+                                "example": "delete",
+                                "title": "log.cleanup.policy",
+                                "type": "string"
+                            }
+                        },
+                        "title": "Configure log cleaner for topic compaction",
+                        "type": "object"
+                    },
+                    "log_flush_interval_messages": {
+                        "description": "The number of messages accumulated on a log partition before messages are flushed to disk",
+                        "example": 9223372036854776000,
+                        "maximum": 9223372036854776000,
+                        "minimum": 1,
+                        "title": "log.flush.interval.messages",
+                        "type": "integer"
+                    },
+                    "log_flush_interval_ms": {
+                        "description": "The maximum time in ms that a message in any topic is kept in memory before flushed to disk. If not set, the value in log.flush.scheduler.interval.ms is used",
+                        "maximum": 9223372036854776000,
+                        "minimum": 0,
+                        "title": "log.flush.interval.ms",
+                        "type": "integer"
+                    },
+                    "log_index_interval_bytes": {
+                        "description": "The interval with which Kafka adds an entry to the offset index",
+                        "example": 4096,
+                        "maximum": 104857600,
+                        "minimum": 0,
+                        "title": "log.index.interval.bytes",
+                        "type": "integer"
+                    },
+                    "log_index_size_max_bytes": {
+                        "description": "The maximum size in bytes of the offset index",
+                        "example": 10485760,
+                        "maximum": 104857600,
+                        "minimum": 1048576,
+                        "title": "log.index.size.max.bytes",
+                        "type": "integer"
+                    },
+                    "log_local_retention_bytes": {
+                        "description": "The maximum size of local log segments that can grow for a partition before it gets eligible for deletion. If set to -2, the value of log.retention.bytes is used. The effective value should always be less than or equal to log.retention.bytes value.",
+                        "maximum": 9223372036854776000,
+                        "minimum": -2,
+                        "title": "log.local.retention.bytes",
+                        "type": "integer"
+                    },
+                    "log_local_retention_ms": {
+                        "description": "The number of milliseconds to keep the local log segments before it gets eligible for deletion. If set to -2, the value of log.retention.ms is used. The effective value should always be less than or equal to log.retention.ms value.",
+                        "maximum": 9223372036854776000,
+                        "minimum": -2,
+                        "title": "log.local.retention.ms",
+                        "type": "integer"
+                    },
+                    "log_message_downconversion_enable": {
+                        "description": "This configuration controls whether down-conversion of message formats is enabled to satisfy consume requests. ",
+                        "example": true,
+                        "title": "log.message.downconversion.enable",
+                        "type": "boolean"
+                    },
+                    "log_message_timestamp_difference_max_ms": {
+                        "description": "The maximum difference allowed between the timestamp when a broker receives a message and the timestamp specified in the message",
+                        "maximum": 9223372036854776000,
+                        "minimum": 0,
+                        "title": "log.message.timestamp.difference.max.ms",
+                        "type": "integer"
+                    },
+                    "log_message_timestamp_type": {
+                        "description": "Define whether the timestamp in the message is message create time or log append time.",
+                        "enum": [
+                            "CreateTime",
+                            "LogAppendTime"
+                        ],
+                        "title": "log.message.timestamp.type",
+                        "type": "string"
+                    },
+                    "log_preallocate": {
+                        "description": "Should pre allocate file when create new segment?",
+                        "example": false,
+                        "title": "log.preallocate",
+                        "type": "boolean"
+                    },
+                    "log_retention_bytes": {
+                        "description": "The maximum size of the log before deleting messages",
+                        "maximum": 9223372036854776000,
+                        "minimum": -1,
+                        "title": "log.retention.bytes",
+                        "type": "integer"
+                    },
+                    "log_retention_hours": {
+                        "description": "The number of hours to keep a log file before deleting it",
+                        "maximum": 2147483647,
+                        "minimum": -1,
+                        "title": "log.retention.hours",
+                        "type": "integer"
+                    },
+                    "log_retention_ms": {
+                        "description": "The number of milliseconds to keep a log file before deleting it (in milliseconds), If not set, the value in log.retention.minutes is used. If set to -1, no time limit is applied.",
+                        "maximum": 9223372036854776000,
+                        "minimum": -1,
+                        "title": "log.retention.ms",
+                        "type": "integer"
+                    },
+                    "log_roll_jitter_ms": {
+                        "description": "The maximum jitter to subtract from logRollTimeMillis (in milliseconds). If not set, the value in log.roll.jitter.hours is used",
+                        "maximum": 9223372036854776000,
+                        "minimum": 0,
+                        "title": "log.roll.jitter.ms",
+                        "type": "integer"
+                    },
+                    "log_roll_ms": {
+                        "description": "The maximum time before a new log segment is rolled out (in milliseconds).",
+                        "maximum": 9223372036854776000,
+                        "minimum": 1,
+                        "title": "log.roll.ms",
+                        "type": "integer"
+                    },
+                    "log_segment_bytes": {
+                        "description": "The maximum size of a single log file",
+                        "maximum": 1073741824,
+                        "minimum": 10485760,
+                        "title": "log.segment.bytes",
+                        "type": "integer"
+                    },
+                    "log_segment_delete_delay_ms": {
+                        "description": "The amount of time to wait before deleting a file from the filesystem",
+                        "example": 60000,
+                        "maximum": 3600000,
+                        "minimum": 0,
+                        "title": "log.segment.delete.delay.ms",
+                        "type": "integer"
+                    },
+                    "max_connections_per_ip": {
+                        "description": "The maximum number of connections allowed from each ip address (defaults to 2147483647).",
+                        "maximum": 2147483647,
+                        "minimum": 256,
+                        "title": "max.connections.per.ip",
+                        "type": "integer"
+                    },
+                    "max_incremental_fetch_session_cache_slots": {
+                        "description": "The maximum number of incremental fetch sessions that the broker will maintain.",
+                        "example": 1000,
+                        "maximum": 10000,
+                        "minimum": 1000,
+                        "title": "max.incremental.fetch.session.cache.slots",
+                        "type": "integer"
+                    },
+                    "message_max_bytes": {
+                        "description": "The maximum size of message that the server can receive.",
+                        "example": 1048588,
+                        "maximum": 100001200,
+                        "minimum": 0,
+                        "title": "message.max.bytes",
+                        "type": "integer"
+                    },
+                    "min_insync_replicas": {
+                        "description": "When a producer sets acks to 'all' (or '-1'), min.insync.replicas specifies the minimum number of replicas that must acknowledge a write for the write to be considered successful.",
+                        "example": 1,
+                        "maximum": 7,
+                        "minimum": 1,
+                        "title": "min.insync.replicas",
+                        "type": "integer"
+                    },
+                    "num_partitions": {
+                        "description": "Number of partitions for autocreated topics",
+                        "maximum": 1000,
+                        "minimum": 1,
+                        "title": "num.partitions",
+                        "type": "integer"
+                    },
+                    "offsets_retention_minutes": {
+                        "description": "Log retention window in minutes for offsets topic",
+                        "example": 10080,
+                        "maximum": 2147483647,
+                        "minimum": 1,
+                        "title": "offsets.retention.minutes",
+                        "type": "integer"
+                    },
+                    "producer_purgatory_purge_interval_requests": {
+                        "description": "The purge interval (in number of requests) of the producer request purgatory(defaults to 1000).",
+                        "maximum": 10000,
+                        "minimum": 10,
+                        "title": "producer.purgatory.purge.interval.requests",
+                        "type": "integer"
+                    },
+                    "replica_fetch_max_bytes": {
+                        "description": "The number of bytes of messages to attempt to fetch for each partition (defaults to 1048576). This is not an absolute maximum, if the first record batch in the first non-empty partition of the fetch is larger than this value, the record batch will still be returned to ensure that progress can be made.",
+                        "maximum": 104857600,
+                        "minimum": 1048576,
+                        "title": "replica.fetch.max.bytes",
+                        "type": "integer"
+                    },
+                    "replica_fetch_response_max_bytes": {
+                        "description": "Maximum bytes expected for the entire fetch response (defaults to 10485760). Records are fetched in batches, and if the first record batch in the first non-empty partition of the fetch is larger than this value, the record batch will still be returned to ensure that progress can be made. As such, this is not an absolute maximum.",
+                        "maximum": 1048576000,
+                        "minimum": 10485760,
+                        "title": "replica.fetch.response.max.bytes",
+                        "type": "integer"
+                    },
+                    "sasl_oauthbearer_expected_audience": {
+                        "description": "The (optional) comma-delimited setting for the broker to use to verify that the JWT was issued for one of the expected audiences.",
+                        "maxLength": 128,
+                        "title": "sasl.oauthbearer.expected.audience",
+                        "type": "string"
+                    },
+                    "sasl_oauthbearer_expected_issuer": {
+                        "description": "Optional setting for the broker to use to verify that the JWT was created by the expected issuer.",
+                        "maxLength": 128,
+                        "title": "sasl.oauthbearer.expected.issuer",
+                        "type": "string"
+                    },
+                    "sasl_oauthbearer_jwks_endpoint_url": {
+                        "description": "OIDC JWKS endpoint URL. By setting this the SASL SSL OAuth2/OIDC authentication is enabled. See also other options for SASL OAuth2/OIDC. ",
+                        "maxLength": 2048,
+                        "title": "sasl.oauthbearer.jwks.endpoint.url",
+                        "type": "string"
+                    },
+                    "sasl_oauthbearer_sub_claim_name": {
+                        "description": "Name of the scope from which to extract the subject claim from the JWT. Defaults to sub.",
+                        "maxLength": 128,
+                        "title": "sasl.oauthbearer.sub.claim.name",
+                        "type": "string"
+                    },
+                    "socket_request_max_bytes": {
+                        "description": "The maximum number of bytes in a socket request (defaults to 104857600).",
+                        "maximum": 209715200,
+                        "minimum": 10485760,
+                        "title": "socket.request.max.bytes",
+                        "type": "integer"
+                    },
+                    "transaction_remove_expired_transaction_cleanup_interval_ms": {
+                        "description": "The interval at which to remove transactions that have expired due to transactional.id.expiration.ms passing (defaults to 3600000 (1 hour)).",
+                        "example": 3600000,
+                        "maximum": 3600000,
+                        "minimum": 600000,
+                        "title": "transaction.remove.expired.transaction.cleanup.interval.ms",
+                        "type": "integer"
+                    },
+                    "transaction_state_log_segment_bytes": {
+                        "description": "The transaction topic segment bytes should be kept relatively small in order to facilitate faster log compaction and cache loads (defaults to 104857600 (100 mebibytes)).",
+                        "example": 104857600,
+                        "maximum": 2147483647,
+                        "minimum": 1048576,
+                        "title": "transaction.state.log.segment.bytes",
+                        "type": "integer"
+                    }
+                },
+                "title": "Kafka broker configuration values",
+                "type": "object"
+            },
+            "json-schema-kafka-connect": {
+                "additionalProperties": false,
+                "properties": {
+                    "connector_client_config_override_policy": {
+                        "description": "Defines what client configurations can be overridden by the connector. Default is None",
+                        "enum": [
+                            "All",
+                            "None"
+                        ],
+                        "title": "Client config override policy",
+                        "type": "string"
+                    },
+                    "consumer_auto_offset_reset": {
+                        "description": "What to do when there is no initial offset in Kafka or if the current offset does not exist any more on the server. Default is earliest",
+                        "enum": [
+                            "earliest",
+                            "latest"
+                        ],
+                        "title": "Consumer auto offset reset",
+                        "type": "string"
+                    },
+                    "consumer_fetch_max_bytes": {
+                        "description": "Records are fetched in batches by the consumer, and if the first record batch in the first non-empty partition of the fetch is larger than this value, the record batch will still be returned to ensure that the consumer can make progress. As such, this is not a absolute maximum.",
+                        "example": 52428800,
+                        "maximum": 104857600,
+                        "minimum": 1048576,
+                        "title": "The maximum amount of data the server should return for a fetch request",
+                        "type": "integer"
+                    },
+                    "consumer_isolation_level": {
+                        "description": "Transaction read isolation level. read_uncommitted is the default, but read_committed can be used if consume-exactly-once behavior is desired.",
+                        "enum": [
+                            "read_committed",
+                            "read_uncommitted"
+                        ],
+                        "title": "Consumer isolation level",
+                        "type": "string"
+                    },
+                    "consumer_max_partition_fetch_bytes": {
+                        "description": "Records are fetched in batches by the consumer.If the first record batch in the first non-empty partition of the fetch is larger than this limit, the batch will still be returned to ensure that the consumer can make progress. ",
+                        "example": 1048576,
+                        "maximum": 104857600,
+                        "minimum": 1048576,
+                        "title": "The maximum amount of data per-partition the server will return.",
+                        "type": "integer"
+                    },
+                    "consumer_max_poll_interval_ms": {
+                        "description": "The maximum delay in milliseconds between invocations of poll() when using consumer group management (defaults to 300000).",
+                        "example": 300000,
+                        "maximum": 2147483647,
+                        "minimum": 1,
+                        "title": "The maximum delay between polls when using consumer group management",
+                        "type": "integer"
+                    },
+                    "consumer_max_poll_records": {
+                        "description": "The maximum number of records returned in a single call to poll() (defaults to 500).",
+                        "example": 500,
+                        "maximum": 10000,
+                        "minimum": 1,
+                        "title": "The maximum number of records returned by a single poll",
+                        "type": "integer"
+                    },
+                    "offset_flush_interval_ms": {
+                        "description": "The interval at which to try committing offsets for tasks (defaults to 60000).",
+                        "example": 60000,
+                        "maximum": 100000000,
+                        "minimum": 1,
+                        "title": "The interval at which to try committing offsets for tasks",
+                        "type": "integer"
+                    },
+                    "offset_flush_timeout_ms": {
+                        "description": "Maximum number of milliseconds to wait for records to flush and partition offset data to be committed to offset storage before cancelling the process and restoring the offset data to be committed in a future attempt (defaults to 5000).",
+                        "example": 5000,
+                        "maximum": 2147483647,
+                        "minimum": 1,
+                        "title": "Offset flush timeout",
+                        "type": "integer"
+                    },
+                    "producer_batch_size": {
+                        "description": "This setting gives the upper bound of the batch size to be sent. If there are fewer than this many bytes accumulated for this partition, the producer will 'linger' for the linger.ms time waiting for more records to show up. A batch size of zero will disable batching entirely (defaults to 16384).",
+                        "example": 1024,
+                        "maximum": 5242880,
+                        "minimum": 0,
+                        "title": "The batch size in bytes the producer will attempt to collect for the same partition before publishing to broker",
+                        "type": "integer"
+                    },
+                    "producer_buffer_memory": {
+                        "description": "The total bytes of memory the producer can use to buffer records waiting to be sent to the broker (defaults to 33554432).",
+                        "example": 8388608,
+                        "maximum": 134217728,
+                        "minimum": 5242880,
+                        "title": "The total bytes of memory the producer can use to buffer records waiting to be sent to the broker",
+                        "type": "integer"
+                    },
+                    "producer_compression_type": {
+                        "description": "Specify the default compression type for producers. This configuration accepts the standard compression codecs ('gzip', 'snappy', 'lz4', 'zstd'). It additionally accepts 'none' which is the default and equivalent to no compression.",
+                        "enum": [
+                            "gzip",
+                            "lz4",
+                            "none",
+                            "snappy",
+                            "zstd"
+                        ],
+                        "title": "The default compression type for producers",
+                        "type": "string"
+                    },
+                    "producer_linger_ms": {
+                        "description": "This setting gives the upper bound on the delay for batching: once there is batch.size worth of records for a partition it will be sent immediately regardless of this setting, however if there are fewer than this many bytes accumulated for this partition the producer will 'linger' for the specified time waiting for more records to show up. Defaults to 0.",
+                        "example": 100,
+                        "maximum": 5000,
+                        "minimum": 0,
+                        "title": "Wait for up to the given delay to allow batching records together",
+                        "type": "integer"
+                    },
+                    "producer_max_request_size": {
+                        "description": "This setting will limit the number of record batches the producer will send in a single request to avoid sending huge requests.",
+                        "example": 1048576,
+                        "maximum": 67108864,
+                        "minimum": 131072,
+                        "title": "The maximum size of a request in bytes",
+                        "type": "integer"
+                    },
+                    "scheduled_rebalance_max_delay_ms": {
+                        "description": "The maximum delay that is scheduled in order to wait for the return of one or more departed workers before rebalancing and reassigning their connectors and tasks to the group. During this period the connectors and tasks of the departed workers remain unassigned.  Defaults to 5 minutes.",
+                        "example": 300000,
+                        "maximum": 600000,
+                        "minimum": 0,
+                        "title": "The maximum delay of rebalancing connector workers",
+                        "type": "integer"
+                    },
+                    "session_timeout_ms": {
+                        "description": "The timeout in milliseconds used to detect failures when using Kafka\u2019s group management facilities (defaults to 10000).",
+                        "example": 10000,
+                        "maximum": 2147483647,
+                        "minimum": 1,
+                        "title": "The timeout used to detect failures when using Kafka\u2019s group management facilities",
+                        "type": "integer"
+                    }
+                },
+                "title": "Kafka Connect configuration values",
+                "type": "object"
+            },
+            "json-schema-kafka-rest": {
+                "additionalProperties": false,
+                "properties": {
+                    "consumer_enable_auto_commit": {
+                        "default": true,
+                        "description": "If true the consumer's offset will be periodically committed to Kafka in the background",
+                        "title": "consumer.enable.auto.commit",
+                        "type": "boolean"
+                    },
+                    "consumer_request_max_bytes": {
+                        "default": 67108864,
+                        "description": "Maximum number of bytes in unencoded message keys and values by a single request",
+                        "maximum": 671088640,
+                        "minimum": 0,
+                        "title": "consumer.request.max.bytes",
+                        "type": "integer"
+                    },
+                    "consumer_request_timeout_ms": {
+                        "default": 1000,
+                        "description": "The maximum total time to wait for messages for a request if the maximum number of messages has not yet been reached",
+                        "enum": [
+                            1000,
+                            15000,
+                            30000
+                        ],
+                        "maximum": 30000,
+                        "minimum": 1000,
+                        "title": "consumer.request.timeout.ms",
+                        "type": "integer"
+                    },
+                    "producer_acks": {
+                        "default": "1",
+                        "description": "The number of acknowledgments the producer requires the leader to have received before considering a request complete. If set to 'all' or '-1', the leader will wait for the full set of in-sync replicas to acknowledge the record.",
+                        "enum": [
+                            "-1",
+                            "0",
+                            "1",
+                            "all"
+                        ],
+                        "title": "producer.acks",
+                        "type": "string"
+                    },
+                    "producer_compression_type": {
+                        "description": "Specify the default compression type for producers. This configuration accepts the standard compression codecs ('gzip', 'snappy', 'lz4', 'zstd'). It additionally accepts 'none' which is the default and equivalent to no compression.",
+                        "enum": [
+                            "gzip",
+                            "lz4",
+                            "none",
+                            "snappy",
+                            "zstd"
+                        ],
+                        "title": "producer.compression.type",
+                        "type": "string"
+                    },
+                    "producer_linger_ms": {
+                        "default": 0,
+                        "description": "Wait for up to the given delay to allow batching records together",
+                        "maximum": 5000,
+                        "minimum": 0,
+                        "title": "producer.linger.ms",
+                        "type": "integer"
+                    },
+                    "producer_max_request_size": {
+                        "default": 1048576,
+                        "description": "The maximum size of a request in bytes. Note that Kafka broker can also cap the record batch size.",
+                        "maximum": 2147483647,
+                        "minimum": 0,
+                        "title": "producer.max.request.size",
+                        "type": "integer"
+                    },
+                    "simpleconsumer_pool_size_max": {
+                        "default": 25,
+                        "description": "Maximum number of SimpleConsumers that can be instantiated per broker",
+                        "maximum": 250,
+                        "minimum": 10,
+                        "title": "simpleconsumer.pool.size.max",
+                        "type": "integer"
+                    }
+                },
+                "title": "Kafka REST configuration",
+                "type": "object"
+            },
+            "json-schema-mysql": {
+                "additionalProperties": false,
+                "properties": {
+                    "connect_timeout": {
+                        "description": "The number of seconds that the mysqld server waits for a connect packet before responding with Bad handshake",
+                        "example": 10,
+                        "maximum": 3600,
+                        "minimum": 2,
+                        "title": "connect_timeout",
+                        "type": "integer"
+                    },
+                    "default_time_zone": {
+                        "description": "Default server time zone as an offset from UTC (from -12:00 to +12:00), a time zone name, or 'SYSTEM' to use the MySQL server default.",
+                        "example": "+03:00",
+                        "maxLength": 100,
+                        "minLength": 2,
+                        "title": "default_time_zone",
+                        "type": "string"
+                    },
+                    "group_concat_max_len": {
+                        "description": "The maximum permitted result length in bytes for the GROUP_CONCAT() function.",
+                        "example": 1024,
+                        "maximum": 18446744073709552000,
+                        "minimum": 4,
+                        "title": "group_concat_max_len",
+                        "type": "integer"
+                    },
+                    "information_schema_stats_expiry": {
+                        "description": "The time, in seconds, before cached statistics expire",
+                        "example": 86400,
+                        "maximum": 31536000,
+                        "minimum": 900,
+                        "title": "information_schema_stats_expiry",
+                        "type": "integer"
+                    },
+                    "innodb_change_buffer_max_size": {
+                        "description": "Maximum size for the InnoDB change buffer, as a percentage of the total size of the buffer pool. Default is 25",
+                        "example": 30,
+                        "maximum": 50,
+                        "minimum": 0,
+                        "title": "innodb_change_buffer_max_size",
+                        "type": "integer"
+                    },
+                    "innodb_flush_neighbors": {
+                        "description": "Specifies whether flushing a page from the InnoDB buffer pool also flushes other dirty pages in the same extent (default is 1): 0 - dirty pages in the same extent are not flushed,  1 - flush contiguous dirty pages in the same extent,  2 - flush dirty pages in the same extent",
+                        "example": 0,
+                        "maximum": 2,
+                        "minimum": 0,
+                        "title": "innodb_flush_neighbors",
+                        "type": "integer"
+                    },
+                    "innodb_ft_min_token_size": {
+                        "description": "Minimum length of words that are stored in an InnoDB FULLTEXT index. Changing this parameter will lead to a restart of the MySQL service.",
+                        "example": 3,
+                        "maximum": 16,
+                        "minimum": 0,
+                        "title": "innodb_ft_min_token_size",
+                        "type": "integer"
+                    },
+                    "innodb_ft_server_stopword_table": {
+                        "description": "This option is used to specify your own InnoDB FULLTEXT index stopword list for all InnoDB tables.",
+                        "example": "db_name/table_name",
+                        "maxLength": 1024,
+                        "nullable": true,
+                        "pattern": "^.+/.+$",
+                        "title": "innodb_ft_server_stopword_table",
+                        "type": "string"
+                    },
+                    "innodb_lock_wait_timeout": {
+                        "description": "The length of time in seconds an InnoDB transaction waits for a row lock before giving up. Default is 120.",
+                        "example": 50,
+                        "maximum": 3600,
+                        "minimum": 1,
+                        "title": "innodb_lock_wait_timeout",
+                        "type": "integer"
+                    },
+                    "innodb_log_buffer_size": {
+                        "description": "The size in bytes of the buffer that InnoDB uses to write to the log files on disk.",
+                        "example": 16777216,
+                        "maximum": 4294967295,
+                        "minimum": 1048576,
+                        "title": "innodb_log_buffer_size",
+                        "type": "integer"
+                    },
+                    "innodb_online_alter_log_max_size": {
+                        "description": "The upper limit in bytes on the size of the temporary log files used during online DDL operations for InnoDB tables.",
+                        "example": 134217728,
+                        "maximum": 1099511627776,
+                        "minimum": 65536,
+                        "title": "innodb_online_alter_log_max_size",
+                        "type": "integer"
+                    },
+                    "innodb_print_all_deadlocks": {
+                        "description": "When enabled, information about all deadlocks in InnoDB user transactions is recorded in the error log. Disabled by default.",
+                        "example": true,
+                        "title": "innodb_print_all_deadlocks",
+                        "type": "boolean"
+                    },
+                    "innodb_read_io_threads": {
+                        "description": "The number of I/O threads for read operations in InnoDB. Default is 4. Changing this parameter will lead to a restart of the MySQL service.",
+                        "example": 10,
+                        "maximum": 64,
+                        "minimum": 1,
+                        "title": "innodb_read_io_threads",
+                        "type": "integer"
+                    },
+                    "innodb_rollback_on_timeout": {
+                        "description": "When enabled a transaction timeout causes InnoDB to abort and roll back the entire transaction. Changing this parameter will lead to a restart of the MySQL service.",
+                        "example": true,
+                        "title": "innodb_rollback_on_timeout",
+                        "type": "boolean"
+                    },
+                    "innodb_thread_concurrency": {
+                        "description": "Defines the maximum number of threads permitted inside of InnoDB. Default is 0 (infinite concurrency - no limit)",
+                        "example": 10,
+                        "maximum": 1000,
+                        "minimum": 0,
+                        "title": "innodb_thread_concurrency",
+                        "type": "integer"
+                    },
+                    "innodb_write_io_threads": {
+                        "description": "The number of I/O threads for write operations in InnoDB. Default is 4. Changing this parameter will lead to a restart of the MySQL service.",
+                        "example": 10,
+                        "maximum": 64,
+                        "minimum": 1,
+                        "title": "innodb_write_io_threads",
+                        "type": "integer"
+                    },
+                    "interactive_timeout": {
+                        "description": "The number of seconds the server waits for activity on an interactive connection before closing it.",
+                        "example": 3600,
+                        "maximum": 604800,
+                        "minimum": 30,
+                        "title": "interactive_timeout",
+                        "type": "integer"
+                    },
+                    "internal_tmp_mem_storage_engine": {
+                        "description": "The storage engine for in-memory internal temporary tables.",
+                        "enum": [
+                            "MEMORY",
+                            "TempTable"
+                        ],
+                        "example": "TempTable",
+                        "title": "internal_tmp_mem_storage_engine",
+                        "type": "string"
+                    },
+                    "long_query_time": {
+                        "description": "The slow_query_logs work as SQL statements that take more than long_query_time seconds to execute. Default is 10s",
+                        "example": 10,
+                        "maximum": 3600,
+                        "minimum": 0,
+                        "title": "long_query_time",
+                        "type": "number"
+                    },
+                    "max_allowed_packet": {
+                        "description": "Size of the largest message in bytes that can be received by the server. Default is 67108864 (64M)",
+                        "example": 67108864,
+                        "maximum": 1073741824,
+                        "minimum": 102400,
+                        "title": "max_allowed_packet",
+                        "type": "integer"
+                    },
+                    "max_heap_table_size": {
+                        "description": "Limits the size of internal in-memory tables. Also set tmp_table_size. Default is 16777216 (16M)",
+                        "example": 16777216,
+                        "maximum": 1073741824,
+                        "minimum": 1048576,
+                        "title": "max_heap_table_size",
+                        "type": "integer"
+                    },
+                    "net_buffer_length": {
+                        "description": "Start sizes of connection buffer and result buffer. Default is 16384 (16K). Changing this parameter will lead to a restart of the MySQL service.",
+                        "example": 16384,
+                        "maximum": 1048576,
+                        "minimum": 1024,
+                        "title": "net_buffer_length",
+                        "type": "integer"
+                    },
+                    "net_read_timeout": {
+                        "description": "The number of seconds to wait for more data from a connection before aborting the read.",
+                        "example": 30,
+                        "maximum": 3600,
+                        "minimum": 1,
+                        "title": "net_read_timeout",
+                        "type": "integer"
+                    },
+                    "net_write_timeout": {
+                        "description": "The number of seconds to wait for a block to be written to a connection before aborting the write.",
+                        "example": 30,
+                        "maximum": 3600,
+                        "minimum": 1,
+                        "title": "net_write_timeout",
+                        "type": "integer"
+                    },
+                    "slow_query_log": {
+                        "description": "Slow query log enables capturing of slow queries. Setting slow_query_log to false also truncates the mysql.slow_log table. Default is off",
+                        "example": true,
+                        "title": "slow_query_log",
+                        "type": "boolean"
+                    },
+                    "sort_buffer_size": {
+                        "description": "Sort buffer size in bytes for ORDER BY optimization. Default is 262144 (256K)",
+                        "example": 262144,
+                        "maximum": 1073741824,
+                        "minimum": 32768,
+                        "title": "sort_buffer_size",
+                        "type": "integer"
+                    },
+                    "sql_mode": {
+                        "description": "Global SQL mode. Set to empty to use MySQL server defaults. When creating a new service and not setting this field Aiven default SQL mode (strict, SQL standard compliant) will be assigned.",
+                        "example": "ANSI,TRADITIONAL",
+                        "maxLength": 1024,
+                        "pattern": "^[A-Z_]*(,[A-Z_]+)*$",
+                        "title": "sql_mode",
+                        "type": "string"
+                    },
+                    "sql_require_primary_key": {
+                        "description": "Require primary key to be defined for new tables or old tables modified with ALTER TABLE and fail if missing. It is recommended to always have primary keys because various functionality may break if any large table is missing them.",
+                        "example": true,
+                        "title": "sql_require_primary_key",
+                        "type": "boolean"
+                    },
+                    "tmp_table_size": {
+                        "description": "Limits the size of internal in-memory tables. Also set max_heap_table_size. Default is 16777216 (16M)",
+                        "example": 16777216,
+                        "maximum": 1073741824,
+                        "minimum": 1048576,
+                        "title": "tmp_table_size",
+                        "type": "integer"
+                    },
+                    "wait_timeout": {
+                        "description": "The number of seconds the server waits for activity on a noninteractive connection before closing it.",
+                        "example": 28800,
+                        "maximum": 2147483,
+                        "minimum": 1,
+                        "title": "wait_timeout",
+                        "type": "integer"
+                    }
+                },
+                "title": "mysql.conf configuration values",
+                "type": "object"
+            },
+            "json-schema-opensearch": {
+                "additionalProperties": false,
+                "properties": {
+                    "action_auto_create_index_enabled": {
+                        "description": "Explicitly allow or block automatic creation of indices. Defaults to true",
+                        "example": false,
+                        "title": "action.auto_create_index",
+                        "type": "boolean"
+                    },
+                    "action_destructive_requires_name": {
+                        "example": true,
+                        "nullable": true,
+                        "title": "Require explicit index names when deleting",
+                        "type": "boolean"
+                    },
+                    "auth_failure_listeners": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "internal_authentication_backend_limiting": {
+                                "additionalProperties": false,
+                                "properties": {
+                                    "allowed_tries": {
+                                        "description": "The number of login attempts allowed before login is blocked",
+                                        "example": 10,
+                                        "maximum": 2147483647,
+                                        "minimum": 0,
+                                        "title": "internal_authentication_backend_limiting.allowed_tries",
+                                        "type": "integer"
+                                    },
+                                    "authentication_backend": {
+                                        "description": "The internal backend. Enter `internal`",
+                                        "enum": [
+                                            "internal"
+                                        ],
+                                        "example": "internal",
+                                        "maxLength": 1024,
+                                        "title": "internal_authentication_backend_limiting.authentication_backend",
+                                        "type": "string"
+                                    },
+                                    "block_expiry_seconds": {
+                                        "description": "The duration of time that login remains blocked after a failed login",
+                                        "example": 600,
+                                        "maximum": 2147483647,
+                                        "minimum": 0,
+                                        "title": "internal_authentication_backend_limiting.block_expiry_seconds",
+                                        "type": "integer"
+                                    },
+                                    "max_blocked_clients": {
+                                        "description": "The maximum number of blocked IP addresses",
+                                        "example": 100000,
+                                        "maximum": 2147483647,
+                                        "minimum": 0,
+                                        "title": "internal_authentication_backend_limiting.max_blocked_clients",
+                                        "type": "integer"
+                                    },
+                                    "max_tracked_clients": {
+                                        "description": "The maximum number of tracked IP addresses that have failed login",
+                                        "example": 100000,
+                                        "maximum": 2147483647,
+                                        "minimum": 0,
+                                        "title": "internal_authentication_backend_limiting.max_tracked_clients",
+                                        "type": "integer"
+                                    },
+                                    "time_window_seconds": {
+                                        "description": "The window of time in which the value for `allowed_tries` is enforced",
+                                        "example": 3600,
+                                        "maximum": 2147483647,
+                                        "minimum": 0,
+                                        "title": "internal_authentication_backend_limiting.time_window_seconds",
+                                        "type": "integer"
+                                    },
+                                    "type": {
+                                        "description": "The type of rate limiting",
+                                        "enum": [
+                                            "username"
+                                        ],
+                                        "example": "username",
+                                        "maxLength": 1024,
+                                        "title": "internal_authentication_backend_limiting.type",
+                                        "type": "string"
+                                    }
+                                },
+                                "title": "Internal Authentication Backend Limiting",
+                                "type": "object"
+                            },
+                            "ip_rate_limiting": {
+                                "additionalProperties": false,
+                                "properties": {
+                                    "allowed_tries": {
+                                        "description": "The number of login attempts allowed before login is blocked",
+                                        "example": 10,
+                                        "maximum": 2147483647,
+                                        "minimum": 1,
+                                        "title": "ip_rate_limiting.allowed_tries",
+                                        "type": "integer"
+                                    },
+                                    "block_expiry_seconds": {
+                                        "description": "The duration of time that login remains blocked after a failed login",
+                                        "example": 600,
+                                        "maximum": 36000,
+                                        "minimum": 1,
+                                        "title": "ip_rate_limiting.block_expiry_seconds",
+                                        "type": "integer"
+                                    },
+                                    "max_blocked_clients": {
+                                        "description": "The maximum number of blocked IP addresses",
+                                        "example": 100000,
+                                        "maximum": 2147483647,
+                                        "minimum": 0,
+                                        "title": "ip_rate_limiting.max_blocked_clients",
+                                        "type": "integer"
+                                    },
+                                    "max_tracked_clients": {
+                                        "description": "The maximum number of tracked IP addresses that have failed login",
+                                        "example": 100000,
+                                        "maximum": 2147483647,
+                                        "minimum": 0,
+                                        "title": "ip_rate_limiting.max_tracked_clients",
+                                        "type": "integer"
+                                    },
+                                    "time_window_seconds": {
+                                        "description": "The window of time in which the value for `allowed_tries` is enforced",
+                                        "example": 3600,
+                                        "maximum": 36000,
+                                        "minimum": 1,
+                                        "title": "ip_rate_limiting.time_window_seconds",
+                                        "type": "integer"
+                                    },
+                                    "type": {
+                                        "description": "The type of rate limiting",
+                                        "enum": [
+                                            "ip"
+                                        ],
+                                        "example": "ip",
+                                        "maxLength": 1024,
+                                        "title": "ip_rate_limiting.type",
+                                        "type": "string"
+                                    }
+                                },
+                                "title": "IP address rate limiting settings",
+                                "type": "object"
+                            }
+                        },
+                        "title": "Opensearch Security Plugin Settings",
+                        "type": "object"
+                    },
+                    "cluster_max_shards_per_node": {
+                        "description": "Controls the number of shards allowed in the cluster per data node",
+                        "example": 1000,
+                        "maximum": 10000,
+                        "minimum": 100,
+                        "title": "cluster.max_shards_per_node",
+                        "type": "integer"
+                    },
+                    "cluster_routing_allocation_node_concurrent_recoveries": {
+                        "description": "How many concurrent incoming/outgoing shard recoveries (normally replicas) are allowed to happen on a node. Defaults to 2.",
+                        "maximum": 16,
+                        "minimum": 2,
+                        "title": "Concurrent incoming/outgoing shard recoveries per node",
+                        "type": "integer"
+                    },
+                    "email-sender": {
+                        "properties": {
+                            "email_sender_name": {
+                                "description": "This should be identical to the Sender name defined in Opensearch dashboards",
+                                "example": "alert-sender",
+                                "maxLength": 40,
+                                "pattern": "^[a-zA-Z0-9-_]+$",
+                                "title": "Sender name placeholder to be used in Opensearch Dashboards and Opensearch keystore",
+                                "type": "string"
+                            },
+                            "email_sender_password": {
+                                "description": "Sender password for Opensearch alerts to authenticate with SMTP server",
+                                "example": "very-secure-mail-password",
+                                "maxLength": 1024,
+                                "pattern": "^[^\\x00-\\x1F]+$",
+                                "title": "Sender password for Opensearch alerts to authenticate with SMTP server",
+                                "type": "string"
+                            },
+                            "email_sender_username": {
+                                "example": "jane@example.com",
+                                "maxLength": 320,
+                                "pattern": "^[^\\x00-\\x1F]+$",
+                                "title": "Sender username for Opensearch alerts",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "email_sender_name",
+                            "email_sender_password",
+                            "email_sender_username"
+                        ],
+                        "title": "Opensearch Email Sender Settings",
+                        "type": "object"
+                    },
+                    "http_max_content_length": {
+                        "description": "Maximum content length for HTTP requests to the OpenSearch HTTP API, in bytes.",
+                        "maximum": 2147483647,
+                        "minimum": 1,
+                        "title": "http.max_content_length",
+                        "type": "integer"
+                    },
+                    "http_max_header_size": {
+                        "description": "The max size of allowed headers, in bytes",
+                        "example": 8192,
+                        "maximum": 262144,
+                        "minimum": 1024,
+                        "title": "http.max_header_size",
+                        "type": "integer"
+                    },
+                    "http_max_initial_line_length": {
+                        "description": "The max length of an HTTP URL, in bytes",
+                        "example": 4096,
+                        "maximum": 65536,
+                        "minimum": 1024,
+                        "title": "http.max_initial_line_length",
+                        "type": "integer"
+                    },
+                    "indices_fielddata_cache_size": {
+                        "default": null,
+                        "description": "Relative amount. Maximum amount of heap memory used for field data cache. This is an expert setting; decreasing the value too much will increase overhead of loading field data; too much memory used for field data cache will decrease amount of heap available for other operations.",
+                        "maximum": 100,
+                        "minimum": 3,
+                        "nullable": true,
+                        "title": "indices.fielddata.cache.size",
+                        "type": "integer"
+                    },
+                    "indices_memory_index_buffer_size": {
+                        "description": "Percentage value. Default is 10%. Total amount of heap used for indexing buffer, before writing segments to disk. This is an expert setting. Too low value will slow down indexing; too high value will increase indexing performance but causes performance issues for query performance.",
+                        "maximum": 40,
+                        "minimum": 3,
+                        "title": "indices.memory.index_buffer_size",
+                        "type": "integer"
+                    },
+                    "indices_queries_cache_size": {
+                        "description": "Percentage value. Default is 10%. Maximum amount of heap used for query cache. This is an expert setting. Too low value will decrease query performance and increase performance for other operations; too high value will cause issues with other OpenSearch functionality.",
+                        "maximum": 40,
+                        "minimum": 3,
+                        "title": "indices.queries.cache.size",
+                        "type": "integer"
+                    },
+                    "indices_query_bool_max_clause_count": {
+                        "description": "Maximum number of clauses Lucene BooleanQuery can have. The default value (1024) is relatively high, and increasing it may cause performance issues. Investigate other approaches first before increasing this value.",
+                        "maximum": 4096,
+                        "minimum": 64,
+                        "title": "indices.query.bool.max_clause_count",
+                        "type": "integer"
+                    },
+                    "indices_recovery_max_bytes_per_sec": {
+                        "description": "Limits total inbound and outbound recovery traffic for each node. Applies to both peer recoveries as well as snapshot recoveries (i.e., restores from a snapshot). Defaults to 40mb",
+                        "maximum": 400,
+                        "minimum": 40,
+                        "title": "indices.recovery.max_bytes_per_sec",
+                        "type": "integer"
+                    },
+                    "indices_recovery_max_concurrent_file_chunks": {
+                        "description": "Number of file chunks sent in parallel for each recovery. Defaults to 2.",
+                        "maximum": 5,
+                        "minimum": 2,
+                        "title": "indices.recovery.max_concurrent_file_chunks",
+                        "type": "integer"
+                    },
+                    "ism-history": {
+                        "properties": {
+                            "ism_enabled": {
+                                "default": true,
+                                "example": true,
+                                "nullable": true,
+                                "title": "Specifies whether ISM is enabled or not",
+                                "type": "boolean"
+                            },
+                            "ism_history_enabled": {
+                                "default": true,
+                                "example": true,
+                                "nullable": true,
+                                "title": "Specifies whether audit history is enabled or not. The logs from ISM are automatically indexed to a logs document.",
+                                "type": "boolean"
+                            },
+                            "ism_history_max_age": {
+                                "default": 24,
+                                "example": 24,
+                                "maximum": 2147483647,
+                                "minimum": 1,
+                                "nullable": true,
+                                "title": "The maximum age before rolling over the audit history index in hours",
+                                "type": "integer"
+                            },
+                            "ism_history_max_docs": {
+                                "default": 2500000,
+                                "example": 2500000,
+                                "maximum": 9223372036854776000,
+                                "minimum": 1,
+                                "nullable": true,
+                                "title": "The maximum number of documents before rolling over the audit history index.",
+                                "type": "integer"
+                            },
+                            "ism_history_rollover_check_period": {
+                                "default": 8,
+                                "example": 8,
+                                "maximum": 2147483647,
+                                "minimum": 1,
+                                "nullable": true,
+                                "title": "The time between rollover checks for the audit history index in hours.",
+                                "type": "integer"
+                            },
+                            "ism_history_rollover_retention_period": {
+                                "default": 30,
+                                "example": 30,
+                                "maximum": 2147483647,
+                                "minimum": 1,
+                                "nullable": true,
+                                "title": "How long audit history indices are kept in days.",
+                                "type": "integer"
+                            }
+                        },
+                        "required": [
+                            "ism_enabled"
+                        ],
+                        "title": "Opensearch ISM History Settings",
+                        "type": "object"
+                    },
+                    "override_main_response_version": {
+                        "description": "Compatibility mode sets OpenSearch to report its version as 7.10 so clients continue to work. Default is false",
+                        "example": true,
+                        "title": "compatibility.override_main_response_version",
+                        "type": "boolean"
+                    },
+                    "reindex_remote_whitelist": {
+                        "description": "Whitelisted addresses for reindexing. Changing this value will cause all OpenSearch instances to restart.",
+                        "items": {
+                            "example": "anotherservice.aivencloud.com:12398",
+                            "maxLength": 261,
+                            "nullable": true,
+                            "title": "Address (hostname:port or IP:port)",
+                            "type": "string"
+                        },
+                        "maxItems": 32,
+                        "nullable": true,
+                        "title": "reindex_remote_whitelist",
+                        "type": "array"
+                    },
+                    "script_max_compilations_rate": {
+                        "description": "Script compilation circuit breaker limits the number of inline script compilations within a period of time. Default is use-context",
+                        "example": "75/5m",
+                        "maxLength": 1024,
+                        "title": "Script max compilation rate - circuit breaker to prevent/minimize OOMs",
+                        "type": "string"
+                    },
+                    "search_max_buckets": {
+                        "description": "Maximum number of aggregation buckets allowed in a single response. OpenSearch default value is used when this is not defined.",
+                        "example": 10000,
+                        "maximum": 65536,
+                        "minimum": 1,
+                        "nullable": true,
+                        "title": "search.max_buckets",
+                        "type": "integer"
+                    },
+                    "thread_pool_analyze_queue_size": {
+                        "description": "Size for the thread pool queue. See documentation for exact details.",
+                        "maximum": 2000,
+                        "minimum": 10,
+                        "title": "analyze thread pool queue size",
+                        "type": "integer"
+                    },
+                    "thread_pool_analyze_size": {
+                        "description": "Size for the thread pool. See documentation for exact details. Do note this may have maximum value depending on CPU count - value is automatically lowered if set to higher than maximum value.",
+                        "maximum": 128,
+                        "minimum": 1,
+                        "title": "analyze thread pool size",
+                        "type": "integer"
+                    },
+                    "thread_pool_force_merge_size": {
+                        "description": "Size for the thread pool. See documentation for exact details. Do note this may have maximum value depending on CPU count - value is automatically lowered if set to higher than maximum value.",
+                        "maximum": 128,
+                        "minimum": 1,
+                        "title": "force_merge thread pool size",
+                        "type": "integer"
+                    },
+                    "thread_pool_get_queue_size": {
+                        "description": "Size for the thread pool queue. See documentation for exact details.",
+                        "maximum": 2000,
+                        "minimum": 10,
+                        "title": "get thread pool queue size",
+                        "type": "integer"
+                    },
+                    "thread_pool_get_size": {
+                        "description": "Size for the thread pool. See documentation for exact details. Do note this may have maximum value depending on CPU count - value is automatically lowered if set to higher than maximum value.",
+                        "maximum": 128,
+                        "minimum": 1,
+                        "title": "get thread pool size",
+                        "type": "integer"
+                    },
+                    "thread_pool_search_queue_size": {
+                        "description": "Size for the thread pool queue. See documentation for exact details.",
+                        "maximum": 2000,
+                        "minimum": 10,
+                        "title": "search thread pool queue size",
+                        "type": "integer"
+                    },
+                    "thread_pool_search_size": {
+                        "description": "Size for the thread pool. See documentation for exact details. Do note this may have maximum value depending on CPU count - value is automatically lowered if set to higher than maximum value.",
+                        "maximum": 128,
+                        "minimum": 1,
+                        "title": "search thread pool size",
+                        "type": "integer"
+                    },
+                    "thread_pool_search_throttled_queue_size": {
+                        "description": "Size for the thread pool queue. See documentation for exact details.",
+                        "maximum": 2000,
+                        "minimum": 10,
+                        "title": "search_throttled thread pool queue size",
+                        "type": "integer"
+                    },
+                    "thread_pool_search_throttled_size": {
+                        "description": "Size for the thread pool. See documentation for exact details. Do note this may have maximum value depending on CPU count - value is automatically lowered if set to higher than maximum value.",
+                        "maximum": 128,
+                        "minimum": 1,
+                        "title": "search_throttled thread pool size",
+                        "type": "integer"
+                    },
+                    "thread_pool_write_queue_size": {
+                        "description": "Size for the thread pool queue. See documentation for exact details.",
+                        "maximum": 2000,
+                        "minimum": 10,
+                        "title": "write thread pool queue size",
+                        "type": "integer"
+                    },
+                    "thread_pool_write_size": {
+                        "description": "Size for the thread pool. See documentation for exact details. Do note this may have maximum value depending on CPU count - value is automatically lowered if set to higher than maximum value.",
+                        "maximum": 128,
+                        "minimum": 1,
+                        "title": "write thread pool size",
+                        "type": "integer"
+                    }
+                },
+                "title": "OpenSearch settings",
+                "type": "object"
+            },
+            "json-schema-pg": {
+                "additionalProperties": false,
+                "properties": {
+                    "autovacuum": {
+                        "properties": {
+                            "autovacuum_analyze_scale_factor": {
+                                "description": "Specifies a fraction of the table size to add to autovacuum_analyze_threshold when deciding whether to trigger an ANALYZE. The default is 0.2 (20% of table size)",
+                                "maximum": 1,
+                                "minimum": 0,
+                                "title": "autovacuum_analyze_scale_factor",
+                                "type": "number"
+                            },
+                            "autovacuum_analyze_threshold": {
+                                "description": "Specifies the minimum number of inserted, updated or deleted tuples needed to trigger an  ANALYZE in any one table. The default is 50 tuples.",
+                                "maximum": 2147483647,
+                                "minimum": 0,
+                                "title": "autovacuum_analyze_threshold",
+                                "type": "integer"
+                            },
+                            "autovacuum_freeze_max_age": {
+                                "description": "Specifies the maximum age (in transactions) that a table's pg_class.relfrozenxid field can attain before a VACUUM operation is forced to prevent transaction ID wraparound within the table. Note that the system will launch autovacuum processes to prevent wraparound even when autovacuum is otherwise disabled. This parameter will cause the server to be restarted.",
+                                "example": 200000000,
+                                "maximum": 1500000000,
+                                "minimum": 200000000,
+                                "title": "autovacuum_freeze_max_age",
+                                "type": "integer"
+                            },
+                            "autovacuum_max_workers": {
+                                "description": "Specifies the maximum number of autovacuum processes (other than the autovacuum launcher) that may be running at any one time. The default is three. This parameter can only be set at server start.",
+                                "maximum": 20,
+                                "minimum": 1,
+                                "title": "autovacuum_max_workers",
+                                "type": "integer"
+                            },
+                            "autovacuum_naptime": {
+                                "description": "Specifies the minimum delay between autovacuum runs on any given database. The delay is measured in seconds, and the default is one minute",
+                                "maximum": 86400,
+                                "minimum": 1,
+                                "title": "autovacuum_naptime",
+                                "type": "integer"
+                            },
+                            "autovacuum_vacuum_cost_delay": {
+                                "description": "Specifies the cost delay value that will be used in automatic VACUUM operations. If -1 is specified, the regular vacuum_cost_delay value will be used. The default value is 20 milliseconds",
+                                "maximum": 100,
+                                "minimum": -1,
+                                "title": "autovacuum_vacuum_cost_delay",
+                                "type": "integer"
+                            },
+                            "autovacuum_vacuum_cost_limit": {
+                                "description": "Specifies the cost limit value that will be used in automatic VACUUM operations. If -1 is specified (which is the default), the regular vacuum_cost_limit value will be used.",
+                                "maximum": 10000,
+                                "minimum": -1,
+                                "title": "autovacuum_vacuum_cost_limit",
+                                "type": "integer"
+                            },
+                            "autovacuum_vacuum_scale_factor": {
+                                "description": "Specifies a fraction of the table size to add to autovacuum_vacuum_threshold when deciding whether to trigger a VACUUM. The default is 0.2 (20% of table size)",
+                                "maximum": 1,
+                                "minimum": 0,
+                                "title": "autovacuum_vacuum_scale_factor",
+                                "type": "number"
+                            },
+                            "autovacuum_vacuum_threshold": {
+                                "description": "Specifies the minimum number of updated or deleted tuples needed to trigger a VACUUM in any one table. The default is 50 tuples",
+                                "maximum": 2147483647,
+                                "minimum": 0,
+                                "title": "autovacuum_vacuum_threshold",
+                                "type": "integer"
+                            },
+                            "log_autovacuum_min_duration": {
+                                "description": "Causes each action executed by autovacuum to be logged if it ran for at least the specified number of milliseconds. Setting this to zero logs all autovacuum actions. Minus-one (the default) disables logging autovacuum actions.",
+                                "maximum": 2147483647,
+                                "minimum": -1,
+                                "title": "log_autovacuum_min_duration",
+                                "type": "integer"
+                            }
+                        },
+                        "title": "Autovacuum settings",
+                        "type": "object"
+                    },
+                    "bg-writer": {
+                        "properties": {
+                            "bgwriter_delay": {
+                                "description": "Specifies the delay between activity rounds for the background writer in milliseconds. Default is 200.",
+                                "example": 200,
+                                "maximum": 10000,
+                                "minimum": 10,
+                                "title": "bgwriter_delay",
+                                "type": "integer"
+                            },
+                            "bgwriter_flush_after": {
+                                "description": "Whenever more than bgwriter_flush_after bytes have been written by the background writer, attempt to force the OS to issue these writes to the underlying storage. Specified in kilobytes, default is 512. Setting of 0 disables forced writeback.",
+                                "example": 512,
+                                "maximum": 2048,
+                                "minimum": 0,
+                                "title": "bgwriter_flush_after",
+                                "type": "integer"
+                            },
+                            "bgwriter_lru_maxpages": {
+                                "description": "In each round, no more than this many buffers will be written by the background writer. Setting this to zero disables background writing. Default is 100.",
+                                "example": 100,
+                                "maximum": 1073741823,
+                                "minimum": 0,
+                                "title": "bgwriter_lru_maxpages",
+                                "type": "integer"
+                            },
+                            "bgwriter_lru_multiplier": {
+                                "description": "The average recent need for new buffers is multiplied by bgwriter_lru_multiplier to arrive at an estimate of the number that will be needed during the next round, (up to bgwriter_lru_maxpages). 1.0 represents a \u201cjust in time\u201d policy of writing exactly the number of buffers predicted to be needed. Larger values provide some cushion against spikes in demand, while smaller values intentionally leave writes to be done by server processes. The default is 2.0.",
+                                "example": 2,
+                                "maximum": 10,
+                                "minimum": 0,
+                                "title": "bgwriter_lru_multiplier",
+                                "type": "number"
+                            }
+                        },
+                        "title": "Background (BG) writer settings",
+                        "type": "object"
+                    },
+                    "deadlock_timeout": {
+                        "description": "This is the amount of time, in milliseconds, to wait on a lock before checking to see if there is a deadlock condition.",
+                        "example": 1000,
+                        "maximum": 1800000,
+                        "minimum": 500,
+                        "title": "deadlock_timeout",
+                        "type": "integer"
+                    },
+                    "default_toast_compression": {
+                        "description": "Specifies the default TOAST compression method for values of compressible columns (the default is lz4).",
+                        "enum": [
+                            "lz4",
+                            "pglz"
+                        ],
+                        "example": "lz4",
+                        "title": "default_toast_compression",
+                        "type": "string"
+                    },
+                    "idle_in_transaction_session_timeout": {
+                        "description": "Time out sessions with open transactions after this number of milliseconds",
+                        "maximum": 604800000,
+                        "minimum": 0,
+                        "title": "idle_in_transaction_session_timeout",
+                        "type": "integer"
+                    },
+                    "jit": {
+                        "description": "Controls system-wide use of Just-in-Time Compilation (JIT).",
+                        "example": true,
+                        "title": "jit",
+                        "type": "boolean"
+                    },
+                    "log_error_verbosity": {
+                        "description": "Controls the amount of detail written in the server log for each message that is logged.",
+                        "enum": [
+                            "DEFAULT",
+                            "TERSE",
+                            "VERBOSE"
+                        ],
+                        "title": "log_error_verbosity",
+                        "type": "string"
+                    },
+                    "log_line_prefix": {
+                        "description": "Choose from one of the available log-formats. These can support popular log analyzers like pgbadger, pganalyze etc.",
+                        "enum": [
+                            "'%m [%p] %q[user=%u,db=%d,app=%a] '",
+                            "'%t [%p]: [%l-1] user=%u,db=%d,app=%a,client=%h '",
+                            "'pid=%p,user=%u,db=%d,app=%a,client=%h '"
+                        ],
+                        "title": "log_line_prefix",
+                        "type": "string"
+                    },
+                    "log_min_duration_statement": {
+                        "description": "Log statements that take more than this number of milliseconds to run, -1 disables",
+                        "maximum": 86400000,
+                        "minimum": -1,
+                        "title": "log_min_duration_statement",
+                        "type": "integer"
+                    },
+                    "log_temp_files": {
+                        "description": "Log statements for each temporary file created larger than this number of kilobytes, -1 disables",
+                        "maximum": 2147483647,
+                        "minimum": -1,
+                        "title": "log_temp_files",
+                        "type": "integer"
+                    },
+                    "max_files_per_process": {
+                        "description": "PostgreSQL maximum number of files that can be open per process",
+                        "maximum": 4096,
+                        "minimum": 1000,
+                        "title": "max_files_per_process",
+                        "type": "integer"
+                    },
+                    "max_locks_per_transaction": {
+                        "description": "PostgreSQL maximum locks per transaction",
+                        "maximum": 6400,
+                        "minimum": 64,
+                        "title": "max_locks_per_transaction",
+                        "type": "integer"
+                    },
+                    "max_logical_replication_workers": {
+                        "description": "PostgreSQL maximum logical replication workers (taken from the pool of max_parallel_workers)",
+                        "maximum": 64,
+                        "minimum": 4,
+                        "title": "max_logical_replication_workers",
+                        "type": "integer"
+                    },
+                    "max_parallel_workers": {
+                        "description": "Sets the maximum number of workers that the system can support for parallel queries",
+                        "maximum": 96,
+                        "minimum": 0,
+                        "title": "max_parallel_workers",
+                        "type": "integer"
+                    },
+                    "max_parallel_workers_per_gather": {
+                        "description": "Sets the maximum number of workers that can be started by a single Gather or Gather Merge node",
+                        "maximum": 96,
+                        "minimum": 0,
+                        "title": "max_parallel_workers_per_gather",
+                        "type": "integer"
+                    },
+                    "max_pred_locks_per_transaction": {
+                        "description": "PostgreSQL maximum predicate locks per transaction",
+                        "maximum": 5120,
+                        "minimum": 64,
+                        "title": "max_pred_locks_per_transaction",
+                        "type": "integer"
+                    },
+                    "max_prepared_transactions": {
+                        "description": "PostgreSQL maximum prepared transactions",
+                        "maximum": 10000,
+                        "minimum": 0,
+                        "title": "max_prepared_transactions",
+                        "type": "integer"
+                    },
+                    "max_replication_slots": {
+                        "description": "PostgreSQL maximum replication slots",
+                        "maximum": 64,
+                        "minimum": 8,
+                        "title": "max_replication_slots",
+                        "type": "integer"
+                    },
+                    "max_stack_depth": {
+                        "description": "Maximum depth of the stack in bytes",
+                        "maximum": 6291456,
+                        "minimum": 2097152,
+                        "title": "max_stack_depth",
+                        "type": "integer"
+                    },
+                    "max_standby_archive_delay": {
+                        "description": "Max standby archive delay in milliseconds",
+                        "maximum": 43200000,
+                        "minimum": 1,
+                        "title": "max_standby_archive_delay",
+                        "type": "integer"
+                    },
+                    "max_standby_streaming_delay": {
+                        "description": "Max standby streaming delay in milliseconds",
+                        "maximum": 43200000,
+                        "minimum": 1,
+                        "title": "max_standby_streaming_delay",
+                        "type": "integer"
+                    },
+                    "max_worker_processes": {
+                        "description": "Sets the maximum number of background processes that the system can support",
+                        "maximum": 96,
+                        "minimum": 8,
+                        "title": "max_worker_processes",
+                        "type": "integer"
+                    },
+                    "pg_partman_bgw.interval": {
+                        "description": "Sets the time interval to run pg_partman's scheduled tasks",
+                        "example": 3600,
+                        "maximum": 604800,
+                        "minimum": 3600,
+                        "title": "pg_partman_bgw.interval",
+                        "type": "integer"
+                    },
+                    "pg_partman_bgw.role": {
+                        "description": "Controls which role to use for pg_partman's scheduled background tasks.",
+                        "example": "myrolename",
+                        "maxLength": 64,
+                        "pattern": "^[_A-Za-z0-9][-._A-Za-z0-9]{0,63}$",
+                        "title": "pg_partman_bgw.role",
+                        "type": "string"
+                    },
+                    "pg_stat_monitor.pgsm_enable_query_plan": {
+                        "description": "Enables or disables query plan monitoring",
+                        "example": false,
+                        "title": "pg_stat_monitor.pgsm_enable_query_plan",
+                        "type": "boolean"
+                    },
+                    "pg_stat_monitor.pgsm_max_buckets": {
+                        "description": "Sets the maximum number of buckets ",
+                        "example": 10,
+                        "maximum": 10,
+                        "minimum": 1,
+                        "title": "pg_stat_monitor.pgsm_max_buckets",
+                        "type": "integer"
+                    },
+                    "pg_stat_statements.track": {
+                        "description": "Controls which statements are counted. Specify top to track top-level statements (those issued directly by clients), all to also track nested statements (such as statements invoked within functions), or none to disable statement statistics collection. The default value is top.",
+                        "enum": [
+                            "all",
+                            "none",
+                            "top"
+                        ],
+                        "title": "pg_stat_statements.track",
+                        "type": "string"
+                    },
+                    "temp_file_limit": {
+                        "description": "PostgreSQL temporary file limit in KiB, -1 for unlimited",
+                        "example": 5000000,
+                        "maximum": 2147483647,
+                        "minimum": -1,
+                        "title": "temp_file_limit",
+                        "type": "integer"
+                    },
+                    "timezone": {
+                        "description": "PostgreSQL service timezone",
+                        "example": "Europe/Helsinki",
+                        "maxLength": 64,
+                        "title": "timezone",
+                        "type": "string"
+                    },
+                    "track_activity_query_size": {
+                        "description": "Specifies the number of bytes reserved to track the currently executing command for each active session.",
+                        "example": 1024,
+                        "maximum": 10240,
+                        "minimum": 1024,
+                        "title": "track_activity_query_size",
+                        "type": "integer"
+                    },
+                    "track_commit_timestamp": {
+                        "description": "Record commit time of transactions.",
+                        "enum": [
+                            "off",
+                            "on"
+                        ],
+                        "example": "off",
+                        "title": "track_commit_timestamp",
+                        "type": "string"
+                    },
+                    "track_functions": {
+                        "description": "Enables tracking of function call counts and time used.",
+                        "enum": [
+                            "all",
+                            "none",
+                            "pl"
+                        ],
+                        "title": "track_functions",
+                        "type": "string"
+                    },
+                    "track_io_timing": {
+                        "description": "Enables timing of database I/O calls. This parameter is off by default, because it will repeatedly query the operating system for the current time, which may cause significant overhead on some platforms.",
+                        "enum": [
+                            "off",
+                            "on"
+                        ],
+                        "example": "off",
+                        "title": "track_io_timing",
+                        "type": "string"
+                    },
+                    "wal": {
+                        "properties": {
+                            "max_slot_wal_keep_size": {
+                                "description": "PostgreSQL maximum WAL size (MB) reserved for replication slots. Default is -1 (unlimited). wal_keep_size minimum WAL size setting takes precedence over this.",
+                                "maximum": 2147483647,
+                                "minimum": -1,
+                                "title": "max_slot_wal_keep_size",
+                                "type": "integer"
+                            },
+                            "max_wal_senders": {
+                                "description": "PostgreSQL maximum WAL senders",
+                                "maximum": 64,
+                                "minimum": 20,
+                                "title": "max_wal_senders",
+                                "type": "integer"
+                            },
+                            "wal_sender_timeout": {
+                                "anyOf": [
+                                    {
+                                        "maximum": 0,
+                                        "minimum": 0
+                                    },
+                                    {
+                                        "maximum": 10800000,
+                                        "minimum": 5000
+                                    }
+                                ],
+                                "description": "Terminate replication connections that are inactive for longer than this amount of time, in milliseconds. Setting this value to zero disables the timeout.",
+                                "example": 60000,
+                                "title": "wal_sender_timeout",
+                                "type": "integer"
+                            },
+                            "wal_writer_delay": {
+                                "description": "WAL flush interval in milliseconds. Note that setting this value to lower than the default 200ms may negatively impact performance",
+                                "example": 50,
+                                "maximum": 200,
+                                "minimum": 10,
+                                "title": "wal_writer_delay",
+                                "type": "integer"
+                            }
+                        },
+                        "title": "Write-ahead log (WAL) settings",
+                        "type": "object"
+                    }
+                },
+                "title": "postgresql.conf configuration values",
+                "type": "object"
+            },
+            "json-schema-pgbouncer": {
+                "additionalProperties": false,
+                "properties": {
+                    "autodb_idle_timeout": {
+                        "example": 3600,
+                        "maximum": 86400,
+                        "minimum": 0,
+                        "title": "If the automatically created database pools have been unused this many seconds, they are freed. If 0 then timeout is disabled. [seconds]",
+                        "type": "integer"
+                    },
+                    "autodb_max_db_connections": {
+                        "example": 0,
+                        "maximum": 2147483647,
+                        "minimum": 0,
+                        "title": "Do not allow more than this many server connections per database (regardless of user). Setting it to 0 means unlimited.",
+                        "type": "integer"
+                    },
+                    "autodb_pool_mode": {
+                        "enum": [
+                            "session",
+                            "statement",
+                            "transaction"
+                        ],
+                        "example": "session",
+                        "title": "PGBouncer pool mode",
+                        "type": "string"
+                    },
+                    "autodb_pool_size": {
+                        "example": 0,
+                        "maximum": 10000,
+                        "minimum": 0,
+                        "title": "If non-zero then create automatically a pool of that size per user when a pool doesn't exist.",
+                        "type": "integer"
+                    },
+                    "ignore_startup_parameters": {
+                        "example": [
+                            "extra_float_digits",
+                            "search_path"
+                        ],
+                        "items": {
+                            "enum": [
+                                "extra_float_digits",
+                                "search_path"
+                            ],
+                            "title": "Enum of parameters to ignore when given in startup packet",
+                            "type": "string"
+                        },
+                        "maxItems": 32,
+                        "title": "List of parameters to ignore when given in startup packet",
+                        "type": "array"
+                    },
+                    "min_pool_size": {
+                        "example": 0,
+                        "maximum": 10000,
+                        "minimum": 0,
+                        "title": "Add more server connections to pool if below this number. Improves behavior when usual load comes suddenly back after period of total inactivity. The value is effectively capped at the pool size.",
+                        "type": "integer"
+                    },
+                    "server_idle_timeout": {
+                        "example": 600,
+                        "maximum": 86400,
+                        "minimum": 0,
+                        "title": "If a server connection has been idle more than this many seconds it will be dropped. If 0 then timeout is disabled. [seconds]",
+                        "type": "integer"
+                    },
+                    "server_lifetime": {
+                        "example": 3600,
+                        "maximum": 86400,
+                        "minimum": 60,
+                        "title": "The pooler will close an unused server connection that has been connected longer than this. [seconds]",
+                        "type": "integer"
+                    },
+                    "server_reset_query_always": {
+                        "example": false,
+                        "title": "Run server_reset_query (DISCARD ALL) in all pooling modes",
+                        "type": "boolean"
+                    }
+                },
+                "title": "PGBouncer connection pooling settings",
+                "type": "object"
+            },
+            "json-schema-pglookout": {
+                "additionalProperties": false,
+                "default": {
+                    "max_failover_replication_time_lag": 60
+                },
+                "properties": {
+                    "max_failover_replication_time_lag": {
+                        "default": 60,
+                        "description": "Number of seconds of master unavailability before triggering database failover to standby",
+                        "maximum": 9223372036854776000,
+                        "minimum": 10,
+                        "title": "max_failover_replication_time_lag",
+                        "type": "integer"
+                    }
+                },
+                "title": "PGLookout settings",
+                "type": "object"
+            },
+            "json-schema-redis": {
+                "properties": {
+                    "acl_channels_default": {
+                        "description": "Determines default pub/sub channels' ACL for new users if ACL is not supplied. When this option is not defined, all_channels is assumed to keep backward compatibility. This option doesn't affect Redis configuration acl-pubsub-default.",
+                        "enum": [
+                            "allchannels",
+                            "resetchannels"
+                        ],
+                        "title": "Default ACL for pub/sub channels used when Redis user is created",
+                        "type": "string"
+                    },
+                    "io_threads": {
+                        "description": "Set Redis IO thread count. Changing this will cause a restart of the Redis service.",
+                        "example": 1,
+                        "maximum": 32,
+                        "minimum": 1,
+                        "title": "Redis IO thread count",
+                        "type": "integer"
+                    },
+                    "lfu_decay_time": {
+                        "default": 1,
+                        "maximum": 120,
+                        "minimum": 1,
+                        "title": "LFU maxmemory-policy counter decay time in minutes",
+                        "type": "integer"
+                    },
+                    "lfu_log_factor": {
+                        "default": 10,
+                        "maximum": 100,
+                        "minimum": 0,
+                        "title": "Counter logarithm factor for volatile-lfu and allkeys-lfu maxmemory-policies",
+                        "type": "integer"
+                    },
+                    "maxmemory_policy": {
+                        "default": "noeviction",
+                        "enum": [
+                            "allkeys-lfu",
+                            "allkeys-lru",
+                            "allkeys-random",
+                            "noeviction",
+                            "volatile-lfu",
+                            "volatile-lru",
+                            "volatile-random",
+                            "volatile-ttl"
+                        ],
+                        "nullable": true,
+                        "title": "Redis maxmemory-policy",
+                        "type": "string"
+                    },
+                    "notify_keyspace_events": {
+                        "default": "",
+                        "maxLength": 32,
+                        "pattern": "^[KEg\\$lshzxeA]*$",
+                        "title": "Set notify-keyspace-events option",
+                        "type": "string"
+                    },
+                    "number_of_databases": {
+                        "description": "Set number of Redis databases. Changing this will cause a restart of the Redis service.",
+                        "example": 16,
+                        "maximum": 128,
+                        "minimum": 1,
+                        "title": "Number of Redis databases",
+                        "type": "integer"
+                    },
+                    "persistence": {
+                        "description": "When persistence is 'rdb', Redis does RDB dumps each 10 minutes if any key is changed. Also RDB dumps are done according to backup schedule for backup purposes. When persistence is 'off', no RDB dumps and backups are done, so data can be lost at any moment if service is restarted for any reason, or if service is powered off. Also service can't be forked.",
+                        "enum": [
+                            "off",
+                            "rdb"
+                        ],
+                        "title": "Redis persistence",
+                        "type": "string"
+                    },
+                    "pubsub_client_output_buffer_limit": {
+                        "description": "Set output buffer limit for pub / sub clients in MB. The value is the hard limit, the soft limit is 1/4 of the hard limit. When setting the limit, be mindful of the available memory in the selected service plan.",
+                        "example": 64,
+                        "maximum": 512,
+                        "minimum": 32,
+                        "title": "Pub/sub client output buffer hard limit in MB",
+                        "type": "integer"
+                    },
+                    "ssl": {
+                        "default": true,
+                        "title": "Require SSL to access Redis",
+                        "type": "boolean"
+                    },
+                    "timeout": {
+                        "default": 300,
+                        "maximum": 31536000,
+                        "minimum": 0,
+                        "title": "Redis idle connection timeout in seconds",
+                        "type": "integer"
+                    }
+                },
+                "title": "Redis settings",
+                "type": "object"
+            },
+            "json-schema-schema-registry": {
+                "additionalProperties": false,
+                "properties": {
+                    "leader_eligibility": {
+                        "description": "If true, Karapace / Schema Registry on the service nodes can participate in leader election. It might be needed to disable this when the schemas topic is replicated to a secondary cluster and Karapace / Schema Registry there must not participate in leader election. Defaults to `true`.",
+                        "example": true,
+                        "title": "leader_eligibility",
+                        "type": "boolean"
+                    },
+                    "topic_name": {
+                        "description": "The durable single partition topic that acts as the durable log for the data. This topic must be compacted to avoid losing data due to retention policy. Please note that changing this configuration in an existing Schema Registry / Karapace setup leads to previous schemas being inaccessible, data encoded with them potentially unreadable and schema ID sequence put out of order. It's only possible to do the switch while Schema Registry / Karapace is disabled. Defaults to `_schemas`.",
+                        "example": "_schemas",
+                        "maxLength": 249,
+                        "minLength": 1,
+                        "pattern": "^(?!\\.$|\\.\\.$)[-_.A-Za-z0-9]+$",
+                        "title": "topic_name",
+                        "type": "string"
+                    }
+                },
+                "title": "Schema Registry configuration",
+                "type": "object"
+            },
+            "json-schema-timescaledb": {
+                "additionalProperties": false,
+                "properties": {
+                    "max_background_workers": {
+                        "description": "The number of background workers for timescaledb operations. You should configure this setting to the sum of your number of databases and the total number of concurrent background workers you want running at any given point in time.",
+                        "example": 8,
+                        "maximum": 4096,
+                        "minimum": 1,
+                        "title": "timescaledb.max_background_workers",
+                        "type": "integer"
+                    }
+                },
+                "title": "TimescaleDB extension configuration values",
+                "type": "object"
+            },
             "kubelet-image-gc": {
                 "description": "Kubelet image GC options",
                 "properties": {
                     "high-threshold": {
                         "exclusiveMinimum": false,
                         "format": "int64",
                         "minimum": 0,
@@ -4109,15 +6893,15 @@
                         "description": "Private Network ID",
                         "format": "uuid",
                         "readOnly": true,
                         "type": "string"
                     },
                     "labels": {
                         "$ref": "#/components/schemas/labels",
-                        "description": "Private Network labels"
+                        "description": "Resource labels"
                     },
                     "leases": {
                         "description": "Private Network leased IP addresses",
                         "items": {
                             "$ref": "#/components/schemas/private-network-lease"
                         },
                         "readOnly": true,
@@ -4368,14 +7152,15 @@
                 "description": "SKS Cluster",
                 "properties": {
                     "addons": {
                         "description": "Cluster addons",
                         "items": {
                             "enum": [
                                 "exoscale-cloud-controller",
+                                "exoscale-container-storage-interface",
                                 "metrics-server"
                             ],
                             "type": "string"
                         },
                         "type": "array",
                         "uniqueItems": true
                     },
@@ -4553,14 +7338,18 @@
                         "minLength": 1,
                         "type": "string"
                     },
                     "instance-type": {
                         "$ref": "#/components/schemas/instance-type",
                         "description": "Nodepool Instances type"
                     },
+                    "kubelet-image-gc": {
+                        "$ref": "#/components/schemas/kubelet-image-gc",
+                        "description": "Kubelet image GC options"
+                    },
                     "labels": {
                         "$ref": "#/components/schemas/labels",
                         "description": "Nodepool labels"
                     },
                     "name": {
                         "description": "Nodepool name",
                         "maxLength": 255,
@@ -4935,18 +7724,30 @@
                     }
                 },
                 "type": "object"
             },
             "zone": {
                 "description": "Zone",
                 "properties": {
+                    "api-endpoint": {
+                        "description": "Zone API endpoint",
+                        "readOnly": true,
+                        "type": "string",
+                        "x-go-type": "Endpoint"
+                    },
                     "name": {
                         "$ref": "#/components/schemas/zone-name",
                         "description": "Zone short name",
                         "readOnly": true
+                    },
+                    "sos-endpoint": {
+                        "description": "Zone SOS endpoint",
+                        "readOnly": true,
+                        "type": "string",
+                        "x-go-type": "Endpoint"
                     }
                 },
                 "type": "object"
             },
             "zone-name": {
                 "enum": [
                     "at-vie-1",
@@ -5001,15 +7802,15 @@
                 },
                 "summary": "List IAM Access Keys",
                 "tags": [
                     "iam"
                 ]
             },
             "post": {
-                "description": "This operation creates a new IAM Access Key, which can either be restricted to specific API operations or unrestricted. The corresponding secret is only available in the response returned by this operation, the caller must take care of storing it safely as there is no other way to retrieve it.",
+                "description": "This operation creates a legacy IAM Access Key, to create a key for use with IAM roles use the api-key endpoint.The corresponding secret is only available in the response returned by this operation, the caller must take care of storing it safely as there is no other way to retrieve it.",
                 "operationId": "create-access-key",
                 "parameters": [],
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "description": "IAM Access Key",
@@ -5054,15 +7855,15 @@
                                     "$ref": "#/components/schemas/access-key"
                                 }
                             }
                         },
                         "description": "200"
                     }
                 },
-                "summary": "Create an IAM Access Key",
+                "summary": "Create a legacy IAM Access Key",
                 "tags": [
                     "iam"
                 ]
             }
         },
         "/access-key-known-operations": {
             "get": {
@@ -5351,15 +8152,15 @@
                                     "type": "object"
                                 }
                             }
                         },
                         "description": "200"
                     }
                 },
-                "summary": "List v3 API keys",
+                "summary": "List API keys",
                 "tags": [
                     "iam"
                 ]
             },
             "post": {
                 "description": null,
                 "operationId": "create-api-key",
@@ -5367,14 +8168,16 @@
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "name": {
                                         "description": "IAM API Key Name",
+                                        "maxLength": 255,
+                                        "minLength": 1,
                                         "type": "string"
                                     },
                                     "role-id": {
                                         "description": "IAM API Key Role ID",
                                         "format": "uuid",
                                         "type": "string"
                                     }
@@ -5397,15 +8200,15 @@
                                     "$ref": "#/components/schemas/iam-api-key-created"
                                 }
                             }
                         },
                         "description": "200"
                     }
                 },
-                "summary": "Create a new v3 API key",
+                "summary": "Create a new API key",
                 "tags": [
                     "iam"
                 ]
             }
         },
         "/api-key/{id}": {
             "delete": {
@@ -5429,15 +8232,15 @@
                                     "$ref": "#/components/schemas/operation"
                                 }
                             }
                         },
                         "description": "200"
                     }
                 },
-                "summary": "Delete a v3 API key",
+                "summary": "Delete an API key",
                 "tags": [
                     "iam"
                 ]
             },
             "get": {
                 "description": null,
                 "operationId": "get-api-key",
@@ -5459,20 +8262,576 @@
                                     "$ref": "#/components/schemas/iam-api-key"
                                 }
                             }
                         },
                         "description": "200"
                     }
                 },
-                "summary": "Get v3 API key",
+                "summary": "Get API key",
                 "tags": [
                     "iam"
                 ]
             }
         },
+        "/block-storage": {
+            "get": {
+                "description": "",
+                "operationId": "list-block-storage-volumes",
+                "parameters": [
+                    {
+                        "in": "query",
+                        "name": "instance-id",
+                        "required": false,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "properties": {
+                                        "block-storage-volumes": {
+                                            "items": {
+                                                "$ref": "#/components/schemas/block-storage-volume"
+                                            },
+                                            "type": "array"
+                                        }
+                                    },
+                                    "type": "object"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "List block storage volumes",
+                "tags": [
+                    "block-storage"
+                ]
+            },
+            "post": {
+                "description": "",
+                "operationId": "create-block-storage-volume",
+                "parameters": [],
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "properties": {
+                                    "block-storage-snapshot": {
+                                        "$ref": "#/components/schemas/block-storage-snapshot-target",
+                                        "description": "Block storage snapshot"
+                                    },
+                                    "labels": {
+                                        "$ref": "#/components/schemas/labels",
+                                        "description": "Resource labels"
+                                    },
+                                    "name": {
+                                        "description": "Volume name",
+                                        "maxLength": 255,
+                                        "type": "string"
+                                    },
+                                    "size": {
+                                        "description": "Volume size in GB.\n                            When a snapshot ID is supplied, this defaults to the size of the source volume, but can be set to a larger value.",
+                                        "exclusiveMinimum": false,
+                                        "format": "int64",
+                                        "minimum": 10,
+                                        "type": "integer"
+                                    }
+                                },
+                                "type": "object"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Create a block storage volume",
+                "tags": [
+                    "block-storage"
+                ]
+            }
+        },
+        "/block-storage-snapshot": {
+            "get": {
+                "description": "",
+                "operationId": "list-block-storage-snapshots",
+                "parameters": [],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "properties": {
+                                        "block-storage-snapshots": {
+                                            "items": {
+                                                "$ref": "#/components/schemas/block-storage-snapshot"
+                                            },
+                                            "type": "array"
+                                        }
+                                    },
+                                    "type": "object"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "List block storage snapshots",
+                "tags": [
+                    "block-storage"
+                ]
+            }
+        },
+        "/block-storage-snapshot/{id}": {
+            "delete": {
+                "description": "",
+                "operationId": "delete-block-storage-snapshot",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "id",
+                        "required": true,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Delete a block storage snapshot, data will be unrecoverable",
+                "tags": [
+                    "block-storage"
+                ]
+            },
+            "get": {
+                "description": "",
+                "operationId": "get-block-storage-snapshot",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "id",
+                        "required": true,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/block-storage-snapshot"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Retrieve block storage snapshot details",
+                "tags": [
+                    "block-storage"
+                ]
+            },
+            "put": {
+                "description": "",
+                "operationId": "update-block-storage-snapshot",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "id",
+                        "required": true,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "properties": {
+                                    "labels": {
+                                        "$ref": "#/components/schemas/labels",
+                                        "description": "Resource labels",
+                                        "nullable": true
+                                    },
+                                    "name": {
+                                        "description": "Snapshot name",
+                                        "maxLength": 255,
+                                        "nullable": true,
+                                        "type": "string"
+                                    }
+                                },
+                                "type": "object"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Update block storage volume snapshot",
+                "tags": [
+                    "block-storage"
+                ]
+            }
+        },
+        "/block-storage/{id}": {
+            "delete": {
+                "description": "",
+                "operationId": "delete-block-storage-volume",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "id",
+                        "required": true,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Delete a block storage volume, data will be unrecoverable",
+                "tags": [
+                    "block-storage"
+                ]
+            },
+            "get": {
+                "description": "",
+                "operationId": "get-block-storage-volume",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "id",
+                        "required": true,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/block-storage-volume"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Retrieve block storage volume details",
+                "tags": [
+                    "block-storage"
+                ]
+            },
+            "put": {
+                "description": "",
+                "operationId": "update-block-storage-volume",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "id",
+                        "required": true,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "properties": {
+                                    "labels": {
+                                        "$ref": "#/components/schemas/labels",
+                                        "description": "Resource labels",
+                                        "nullable": true
+                                    },
+                                    "name": {
+                                        "description": "Volume name",
+                                        "maxLength": 255,
+                                        "nullable": true,
+                                        "type": "string"
+                                    }
+                                },
+                                "type": "object"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Update block storage volume",
+                "tags": [
+                    "block-storage"
+                ]
+            }
+        },
+        "/block-storage/{id}:attach": {
+            "put": {
+                "description": "",
+                "operationId": "attach-block-storage-volume-to-instance",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "id",
+                        "required": true,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "properties": {
+                                    "instance": {
+                                        "$ref": "#/components/schemas/instance-target",
+                                        "description": "Instance to attach to, this can only be done if the volume is not currently attached"
+                                    }
+                                },
+                                "required": [
+                                    "instance"
+                                ],
+                                "type": "object"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Attach block storage volume to an instance",
+                "tags": [
+                    "block-storage"
+                ]
+            }
+        },
+        "/block-storage/{id}:create-snapshot": {
+            "post": {
+                "description": "",
+                "operationId": "create-block-storage-snapshot",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "id",
+                        "required": true,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "properties": {
+                                    "labels": {
+                                        "$ref": "#/components/schemas/labels",
+                                        "description": "Resource labels"
+                                    },
+                                    "name": {
+                                        "description": "Snapshot name",
+                                        "maxLength": 255,
+                                        "minLength": 1,
+                                        "type": "string"
+                                    }
+                                },
+                                "type": "object"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Create a block storage snapshot",
+                "tags": [
+                    "block-storage"
+                ]
+            }
+        },
+        "/block-storage/{id}:detach": {
+            "put": {
+                "description": "",
+                "operationId": "detach-block-storage-volume",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "id",
+                        "required": true,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Detach block storage volume",
+                "tags": [
+                    "block-storage"
+                ]
+            }
+        },
+        "/block-storage/{id}:resize-volume": {
+            "put": {
+                "description": "This operation resizes a Block storage volume. Note: the volume can only grow, cannot be shrunk.",
+                "operationId": "resize-block-storage-volume",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "id",
+                        "required": true,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "properties": {
+                                    "size": {
+                                        "description": "Volume size in GB",
+                                        "exclusiveMinimum": false,
+                                        "format": "int64",
+                                        "minimum": 11,
+                                        "type": "integer"
+                                    }
+                                },
+                                "required": [
+                                    "size"
+                                ],
+                                "type": "object"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/block-storage-volume"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Resize a block storage volume",
+                "tags": [
+                    "block-storage"
+                ]
+            }
+        },
         "/dbaas-ca-certificate": {
             "get": {
                 "description": "Returns a CA Certificate required to reach a DBaaS service through a TLS-protected connection.",
                 "operationId": "get-dbaas-ca-certificate",
                 "parameters": [],
                 "responses": {
                     "200": {
@@ -5577,44 +8936,16 @@
                             "schema": {
                                 "properties": {
                                     "fork-from-service": {
                                         "$ref": "#/components/schemas/dbaas-service-name",
                                         "description": "Service to fork from"
                                     },
                                     "grafana-settings": {
-                                        "description": "Grafana specific settings",
-                                        "type": "object"
-                                    },
-                                    "integrations": {
-                                        "description": "Service integrations to enable for the service. Some integration types affect how a service is created and they must be provided as part of the creation call instead of being defined later.",
-                                        "items": {
-                                            "properties": {
-                                                "dest-service": {
-                                                    "$ref": "#/components/schemas/dbaas-service-name",
-                                                    "description": "A destination service"
-                                                },
-                                                "settings": {
-                                                    "description": "Integration settings",
-                                                    "type": "object"
-                                                },
-                                                "source-service": {
-                                                    "$ref": "#/components/schemas/dbaas-service-name",
-                                                    "description": "A source service"
-                                                },
-                                                "type": {
-                                                    "$ref": "#/components/schemas/enum-integration-types",
-                                                    "description": "Integration type"
-                                                }
-                                            },
-                                            "required": [
-                                                "type"
-                                            ],
-                                            "type": "object"
-                                        },
-                                        "type": "array"
+                                        "$ref": "#/components/schemas/json-schema-grafana",
+                                        "description": "Grafana specific settings"
                                     },
                                     "ip-filter": {
                                         "description": "Allowed CIDR address blocks for incoming connections",
                                         "items": {
                                             "type": "string"
                                         },
                                         "type": "array"
@@ -5701,16 +9032,16 @@
                 ],
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "grafana-settings": {
-                                        "description": "Grafana specific settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-grafana",
+                                        "description": "Grafana specific settings"
                                     },
                                     "ip-filter": {
                                         "description": "Allowed CIDR address blocks for incoming connections",
                                         "items": {
                                             "type": "string"
                                         },
                                         "type": "array"
@@ -5823,17 +9154,16 @@
                             "schema": {
                                 "properties": {
                                     "dest-service": {
                                         "$ref": "#/components/schemas/dbaas-service-name",
                                         "description": "A destination service"
                                     },
                                     "integration-type": {
-                                        "description": "Integration type",
-                                        "minLength": 1,
-                                        "type": "string"
+                                        "$ref": "#/components/schemas/enum-integration-types",
+                                        "description": "Integration type"
                                     },
                                     "settings": {
                                         "description": "Integration settings",
                                         "type": "object"
                                     },
                                     "source-service": {
                                         "$ref": "#/components/schemas/dbaas-service-name",
@@ -6171,68 +9501,40 @@
                                             "sasl": {
                                                 "description": "Enable SASL authentication",
                                                 "type": "boolean"
                                             }
                                         },
                                         "type": "object"
                                     },
-                                    "integrations": {
-                                        "description": "Service integrations to enable for the service. Some integration types affect how a service is created and they must be provided as part of the creation call instead of being defined later.",
-                                        "items": {
-                                            "properties": {
-                                                "dest-service": {
-                                                    "$ref": "#/components/schemas/dbaas-service-name",
-                                                    "description": "A destination service"
-                                                },
-                                                "settings": {
-                                                    "description": "Integration settings",
-                                                    "type": "object"
-                                                },
-                                                "source-service": {
-                                                    "$ref": "#/components/schemas/dbaas-service-name",
-                                                    "description": "A source service"
-                                                },
-                                                "type": {
-                                                    "$ref": "#/components/schemas/enum-integration-types",
-                                                    "description": "Integration type"
-                                                }
-                                            },
-                                            "required": [
-                                                "type"
-                                            ],
-                                            "type": "object"
-                                        },
-                                        "type": "array"
-                                    },
                                     "ip-filter": {
                                         "description": "Allow incoming connections from CIDR address block, e.g. '10.20.0.0/16'",
                                         "items": {
                                             "type": "string"
                                         },
                                         "type": "array"
                                     },
                                     "kafka-connect-enabled": {
                                         "description": "Allow clients to connect to kafka_connect from the public internet for service nodes that are in a project VPC or another type of private network",
                                         "type": "boolean"
                                     },
                                     "kafka-connect-settings": {
-                                        "description": "Kafka Connect configuration values",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-kafka-connect",
+                                        "description": "Kafka Connect configuration values"
                                     },
                                     "kafka-rest-enabled": {
                                         "description": "Enable Kafka-REST service",
                                         "type": "boolean"
                                     },
                                     "kafka-rest-settings": {
-                                        "description": "Kafka REST configuration",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-kafka-rest",
+                                        "description": "Kafka REST configuration"
                                     },
                                     "kafka-settings": {
-                                        "description": "Kafka-specific settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-kafka",
+                                        "description": "Kafka-specific settings"
                                     },
                                     "maintenance": {
                                         "description": "Automatic maintenance settings",
                                         "properties": {
                                             "dow": {
                                                 "description": "Day of week for installing updates",
                                                 "enum": [
@@ -6267,16 +9569,16 @@
                                         "type": "string"
                                     },
                                     "schema-registry-enabled": {
                                         "description": "Enable Schema-Registry service",
                                         "type": "boolean"
                                     },
                                     "schema-registry-settings": {
-                                        "description": "Schema Registry configuration",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-schema-registry",
+                                        "description": "Schema Registry configuration"
                                     },
                                     "termination-protection": {
                                         "description": "Service is protected against termination and powering off",
                                         "type": "boolean"
                                     },
                                     "version": {
                                         "description": "Kafka major version",
@@ -6350,28 +9652,28 @@
                                         "type": "array"
                                     },
                                     "kafka-connect-enabled": {
                                         "description": "Allow clients to connect to kafka_connect from the public internet for service nodes that are in a project VPC or another type of private network",
                                         "type": "boolean"
                                     },
                                     "kafka-connect-settings": {
-                                        "description": "Kafka Connect configuration values",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-kafka-connect",
+                                        "description": "Kafka Connect configuration values"
                                     },
                                     "kafka-rest-enabled": {
                                         "description": "Enable Kafka-REST service",
                                         "type": "boolean"
                                     },
                                     "kafka-rest-settings": {
-                                        "description": "Kafka REST configuration",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-kafka-rest",
+                                        "description": "Kafka REST configuration"
                                     },
                                     "kafka-settings": {
-                                        "description": "Kafka-specific settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-kafka",
+                                        "description": "Kafka-specific settings"
                                     },
                                     "maintenance": {
                                         "description": "Automatic maintenance settings",
                                         "properties": {
                                             "dow": {
                                                 "description": "Day of week for installing updates",
                                                 "enum": [
@@ -6406,20 +9708,25 @@
                                         "type": "string"
                                     },
                                     "schema-registry-enabled": {
                                         "description": "Enable Schema-Registry service",
                                         "type": "boolean"
                                     },
                                     "schema-registry-settings": {
-                                        "description": "Schema Registry configuration",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-schema-registry",
+                                        "description": "Schema Registry configuration"
                                     },
                                     "termination-protection": {
                                         "description": "Service is protected against termination and powering off",
                                         "type": "boolean"
+                                    },
+                                    "version": {
+                                        "description": "Kafka major version",
+                                        "minLength": 1,
+                                        "type": "string"
                                     }
                                 },
                                 "type": "object"
                             }
                         }
                     },
                     "required": true
@@ -6813,14 +10120,54 @@
                 },
                 "summary": "Reset the credentials of a DBaaS Kafka user",
                 "tags": [
                     "dbaas"
                 ]
             }
         },
+        "/dbaas-kafka/{service-name}/user/{username}/password/reveal": {
+            "get": {
+                "description": null,
+                "operationId": "reveal-dbaas-kafka-user-password",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "service-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-service-name"
+                        }
+                    },
+                    {
+                        "in": "path",
+                        "name": "username",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-user-username"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/dbaas-user-kafka-secrets"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Reveal the secrets of a DBaaS Kafka user",
+                "tags": [
+                    "dbaas"
+                ]
+            }
+        },
         "/dbaas-migration-status/{name}": {
             "get": {
                 "description": "Get a DBaaS migration status",
                 "operationId": "get-dbaas-migration-status",
                 "parameters": [
                     {
                         "in": "path",
@@ -6975,15 +10322,15 @@
                                         "type": "integer"
                                     },
                                     "fork-from-service": {
                                         "$ref": "#/components/schemas/dbaas-service-name",
                                         "description": "Service to fork from"
                                     },
                                     "integrations": {
-                                        "description": "Service integrations to enable for the service. Some integration types affect how a service is created and they must be provided as part of the creation call instead of being defined later.",
+                                        "description": "Service integrations to be enabled when creating the service.",
                                         "items": {
                                             "properties": {
                                                 "dest-service": {
                                                     "$ref": "#/components/schemas/dbaas-service-name",
                                                     "description": "A destination service"
                                                 },
                                                 "settings": {
@@ -6991,16 +10338,19 @@
                                                     "type": "object"
                                                 },
                                                 "source-service": {
                                                     "$ref": "#/components/schemas/dbaas-service-name",
                                                     "description": "A source service"
                                                 },
                                                 "type": {
-                                                    "$ref": "#/components/schemas/enum-integration-types",
-                                                    "description": "Integration type"
+                                                    "description": "Integration type",
+                                                    "enum": [
+                                                        "read_replica"
+                                                    ],
+                                                    "type": "string"
                                                 }
                                             },
                                             "required": [
                                                 "type"
                                             ],
                                             "type": "object"
                                         },
@@ -7097,16 +10447,16 @@
                                         "required": [
                                             "host",
                                             "port"
                                         ],
                                         "type": "object"
                                     },
                                     "mysql-settings": {
-                                        "description": "MySQL-specific settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-mysql",
+                                        "description": "MySQL-specific settings"
                                     },
                                     "plan": {
                                         "description": "Subscription plan",
                                         "maxLength": 128,
                                         "minLength": 1,
                                         "type": "string"
                                     },
@@ -7292,16 +10642,16 @@
                                         "required": [
                                             "host",
                                             "port"
                                         ],
                                         "type": "object"
                                     },
                                     "mysql-settings": {
-                                        "description": "MySQL-specific settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-mysql",
+                                        "description": "MySQL-specific settings"
                                     },
                                     "plan": {
                                         "description": "Subscription plan",
                                         "maxLength": 128,
                                         "minLength": 1,
                                         "type": "string"
                                     },
@@ -7394,14 +10744,105 @@
                 },
                 "summary": "Stop a DBaaS MySQL migration",
                 "tags": [
                     "dbaas"
                 ]
             }
         },
+        "/dbaas-mysql/{service-name}/database": {
+            "post": {
+                "description": null,
+                "operationId": "create-dbaas-mysql-database",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "service-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-service-name"
+                        }
+                    }
+                ],
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "properties": {
+                                    "database-name": {
+                                        "$ref": "#/components/schemas/dbaas-database-name",
+                                        "description": "Service database name"
+                                    }
+                                },
+                                "required": [
+                                    "database-name"
+                                ],
+                                "type": "object"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Create a DBaaS MySQL database",
+                "tags": [
+                    "dbaas"
+                ]
+            }
+        },
+        "/dbaas-mysql/{service-name}/database/{database-name}": {
+            "delete": {
+                "description": null,
+                "operationId": "delete-dbaas-mysql-database",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "service-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-service-name"
+                        }
+                    },
+                    {
+                        "in": "path",
+                        "name": "database-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-mysql-database-name"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Delete a DBaaS MySQL database",
+                "tags": [
+                    "dbaas"
+                ]
+            }
+        },
         "/dbaas-mysql/{service-name}/user": {
             "post": {
                 "description": null,
                 "operationId": "create-dbaas-mysql-user",
                 "parameters": [
                     {
                         "in": "path",
@@ -7549,14 +10990,54 @@
                 },
                 "summary": "Reset the credentials of a DBaaS mysql user",
                 "tags": [
                     "dbaas"
                 ]
             }
         },
+        "/dbaas-mysql/{service-name}/user/{username}/password/reveal": {
+            "get": {
+                "description": null,
+                "operationId": "reveal-dbaas-mysql-user-password",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "service-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-service-name"
+                        }
+                    },
+                    {
+                        "in": "path",
+                        "name": "username",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-user-username"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/dbaas-user-mysql-secrets"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Reveal the secrets of a DBaaS MySQL user",
+                "tags": [
+                    "dbaas"
+                ]
+            }
+        },
         "/dbaas-opensearch/{name}": {
             "delete": {
                 "description": null,
                 "operationId": "delete-dbaas-service-opensearch",
                 "parameters": [
                     {
                         "in": "path",
@@ -7694,42 +11175,14 @@
                                                 "maximum": 1024,
                                                 "minimum": 1,
                                                 "type": "integer"
                                             }
                                         },
                                         "type": "object"
                                     },
-                                    "integrations": {
-                                        "description": "Service integrations to enable for the service. Some integration types affect how a service is created and they must be provided as part of the creation call instead of being defined later.",
-                                        "items": {
-                                            "properties": {
-                                                "dest-service": {
-                                                    "$ref": "#/components/schemas/dbaas-service-name",
-                                                    "description": "A destination service"
-                                                },
-                                                "settings": {
-                                                    "description": "Integration settings",
-                                                    "type": "object"
-                                                },
-                                                "source-service": {
-                                                    "$ref": "#/components/schemas/dbaas-service-name",
-                                                    "description": "A source service"
-                                                },
-                                                "type": {
-                                                    "$ref": "#/components/schemas/enum-integration-types",
-                                                    "description": "Integration type"
-                                                }
-                                            },
-                                            "required": [
-                                                "type"
-                                            ],
-                                            "type": "object"
-                                        },
-                                        "type": "array"
-                                    },
                                     "ip-filter": {
                                         "description": "Allow incoming connections from CIDR address block, e.g. '10.20.0.0/16'",
                                         "items": {
                                             "type": "string"
                                         },
                                         "type": "array"
                                     },
@@ -7799,16 +11252,16 @@
                                                 "minimum": 5000,
                                                 "type": "integer"
                                             }
                                         },
                                         "type": "object"
                                     },
                                     "opensearch-settings": {
-                                        "description": "OpenSearch-specific settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-opensearch",
+                                        "description": "OpenSearch-specific settings"
                                     },
                                     "plan": {
                                         "description": "Subscription plan",
                                         "maxLength": 128,
                                         "minLength": 1,
                                         "type": "string"
                                     },
@@ -8006,16 +11459,16 @@
                                                 "minimum": 5000,
                                                 "type": "integer"
                                             }
                                         },
                                         "type": "object"
                                     },
                                     "opensearch-settings": {
-                                        "description": "OpenSearch-specific settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-opensearch",
+                                        "description": "OpenSearch-specific settings"
                                     },
                                     "plan": {
                                         "description": "Subscription plan",
                                         "maxLength": 128,
                                         "minLength": 1,
                                         "type": "string"
                                     },
@@ -8299,14 +11752,54 @@
                 },
                 "summary": "Reset the credentials of a DBaaS OpenSearch user",
                 "tags": [
                     "dbaas"
                 ]
             }
         },
+        "/dbaas-opensearch/{service-name}/user/{username}/password/reveal": {
+            "get": {
+                "description": null,
+                "operationId": "reveal-dbaas-opensearch-user-password",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "service-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-service-name"
+                        }
+                    },
+                    {
+                        "in": "path",
+                        "name": "username",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-user-username"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/dbaas-user-opensearch-secrets"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Reveal the secrets of a DBaaS OpenSearch user",
+                "tags": [
+                    "dbaas"
+                ]
+            }
+        },
         "/dbaas-postgres/{name}": {
             "delete": {
                 "description": null,
                 "operationId": "delete-dbaas-service-pg",
                 "parameters": [
                     {
                         "in": "path",
@@ -8420,15 +11913,15 @@
                                         "type": "object"
                                     },
                                     "fork-from-service": {
                                         "$ref": "#/components/schemas/dbaas-service-name",
                                         "description": "Service to fork from"
                                     },
                                     "integrations": {
-                                        "description": "Service integrations to enable for the service. Some integration types affect how a service is created and they must be provided as part of the creation call instead of being defined later.",
+                                        "description": "Service integrations to be enabled when creating the service.",
                                         "items": {
                                             "properties": {
                                                 "dest-service": {
                                                     "$ref": "#/components/schemas/dbaas-service-name",
                                                     "description": "A destination service"
                                                 },
                                                 "settings": {
@@ -8436,16 +11929,19 @@
                                                     "type": "object"
                                                 },
                                                 "source-service": {
                                                     "$ref": "#/components/schemas/dbaas-service-name",
                                                     "description": "A source service"
                                                 },
                                                 "type": {
-                                                    "$ref": "#/components/schemas/enum-integration-types",
-                                                    "description": "Integration type"
+                                                    "description": "Integration type",
+                                                    "enum": [
+                                                        "read_replica"
+                                                    ],
+                                                    "type": "string"
                                                 }
                                             },
                                             "required": [
                                                 "type"
                                             ],
                                             "type": "object"
                                         },
@@ -8542,24 +12038,24 @@
                                         "required": [
                                             "host",
                                             "port"
                                         ],
                                         "type": "object"
                                     },
                                     "pg-settings": {
-                                        "description": "PostgreSQL-specific settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-pg",
+                                        "description": "PostgreSQL-specific settings"
                                     },
                                     "pgbouncer-settings": {
-                                        "description": "PGBouncer connection pooling settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-pgbouncer",
+                                        "description": "PGBouncer connection pooling settings"
                                     },
                                     "pglookout-settings": {
-                                        "description": "PGLookout settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-pglookout",
+                                        "description": "PGLookout settings"
                                     },
                                     "plan": {
                                         "description": "Subscription plan",
                                         "maxLength": 128,
                                         "minLength": 1,
                                         "type": "string"
                                     },
@@ -8582,25 +12078,24 @@
                                         "description": "Synchronous replication type. Note that the service plan also needs to support synchronous replication."
                                     },
                                     "termination-protection": {
                                         "description": "Service is protected against termination and powering off",
                                         "type": "boolean"
                                     },
                                     "timescaledb-settings": {
-                                        "description": "TimescaleDB extension configuration values",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-timescaledb",
+                                        "description": "TimescaleDB extension configuration values"
                                     },
                                     "variant": {
                                         "$ref": "#/components/schemas/enum-pg-variant",
                                         "description": "Variant of the PostgreSQL service, may affect the features that are exposed by default"
                                     },
                                     "version": {
-                                        "description": "PostgreSQL major version",
-                                        "minLength": 1,
-                                        "type": "string"
+                                        "$ref": "#/components/schemas/dbaas-pg-target-versions",
+                                        "description": "PostgreSQL major version"
                                     },
                                     "work-mem": {
                                         "description": "Sets the maximum amount of memory to be used by a query operation (such as a sort or hash table) before writing to temporary disk files, in MB. Default is 1MB + 0.075% of total RAM (up to 32MB).",
                                         "exclusiveMaximum": false,
                                         "exclusiveMinimum": false,
                                         "format": "int64",
                                         "maximum": 1024,
@@ -8766,24 +12261,24 @@
                                         "required": [
                                             "host",
                                             "port"
                                         ],
                                         "type": "object"
                                     },
                                     "pg-settings": {
-                                        "description": "PostgreSQL-specific settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-pg",
+                                        "description": "PostgreSQL-specific settings"
                                     },
                                     "pgbouncer-settings": {
-                                        "description": "PGBouncer connection pooling settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-pgbouncer",
+                                        "description": "PGBouncer connection pooling settings"
                                     },
                                     "pglookout-settings": {
-                                        "description": "PGLookout settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-pglookout",
+                                        "description": "PGLookout settings"
                                     },
                                     "plan": {
                                         "description": "Subscription plan",
                                         "maxLength": 128,
                                         "minLength": 1,
                                         "type": "string"
                                     },
@@ -8801,16 +12296,16 @@
                                         "description": "Synchronous replication type. Note that the service plan also needs to support synchronous replication."
                                     },
                                     "termination-protection": {
                                         "description": "Service is protected against termination and powering off",
                                         "type": "boolean"
                                     },
                                     "timescaledb-settings": {
-                                        "description": "TimescaleDB extension configuration values",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-timescaledb",
+                                        "description": "TimescaleDB extension configuration values"
                                     },
                                     "variant": {
                                         "$ref": "#/components/schemas/enum-pg-variant",
                                         "description": "Variant of the PostgreSQL service, may affect the features that are exposed by default"
                                     },
                                     "version": {
                                         "description": "Version",
@@ -8930,15 +12425,15 @@
                 ],
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "database-name": {
-                                        "$ref": "#/components/schemas/dbaas-pg-database-name",
+                                        "$ref": "#/components/schemas/dbaas-database-name",
                                         "description": "Service database name"
                                     },
                                     "mode": {
                                         "$ref": "#/components/schemas/enum-pg-pool-mode",
                                         "description": "PGBouncer pool mode"
                                     },
                                     "name": {
@@ -9044,15 +12539,15 @@
                 ],
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "database-name": {
-                                        "$ref": "#/components/schemas/dbaas-pg-database-name",
+                                        "$ref": "#/components/schemas/dbaas-database-name",
                                         "description": "Service database name"
                                     },
                                     "mode": {
                                         "$ref": "#/components/schemas/enum-pg-pool-mode",
                                         "description": "PGBouncer pool mode"
                                     },
                                     "size": {
@@ -9084,14 +12579,115 @@
                 },
                 "summary": "Update a DBaaS PostgreSQL connection pool",
                 "tags": [
                     "dbaas"
                 ]
             }
         },
+        "/dbaas-postgres/{service-name}/database": {
+            "post": {
+                "description": null,
+                "operationId": "create-dbaas-pg-database",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "service-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-service-name"
+                        }
+                    }
+                ],
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "properties": {
+                                    "database-name": {
+                                        "$ref": "#/components/schemas/dbaas-database-name",
+                                        "description": "Service database name"
+                                    },
+                                    "lc-collate": {
+                                        "description": "Default string sort order (LC_COLLATE) for PostgreSQL database",
+                                        "maxLength": 128,
+                                        "type": "string"
+                                    },
+                                    "lc-ctype": {
+                                        "description": "Default character classification (LC_CTYPE) for PostgreSQL database",
+                                        "maxLength": 128,
+                                        "type": "string"
+                                    }
+                                },
+                                "required": [
+                                    "database-name"
+                                ],
+                                "type": "object"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Create a DBaaS Postgres database",
+                "tags": [
+                    "dbaas"
+                ]
+            }
+        },
+        "/dbaas-postgres/{service-name}/database/{database-name}": {
+            "delete": {
+                "description": null,
+                "operationId": "delete-dbaas-pg-database",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "service-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-service-name"
+                        }
+                    },
+                    {
+                        "in": "path",
+                        "name": "database-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-pg-database-name"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Delete a DBaaS Postgres database",
+                "tags": [
+                    "dbaas"
+                ]
+            }
+        },
         "/dbaas-postgres/{service-name}/user": {
             "post": {
                 "description": null,
                 "operationId": "create-dbaas-postgres-user",
                 "parameters": [
                     {
                         "in": "path",
@@ -9289,14 +12885,54 @@
                 },
                 "summary": "Reset the credentials of a DBaaS Postgres user",
                 "tags": [
                     "dbaas"
                 ]
             }
         },
+        "/dbaas-postgres/{service-name}/user/{username}/password/reveal": {
+            "get": {
+                "description": null,
+                "operationId": "reveal-dbaas-postgres-user-password",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "service-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-service-name"
+                        }
+                    },
+                    {
+                        "in": "path",
+                        "name": "username",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-user-username"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/dbaas-user-postgres-secrets"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Reveal the secrets of a DBaaS Postgres user",
+                "tags": [
+                    "dbaas"
+                ]
+            }
+        },
         "/dbaas-postgres/{service}/upgrade-check": {
             "post": {
                 "description": "Check whether you can upgrade Postgres service to a newer version",
                 "operationId": "create-dbaas-pg-upgrade-check",
                 "parameters": [
                     {
                         "in": "path",
@@ -9309,23 +12945,16 @@
                 ],
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "target-version": {
-                                        "description": "Target version for upgrade",
-                                        "enum": [
-                                            "11",
-                                            "12",
-                                            "13",
-                                            "14",
-                                            "15"
-                                        ],
-                                        "type": "string"
+                                        "$ref": "#/components/schemas/dbaas-pg-target-versions",
+                                        "description": "Target version for upgrade"
                                     }
                                 },
                                 "required": [
                                     "target-version"
                                 ],
                                 "type": "object"
                             }
@@ -9430,42 +13059,14 @@
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "fork-from-service": {
                                         "$ref": "#/components/schemas/dbaas-service-name",
                                         "description": "Service to fork from"
                                     },
-                                    "integrations": {
-                                        "description": "Service integrations to enable for the service. Some integration types affect how a service is created and they must be provided as part of the creation call instead of being defined later.",
-                                        "items": {
-                                            "properties": {
-                                                "dest-service": {
-                                                    "$ref": "#/components/schemas/dbaas-service-name",
-                                                    "description": "A destination service"
-                                                },
-                                                "settings": {
-                                                    "description": "Integration settings",
-                                                    "type": "object"
-                                                },
-                                                "source-service": {
-                                                    "$ref": "#/components/schemas/dbaas-service-name",
-                                                    "description": "A source service"
-                                                },
-                                                "type": {
-                                                    "$ref": "#/components/schemas/enum-integration-types",
-                                                    "description": "Integration type"
-                                                }
-                                            },
-                                            "required": [
-                                                "type"
-                                            ],
-                                            "type": "object"
-                                        },
-                                        "type": "array"
-                                    },
                                     "ip-filter": {
                                         "description": "Allow incoming connections from CIDR address block, e.g. '10.20.0.0/16'",
                                         "items": {
                                             "type": "string"
                                         },
                                         "type": "array"
                                     },
@@ -9564,16 +13165,16 @@
                                     },
                                     "recovery-backup-name": {
                                         "description": "Name of a backup to recover from for services that support backup names",
                                         "minLength": 1,
                                         "type": "string"
                                     },
                                     "redis-settings": {
-                                        "description": "Redis.conf settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-redis",
+                                        "description": "Redis.conf settings"
                                     },
                                     "termination-protection": {
                                         "description": "Service is protected against termination and powering off",
                                         "type": "boolean"
                                     }
                                 },
                                 "required": [
@@ -9717,16 +13318,16 @@
                                     "plan": {
                                         "description": "Subscription plan",
                                         "maxLength": 128,
                                         "minLength": 1,
                                         "type": "string"
                                     },
                                     "redis-settings": {
-                                        "description": "Redis.conf settings",
-                                        "type": "object"
+                                        "$ref": "#/components/schemas/json-schema-redis",
+                                        "description": "Redis.conf settings"
                                     },
                                     "termination-protection": {
                                         "description": "Service is protected against termination and powering off",
                                         "type": "boolean"
                                     }
                                 },
                                 "type": "object"
@@ -9813,14 +13414,201 @@
                 },
                 "summary": "Stop a DBaaS Redis migration",
                 "tags": [
                     "dbaas"
                 ]
             }
         },
+        "/dbaas-redis/{service-name}/user": {
+            "post": {
+                "description": null,
+                "operationId": "create-dbaas-redis-user",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "service-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-service-name"
+                        }
+                    }
+                ],
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "properties": {
+                                    "username": {
+                                        "$ref": "#/components/schemas/dbaas-user-username",
+                                        "description": "Username"
+                                    }
+                                },
+                                "required": [
+                                    "username"
+                                ],
+                                "type": "object"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Create a DBaaS Redis user",
+                "tags": [
+                    "dbaas"
+                ]
+            }
+        },
+        "/dbaas-redis/{service-name}/user/{username}": {
+            "delete": {
+                "description": null,
+                "operationId": "delete-dbaas-redis-user",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "service-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-service-name"
+                        }
+                    },
+                    {
+                        "in": "path",
+                        "name": "username",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-user-username"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Delete a DBaaS Redis user",
+                "tags": [
+                    "dbaas"
+                ]
+            }
+        },
+        "/dbaas-redis/{service-name}/user/{username}/password/reset": {
+            "put": {
+                "description": "If no password is provided one will be generated automatically.",
+                "operationId": "reset-dbaas-redis-user-password",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "service-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-service-name"
+                        }
+                    },
+                    {
+                        "in": "path",
+                        "name": "username",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-user-username"
+                        }
+                    }
+                ],
+                "requestBody": {
+                    "content": {
+                        "application/json": {
+                            "schema": {
+                                "properties": {
+                                    "password": {
+                                        "$ref": "#/components/schemas/dbaas-user-password",
+                                        "description": "New password"
+                                    }
+                                },
+                                "type": "object"
+                            }
+                        }
+                    },
+                    "required": true
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Reset the credentials of a DBaaS Redis user",
+                "tags": [
+                    "dbaas"
+                ]
+            }
+        },
+        "/dbaas-redis/{service-name}/user/{username}/password/reveal": {
+            "get": {
+                "description": null,
+                "operationId": "reveal-dbaas-redis-user-password",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "service-name",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-service-name"
+                        }
+                    },
+                    {
+                        "in": "path",
+                        "name": "username",
+                        "required": true,
+                        "schema": {
+                            "$ref": "#/components/schemas/dbaas-user-username"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/dbaas-user-redis-secrets"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Reveal the secrets of a DBaaS Redis user",
+                "tags": [
+                    "dbaas"
+                ]
+            }
+        },
         "/dbaas-service": {
             "get": {
                 "description": "List DBaaS services",
                 "operationId": "list-dbaas-services",
                 "parameters": [],
                 "responses": {
                     "200": {
@@ -10782,23 +14570,19 @@
                                         "description": "DNS domain record type",
                                         "enum": [
                                             "A",
                                             "AAAA",
                                             "ALIAS",
                                             "CAA",
                                             "CNAME",
-                                            "DNSKEY",
-                                            "DS",
                                             "HINFO",
                                             "MX",
                                             "NAPTR",
                                             "NS",
                                             "POOL",
-                                            "PTR",
-                                            "SOA",
                                             "SPF",
                                             "SRV",
                                             "SSHFP",
                                             "TXT",
                                             "URL"
                                         ],
                                         "type": "string"
@@ -11145,15 +14929,15 @@
                                     },
                                     "healthcheck": {
                                         "$ref": "#/components/schemas/elastic-ip-healthcheck",
                                         "description": "Elastic IP healthcheck"
                                     },
                                     "labels": {
                                         "$ref": "#/components/schemas/labels",
-                                        "description": "Elastic IP labels"
+                                        "description": "Resource labels"
                                     }
                                 },
                                 "type": "object"
                             }
                         }
                     },
                     "required": true
@@ -11265,15 +15049,15 @@
                                     },
                                     "healthcheck": {
                                         "$ref": "#/components/schemas/elastic-ip-healthcheck",
                                         "description": "Elastic IP healthcheck"
                                     },
                                     "labels": {
                                         "$ref": "#/components/schemas/labels",
-                                        "description": "Elastic IP labels"
+                                        "description": "Resource labels"
                                     }
                                 },
                                 "type": "object"
                             }
                         }
                     },
                     "required": true
@@ -11357,15 +15141,15 @@
                 ],
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "instance": {
-                                        "$ref": "#/components/schemas/instance",
+                                        "$ref": "#/components/schemas/instance-target",
                                         "description": "Compute instance"
                                     }
                                 },
                                 "required": [
                                     "instance"
                                 ],
                                 "type": "object"
@@ -11409,15 +15193,15 @@
                 ],
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "instance": {
-                                        "$ref": "#/components/schemas/instance",
+                                        "$ref": "#/components/schemas/instance-target",
                                         "description": "Compute instance"
                                     }
                                 },
                                 "required": [
                                     "instance"
                                 ],
                                 "type": "object"
@@ -11495,18 +15279,15 @@
                 "operationId": "get-iam-organization-policy",
                 "parameters": [],
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
-                                    "items": {
-                                        "$ref": "#/components/schemas/iam-policy"
-                                    },
-                                    "type": "array"
+                                    "$ref": "#/components/schemas/iam-policy"
                                 }
                             }
                         },
                         "description": "200"
                     }
                 },
                 "summary": "Retrieve IAM Organization Policy",
@@ -11583,26 +15364,30 @@
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "description": {
                                         "description": "IAM Role description",
+                                        "maxLength": 255,
+                                        "minLength": 1,
                                         "type": "string"
                                     },
                                     "editable": {
-                                        "description": "Make IAM Role editable (default: true)",
+                                        "description": "Sets if the IAM Role Policy is editable or not (default: true). This setting cannot be changed after creation",
                                         "type": "boolean"
                                     },
                                     "labels": {
                                         "$ref": "#/components/schemas/labels",
                                         "description": "IAM Role labels"
                                     },
                                     "name": {
                                         "description": "IAM Role name",
+                                        "maxLength": 191,
+                                        "minLength": 1,
                                         "type": "string"
                                     },
                                     "permissions": {
                                         "description": "IAM Role permissions",
                                         "items": {
                                             "enum": [
                                                 "bypass-governance-retention"
@@ -11724,14 +15509,16 @@
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "description": {
                                         "description": "IAM Role description",
+                                        "maxLength": 255,
+                                        "minLength": 1,
                                         "type": "string"
                                     },
                                     "labels": {
                                         "$ref": "#/components/schemas/labels",
                                         "description": "IAM Role labels"
                                     },
                                     "permissions": {
@@ -11873,30 +15660,46 @@
                                                     },
                                                     "ipv6-address": {
                                                         "description": "Instance IPv6 address",
                                                         "type": "string"
                                                     },
                                                     "labels": {
                                                         "$ref": "#/components/schemas/labels",
-                                                        "description": "Instance Labels"
+                                                        "description": "Resource labels"
+                                                    },
+                                                    "mac-address": {
+                                                        "description": "Instance MAC address",
+                                                        "type": "string"
                                                     },
                                                     "manager": {
                                                         "$ref": "#/components/schemas/manager",
                                                         "description": "Instance manager"
                                                     },
                                                     "name": {
                                                         "description": "Instance name",
                                                         "maxLength": 255,
                                                         "minLength": 1,
                                                         "type": "string"
                                                     },
                                                     "private-networks": {
                                                         "description": "Instance Private Networks",
                                                         "items": {
-                                                            "$ref": "#/components/schemas/private-network"
+                                                            "description": "Private Network",
+                                                            "properties": {
+                                                                "id": {
+                                                                    "description": "Private Network ID",
+                                                                    "format": "uuid",
+                                                                    "type": "string"
+                                                                },
+                                                                "mac-address": {
+                                                                    "description": "Private Network MAC address",
+                                                                    "type": "string"
+                                                                }
+                                                            },
+                                                            "type": "object"
                                                         },
                                                         "type": "array"
                                                     },
                                                     "public-ip": {
                                                         "description": "Instance public IPv4 address",
                                                         "format": "ipv4",
                                                         "type": "string"
@@ -11920,27 +15723,16 @@
                                                         "description": "Instance SSH Keys",
                                                         "items": {
                                                             "$ref": "#/components/schemas/ssh-key"
                                                         },
                                                         "type": "array"
                                                     },
                                                     "state": {
-                                                        "description": "Instance state",
-                                                        "enum": [
-                                                            "destroyed",
-                                                            "destroying",
-                                                            "error",
-                                                            "expunging",
-                                                            "migrating",
-                                                            "running",
-                                                            "starting",
-                                                            "stopped",
-                                                            "stopping"
-                                                        ],
-                                                        "type": "string"
+                                                        "$ref": "#/components/schemas/instance-state",
+                                                        "description": "Instance state"
                                                     },
                                                     "template": {
                                                         "$ref": "#/components/schemas/template",
                                                         "description": "Instance Template"
                                                     }
                                                 },
                                                 "type": "object"
@@ -12000,15 +15792,15 @@
                                     },
                                     "ipv6-enabled": {
                                         "description": "Enable IPv6. DEPRECATED: use `public-ip-assignments`.",
                                         "type": "boolean"
                                     },
                                     "labels": {
                                         "$ref": "#/components/schemas/labels",
-                                        "description": "Instance Labels"
+                                        "description": "Resource labels"
                                     },
                                     "name": {
                                         "description": "Instance name",
                                         "maxLength": 255,
                                         "minLength": 1,
                                         "type": "string"
                                     },
@@ -12038,14 +15830,15 @@
                                     },
                                     "template": {
                                         "$ref": "#/components/schemas/template",
                                         "description": "Instance Template"
                                     },
                                     "user-data": {
                                         "description": "Instance Cloud-init user-data",
+                                        "maxLength": 32768,
                                         "minLength": 1,
                                         "type": "string"
                                     }
                                 },
                                 "required": [
                                     "disk-size",
                                     "instance-type",
@@ -12783,28 +16576,29 @@
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "labels": {
                                         "$ref": "#/components/schemas/labels",
-                                        "description": "Instance labels"
+                                        "description": "Resource labels"
                                     },
                                     "name": {
                                         "description": "Instance name",
                                         "maxLength": 255,
                                         "minLength": 1,
                                         "type": "string"
                                     },
                                     "public-ip-assignment": {
                                         "$ref": "#/components/schemas/public-ip-assignment",
                                         "description": "Assign public IP to the Instance"
                                     },
                                     "user-data": {
                                         "description": "Instance Cloud-init user-data",
+                                        "maxLength": 32768,
                                         "minLength": 1,
                                         "type": "string"
                                     }
                                 },
                                 "type": "object"
                             }
                         }
@@ -12889,15 +16683,15 @@
                     }
                 ],
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
-                                    "type": "object"
+                                    "$ref": "#/components/schemas/operation"
                                 }
                             }
                         },
                         "description": "200"
                     }
                 },
                 "summary": "Set instance destruction protection",
@@ -13022,15 +16816,15 @@
                     }
                 ],
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
-                                    "type": "object"
+                                    "$ref": "#/components/schemas/operation"
                                 }
                             }
                         },
                         "description": "200"
                     }
                 },
                 "summary": "Remove instance destruction protection",
@@ -13093,14 +16887,47 @@
                 },
                 "summary": "Reset a Compute instance to a base/target template",
                 "tags": [
                     "instance"
                 ]
             }
         },
+        "/instance/{id}:reset-password": {
+            "put": {
+                "description": "",
+                "operationId": "reset-instance-password",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "id",
+                        "required": true,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/operation"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Reset a compute instance password",
+                "tags": [
+                    "instance"
+                ]
+            }
+        },
         "/instance/{id}:resize-disk": {
             "put": {
                 "description": "This operation resizes a Compute instance's disk volume. Note: the disk can only grow, cannot be shrunk.",
                 "operationId": "resize-instance-disk",
                 "parameters": [
                     {
                         "in": "path",
@@ -13506,22 +17333,25 @@
                 ],
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "description": {
+                                        "description": "Load Balancer description",
                                         "maxLength": 255,
                                         "type": "string"
                                     },
                                     "labels": {
                                         "$ref": "#/components/schemas/labels"
                                     },
                                     "name": {
+                                        "description": "Load Balancer name",
                                         "maxLength": 255,
+                                        "minLength": 1,
                                         "type": "string"
                                     }
                                 },
                                 "type": "object"
                             }
                         }
                     },
@@ -14013,15 +17843,15 @@
                                     "end-ip": {
                                         "description": "Private Network end IP address",
                                         "format": "ipv4",
                                         "type": "string"
                                     },
                                     "labels": {
                                         "$ref": "#/components/schemas/labels",
-                                        "description": "Private Network labels"
+                                        "description": "Resource labels"
                                     },
                                     "name": {
                                         "description": "Private Network name",
                                         "maxLength": 255,
                                         "minLength": 1,
                                         "type": "string"
                                     },
@@ -14153,15 +17983,15 @@
                                     "end-ip": {
                                         "description": "Private Network end IP address",
                                         "format": "ipv4",
                                         "type": "string"
                                     },
                                     "labels": {
                                         "$ref": "#/components/schemas/labels",
-                                        "description": "Private Network labels"
+                                        "description": "Resource labels"
                                     },
                                     "name": {
                                         "description": "Private Network name",
                                         "maxLength": 255,
                                         "minLength": 1,
                                         "type": "string"
                                     },
@@ -14377,26 +18207,32 @@
                 ],
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "instance": {
-                                        "$ref": "#/components/schemas/instance",
-                                        "description": "Compute instance"
+                                        "properties": {
+                                            "id": {
+                                                "description": "Instance ID",
+                                                "format": "uuid",
+                                                "type": "string"
+                                            }
+                                        },
+                                        "required": [
+                                            "id"
+                                        ],
+                                        "type": "object"
                                     },
                                     "ip": {
                                         "description": "Static IP address lease for the corresponding network interface",
                                         "format": "ipv4",
                                         "type": "string"
                                     }
                                 },
-                                "required": [
-                                    "instance"
-                                ],
                                 "type": "object"
                             }
                         }
                     },
                     "required": true
                 },
                 "responses": {
@@ -15273,14 +19109,15 @@
                             "schema": {
                                 "properties": {
                                     "addons": {
                                         "description": "Cluster addons",
                                         "items": {
                                             "enum": [
                                                 "exoscale-cloud-controller",
+                                                "exoscale-container-storage-interface",
                                                 "metrics-server"
                                             ],
                                             "type": "string"
                                         },
                                         "type": "array",
                                         "uniqueItems": true
                                     },
@@ -15295,14 +19132,15 @@
                                             "cilium"
                                         ],
                                         "type": "string"
                                     },
                                     "description": {
                                         "description": "Cluster description",
                                         "maxLength": 255,
+                                        "nullable": true,
                                         "type": "string"
                                     },
                                     "labels": {
                                         "$ref": "#/components/schemas/labels",
                                         "description": "Cluster Labels"
                                     },
                                     "level": {
@@ -15564,39 +19402,46 @@
                             "schema": {
                                 "properties": {
                                     "addons": {
                                         "description": "Cluster addons",
                                         "items": {
                                             "enum": [
                                                 "exoscale-cloud-controller",
+                                                "exoscale-container-storage-interface",
                                                 "metrics-server"
                                             ],
                                             "type": "string"
                                         },
                                         "type": "array",
                                         "uniqueItems": true
                                     },
                                     "auto-upgrade": {
                                         "description": "Enable auto upgrade of the control plane to the latest patch version available",
                                         "type": "boolean"
                                     },
                                     "description": {
                                         "description": "Cluster description",
                                         "maxLength": 255,
+                                        "nullable": true,
                                         "type": "string"
                                     },
                                     "labels": {
                                         "$ref": "#/components/schemas/labels",
                                         "description": "Cluster labels"
                                     },
                                     "name": {
                                         "description": "Cluster name",
                                         "maxLength": 255,
                                         "minLength": 1,
                                         "type": "string"
+                                    },
+                                    "oidc": {
+                                        "$ref": "#/components/schemas/sks-oidc",
+                                        "description": "Cluster OpenID configmap",
+                                        "nullable": true
                                     }
                                 },
                                 "type": "object"
                             }
                         }
                     },
                     "required": true
@@ -15666,14 +19511,48 @@
                 },
                 "summary": "Get the certificate for a SKS cluster authority",
                 "tags": [
                     "sks"
                 ]
             }
         },
+        "/sks-cluster/{id}/inspection": {
+            "get": {
+                "description": "Helps troubleshoot common problems when deploying a kubernetes cluster. Inspections run every couple of minutes.",
+                "operationId": "get-sks-cluster-inspection",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "id",
+                        "required": true,
+                        "schema": {
+                            "format": "uuid",
+                            "type": "string"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "additionalProperties": {},
+                                    "type": "object"
+                                }
+                            }
+                        },
+                        "description": "200"
+                    }
+                },
+                "summary": "Get the latest inspection result",
+                "tags": [
+                    "sks"
+                ]
+            }
+        },
         "/sks-cluster/{id}/nodepool": {
             "post": {
                 "description": "",
                 "operationId": "create-sks-nodepool",
                 "parameters": [
                     {
                         "in": "path",
@@ -16704,15 +20583,16 @@
                 "parameters": [],
                 "requestBody": {
                     "content": {
                         "application/json": {
                             "schema": {
                                 "properties": {
                                     "name": {
-                                        "description": "Private Network name",
+                                        "description": "SSH key name",
+                                        "pattern": "^[a-zA-Z]{1}[a-zA-Z0-9._-]{0,254}$",
                                         "type": "string"
                                     },
                                     "public-key": {
                                         "description": "Public key value",
                                         "type": "string"
                                     }
                                 },
@@ -17170,36 +21050,23 @@
         {
             "url": "https://api-{zone}.exoscale.com/v2",
             "variables": {
                 "zone": {
                     "default": "ch-gva-2",
                     "enum": [
                         "at-vie-1",
+                        "at-vie-2",
                         "bg-sof-1",
+                        "ch-dk-2",
                         "ch-gva-2",
-                        "ch-zrh-1",
                         "de-fra-1",
                         "de-muc-1"
                     ]
                 }
             }
-        },
-        {
-            "url": "https://ppapi-{zone}.exoscale.com/v2",
-            "variables": {
-                "zone": {
-                    "default": "ch-gva-2",
-                    "enum": [
-                        "at-vie-1",
-                        "ch-gva-2",
-                        "ch-zrh-1",
-                        "de-fra-1"
-                    ]
-                }
-            }
         }
     ],
     "tags": [
         {
             "description": "\nSecurity Groups are groups of firewall rules that regulate network traffic to and from your Compute instances.\n\n[Read more](https://community.exoscale.com/documentation/compute/security-groups/)",
             "externalDocs": {
                 "description": "Read more",
@@ -17244,14 +21111,22 @@
             "externalDocs": {
                 "description": "Read more",
                 "url": "https://www.exoscale.com/compute/"
             },
             "name": "instances"
         },
         {
+            "description": "\nExoscale's Block Storage offers persistent\nexternally attached volumes for your workloads.",
+            "externalDocs": {
+                "description": "Read more",
+                "url": "https://community.exoscale.com/documentation/compute/"
+            },
+            "name": "block-storage"
+        },
+        {
             "description": "\nSnapshots provide a way to get point-in-time recovery for your Compute instance.\n\n[Read more](https://community.exoscale.com/documentation/compute/snapshots/)",
             "externalDocs": {
                 "description": "Read more",
                 "url": "https://community.exoscale.com/documentation/compute/snapshots/"
             },
             "name": "snapshots"
         },
@@ -17294,16 +21169,16 @@
                 "url": "https://www.exoscale.com/scalable-kubernetes-service/"
             },
             "name": "sks"
         }
     ],
     "x-topics": [
         {
-            "content": "\nIn order to authenticate legitimate users, the Exoscale API requires incoming requests to be signed using valid Exoscale API account credentials with the following mechanism.\n\n## Signature Mechanism\n\nThe *message* (i.e. content) to sign contains several segments concatenated using a line return character (`\\n`).\n\nAll segments must be included and in the described order, including empty ones depending on the context of the request (e.g. no request body).\n\n* Request method and request URL (path only), separated by a space character\n* Request body\n* Request URL parameters (Query String) values, concatenated without separator. The matching parameter names have to be specified in the resulting signature header `signed-query-args=` pragma, separated by semicolons (e.g. `p1;p2;pN`).\n* Request header values, concatenated without separator (none at the moment, leave empty)\n* Request expiration date in UNIX timestamp format\n\nExample *message* to sign for `GET /v2/resource/a02baf5a-a3e4-49a0-857b-8a08d276c1c0?p1=v1&p2=v2`:\n\n```\nGET /v2/resource/a02baf5a-a3e4-49a0-857b-8a08d276c1c0\nv1v2\n1599140767\n```\n\nThe request signature consists of the base64-encoded [HMAC](https://en.wikipedia.org/wiki/HMAC) hash of the UTF-8 encoded *message* and the Exoscale API secret using the SHA265 function:\n\n```\nsignature = BASE64_ENCODE(HMAC_SHA256(Exoscale API secret, message))\n```\n\nFinally, the computed signature must be added to the API request in a `Authorization` header such as:\n\n```\nAuthorization: EXO2-HMAC-SHA256 credential=<Exoscale API key>,expires=<expiration date UNIX timestamp>,signature=<signature>\n```\n\nExample API query:\n\n```\nGET /v2/resource/a02baf5a-a3e4-49a0-857b-8a08d276c1c0?p1=v1&p2=v2 HTTP/1.1\nHost: api-ch-gva-2.exoscale.com\nAuthorization: EXO2-HMAC-SHA256 credential=EXO29147e9f89102b7ac1e88514,signed-query-args=p1;p2,expires=1599140767,signature=2AOBQsbElQb4FpKT/FM/9T4NobjlmZkSGvvdUth/xlY=\n```\n\n## Reference Implementations\n\nYou can look up the following existing reference implementations:\n\n* Go: [github.com/exoscale/egoscale/api/v2 > `SecurityProviderExoscale.signRequest`](https://github.com/exoscale/egoscale/blob/master/v2/api/security.go)\n* Python: [requests-exoscale-auth > `ExoscaleV2Auth`](https://github.com/exoscale/requests-exoscale-auth/blob/master/exoscale_auth.py)\n\n",
+            "content": "\nIn order to authenticate legitimate users, the Exoscale API requires incoming requests to be signed using valid Exoscale API account credentials with the following mechanism.\n\n## Signature Mechanism\n\nThe *message* (i.e. content) to sign contains several segments concatenated using a line return character (`\\n`).\n\nAll segments must be included and in the described order. For cases where a segment doesn't fit the context of the request (e.g. no request body) **an empty line must be used instead**.\n\n* Request method and request URL (path only), separated by a space character\n* Request body\n* Request URL parameters (Query String) values, concatenated without separator. The matching parameter names have to be specified in the resulting signature header `signed-query-args=` pragma, separated by semicolons (e.g. `p1;p2;pN`).\n* Request header values, concatenated without separator (none at the moment, leave empty)\n* Request expiration date in UNIX timestamp format\n\nExample *message* to sign for `GET /v2/resource/a02baf5a-a3e4-49a0-857b-8a08d276c1c0?p1=v1&p2=v2`:\n\n```\nGET /v2/resource/a02baf5a-a3e4-49a0-857b-8a08d276c1c0\n\nv1v2\n\n1599140767\n```\n\nThe two blank lines above are due to the absence of a request body and signed headers.\n\nExample *message* to [create a security group](https://openapi-v2.exoscale.com/operation/operation-create-security-group)\n\n```\nPOST /v2/security-group\n{\"name\": \"my-security-group\"}\n\n\n1599140767\n```\n\nThe two blank lines above are due to the absence of query parameters and signed headers.\n\nThe request signature consists of the base64-encoded [HMAC](https://en.wikipedia.org/wiki/HMAC) hash of the UTF-8 encoded *message* and the Exoscale API secret using the SHA265 function:\n\n```\nsignature = BASE64_ENCODE(HMAC_SHA256(Exoscale API secret, message))\n```\n\nFinally, the computed signature must be added to the API request in a `Authorization` header such as:\n\n```\nAuthorization: EXO2-HMAC-SHA256 credential=<Exoscale API key>,expires=<expiration date UNIX timestamp>,signature=<signature>\n```\n\nExample API query:\n\n```\nGET /v2/resource/a02baf5a-a3e4-49a0-857b-8a08d276c1c0?p1=v1&p2=v2 HTTP/1.1\nHost: api-ch-gva-2.exoscale.com\nAuthorization: EXO2-HMAC-SHA256 credential=EXO29147e9f89102b7ac1e88514,signed-query-args=p1;p2,expires=1599140767,signature=2AOBQsbElQb4FpKT/FM/9T4NobjlmZkSGvvdUth/xlY=\n```\n\n## Reference Implementations\n\nYou can look up the following existing reference implementations:\n\n* Go: [github.com/exoscale/egoscale/api/v2 > `SecurityProviderExoscale.signRequest`](https://github.com/exoscale/egoscale/blob/master/v2/api/security.go)\n* Python: [requests-exoscale-auth > `ExoscaleV2Auth`](https://github.com/exoscale/requests-exoscale-auth/blob/master/exoscale_auth.py)\n\n",
             "title": "API Request Signature"
         },
         {
-            "content": "\nThe API is deployed across multiple zones: `ch-gva-2`, `ch-dk-2`, `de-fra-1`, `de-muc-1`, `at-vie-1`, `bg-sof-1`. When performing a compute call, you should use the relevant zone for your resource.\nFor example: https://api-de-fra-1.exoscale.com/v2/instance would return only the instances from `de-fra-1`, https://api-ch-gva-2.exoscale.com/v2/instance from `ch-gva-2`.\nTo obtain a list of all instances across all zones, you would need to do the corresponding request per zone.\n\nNote that if no zone is specified during the call `ch-gva-2` will be used by default.\n",
+            "content": "\nThe API is deployed across multiple zones: `ch-gva-2`, `ch-dk-2`, `de-fra-1`, `de-muc-1`, `at-vie-1`, `at-vie-2`, `bg-sof-1`. When performing a compute call, you should use the relevant zone for your resource.\nFor example: https://api-de-fra-1.exoscale.com/v2/instance would return only the instances from `de-fra-1`, https://api-ch-gva-2.exoscale.com/v2/instance from `ch-gva-2`.\nTo obtain a list of all instances across all zones, you would need to do the corresponding request per zone.\n\nNote that if no zone is specified during the call `ch-gva-2` will be used by default.\n",
             "title": "Zone local resources"
         }
     ]
 }
```

### Comparing `exoscale-0.8.0/exoscale/api/v2.py` & `exoscale-0.9.1/exoscale/api/v2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+"""
+
+``exoscale.api.v2`` provides a low-level client targeting Exoscale's
+OpenAPI-based V2 API. This client is dynamically generated from the OpenAPI
+definition shipped with the package.
+
+Examples:
+    Creating a client targeting one of the available zones:
+
+    >>> from exoscale.api.v2 import Client
+    >>> c = Client("api-key", "api-secret", zone="de-fra-1")
+    >>> c.list_instances()
+    {'instances': []}
+
+    Creating a client targeting an endpoint specifically:
+
+    >>> from exoscale.api.v2 import Client
+    >>> c = Client("api-key", "api-secret", url="https://api-ch-gva-2.exoscale.com/v2")
+    >>> c.list_instances()
+    {'instances': []}
+
+"""
+
+import copy
 import json
 from itertools import chain
 from pathlib import Path
 
 from exoscale_auth import ExoscaleV2Auth
 
 import requests
@@ -30,52 +54,68 @@
         BY_OPERATION[operation["operationId"]] = {
             "verb": verb,
             "path": path,
             "operation": operation,
         }
 
 
+def _get_in(payload, keys):
+    """
+    Returns the value in a nested dict, where items is a sequence of keys.
+    """
+    k, *ks = keys
+    ret = payload[k]
+    if ks:
+        return _get_in(ret, ks)
+    else:
+        return ret
+
+
 def _get_ref(path):
     root, *parts = path.split("/")
     if root != "#":
         raise AssertionError("Non-root path start", root, path)
 
-    payload = API_SPEC
-    while parts:
-        item, *parts = parts
-        payload = payload[item]
+    # We're going to mutate payload later on, so make a full copy to avoid
+    # altering API_SPEC.
+    payload = copy.deepcopy(_get_in(API_SPEC, parts))
 
     for name, desc in payload.get("properties", {}).items():
         if "$ref" in desc:
             resolved_schema = _get_ref(desc["$ref"])
             for k, v in desc.items():
                 if k != "$ref":
                     resolved_schema[k] = v
             payload["properties"][name] = resolved_schema
     payload["$schema"] = "http://json-schema.org/draft-04/schema"
     return payload
 
 
 class BaseClient:
     def __init__(self, key, secret, url=None, **kwargs):
-        for server in API_SPEC["servers"]:
-            if server["url"] == url:
-                break
-        else:
+        if url is None:
             server = API_SPEC["servers"][0]
-        variables = {
-            var_name: var["default"]
-            for var_name, var in server["variables"].items()
-        }
-        for k, v in kwargs.items():
-            if k not in server["variables"]:
-                raise TypeError(f"Unhandled keyword argument {k!r}.")
-            variables[k] = v
+            variables = {
+                var_name: var["default"]
+                for var_name, var in server["variables"].items()
+            }
+            for k, v in kwargs.items():
+                if k not in server["variables"]:
+                    raise TypeError(f"Unhandled keyword argument {k!r}.")
+                if choices := server["variables"][k].get("enum"):
+                    if v not in choices:
+                        choices_repr = "', '".join(choices)
+                        raise TypeError(
+                            f"Invalid {k}: must be one of '{choices_repr}'."
+                        )
+                variables[k] = v
 
-        self.endpoint = server["url"].format(**variables)
+            self.endpoint = server["url"].format(**variables)
+        else:
+            self.endpoint = url
 
         session = requests.Session()
         session.auth = ExoscaleV2Auth(key, secret)
         self.session = session
         self.key = key
 
     def __repr__(self):
@@ -85,28 +125,30 @@
         )
 
     def _call_operation(self, operation_id, parameters=None, body=None):
         op = BY_OPERATION[operation_id]
 
         path = op["path"]
         query_params = {}
+        path_params = {}
         if parameters is None:
             parameters = {}
         for param in op["operation"].get("parameters", []):
             name = param["name"]
             if param["required"] and name not in parameters:
                 raise ValueError(f"Missing mandatory param {name!r}")
             if name in parameters:
                 value = parameters[name]
                 if param["in"] == "path":
-                    # TODO validate
-                    path = path.format(**{name: value})
+                    path_params[name] = value
                 elif param["in"] == "query":
                     query_params[name] = value
 
+        path = path.format(**path_params)
+
         url = f"{self.endpoint}{path}"
 
         json = {}
         if body is not None:
             # TODO validate
             json["json"] = body
 
@@ -129,15 +171,42 @@
     [status_code] = operation["responses"].keys()
     [ctype] = operation["responses"][status_code]["content"].keys()
     return_schema = operation["responses"][status_code]["content"][ctype][
         "schema"
     ]
     if "$ref" in return_schema:
         ref = _get_ref(return_schema["$ref"])
-        if "description" in ref:
+        if (
+            "properties" in ref
+            and ref["type"] == "object"
+            and "description" in ref
+        ):
+            body = {}
+            for name, prop in ref["properties"].items():
+                if "$ref" in prop:
+                    _ref = _get_ref(prop["$ref"])
+                    item = _ref
+                else:
+                    item = prop
+                typ = _type_translations[item["type"]]
+                desc = prop.get("description")
+                if "enum" in item:
+                    choices = "``, ``".join(map(repr, item["enum"]))
+                    desc += f". Values are ``{choices}``"
+                suffix = f": {desc}" if desc else ""
+                normalized_name = name.replace("-", "_")
+                body[normalized_name] = (
+                    f"**{normalized_name}** ({typ}){suffix}."
+                )
+
+            doc = (
+                f"dict: {ref['description']}. A dictionnary with the following keys:"
+                + "\n\n          * ".join([""] + list(body.values()))
+            )
+        elif "description" in ref:
             doc = f'{_type_translations[ref["type"]]}: {ref["description"]}.'
         else:
             doc = _type_translations[ref["type"]]
     else:
         doc = _type_translations[return_schema["type"]]
     return doc
 
@@ -233,16 +302,15 @@
     template = """Create an API client.
 
     Args:
         key (str): Exoscale API key.
 
         secret (str): Exoscale API secret.
 
-        url (str): Endpoint URL template to use. Must be one of ``{servers}``.
-            Defaults to ``{default_server!r}``.
+        url (str): Endpoint URL to use. Defaults to ``{default_server!r}``.
 
         {dynamic_args}
 
     Returns:
         Client: A configured API client.
     """
     servers = []
```

### Comparing `exoscale-0.8.0/LICENSE` & `exoscale-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exoscale-0.8.0/pyproject.toml` & `exoscale-0.9.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -18,33 +18,27 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "attrs>=20.1.0",
-    "boto3>=1.9.176",
-    "cs>=2.7.1",
     "requests-exoscale-auth>=1.1.2",
     "requests>=2.22.0",
-    "toml>=0.10.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/exoscale/python-exoscale"
 "Bug Tracker" = "https://github.com/exoscale/python-exoscale/issues"
 
 [project.optional-dependencies]
 dev = [
-    "pytest-timeout>=1.4.2",
     "pytest>=5.0.0",
     "recommonmark>=0.5.0",
-    "requests-mock>=1.8.0",
     "sphinx-markdown-parser>=0.1.1",
     "sphinx-rtd-theme>=0.4.3",
     "sphinx>=2.1.2",
 ]
 
 [tool.hatch.version]
 path = "exoscale/__init__.py"
```

### Comparing `exoscale-0.8.0/PKG-INFO` & `exoscale-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: exoscale
-Version: 0.8.0
+Version: 0.9.1
 Summary: Clients for Exoscale IaaS APIs
 Project-URL: Homepage, https://github.com/exoscale/python-exoscale
 Project-URL: Bug Tracker, https://github.com/exoscale/python-exoscale/issues
 Author-email: Exoscale <support@exoscale.com>
 License-Expression: ISC
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -14,49 +14,34 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Requires-Dist: attrs>=20.1.0
-Requires-Dist: boto3>=1.9.176
-Requires-Dist: cs>=2.7.1
 Requires-Dist: requests-exoscale-auth>=1.1.2
 Requires-Dist: requests>=2.22.0
-Requires-Dist: toml>=0.10.0
 Provides-Extra: dev
-Requires-Dist: pytest-timeout>=1.4.2; extra == 'dev'
 Requires-Dist: pytest>=5.0.0; extra == 'dev'
 Requires-Dist: recommonmark>=0.5.0; extra == 'dev'
-Requires-Dist: requests-mock>=1.8.0; extra == 'dev'
 Requires-Dist: sphinx-markdown-parser>=0.1.1; extra == 'dev'
 Requires-Dist: sphinx-rtd-theme>=0.4.3; extra == 'dev'
 Requires-Dist: sphinx>=2.1.2; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # python-exoscale: Python bindings for Exoscale API
 
 [![Actions Status](https://github.com/exoscale/python-exoscale/workflows/CI/badge.svg)](https://github.com/exoscale/python-exoscale/actions?query=workflow%3ACI)
 
-This library allows developpers to use the [Exoscale] cloud platform API with
-high-level Python bindings. API documentation and usage examples can be found
+This library allows developers to use the [Exoscale] cloud platform API with
+extensive Python bindings. API documentation and usage examples can be found
 at this address: https://exoscale.github.io/python-exoscale
 
 ## Development
 
-First create a new virtual environment and run `make installrequirements`.
-Then create a configuration file with your **production** user's API keys.
-This file may be create for example in `junk/config.toml`. Here is an example:
+First create a new virtual environment and run `python -m pip install -e .[dev]`.
 
-    default_profile = "prod:you"
+You can then run pytest with the following command:
 
-    [[profiles]]
-    name       = "prod:you"
-    api_key    = "EXOxxxx"
-    api_secret = "yyyy"
-
-Once this file is created you can run pytest with the following command:
-
-    EXOSCALE_CONFIG_FILE=./junk/config.toml pytest -x -s -vvv tests/*.py
+    pytest -x -s -vvv
 
 [exoscale]: https://www.exoscale.com/
```

