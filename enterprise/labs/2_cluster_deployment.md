[root@ip-172-31-7-126 ~]# curl mihenn87:cloudera@localhost:7180/api/v2/cm/deployment

```json
{
  "timestamp" : "2017-03-08T09:56:46.348Z",
  "clusters" : [ {
    "name" : "mihenn87",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "593494016"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "593494016"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "3433247539"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "577"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-7-126.us-west-2.compute.internal"
        }, {
          "name" : "hive_metastore_database_name",
          "value" : "hive"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "cloudera"
        }, {
          "name" : "hive_metastore_database_user",
          "value" : "cloudera"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-15288b6180999cc15b90039739dd9424",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-02e737fe934bbaa95"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-3cbf9e0f8e241c2634104ef25c1d1f55",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-09c874782fe1853ec"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-52677fcb6fb7b741baab730b66fb55f4",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-03462b2947a8cfdd9"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-5c30b39330e6393978c4ce91369155ea",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-032e0aa2052aa7709"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-6b01b01f004ad1a68bbeb02863bdce1d",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0d18e01ee2716d480"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-6b01b01f004ad1a68bbeb02863bdce1d",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "i-0d18e01ee2716d480"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "e8we684bcy042mj536b90cgui"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-6b01b01f004ad1a68bbeb02863bdce1d",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "i-0d18e01ee2716d480"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8ch6qrep3i8a5yahv7fk78fzk"
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
            "value" : "593494016"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-3cbf9e0f8e241c2634104ef25c1d1f55",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-09c874782fe1853ec"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5xku91125pimlljark346kgef"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-52677fcb6fb7b741baab730b66fb55f4",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-03462b2947a8cfdd9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3yr0vwnaoga5j9n479js93ch8"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-6b01b01f004ad1a68bbeb02863bdce1d",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-0d18e01ee2716d480"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "f0l6cfq2vk1k7mm5l5o2nooom"
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
          "value" : "ip-172-31-7-126.us-west-2.compute.internal"
        }, {
          "name" : "database_password",
          "value" : "cloudera"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "database_user",
          "value" : "cloudera"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-6b01b01f004ad1a68bbeb02863bdce1d"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-6b01b01f004ad1a68bbeb02863bdce1d",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "i-0d18e01ee2716d480"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1rri42vwioeeob1thwlkxw2va"
          }, {
            "name" : "secret_key",
            "value" : "NTNJUPEVrT7PorZnCMmAOgpAjpA44h"
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
            "value" : "ip-172-31-7-126.us-west-2.compute.internal"
          }, {
            "name" : "oozie_database_password",
            "value" : "cloudera"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "cloudera"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "593494016"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "oozie_upload_sharelib_cmd_timeout",
          "value" : "1200"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-6b01b01f004ad1a68bbeb02863bdce1d",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "i-0d18e01ee2716d480"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cknczwnqvp5drl0xo0hv6xpzs"
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
            "value" : "8"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          }, {
            "name" : "mapreduce_map_cpu_vcores",
            "value" : "2"
          }, {
            "name" : "mapreduce_map_java_opts_max_heap",
            "value" : "1717986918"
          }, {
            "name" : "mapreduce_map_memory_mb",
            "value" : "2048"
          }, {
            "name" : "mapreduce_reduce_java_opts_max_heap",
            "value" : "3435973837"
          }, {
            "name" : "mapreduce_reduce_memory_mb",
            "value" : "4096"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "593494016"
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
            "value" : "3537"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "593494016"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "4273"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "90"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "01gmCMn0psOxQzn2a6WwR1kH5kmarc"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-6b01b01f004ad1a68bbeb02863bdce1d",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "i-0d18e01ee2716d480"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3scseltc0ycp4ocjwr9v0tnyw"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-15288b6180999cc15b90039739dd9424",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-02e737fe934bbaa95"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5i9al5vu779nzew7lqold7ywa"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-3cbf9e0f8e241c2634104ef25c1d1f55",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-09c874782fe1853ec"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "58lctb48ph494vqm3idm9rywd"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-52677fcb6fb7b741baab730b66fb55f4",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-03462b2947a8cfdd9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9ggwlkzdhut5d1ufo8tlrhj8v"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-5c30b39330e6393978c4ce91369155ea",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-032e0aa2052aa7709"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dzpg4gvnmoaha3koytcjv6jdu"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-6b01b01f004ad1a68bbeb02863bdce1d",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "i-0d18e01ee2716d480"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "53"
          }, {
            "name" : "role_jceks_password",
            "value" : "2gwtop4412m5pe5pmahl0k7o1"
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
            "value" : "593494016"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "3219965132"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "dfs_datanode_use_datanode_hostname",
            "value" : "true"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/var/log/cloudera/jn"
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
            "value" : "593494016"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_client_use_datanode_hostname",
          "value" : "true"
        }, {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "tLTPfctKu28bSw9emqfZ9piY123Zwx"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "SvqMC25WdvcW1KHPt8lMYuXpchiW2Y"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "QR0fKrl6hOpp8628mWaCuChsJrLT6i"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "10"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-6b01b01f004ad1a68bbeb02863bdce1d",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "i-0d18e01ee2716d480"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-15288b6180999cc15b90039739dd9424",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-02e737fe934bbaa95"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2jrqssjk4kpcxold9g3qt84bt"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-3cbf9e0f8e241c2634104ef25c1d1f55",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-09c874782fe1853ec"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6psv6lni1khhhsn9fw58xfo0i"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-52677fcb6fb7b741baab730b66fb55f4",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-03462b2947a8cfdd9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "b4grc4dqn9phjg9avpvw0w964"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-5c30b39330e6393978c4ce91369155ea",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-032e0aa2052aa7709"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ezw878kw0ppxtdz7bb9z248p6"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-5c30b39330e6393978c4ce91369155ea",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "i-032e0aa2052aa7709"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dnvhr1l8844t7izyt1xq94tf5"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-6b01b01f004ad1a68bbeb02863bdce1d",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "i-0d18e01ee2716d480"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "93cdziqfgfvmtwharhk5t558n"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-6b01b01f004ad1a68bbeb02863bdce1d",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "i-0d18e01ee2716d480"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dwtrez0qr52lnooi0vhnttahj"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-15288b6180999cc15b90039739dd9424",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-02e737fe934bbaa95"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bjvxh8mfrmksry36rbnaxa8cr"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-3cbf9e0f8e241c2634104ef25c1d1f55",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-09c874782fe1853ec"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8n4xqxqxg122v4m188wc83kpj"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-52677fcb6fb7b741baab730b66fb55f4",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-03462b2947a8cfdd9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8y24pfzpkjy2v3n7bw98xt38y"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-5c30b39330e6393978c4ce91369155ea",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-032e0aa2052aa7709"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "61"
          }, {
            "name" : "role_jceks_password",
            "value" : "7r3qedvb6clgywmxgrjerbikx"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-6b01b01f004ad1a68bbeb02863bdce1d",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-0d18e01ee2716d480"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "55"
          }, {
            "name" : "role_jceks_password",
            "value" : "6mchgj1ihpjwfu9topsks48nc"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "i-0d18e01ee2716d480",
    "ipAddress" : "172.31.11.113",
    "hostname" : "ip-172-31-11-113.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-09c874782fe1853ec",
    "ipAddress" : "172.31.3.32",
    "hostname" : "ip-172-31-3-32.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-03462b2947a8cfdd9",
    "ipAddress" : "172.31.4.130",
    "hostname" : "ip-172-31-4-130.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-032e0aa2052aa7709",
    "ipAddress" : "172.31.4.23",
    "hostname" : "ip-172-31-4-23.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ {
        "name" : "memory_overcommit_threshold",
        "value" : "0.9"
      } ]
    }
  }, {
    "hostId" : "i-02e737fe934bbaa95",
    "ipAddress" : "172.31.7.126",
    "hostname" : "ip-172-31-7-126.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__daf9539b-86f6-4bc2-937a-6e7f48d9fe1f",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "e188e5979a0b77226b058b92dea1aa8b4cc744a1d477b80722b6e8d6ab8e37fc",
    "pwSalt" : 2682283483661516791,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-6b01b01f004ad1a68bbeb02863bdce1d",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "843ccd14abff839e16f61b6257a5aba32f331e90d2b1b8e5a0ad3bc5ae9c68e9",
    "pwSalt" : -1619327350753342916,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-6b01b01f004ad1a68bbeb02863bdce1d",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "cf473d28f56692efe02a01d9aefaa065de1d99aefb326b1febefd651e1e7b8b6",
    "pwSalt" : 5338766305125911512,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-6b01b01f004ad1a68bbeb02863bdce1d",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "c229da24f706057bfa929d6a25ef3689c8624ed4404c304557ebc69d91498bbc",
    "pwSalt" : 4680369215934710954,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-6b01b01f004ad1a68bbeb02863bdce1d",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "8117cb7ce046a6b9abeb345d748f2177c81be99e349ff4dfe882dd454273c881",
    "pwSalt" : -2536068185689065487,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "05fe9dfefd403705fa2ea66b36af71e50b8fbb707b4c77093f427a1f647c0c0e",
    "pwSalt" : 7099328857793136011,
    "pwLogin" : true
  }, {
    "name" : "mihenn87",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "ef1297343b1201696ae8de676d1a8ee9a66e6bfe2ffc51f3ba1aa58135243d65",
    "pwSalt" : 8417431885589601668,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "973721e4e3842f21049c6bd1e5f90375ccec9081c9e9c694d2388c9e2742f81b",
    "pwSalt" : 8511785759018419018,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.8.3",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20161019-1013",
    "gitHash" : "518f0d6d44abc87bc392646e4369a20c8192b7cf",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "593494016"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-7-126.us-west-2.compute.internal"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rm"
        }, {
          "name" : "headlamp_database_password",
          "value" : "cloudera"
        }, {
          "name" : "headlamp_database_user",
          "value" : "cloudera"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "593494016"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-6b01b01f004ad1a68bbeb02863bdce1d",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "i-0d18e01ee2716d480"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "m37ue2xbfkgdx7btk4zrbu0i"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-6b01b01f004ad1a68bbeb02863bdce1d",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "i-0d18e01ee2716d480"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "2ch5sgjrluhqip1dixczaiym1"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-6b01b01f004ad1a68bbeb02863bdce1d",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "i-0d18e01ee2716d480"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "eun8xv9ulirgc4lxgv4eru5q2"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-6b01b01f004ad1a68bbeb02863bdce1d",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "i-0d18e01ee2716d480"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "53vw97c817y1rle012mt7qh2n"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-6b01b01f004ad1a68bbeb02863bdce1d",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "i-0d18e01ee2716d480"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "27al869fvl288b7y6tmotrhbf"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/27/2012 14:50"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  }
}```
