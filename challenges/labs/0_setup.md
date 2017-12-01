<h1>

<h2>

<br>
<b>1</b><br>
List the cloud provider you are using (AWS, GCE, Azure, CloudCat, other)<br>
<b>
Microsoft Azure<br>
<code>https://portal.azure.com/#resource/subscriptions/b335b92c-330e-4c52-b013-3fb701403517/resourceGroups/lotnavarro/overview</code><br>
</b>
List your instances by IP address and DNS name (don't use /etc/hosts for this)<br>
<code>
[root@rkn1 raken]# cat /etc/hosts</code><br>
127.0.0.1   localhost localhost.localdomain localhost4 localhost4.localdomain4<br>
::1         localhost localhost.localdomain localhost6 localhost6.localdomain6<br>
<br>
<code>[root@rkn1 raken]# ping rkn1.northcentralus.cloudapp.azure.com<br></code>

64 bytes from rkn1.northcentralus.cloudapp.azure.com (10.0.1.9): icmp_seq=1 ttl=64 time=0.029 ms<br>
64 bytes from rkn1.northcentralus.cloudapp.azure.com (10.0.1.9): icmp_seq=2 ttl=64 time=0.028 ms<br>
64 bytes from rkn1.northcentralus.cloudapp.azure.com (10.0.1.9): icmp_seq=3 ttl=64 time=0.030 ms<br>
^C<br>
--- rkn1.northcentralus.cloudapp.azure.com ping statistics ---<br>
3 packets transmitted, 3 received, 0% packet loss, time 2000ms<br>
rtt min/avg/max/mdev = 0.028/0.029/0.030/0.000 ms<br>
<code>[root@rkn1 raken]# ping rkn2.northcentralus.cloudapp.azure.com<br></code>
PING rkn2.northcentralus.cloudapp.azure.com (10.0.1.5) 56(84) bytes of data.<br>
64 bytes from cdh1.northcentralus.cloudapp.azure.com (10.0.1.5): icmp_seq=1 ttl=64 time=2.36 ms<br>
64 bytes from cdh1.northcentralus.cloudapp.azure.com (10.0.1.5): icmp_seq=2 ttl=64 time=0.599 ms<br>
64 bytes from cdh1.northcentralus.cloudapp.azure.com (10.0.1.5): icmp_seq=3 ttl=64 time=1.38 ms<br>
^C<br>
--- rkn2.northcentralus.cloudapp.azure.com ping statistics ---<br>
3 packets transmitted, 3 received, 0% packet loss, time 2001ms<br>
rtt min/avg/max/mdev = 0.599/1.451/2.366/0.723 ms<br>
<code>[root@rkn1 raken]# ping rkn3.northcentralus.cloudapp.azure.com<br></code>
PING rkn3.northcentralus.cloudapp.azure.com (10.0.1.6) 56(84) bytes of data.<br>
64 bytes from cdh2.northcentralus.cloudapp.azure.com (10.0.1.6): icmp_seq=1 ttl=64 time=8.57 ms<br>
64 bytes from cdh2.northcentralus.cloudapp.azure.com (10.0.1.6): icmp_seq=2 ttl=64 time=0.589 ms<br>
64 bytes from cdh2.northcentralus.cloudapp.azure.com (10.0.1.6): icmp_seq=3 ttl=64 time=1.42 ms<br>
^C<br>
--- rkn3.northcentralus.cloudapp.azure.com ping statistics ---<br>
3 packets transmitted, 3 received, 0% packet loss, time 2002ms<br>
rtt min/avg/max/mdev = 0.589/3.531/8.578/3.585 ms<br>
<code>[root@rkn1 raken]# ping rkn4.northcentralus.cloudapp.azure.com<br></code>
PING rkn4.northcentralus.cloudapp.azure.com (10.0.1.7) 56(84) bytes of data.<br>
64 bytes from cdh3.northcentralus.cloudapp.azure.com (10.0.1.7): icmp_seq=1 ttl=64 time=8.36 ms<br>
64 bytes from cdh3.northcentralus.cloudapp.azure.com (10.0.1.7): icmp_seq=2 ttl=64 time=0.734 ms<br>
64 bytes from cdh3.northcentralus.cloudapp.azure.com (10.0.1.7): icmp_seq=3 ttl=64 time=0.678 ms<br>
^C<br>
--- rkn4.northcentralus.cloudapp.azure.com ping statistics ---<br>
3 packets transmitted, 3 received, 0% packet loss, time 2001ms<br>
rtt min/avg/max/mdev = 0.678/3.258/8.362/3.609 ms<br>
[root@rkn1 raken]# <br>
<br>



List the Linux release you are using<br>
<code>[root@rkn1 raken]# cat /etc/*release</code><br>
Oracle Linux Server release 7.3<br>
NAME="Oracle Linux Server"<br>
VERSION="7.3"<br>
ID="ol"<br>
VERSION_ID="7.3"<br>
PRETTY_NAME="Oracle Linux Server 7.3"<br>
ANSI_COLOR="0;31"<br>
CPE_NAME="cpe:/o:oracle:linux:7:3:server"<br>
HOME_URL="https://linux.oracle.com/"<br>
BUG_REPORT_URL="https://bugzilla.oracle.com/"<br>
<br>
ORACLE_BUGZILLA_PRODUCT="Oracle Linux 7"<br>
ORACLE_BUGZILLA_PRODUCT_VERSION=7.3<br>
ORACLE_SUPPORT_PRODUCT="Oracle Linux"<br>
ORACLE_SUPPORT_PRODUCT_VERSION=7.3<br>
<b>Red Hat Enterprise Linux Server release 7.3 (Maipo)</b><br>
<b>Oracle Linux Server release 7.3</b><br>
[root@rkn1 raken]# 






List the file system capacity for the first node<br>
<code>

</code>

List the command and output for yum repolist enabled<br>
<code>

</code>

