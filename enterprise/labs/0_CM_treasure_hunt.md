<h1>CM Monitoring & Customizing</h1><br>
<h2>CM Monitoring Lab</h2><br>
*What is ubertask optimization?*<br>
<b>Es una configuración de mapreduce que permite ejecutar jobs pequeños de forma secuencial en un mismo "contenedor" JVM<br></b>
*Where in CM is the Kerberos Security Realm value displayed?*<br>
<b>En la siguiente "ruta": Administración->Ajustes->Kerberos->Dominio de seguridad kerberos<br></b>
*Which CDH service(s) host a property for enabling Kerberos authentication?*<br>
<b>Los servicios cliente de autentificación de kerberos: EAuthentication Service (AS) and Ticket Granting Service (TGS) <br></b>
*How do you upgrade the CM agents?*<br>
<b>Actualizando el servidor y el agente de cloudera manager (a la versión deseada) y despues utilizando el asistente que se manda llamar cuando te conectas a la consola de administración ó instalar manualmente todos los paquetes <br></b>
*Give the tsquery statement used to chart Hue's CPU utilization?*<br>
<b>select cpu_system_rate + cpu_user_rate where category=ROLE and serviceName=$SERVICENAME<br></b>
*Name all the roles that make up the Hive service*<br>
<b>metastore server, hive server 2<br></b>
*What steps must be completed before integrating Cloudera Manager with Kerberos?*<br>
<b>

-instalar un KDC funcionando.<br>
-el KDC debe estar configurado para entregar tickets renovables.<br>
-asegurarse que las librerias de LDAP y kerberos esten instaladas en cada cliente<br>
-cloudera manager necesita una cuenta que tenga permisos para crear usuarios en el KDC.<br>
<br></b>



