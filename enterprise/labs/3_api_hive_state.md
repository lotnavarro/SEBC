<h1>CM Lab - Use the API</h1><br>
<h2>Write curl statements that stop, start, and check the current state of your Hive service.</h2><br>
<br>
<b>Start Hive Service</b><br>

<code>[raken@cdh1 ~]$ curl -X POST -u lotnavarro:cloudera  'http://localhost:7180/api/v14/clusters/lotnavarro/services/hive/commands/stop'</code><br>
{<br>
  "id" : 1192,<br>
  "name" : "Stop",<br>
  "startTime" : "2017-11-30T18:16:54.684Z",<br>
  "active" : true,<br>
  "serviceRef" : {<br>
    "clusterName" : "cluster",<br>
    "serviceName" : "hive"<br>
  }<br>
}[raken@cdh1 ~]$ <br>

<b>Check Hive Service</b><br>
<code>[raken@cdh1 ~]$ curl u lotnavarro:cloudera  'http://localhost:7180/api/v12/clusters/lotnavarro/services/hive/'</code><br>
{<br>
  "name" : "hive",<br>
  "type" : "HIVE",<br>
  "clusterRef" : {<br>
    "clusterName" : "cluster"<br>
  },<br>
  "serviceUrl" : "http://cdh1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/hive",<br>
  "roleInstancesUrl" : "http://cdh1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/hive/instances",<br>
  "serviceState" : "STOPPED",<br>
  "healthSummary" : "DISABLED",<br>
  "healthChecks" : [ {<br>
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",<br>
    "summary" : "DISABLED",<br>
    "suppressed" : false<br>
  }, {<br>
    "name" : "HIVE_HIVESERVER2S_HEALTHY",<br>
    "summary" : "DISABLED",<br>
    "suppressed" : false<br>
  } ],<br>
  "configStalenessStatus" : "FRESH",<br>
  "clientConfigStalenessStatus" : "FRESH",<br>
  "maintenanceMode" : false,<br>
  "maintenanceOwners" : [ ],<br>
  "displayName" : "Hive",<br>
  "entityStatus" : <b>"STOPPED"</b><br>
[raken@cdh1 ~]$ <br>


<br>
<b>Start Hive Service</b><br>

<code>[raken@cdh1 ~]$ curl -X POST -u lotnavarro:cloudera  'http://localhost:7180/api/v14/clusters/lotnavarro/services/hive/commands/start'</code><br>
{<br>
  "id" : 1198,<br>
  "name" : "Start",<br>
  "startTime" : "2017-11-30T18:23:19.313Z",<br>
  "active" : true,<br>
  "serviceRef" : {<br>
    "clusterName" : "cluster",<br>
    "serviceName" : "hive"<br>
  }<br>
}[raken@cdh1 ~]$ <br>


<br>
<b>Check Hive Service</b><br>
<code>[raken@cdh1 ~]$ curl u lotnavarro:cloudera  'http://localhost:7180/api/v12/clusters/lotnavarro/services/hive/'</code><br>
{<br>
  "name" : "hive",<br>
  "type" : "HIVE",<br>
  "clusterRef" : {<br>
    "clusterName" : "cluster"<br>
  },<br>
  "serviceUrl" : "http://cdh1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/hive",<br>
  "roleInstancesUrl" : "http://cdh1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/hive/instances",<br>
  "serviceState" : "STARTED",<br>
  "healthSummary" : "GOOD",<br>
  "healthChecks" : [ {<br>
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",<br>
    "summary" : "GOOD",<br>
    "suppressed" : false<br>
  }, {<br>
    "name" : "HIVE_HIVESERVER2S_HEALTHY",<br>
    "summary" : "GOOD",<br>
    "suppressed" : false<br>
  } ],<br>
  "configStalenessStatus" : "FRESH",<br>
  "clientConfigStalenessStatus" : "FRESH",<br>
  "maintenanceMode" : false,<br>
  "maintenanceOwners" : [ ],<br>
  "displayName" : "Hive",<br>
  "entityStatus" : "<b>GOOD_HEALTH</b>"<br>
[raken@cdh1 ~]$ <br>
<br>
<br>

