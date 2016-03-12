# init
Initialization functions
##AWS 
###AWS Linux AMIs
```
yum -y update
rpm -qa | grep git
yum -y install git

rpm -qa | grep python34
yum -y install python34
yum -y install python34-pip
yum -y install python34-virtualenv

yum -y install httpd
yum -y install nginx
```

####Apache Web Server
Security Group Basic lesson @ 2:00
```
service httpd status
service httpd start
```


```
[root@ip-172-30-0-110 ec2-user]# chkconfig
acpid          	0:off	1:off	2:on	3:on	4:on	5:on	6:off
atd            	0:off	1:off	2:off	3:on	4:on	5:on	6:off
auditd         	0:off	1:off	2:on	3:on	4:on	5:on	6:off
blk-availability	0:off	1:on	2:on	3:on	4:on	5:on	6:off
cgconfig       	0:off	1:off	2:off	3:off	4:off	5:off	6:off
cgred          	0:off	1:off	2:off	3:off	4:off	5:off	6:off
cloud-config   	0:off	1:off	2:on	3:on	4:on	5:on	6:off
cloud-final    	0:off	1:off	2:on	3:on	4:on	5:on	6:off
cloud-init     	0:off	1:off	2:on	3:on	4:on	5:on	6:off
cloud-init-local	0:off	1:off	2:on	3:on	4:on	5:on	6:off
crond          	0:off	1:off	2:on	3:on	4:on	5:on	6:off
htcacheclean   	0:off	1:off	2:off	3:off	4:off	5:off	6:off
httpd          	0:off	1:off	2:off	3:off	4:off	5:off	6:off
ip6tables      	0:off	1:off	2:on	3:on	4:on	5:on	6:off
iptables       	0:off	1:off	2:on	3:on	4:on	5:on	6:off
irqbalance     	0:off	1:off	2:on	3:on	4:on	5:on	6:off
lvm2-monitor   	0:off	1:on	2:on	3:on	4:on	5:on	6:off
mdmonitor      	0:off	1:off	2:on	3:on	4:on	5:on	6:off
messagebus     	0:off	1:off	2:on	3:on	4:on	5:on	6:off
netconsole     	0:off	1:off	2:off	3:off	4:off	5:off	6:off
netfs          	0:off	1:off	2:off	3:on	4:on	5:on	6:off
network        	0:off	1:off	2:on	3:on	4:on	5:on	6:off
nfs            	0:off	1:off	2:off	3:off	4:off	5:off	6:off
nfslock        	0:off	1:off	2:off	3:on	4:on	5:on	6:off
nginx          	0:off	1:off	2:off	3:off	4:off	5:off	6:off
ntpd           	0:off	1:off	2:on	3:on	4:on	5:on	6:off
ntpdate        	0:off	1:off	2:on	3:on	4:on	5:on	6:off
psacct         	0:off	1:off	2:off	3:off	4:off	5:off	6:off
quota_nld      	0:off	1:off	2:off	3:off	4:off	5:off	6:off
rdisc          	0:off	1:off	2:off	3:off	4:off	5:off	6:off
rngd           	0:off	1:off	2:on	3:on	4:on	5:on	6:off
rpcbind        	0:off	1:off	2:on	3:on	4:on	5:on	6:off
rpcgssd        	0:off	1:off	2:off	3:on	4:on	5:on	6:off
rpcsvcgssd     	0:off	1:off	2:off	3:off	4:off	5:off	6:off
rsyslog        	0:off	1:off	2:on	3:on	4:on	5:on	6:off
saslauthd      	0:off	1:off	2:off	3:off	4:off	5:off	6:off
sendmail       	0:off	1:off	2:on	3:on	4:on	5:on	6:off
sshd           	0:off	1:off	2:on	3:on	4:on	5:on	6:off
udev-post      	0:off	1:on	2:on	3:on	4:on	5:on	6:off
```
`chkconfig httpd on`  <= [makes sure httpd is on after system restart](http://linuxcommand.org/man_pages/chkconfig8.html)

`cd /var/www/html`

`yum -y install links` <= needed for `service httpd fullstatus`



