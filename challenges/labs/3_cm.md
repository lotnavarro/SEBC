<h1>CLOUDERA BOOT CAMP - Challenges - Dec 1, 2017 - CDMX</h1>

<h2>Challenge 3 - Install CDH 5.9</h2>

<br>
<b>2</b><br>
<b>Create user directories in HDFS for saturn and haley</b><br>
<br>



[root@rkn1 raken]#  <code>HADOOP_USER_NAME=hdfs hdfs dfs -mkdir /user/saturn></code><br>
[root@rkn1 raken]# <code>HADOOP_USER_NAME=hdfs hdfs dfs -mkdir /user/haley</code><br>
[root@rkn1 raken]# <code>hdfs dfs -ls /user</code><br>
Found 7 items<br>
drwxr-xr-x   - hdfs   supergroup          0 2017-12-01 14:06 /user/haley<br>
drwxrwxrwx   - mapred hadoop              0 2017-12-01 13:49 /user/history<br>
drwxrwxr-t   - hive   hive                0 2017-12-01 13:51 /user/hive<br>
drwxrwxr-x   - hue    hue                 0 2017-12-01 13:51 /user/hue<br>
drwxrwxr-x   - oozie  oozie               0 2017-12-01 13:52 /user/oozie<br>
drwxr-xr-x   - hdfs   supergroup          0 2017-12-01 14:06 /user/saturn<br>
drwxr-x--x   - spark  spark               0 2017-12-01 13:49 /user/spark<br>
[root@rkn1 raken]# <br>

<br>

[root@rkn1 raken]# curl -u lotnavarro:cloudera \<br>
>  'http://localhost:7180/api/v14/hosts'<br>
{<br>
  "items" : [ {<br>
    "hostId" : "73f7d3b6-0b13-49f7-8cab-3d501851ee34",<br>
    "ipAddress" : "10.0.1.9",<br>
    "hostname" : "rkn1.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "hostUrl" : "http://rkn1.northcentralus.cloudapp.azure.com:7180/cmf/hostRedirect/73f7d3b6-0b13-49f7-8cab-3d501851ee34",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "commissionState" : "COMMISSIONED",<br>
    "numCores" : 8,<br>
    "numPhysicalCores" : 4,<br>
    "totalPhysMemBytes" : 33449582592<br>
  }, {<br>
    "hostId" : "edd3831e-4c6e-4e5d-99a7-498eff07b742",<br>
    "ipAddress" : "10.0.1.5",<br>
    "hostname" : "rkn2.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "hostUrl" : "http://rkn1.northcentralus.cloudapp.azure.com:7180/cmf/hostRedirect/edd3831e-4c6e-4e5d-99a7-498eff07b742",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "commissionState" : "COMMISSIONED",<br>
    "numCores" : 8,<br>
    "numPhysicalCores" : 4,<br>
    "totalPhysMemBytes" : 33449582592<br>
  }, {<br>
    "hostId" : "5ca1f182-cbf4-4cf8-a468-cf656e8efcd6",<br>
    "ipAddress" : "10.0.1.6",<br>
    "hostname" : "rkn3.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "hostUrl" : "http://rkn1.northcentralus.cloudapp.azure.com:7180/cmf/hostRedirect/5ca1f182-cbf4-4cf8-a468-cf656e8efcd6",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "commissionState" : "COMMISSIONED",<br>
    "numCores" : 8,<br>
    "numPhysicalCores" : 4,<br>
    "totalPhysMemBytes" : 33449582592<br>
  }, {<br>
    "hostId" : "0d153006-3695-475f-878d-fd9897c5d748",<br>
    "ipAddress" : "10.0.1.7",<br>
    "hostname" : "rkn4.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "hostUrl" : "http://rkn1.northcentralus.cloudapp.azure.com:7180/cmf/hostRedirect/0d153006-3695-475f-878d-fd9897c5d748",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "commissionState" : "COMMISSIONED",<br>
    "numCores" : 8,<br>
    "numPhysicalCores" : 4,<br>
    "totalPhysMemBytes" : 33449582592<br>
  } ]<br>
}[root@rkn1 raken]#<br>

<br>
}[root@rkn1 raken]# <code>curl -u lotnavarro:cloudera  'http://localhost:7180/api/v8/custers/lotnavarro/services'</code><br>
{<br>
  "items" : [ {<br>
    "name" : "hive",<br>
    "type" : "HIVE",<br>
    "clusterRef" : {<br>
      "clusterName" : "cluster"<br>
    },<br>
    "serviceUrl" : "http://rkn1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/hive",<br><br>
    "serviceState" : "STARTED",<br>
    "healthSummary" : "BAD",<br>
    "healthChecks" : [ {<br>
      "name" : "HIVE_HIVEMETASTORES_HEALTHY",<br>
      "summary" : "BAD"<br>
    }, {<br>
      "name" : "HIVE_HIVESERVER2S_HEALTHY",<br>
      "summary" : "BAD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hive"
  }, {
    "name" : "zookeeper",
    "type" : "ZOOKEEPER",
    "clusterRef" : {
      "clusterName" : "cluster"<br>
    },
    "serviceUrl" : "http://rkn1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/zookeeper",<br>
    "serviceState" : "STARTED",
    "healthSummary" : "BAD",
    "healthChecks" : [ {
      "name" : "ZOOKEEPER_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
      "summary" : "BAD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "ZooKeeper"
  }, {
    "name" : "hue",
    "type" : "HUE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://rkn1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/hue",
    "serviceState" : "STARTED",
    "healthSummary" : "BAD",
    "healthChecks" : [ {
      "name" : "HUE_HUE_SERVERS_HEALTHY",
      "summary" : "BAD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hue"
  }, {
    "name" : "oozie",
    "type" : "OOZIE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://rkn1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/oozie",<br>
    "serviceState" : "STARTED",
    "healthSummary" : "BAD",
    "healthChecks" : [ {
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
      "summary" : "BAD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Oozie"
  }, {
    "name" : "yarn",
    "type" : "YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://rkn1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/yarn",<br>
    "serviceState" : "STARTED",
    "healthSummary" : "BAD",
    "healthChecks" : [ {
      "name" : "YARN_JOBHISTORY_HEALTH",
      "summary" : "BAD"
    }, {
      "name" : "YARN_NODE_MANAGERS_HEALTHY",
      "summary" : "BAD"
    }, {
      "name" : "YARN_RESOURCEMANAGERS_HEALTH",
      "summary" : "BAD"
    }, {
      "name" : "YARN_USAGE_AGGREGATION_HEALTH",<br>
      "summary" : "DISABLED"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "YARN (MR2 Included)"
  }, {
    "name" : "spark_on_yarn",
    "type" : "SPARK_ON_YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://rkn1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/spark_on_yarn",<br>
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Spark"
  }, {
    "name" : "hdfs",
    "type" : "HDFS",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://rkn1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/hdfs",<br>
    "serviceState" : "STARTED",
    "healthSummary" : "BAD",
    "healthChecks" : [ {
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",<br>
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_DATA_NODES_HEALTHY",
      "summary" : "BAD"
    }, {
      "name" : "HDFS_FREE_SPACE_REMAINING",<br>
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_HA_NAMENODE_HEALTH",
      "summary" : "BAD"
    }, {
      "name" : "HDFS_MISSING_BLOCKS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",<br>
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],<br>
    "displayName" : "HDFS"<br>
  } ]<br>
}[root@rkn1 raken]# <br>

