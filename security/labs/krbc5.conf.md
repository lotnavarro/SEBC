<h1> Integrating Kerberos with Cloudera Manager</h1><br>
<br>
<h2>/etc/krb5.conf as krb5.conf.md</h2>
<br>

# Configuration snippets may be placed in this directory as well<br>
includedir /etc/krb5.conf.d/<br>
<br>
[logging]<br>
 default = FILE:/var/log/krb5libs.log<br>
 kdc = FILE:/var/log/krb5kdc.log<br>
 admin_server = FILE:/var/log/kadmind.log<br>
<br>
[libdefaults]<br>
 dns_lookup_realm = false<br>
 ticket_lifetime = 24h<br>
 renew_lifetime = 7d<br>
 forwardable = true<br>
 udp_preference_limit = 1<br>
 **default_tgs_enctypes = arcfour-hmac**<br>
 **default_tkt_enctypes = arcfour-hmac**<br>
 rdns = false<br>
 **default_realm = RAKENCDH.COM**<br>
 default_ccache_name = KEYRING:persistent:%{uid}<br>
<br>
[realms]<br>
 **RAKENCDH.COM** = {<br>
  **kdc = standaloneln.northcentralus.cloudapp.azure.com**<br>
  **admin_server = standaloneln.northcentralus.cloudapp.azure.com**<br>
 }<br>
<br>
[domain_realm]<br>
 **.northcentralus.cloudapp.azure.com = RAKENCDH.com**<br>
 **northcentralus.cloudapp.azure.com = RAKENCDH.com**<br>
<br>
