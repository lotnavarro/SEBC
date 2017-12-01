<h1>CLOUDERA BOOT CAMP - Challenges - Dec 1, 2017 - CDMX</h1>

<h2>Challenge 5 KERBEROS</h2>

<br>
<b>1</b><br>
<b>KERBEROS</b><br>
<br>
<H2>KDC CONFIG</H2>
kdcdefaults]<br>
 kdc_ports = 88<br>
 kdc_tcp_ports = 88<br>
<br>
[realms]<br>
 LOTNAVARRO.HQ.COM = {<br>
  #master_key_type = aes256-cts<br>
  acl_file = /var/kerberos/krb5kdc/kadm5.acl<br>
  dict_file = /usr/share/dict/words<br>
  admin_keytab = /var/kerberos/krb5kdc/kadm5.keytab<br>
  supported_enctypes = aes256-cts:normal aes128-cts:normal des3-hmac-sha1:norma$<br>
  max_life = 1d<br>
  max_renewable_life = 7d<br>
 }<br>

<H2>Krb5</H2><br>
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
 default_tgs_enctypes = arcfour-hmac<br>
 default_tkt_enctypes = arcfour-hmac<br>
 rdns = false<br>
 default_realm = LOTNAVARRO.HQ.COM<br>
 default_ccache_name = KEYRING:persistent:%{uid}<br>
<br>
[realms]<br>
 RAKENCDH.COM = {<br>
  kdc = standaloneln.northcentralus.cloudapp.azure.com<br>
  admin_server = standaloneln.northcentralus.cloudapp.azure.com<br>
 }<br>

[domain_realm]<br>
 .northcentralus.cloudapp.azure.com = LOTNAVARRO.HQ.com<br>
 northcentralus.cloudapp.azure.com = LOTNAVARRO.HQ.com<br>
<br>

<H2>acl</H2><br>
<br>


*/admin@LOTNAVARRO.HQ.COM	*
cloudera-scm@LOTNAVARRO.HQ.COM admilc




