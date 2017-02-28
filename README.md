kconnp
======

The connection pool in linux kernel layer.

###Requires：
 * X86 CPU
 * Linux Kernel Version >= 2.6.18
 * Host OR VM (KVM,XEN,Vmware, etc)

### Installation
1. $git clone https://github.com/zzgang/kconnp.git
1. $cd kconnp
1. $./configure
1. $make 
1. $make install

### Usage
#####Commands
kconnp (stats|ldcfg|start|stop|restart)
* stats: output the statistics information
* ldcfg: reload the config
* start: start the service
* stop: shutdown the service
* restart: restart the service

#####Configuration 
######Files
* Global: /etc/kconnp.conf
* White list for ACL: /etc/iports.allow
* Black list for ACL: /etc/iports.deny

######Explains
* The priority of black list is higher than white black list.
* If the iport is specified，the connections will be pre-connected.
* If the connection is configured stateful (tag: (S))，each connection only be use one time before closing. 


**E-Mail:**：zzgang2008@foxmail.com
