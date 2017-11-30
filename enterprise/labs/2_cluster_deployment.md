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
     '''
 "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HUE_SERVER",
          "items" : [ {
            "name" : "hue_server_bind_wildcard",
            "value" : "true"
          } ]
        } ],
        "items" : [ {
          "name" : "database_host",
          "value" : "standaloneln.northcentralus.cloudapp.azure.com"
        }, {
          "name" : "database_password",
          "value" : "Raken.2017"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-822c6fca1cb8956e904cc265f91cbecf"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "sentry_service",
          "value" : "sentry"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-e662c2c98b3922907a045aa058cdac62",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2tzrt3551ssef64ftofbylhph"
          }, {
            "name" : "secret_key",
            "value" : "2cqifcdCnW3t9ckSbLRpsPUc2eQ27p"
          } ]
        }
      }, {
        "name" : "hue-KT_RENEWER-e662c2c98b3922907a045aa058cdac62",
        "type" : "KT_RENEWER",
        "hostRef" : {
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "czrlfih37h54k8hq6ga4k95uj"
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
            "value" : "standaloneln.northcentralus.cloudapp.azure.com"
          }, {
            "name" : "oozie_database_password",
            "value" : "Raken.2017"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
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
        "name" : "oozie-OOZIE_SERVER-4a836da64f38f027c69e2e163c6b6567",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "78cdf155-f531-4368-922d-d79da3053f22"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6uk2spjpa7rkmq3t030mij4x0"
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
            "value" : "12"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "1"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/mnt/resource/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/mnt/resource/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "15433"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "15433"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "6"
          } ]
        } ],
        "items" : [ {
          "name" : "hadoop_secure_web_ui",
          "value" : "true"
        }, {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "80"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "03Knehjejrk04brAwAUoli799pD4PE"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-822c6fca1cb8956e904cc265f91cbecf",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2awplfl52ziogpzynok8ln2yi"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-20f5b03f45b36e2845bc31ac5ab33b99",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5pghgzszybut1q5mxoj1qr6q6"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-4a836da64f38f027c69e2e163c6b6567",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "78cdf155-f531-4368-922d-d79da3053f22"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "29nwt7o6q96vmzqkcyb25hnvt"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-e662c2c98b3922907a045aa058cdac62",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "abslrpeth19m0bk0c8n50jnm3"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-4a836da64f38f027c69e2e163c6b6567",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "78cdf155-f531-4368-922d-d79da3053f22"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "48"
          }, {
            "name" : "role_jceks_password",
            "value" : "aah53mf9gvcgtxti0ij26fy8g"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/mnt/resource/dfs/dn"
          }, {
            "name" : "dfs_datanode_data_dir_perm",
            "value" : "700"
          }, {
            "name" : "dfs_datanode_http_port",
            "value" : "1006"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "dfs_datanode_port",
            "value" : "1004"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "400"
          }, {
            "name" : "rm_io_weight",
            "value" : "200"
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
            "value" : "/mnt/resource/jn"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/mnt/resource/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/mnt/resource/dfs/snn"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_encrypt_data_transfer_algorithm",
          "value" : "AES/CTR/NoPadding"
        }, {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "egsChWomNGnLBTHz0V1qIQcHdW3Ptb"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "QdvwB0DVLMFN3StLAB3cTEE7fS0m1B"
        }, {
          "name" : "hadoop_security_authentication",
          "value" : "kerberos"
        }, {
          "name" : "hadoop_security_authorization",
          "value" : "true"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "0ajPRCMvwFA8sSutFr4pIJjxEsnRff"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "20"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-822c6fca1cb8956e904cc265f91cbecf",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-20f5b03f45b36e2845bc31ac5ab33b99",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ebto0q4j1ssyl66qj31u6k4fw"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-4a836da64f38f027c69e2e163c6b6567",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "78cdf155-f531-4368-922d-d79da3053f22"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4s6ebkb3nu0bnupreck0ajsku"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-e662c2c98b3922907a045aa058cdac62",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"
        },
        "config" : {
          "items" : [ {
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
        "name" : "hdfs-FAILOVERCONTROLLER-e662c2c98b3922907a045aa058cdac62",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "a411qiqgsu9o2zwr5ddw057l3"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-20f5b03f45b36e2845bc31ac5ab33b99",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7hexpmgg5g2fady0ahvl082ed"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-4a836da64f38f027c69e2e163c6b6567",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "78cdf155-f531-4368-922d-d79da3053f22"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1320gbf5krxazy4778spzfkgb"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-e662c2c98b3922907a045aa058cdac62",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4e2vsbsguvjwczgpaix2tgr68"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-822c6fca1cb8956e904cc265f91cbecf",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"
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
            "value" : "50"
          }, {
            "name" : "role_jceks_password",
            "value" : "b58ygwd0lau5ryh9x3o3l2pli"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-e662c2c98b3922907a045aa058cdac62",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7"
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
        "hostRef" : {
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
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "zdov5gqcn3tj8cegbscxnwlm"
          } ]
        }
      } ],
      "displayName" : "Sentry"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4",
    "ipAddress" : "10.0.1.5",
    "hostname" : "cdh1.northcentralus.cloudapp.azure.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "78cdf155-f531-4368-922d-d79da3053f22",
    "ipAddress" : "10.0.1.6",
    "hostname" : "cdh2.northcentralus.cloudapp.azure.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "6cdc1302-344c-42a2-b2db-f3a1111362c7",
    "ipAddress" : "10.0.1.7",
    "hostname" : "cdh3.northcentralus.cloudapp.azure.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "244c9686-c4c6-4582-a12d-b230896fb57f",
    "ipAddress" : "10.0.1.8",
    "hostname" : "cdh4.northcentralus.cloudapp.azure.com",
    "rackId" : "/default",
    "config" : {
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
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.9.1",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170112-1158",
    "gitHash" : "a66d8bbdbe8bc3ee54235e55423f2f76c7d9f3b1",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
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
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-822c6fca1cb8956e904cc265f91cbecf",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "f22e8027-06a2-4674-b81b-10f16110ffa4"
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
  }
}
'''

