<h1>CM Lab</h1><br>

<h2>Use the API</h2><br>

{<br>
  "timestamp" : "2017-11-30T17:19:44.128Z",<br>
  "clusters" : [ {<br>
    "name" : "lotnavarro",<br>
    "version" : "CDH5",<br>
    "services" : [ {<br>
      "name" : "hive",<br>
      "type" : "HIVE",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ {<br>
          "roleType" : "HIVEMETASTORE",<br>
          "items" : [ {<br>
            "name" : "hive_metastore_java_heapsize",<br>
            "value" : "6026166272"<br>
          }, {<br>
            "name" : "hive_metastore_server_max_message_size",<br>
            "value" : "602616627"<br>
          } ]<br>
        }, {<br>
          "roleType" : "HIVESERVER2",<br>
          "items" : [ {<br>
            "name" : "hiveserver2_enable_impersonation",<br>
            "value" : "false"<br>
          }, {<br>
            "name" : "hiveserver2_spark_driver_memory",<br>
            "value" : "966367641"<br>
          }, {<br>
            "name" : "hiveserver2_spark_executor_cores",<br>
            "value" : "4"<br>
          }, {<br>
            "name" : "hiveserver2_spark_executor_memory",<br>
            "value" : "4801377075"<br>
          }, {<br>
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",<br>
            "value" : "102"<br>
          }, {<br>
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",<br>
            "value" : "808"<br>
          } ]<br>
        } ],<br>
        "items" : [ {<br>
          "name" : "hive_metastore_database_host",<br>
          "value" : "standaloneln.northcentralus.cloudapp.azure.com"<br>
        }, {<br>
          "name" : "hive_metastore_database_password",<br>
          "value" : "Raken.2017"<br>
        }, {<br>
          "name" : "hive_proxy_user_groups_list",<br>
          "value" : "hue,hive,sentry"<br>
        }, {<br>
          "name" : "mapreduce_yarn_service",<br>
          "value" : "yarn"<br>
        }, {<br>
          "name" : "sentry_service",<br>
          "value" : "sentry"<br>
        }, {<br>
          "name" : "zookeeper_service",<br>
          "value" : "zookeeper"<br>
        } ]<br>
      },<br>
      "roles" : [ {<br>
        "name" : "hive-GATEWAY-20f5b03f45b36e2845bc31ac5ab33b99",<br>
        "type" : "GATEWAY",<br>
        "hostRef" : {<br>
          "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "hive-GATEWAY-4a836da64f38f027c69e2e163c6b6567",<br>
        "type" : "GATEWAY",<br>
        "hostRef" : {<br>
          "hostId" : "78cdf155-f531-4368-922d-d79da3053f22"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "hive-GATEWAY-822c6fca1cb8956e904cc265f91cbecf",<br>
        "type" : "GATEWAY",<br>
        "hostRef" : {<br>
          "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "hive-GATEWAY-e662c2c98b3922907a045aa058cdac62",<br>
        "type" : "GATEWAY",<br>
        "hostRef" : {<br>
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "hive-HIVEMETASTORE-20f5b03f45b36e2845bc31ac5ab33b99",<br>
        "type" : "HIVEMETASTORE",<br>
        "hostRef" : {<br>
          "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "4ci7f23ncgebhqu2t8iffahnn"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hive-HIVESERVER2-20f5b03f45b36e2845bc31ac5ab33b99",<br>
        "type" : "HIVESERVER2",<br>
        "hostRef" : {<br>
          "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "3p4awv3hkywyyvdzvoitz1mp<br>y"
          } ]<br>
        }<br>
      } ],<br>
      "displayName" : "Hive"<br>
    }, {<br>
      "name" : "zookeeper",<br>
      "type" : "ZOOKEEPER",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ ],<br>
        "items" : [ {<br>
          "name" : "enableSecurity",<br>
          "value" : "true"<br>
        } ]<br>
      },<br>
      "roles" : [ {<br>
        "name" : "zookeeper-SERVER-20f5b03f45b36e2845bc31ac5ab33b99",<br>
        "type" : "SERVER",<br>
        "hostRef" : {<br>
          "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "9n01yajlug08roxdii7l3xvn5"<br>
          }, {<br>
            "name" : "serverId",<br>
            "value" : "3"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "zookeeper-SERVER-822c6fca1cb8956e904cc265f91cbecf",<br>
        "type" : "SERVER",<br>
        "hostRef" : {<br>
          "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "sefiejeescf8v6dbqai3mxz3"<br>
          }, {<br>
            "name" : "serverId",<br>
            "value" : "2"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "zookeeper-SERVER-e662c2c98b3922907a045aa058cdac62",<br>
        "type" : "SERVER",<br>
        "hostRef" : {<br>
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "7yebqzj2t6zhu69q6xc3t78ne"<br>
          }, {<br>
            "name" : "serverId",<br>
            "value" : "1"<br>
          } ]<br>
        }<br>
      } ],<br>
      "displayName" : "ZooKeeper"<br>
    }, {<br>
      "name" : "hue",<br>
     
 "type" : "HUE",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ {<br>
          "roleType" : "HUE_SERVER",<br>
          "items" : [ {<br>
            "name" : "hue_server_bind_wildcard",<br>
            "value" : "true"<br>
          } ]<br>
        } ],<br>
        "items" : [ {<br>
          "name" : "database_host",<br>
          "value" : "standaloneln.northcentralus.cloudapp.azure.com"<br>
        }, {<br>
          "name" : "database_password",<br>
          "value" : "Raken.2017"<br>
        }, {<br>
          "name" : "database_type",<br>
          "value" : "mysql"<br>
        }, {<br>
          "name" : "hive_service",<br>
          "value" : "hive"<br>
        }, {<br>
          "name" : "hue_webhdfs",<br>
          "value" : "hdfs-NAMENODE-822c6fca1cb8956e904cc265f91cbecf"<br>
        }, {<br>
          "name" : "oozie_service",<br>
          "value" : "oozie"<br>
        }, {<br>
          "name" : "sentry_service",<br>
          "value" : "sentry"<br>
        }, {<br>
          "name" : "zookeeper_service",<br>
          "value" : "zookeeper"<br>
        } ]<br>
      },<br>
      "roles" : [ {<br>
        "name" : "hue-HUE_SERVER-e662c2c98b3922907a045aa058cdac62",<br>
        "type" : "HUE_SERVER",<br>
        "hostRef" : {<br>
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "2tzrt3551ssef64ftofbylhph"<br>
          }, {<br>
            "name" : "secret_key",<br>
            "value" : "2cqifcdCnW3t9ckSbLRpsPUc2eQ27p"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hue-KT_RENEWER-e662c2c98b3922907a045aa058cdac62",<br>
        "type" : "KT_RENEWER",<br>
        "hostRef" : {<br>
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "czrlfih37h54k8hq6ga4k95uj"<br>
          } ]<br>
        }<br>
      } ],<br>
      "displayName" : "Hue"<br>
    }, {<br>
      "name" : "oozie",<br>
      "type" : "OOZIE",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ {<br>
          "roleType" : "OOZIE_SERVER",<br>
          "items" : [ {<br>
            "name" : "oozie_database_host",<br>
            "value" : "standaloneln.northcentralus.cloudapp.azure.com"<br>
          }, {<br>
            "name" : "oozie_database_password",<br>
            "value" : "Raken.2017"<br>
          }, {<br>
            "name" : "oozie_database_type",<br>
            "value" : "mysql"<br>
          }, {<br>
            "name" : "oozie_database_user",<br>
            "value" : "oozie"<br>
          } ]<br>
        } ],<br>
        "items" : [ {<br>
          "name" : "hive_service",<br>
          "value" : "hive"<br>
        }, {<br>
          "name" : "mapreduce_yarn_service",<br>
          "value" : "yarn"<br>
        }, {<br>
          "name" : "zookeeper_service",<br>
          "value" : "zookeeper"<br>
        } ]<br>
      },<br>
      "roles" : [ {<br>
        "name" : "oozie-OOZIE_SERVER-4a836da64f38f027c69e2e163c6b6567",<br>
        "type" : "OOZIE_SERVER",<br>
        "hostRef" : {<br>
          "hostId" : "78cdf155-f531-4368-922d-d79da3053f22"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "6uk2spjpa7rkmq3t030mij4x0"<br>
          } ]<br>
        }<br>
      } ],<br>
      "displayName" : "Oozie"<br>
    }, {<br>
      "name" : "yarn",<br>
      "type" : "YARN",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ {<br>
          "roleType" : "GATEWAY",<br>
          "items" : [ {<br>
            "name" : "mapred_reduce_tasks",<br>
            "value" : "12"<br>
          }, {<br>
            "name" : "mapred_submit_replication",<br>
            "value" : "1"<br>
          } ]<br>
        }, {<br>
          "roleType" : "NODEMANAGER",<br>
          "items" : [ {<br>
            "name" : "yarn_nodemanager_heartbeat_interval_ms",<br>
            "value" : "100"<br>
          }, {<br>
            "name" : "yarn_nodemanager_local_dirs",<br>
            "value" : "/mnt/resource/yarn/nm"<br>
          }, {<br>
            "name" : "yarn_nodemanager_log_dirs",<br>
            "value" : "/mnt/resource/yarn/container-logs"<br>
          }, {<br>
            "name" : "yarn_nodemanager_resource_memory_mb",<br>
            "value" : "15433"<br>
          } ]<br>
        }, {<br>
          "roleType" : "RESOURCEMANAGER",<br>
          "items" : [ {<br>
            "name" : "yarn_scheduler_maximum_allocation_mb",<br>
            "value" : "15433"<br>
          }, {<br>
            "name" : "yarn_scheduler_maximum_allocation_vcores",<br>
            "value" : "6"<br>
          } ]<br>
        } ],<br>
        "items" : [ {<br>
          "name" : "hadoop_secure_web_ui",<br>
          "value" : "true"<br>
        }, {<br>
          "name" : "hdfs_service",<br>
          "value" : "hdfs"<br>
        }, {<br>
          "name" : "rm_dirty",<br>
          "value" : "false"<br>
        }, {<br>
          "name" : "rm_last_allocation_percentage",<br>
          "value" : "80"<br>
        }, {<br>
          "name" : "yarn_service_cgroups",<br>
          "value" : "false"<br>
        }, {<br>
          "name" : "yarn_service_lce_always",<br>
          "value" : "false"<br>
        }, {<br>
          "name" : "zk_authorization_secret_key",<br>
          "value" : "03Knehjejrk04brAwAUoli799pD4PE"<br>
        }, {<br>
          "name" : "zookeeper_service",<br>
          "value" : "zookeeper"<br><br>
        } ]<br><br>
      },<br>
      "roles" : [ {<br>
        "name" : "yarn-JOBHISTORY-822c6fca1cb8956e904cc265f91cbecf",<br>
        "type" : "JOBHISTORY",<br>
        "hostRef" : {<br>
          "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "2awplfl52ziogpzynok8ln2yi"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "yarn-NODEMANAGER-20f5b03f45b36e2845bc31ac5ab33b99",<br>
        "type" : "NODEMANAGER",<br>
        "hostRef" : {<br>
          "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "5pghgzszybut1q5mxoj1qr6q6"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "yarn-NODEMANAGER-4a836da64f38f027c69e2e163c6b6567",<br>
        "type" : "NODEMANAGER",<br>
        "hostRef" : {<br>
          "hostId" : "78cdf155-f531-4368-922d-d79da3053f22"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "29nwt7o6q96vmzqkcyb25hnvt"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "yarn-NODEMANAGER-e662c2c98b3922907a045aa058cdac62",<br>
        "type" : "NODEMANAGER",<br>
        "hostRef" : {<br>
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "abslrpeth19m0bk0c8n50jnm3"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "yarn-RESOURCEMANAGER-4a836da64f38f027c69e2e163c6b6567",<br>
        "type" : "RESOURCEMANAGER",<br>
        "hostRef" : {<br>
          "hostId" : "78cdf155-f531-4368-922d-d79da3053f22"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "rm_id",<br>
            "value" : "48"<br>
          }, {<br>
            "name" : "role_jceks_password",<br>
            "value" : "aah53mf9gvcgtxti0ij26fy8g"<br>
          } ]<br>
        }<br>
      } ],<br>
      "displayName" : "YARN (MR2 Included)"<br>
    }, {<br>
      "name" : "hdfs",<br>
      "type" : "HDFS",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ {<br>
          "roleType" : "DATANODE",<br>
          "items" : [ {<br>
            "name" : "datanode_java_heapsize",<br>
            "value" : "1073741824"<br>
          }, {<br>
            "name" : "dfs_data_dir_list",<br>
            "value" : "/mnt/resource/dfs/dn"<br>
          }, {<br>
            "name" : "dfs_datanode_data_dir_perm",<br>
            "value" : "700"<br>
          }, {<br>
            "name" : "dfs_datanode_http_port",<br>
            "value" : "1006"<br>
          }, {<br>
            "name" : "dfs_datanode_max_locked_memory"<br>,
            "value" : "4294967296"<br>
          }, {<br>
            "name" : "dfs_datanode_port",<br>
            "value" : "1004"<br>
          }, {<br>
            "name" : "rm_cpu_shares",<br>
            "value" : "400"<br>
          }, {<br>
            "name" : "rm_io_weight",<br>
            "value" : "200"<br>
          } ]<br>
        }, {<br>
          "roleType" : "GATEWAY",<br>
          "items" : [ {<br>
            "name" : "dfs_client_use_trash",<br>
            "value" : "true"<br>
          } ]<br>
        }, {<br>
          "roleTy<br>pe" : "JOURNALNODE",
          "items"<br> : [ {
            "name" : "dfs_journalnode_edits_dir",<br>
            "value" : "/mnt/resource/jn"<br>
          } ]<br>
        }, {<br>
          "roleType" : "NAMENODE",<br>
          "items" : [ {<br>
            "name" : "dfs_name_dir_list",<br>
            "value" : "/mnt/resource/dfs/nn"<br>
          }, {<br>
            "name" : "dfs_namenode_servicerpc_address",<br>
            "value" : "8022"<br>
          } ]<br>
        }, {<br>
          "roleType" : "SECONDARYNAMENODE",<br>
          "items" : [ {<br>
            "name" : "fs_checkpoint_dir_list",<br>
            "value" : "/mnt/resource/dfs/snn"<br>
          } ]<br>
        } ],<br>
        "items" : [ {<br>
          "name" : "dfs_encrypt_data_transfer_algorithm",<br>
          "value" : "AES/CTR/NoPadding"<br>
        }, {<br>
          "name" : "dfs_ha_fencing_cloudera_manager_secret_<br>key",
          "value" : "egsChWomNGnLBTHz0V1qIQcHdW3Ptb"<br>
        }, {<br>
          "name" : "dfs_ha_fencing_methods",<br>
          "value" : "shell(true)"<br>
        }, {<br>
          "name" : "fc_authorization_secret_key",<br>
          "value" : "QdvwB0DVLMFN3StLAB3cTEE7fS0m1B"<br>
        }, {<br>
          "name" : "hadoop_security_authentication",<br>
          "value" : "kerberos"<br>
        }, {<br>
          "name" : "hadoop_security_authorization",<br>
          "value" : "true"<br>
        }, {<br>
          "name" : "http_auth_signature_secret",<br>
          "value" : "0ajPRCMvwFA8sSutFr4pIJjxEsnRff"<br>
        }, {<br>
          "name" : "rm_dirty",<br>
          "value" : "false"<br>
        }, {<br>
          "name" : "rm_last_allocation_percentage",<br>
          "value" : "20"<br>
        }, {<br>
          "name" : "zookeeper_service",<br>
          "value" : "zookeeper"<br>
        } ]<br>
      },<br>
      "roles" : [ {<br>
        "name" : "hdfs-BALANCER-822c6fca1cb8956e904cc265f91cbecf",<br>
        "type" : "BALANCER",<br>
        "hostRef" : {<br>
          "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-DATANODE-20f5b03f45b36e2845bc31ac5ab33b99",<br>
        "type" : "DATANODE",<br>
        "hostRef" : {<br>
          "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "ebto0q4j1ssyl66qj31u6k4fw"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-DATANODE-4a836da64f38f027c69e2e163c6b6567",<br>
        "type" : "DATANODE",<br>
        "hostRef" : {<br>
          "hostId" : "78cdf155-f531-4368-922d-d79da3053f22"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "4s6ebkb3nu0bnupreck0ajsku"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-DATANODE-e662c2c98b3922907a045aa058cdac62",<br>
        "type" : "DATANODE",<br>
        "hostRef" : {<br>
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",
            "value" : "e544qveytzeu4qfehduyseww5"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-822c6fca1cb8956e904cc265f91cbecf",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "b9uiopeon73rrxiuxju0976a6"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-e662c2c98b3922907a045aa058cdac62",<br>
        "type" : "FAILOVERCONTROLLER",<br>
        "hostRef" : {<br>
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "a411qiqgsu9o2zwr5ddw057l3"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-JOURNALNODE-20f5b03f45b36e2845bc31ac5ab33b99",<br>
        "type" : "JOURNALNODE",<br>
        "hostRef" : {<br>
          "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "7hexpmgg5g2fady0ahvl082ed"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-JOURNALNODE-4a836da64f38f027c69e2e163c6b6567",<br>
        "type" : "JOURNALNODE",<br>
        "hostRef" : {<br>
          "hostId" : "78cdf155-f531-4368-922d-d79da3053f22"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "1320gbf5krxazy4778spzfkgb"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-JOURNALNODE-e662c2c98b3922907a045aa058cdac62",<br>
        "type" : "JOURNALNODE",<br>
        "hostRef" : {<br>
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "4e2vsbsguvjwczgpaix2tgr68"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-NAMENODE-822c6fca1cb8956e904cc265f91cbecf",<br>
        "type" : "NAMENODE",<br>
        "hostRef" : {
          "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"<br>
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "50"
          }, {<br>
            "name" : "role_jceks_password",
            "value" : "b58ygwd0lau5ryh9x3o3l2pli"
          } ]
        }
      }, {<br>
        "name" : "hdfs-NAMENODE-e662c2c98b3922907a045aa058cdac62",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"
        },
        "config" : {<br>
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"<br>
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "55"
          }, {
            "name" : "role_jceks_password",
            "value" : "55iih33hfyelvnfvhjqypj3vh"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    }, {
      "name" : "sentry",
      "type" : "SENTRY",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SENTRY_SERVER",
          "items" : [ {
            "name" : "sentry_server_java_heapsize",
            "value" : "268435456"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "sentry_server_database_host",
          "value" : "standaloneln.northcentralus.cloudapp.azure.com"
        }, {
          "name" : "sentry_server_database_password",
          "value" : "Raken.2017"
        }, {
          "name" : "sentry_service_admin_group",
          "value" : "hive,impala,hue,solr,kafka,lotnavarro"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "sentry-GATEWAY-20f5b03f45b36e2845bc31ac5ab33b99",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-GATEWAY-4a836da64f38f027c69e2e163c6b6567",
        "type" : "GATEWAY",
        "hostRef" : {<br>
          "hostId" : "78cdf155-f531-4368-922d-d79da3053f22"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-GATEWAY-822c6fca1cb8956e904cc265f91cbecf",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-GATEWAY-e662c2c98b3922907a045aa058cdac62",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-SENTRY_SERVER-20f5b03f45b36e2845bc31ac5ab33b99",
        "type" : "SENTRY_SERVER",
        "hostRef" : {
          "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f"
        },
        "config" : {
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "zdov5gqcn3tj8cegbscxnwlm"
          } ]
        }<br>
      } ],
      "displayName" : "Sentry"
    } ]
  } ],
  "hosts" : [ {<br>
    "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4",<br>
    "ipAddress" : "10.0.1.5",<br>
    "hostname" : "cdh1.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "config" : {<br>
      "items" : [ ]<br>
    }<br>
  }, {
    "hostId" : "78cdf155-f531-4368-922d-d79da3053f22",<br>
    "ipAddress" : "10.0.1.6",<br>
    "hostname" : "cdh2.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "config" : {<br>
      "items" : [ ]<br>
    }
  }, {
    "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7",<br>
    "ipAddress" : "10.0.1.7",<br>
    "hostname" : "cdh3.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "config" : {<br>
      "items" : [ ]<br>
    }
  }, {
    "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f",<br>
    "ipAddress" : "10.0.1.8",<br>
    "hostname" : "cdh4.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "config" : {<br>
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-822c6fca1cb8956e904cc265f91cbecf",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "759217eeee4144b0c7e2c7a38170bdd23d080b8cecdfe8316613cb2ec1a684fd",
    "pwSalt" : -5468323244130936141,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-822c6fca1cb8956e904cc265f91cbecf",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "0b9f98efee928396a020b3ccb90291d48e99112736d07977b2940f9dbbc22b61",
    "pwSalt" : -6231879538353390713,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-822c6fca1cb8956e904cc265f91cbecf",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "d46e87cbc3406c153f0755f2ec8d49ab1dd66f9f2f91eadfcb7bc4ab4ffa96ec",
    "pwSalt" : -2261311519882765121,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-822c6fca1cb8956e904cc265f91cbecf",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "a75b46054544b3e4ae1ddb8bccfb52f6b1a530c115a164fd72c39718e8c10d30",
    "pwSalt" : -3028082583089130099,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "7e06471a533666ae32aa18cd4da67fe307a62edf6f4ac1e79ae7bdbfd9ac7033",
    "pwSalt" : -6352644935744501662,
    "pwLogin" : true
  }, {
    "name" : "lotnavarro",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "8017b178fbe1a7dfc57dd5a838723e1d5484ddce818ca76313f8b6b6f9e503b9",
    "pwSalt" : -4437129179947148368,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "d843afa49efa52a8d1bc553180c4480616bf58a71b037b5517e5175ea2b68706",
    "pwSalt" : 2025720191126505121,
    "pwLogin" : true<br>
  } ],
  "versionInfo" : {
    "version" : "5.9.1",
    "buildUser" : "jenkins",<br>
    "buildTimestamp" : "20170112-1158",
    "gitHash" : "a66d8bbdbe8bc3ee54235e55423f2f76c7d9f3b1",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",<br>
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",<br>
          "value" : "1610612736"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "standaloneln.northcentralus.cloudapp.azure.com"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "Raken.2017"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {<br>
          "name" : "firehose_non_java_memory_bytes",<br>
          "value" : "1610612736"<br>
        } ]<br>
      } ],<br>
      "items" : [ ]<br>
    },<br>
    "roles" : [ {<br>
      "name" : "mgmt-ALERTPUBLISHER-822c6fca1cb8956e904cc265f91cbecf",<br>
      "type" : "ALERTPUBLISHER",<br>
      "hostRef" : {<br>
        "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"<br>
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "6ykgx5id3r5k0msbntovnwcl5"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-822c6fca1cb8956e904cc265f91cbecf",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9qfq2y0zlh62yv4jw3zwh8y3r"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-822c6fca1cb8956e904cc265f91cbecf",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "bniwk9jz0dlm1zq0farjgbxaw"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-822c6fca1cb8956e904cc265f91cbecf",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "a3ciupa1gxxey1yjxth9316ov"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-822c6fca1cb8956e904cc265f91cbecf",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "8ekp170v6moz22ixfv157bazw"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "AD_USE_SIMPLE_AUTH",
      "value" : "false"
    }, {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/21/2012 16:50"
    }, {
      "name" : "KDC_ADMIN_PASSWORD",
      "value" : "BQIAAAA/AAEADFJBS0VOQ0RILkNPTQAMY2xvdWRlcmEtc2NtAAAAAVofDAkBABcAEOiX/BhZDvIkN04fZL/YVbUAAAAB"
    }, {
      "name" : "KDC_ADMIN_USER",
      "value" : "cloudera-scm@RAKENCDH.COM"
    }, {
      "name" : "KDC_HOST",
      "value" : "standaloneln.northcentralus.cloudapp.azure.com"
    }, {
      "name" : "KRB_ENC_TYPES",
      "value" : "arcfour-hmac"
    }, {
      "name" : "KRB_MANAGE_KRB5_CONF",
      "value" : "true"
    }, {
      "name" : "MAX_RENEW_LIFE",
      "value" : "604800"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "NOT_ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "http://10.0.1.4:8000,https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    }, {
      "name" : "SECURITY_REALM",
      "value" : "RAKENCDH.COM"
    } ]
  }<br>
}<br>

