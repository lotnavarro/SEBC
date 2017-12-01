<h1>CLOUDERA BOOT CAMP - Challenges - Dec 1, 2017 - CDMX</h1>

<h2>Challenge Setup</h2>

<br>
<b>1</b><br>
<b>List the cloud provider you are using (AWS, GCE, Azure, CloudCat, other)</b><br>
<b>
Microsoft Azure</b><br>
<code>https://portal.azure.com/#resource/subscriptions/b335b92c-330e-4c52-b013-3fb701403517/resourceGroups/lotnavarro/overview</code><br>
</b>
<br>
<b>2</b><br>

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

<br>
<b>3</b><br>

<b>List the Linux release you are using</b><br>
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



<br>
<b>4</b><br>


<b>List the file system capacity for the first node</b><br>
<code>
[root@rkn1 raken]# df -h
</code><br>

Filesystem      Size  Used Avail Use% Mounted on<br>
devtmpfs         16G     0   16G   0% /dev<br>
tmpfs            16G     0   16G   0% /dev/shm<br>
tmpfs            16G  8.3M   16G   1% /run<br>
tmpfs            16G     0   16G   0% /sys/fs/cgroup<br>
/dev/sda2        30G  1.8G   26G   7% /<br>
/dev/sda1       497M  112M  386M  23% /boot<br>
/dev/sdb1       197G  2.1G  185G   2% /mnt/resource<br>
tmpfs           3.2G     0  3.2G   0% /run/user/1000<br>
[root@rkn1 raken]# <br>

<br>
<b>5</b><br>

<b>List the command and output for yum repolist enabled</b>
<code>
[root@rkn1 raken]# yum repolist enabled</code><br>
Loaded plugins: ulninfo<br>
repo id            repo name                                        status<br>
!ol7_UEKR4/x86_64  Latest Unbreakable Enterprise Kernel Release 4 f      394+105<br>
!ol7_addons/x86_64 Oracle Linux 7Server Add ons (x86_64)                  172+77<br>
!ol7_latest/x86_64 Oracle Linux 7Server Latest (x86_64)             18,018+5,194<br>
repolist: 18,584<br>
[root@rkn1 raken]# <br>




