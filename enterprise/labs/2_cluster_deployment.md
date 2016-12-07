```````````
{
  "timestamp" : "2016-12-07T03:04:05.907Z",
  "clusters" : [ {
    "name" : "Cluster 1",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "612368384"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "612368384"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "4679270400"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "787"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-11-110.ap-southeast-1.compute.internal"
        }, {
          "name" : "hive_metastore_database_name",
          "value" : "nav"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "nav_password"
        }, {
          "name" : "hive_metastore_database_user",
          "value" : "nav"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-2326a39c2a7ed079ef95f6959ddbebef",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "f99b7737-911e-4f1a-ba45-87a656f7cb85"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-54c2de84f181de9d5f52b669b4cf65ea",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2f3f0f6b-b067-43c3-b813-50a2e16b82ad"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-9e8499205549d042d79fc4c50951adad",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2d9aa401-54a0-44e4-9eb3-5775ff1ce605"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-c626da03883e0ddcb18acb53c6548617",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-c626da03883e0ddcb18acb53c6548617",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "esle7nfl9cfhdv5p3iydhru6u"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-c626da03883e0ddcb18acb53c6548617",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9o13hbjsbvf9lx955q58cexf9"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "612368384"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-c626da03883e0ddcb18acb53c6548617",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "96iximks00u0mmauec9gucped"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-11-110.ap-southeast-1.compute.internal"
        }, {
          "name" : "database_name",
          "value" : "nav"
        }, {
          "name" : "database_password",
          "value" : "nav_password"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "database_user",
          "value" : "nav"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-c626da03883e0ddcb18acb53c6548617"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-c626da03883e0ddcb18acb53c6548617",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8d6611wpnygh0sl0zqr9kbywm"
          }, {
            "name" : "secret_key",
            "value" : "hJY9LlNLnl8Rg4cc03BHrl7dXuAtBC"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-11-110.ap-southeast-1.compute.internal"
          }, {
            "name" : "oozie_database_name",
            "value" : "rman"
          }, {
            "name" : "oozie_database_password",
            "value" : "rman_password"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "rman"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "612368384"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-c626da03883e0ddcb18acb53c6548617",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5vflru4h7ctkw39zn6yglv46g"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "6"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "1"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "612368384"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "5250"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "612368384"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "5250"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "4"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "D0KBMXVgZhGOfU9P0GNRpuxsg33ksF"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-c626da03883e0ddcb18acb53c6548617",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6yuojz5hc2r4044rf03am9agv"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-2326a39c2a7ed079ef95f6959ddbebef",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "f99b7737-911e-4f1a-ba45-87a656f7cb85"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "czuaxv9bkoan3132xgu06yc6w"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-54c2de84f181de9d5f52b669b4cf65ea",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "2f3f0f6b-b067-43c3-b813-50a2e16b82ad"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "b1dc7rkdy068hgtudsaywrxk4"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-9e8499205549d042d79fc4c50951adad",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "2d9aa401-54a0-44e4-9eb3-5775ff1ce605"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "911zcdfuiy4gbnfqyh9ugytw5"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-c626da03883e0ddcb18acb53c6548617",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "44"
          }, {
            "name" : "role_jceks_password",
            "value" : "10dcc51nbpcipwghjh3aqdm9h"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "BALANCER",
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "612368384"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "845511884"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "612368384"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "l0jKOzjZV0QgcFPhtlqEZb2HmtuRLZ"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "6wWd95QYneoplD39vFHBOe9S2e25uN"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "5fkHY3MjCF6AbOia0JQh2I6SQQYY5N"
        }, {
          "name" : "service_config_suppression_nameservice_namenodes_heap_size_validator",
          "value" : "true"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-c626da03883e0ddcb18acb53c6548617",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-2326a39c2a7ed079ef95f6959ddbebef",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "f99b7737-911e-4f1a-ba45-87a656f7cb85"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9mk9h30swny578bmzna6ni6lp"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-54c2de84f181de9d5f52b669b4cf65ea",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "2f3f0f6b-b067-43c3-b813-50a2e16b82ad"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "a3bhy1yjyaw3zfzipyvx9cqfk"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-9e8499205549d042d79fc4c50951adad",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "2d9aa401-54a0-44e4-9eb3-5775ff1ce605"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6oke19kpwcuf6ccgq8lwcwujf"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-c626da03883e0ddcb18acb53c6548617",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
        },
        "config" : {
          "items" : [ {
            "name" : "namenode_id",
            "value" : "46"
          }, {
            "name" : "role_jceks_password",
            "value" : "9ww26d0krkvta1vwtyoyhszjs"
          } ]
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-c626da03883e0ddcb18acb53c6548617",
        "type" : "SECONDARYNAMENODE",
        "hostRef" : {
          "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "d1c9p6tf7lyfcef8sxmej7d5x"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "6fdac0db-a960-4081-b69c-520c3de52869",
    "ipAddress" : "172.31.11.110",
    "hostname" : "ip-172-31-11-110.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9",
    "ipAddress" : "172.31.7.203",
    "hostname" : "ip-172-31-7-203.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ {
        "name" : "memory_overcommit_threshold",
        "value" : "0.6"
      } ]
    }
  }, {
    "hostId" : "f99b7737-911e-4f1a-ba45-87a656f7cb85",
    "ipAddress" : "172.31.7.204",
    "hostname" : "ip-172-31-7-204.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "2d9aa401-54a0-44e4-9eb3-5775ff1ce605",
    "ipAddress" : "172.31.7.205",
    "hostname" : "ip-172-31-7-205.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "2f3f0f6b-b067-43c3-b813-50a2e16b82ad",
    "ipAddress" : "172.31.7.206",
    "hostname" : "ip-172-31-7-206.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-c626da03883e0ddcb18acb53c6548617",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "34a990a9934dd4c454584704c62495069b853e46c97b709d616be3cc72b24586",
    "pwSalt" : 8575454565933177794,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-c626da03883e0ddcb18acb53c6548617",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "b86bd18802424a336d83776b556be0ce0483773900d6796d996425e02d034dd9",
    "pwSalt" : -7246209358235142330,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-c626da03883e0ddcb18acb53c6548617",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "c9ca61e2beb793e6d9e51ef1168dc2d4d5f90a20012b4ecbf3ce7875d1ff8366",
    "pwSalt" : 3925540128244056017,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-c626da03883e0ddcb18acb53c6548617",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "1873de9c92f56507a441300f60330920fd288d88b6b2a140202bb425a73386cc",
    "pwSalt" : 4247009137225031596,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "279e6f41d4332f947249f1930288326575e69ebb1decbf74575e8fef4b519118",
    "pwSalt" : 377785179603697723,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "f8175f6108dce4cc18a05102d45846c512c9a093642c7753213a65cbd02c29b6",
    "pwSalt" : 1567238895326752894,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.9.0",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20161006-1801",
    "gitHash" : "898a5e032c080e18833dfc58180761f6ef2ea351",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "ACTIVITYMONITOR",
        "items" : [ {
          "name" : "firehose_database_host",
          "value" : "ip-172-31-11-110.ap-southeast-1.compute.internal"
        }, {
          "name" : "firehose_database_name",
          "value" : "amon"
        }, {
          "name" : "firehose_database_password",
          "value" : "amon_password"
        }, {
          "name" : "firehose_database_user",
          "value" : "amon"
        } ]
      }, {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "612368384"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "612368384"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        }, {
          "name" : "health_event_publish_startup_policy",
          "value" : "none"
        } ]
      }, {
        "roleType" : "NAVIGATOR",
        "items" : [ {
          "name" : "navigator_database_host",
          "value" : "ip-172-31-11-110.ap-southeast-1.compute.internal"
        }, {
          "name" : "navigator_database_password",
          "value" : "nav_password"
        } ]
      }, {
        "roleType" : "NAVIGATORMETASERVER",
        "items" : [ {
          "name" : "nav_metaserver_database_host",
          "value" : "ip-172-31-11-110.ap-southeast-1.compute.internal"
        }, {
          "name" : "nav_metaserver_database_password",
          "value" : "navms_password"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-11-110.ap-southeast-1.compute.internal"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_password"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "612368384"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_database_host",
          "value" : "172.31.11.110"
        }, {
          "name" : "firehose_database_name",
          "value" : "amon"
        }, {
          "name" : "firehose_database_password",
          "value" : "amon_password"
        }, {
          "name" : "firehose_database_user",
          "value" : "amon"
        }, {
          "name" : "firehose_heapsize",
          "value" : "612368384"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        }, {
          "name" : "health_event_publish_startup_policy",
          "value" : "none"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-c626da03883e0ddcb18acb53c6548617",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "3fld53ocyqsl9zeymjt2oj4ts"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-c626da03883e0ddcb18acb53c6548617",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "81l04jlr15nsq9r4wv6gli57w"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-c626da03883e0ddcb18acb53c6548617",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "2i3abvoops9jkscoocft1xdkk"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-c626da03883e0ddcb18acb53c6548617",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "gryawldl0e9oz9srjt8e1w0a"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-c626da03883e0ddcb18acb53c6548617",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "66ebbdf1-f2dd-4aec-afa8-7090b5843eb9"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "amdq3l5y7pd0ydcszdplnp52k"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/24/2012 17:50"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  }
} 
``````
