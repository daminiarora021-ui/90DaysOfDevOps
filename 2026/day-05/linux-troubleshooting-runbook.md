## day -05 ##

* Target service / process will be ssh performed on  aws Ec2 ubuntu instance .


**Environment basics**
Command : `uname -a`, `lsb_release -a` (or `cat /etc/os-release`)
observation : kernal version , architecture and ubuntu details .

![1](images/1.jpg)


![2](images/2.jpg)





**Filesystem sanity** 
Command :  mkdir /tmp/textbook-demo
cp /etc/hosts /tmp/textbook-demo/hosts-copy && ls -l /tmp/textbook-demo

Observation: copied file can be seen in listed directory 

![3](images/3.jpg)




**CPU / Memory** 
 top 
 htop 
 free -h

Observation: System memory usage is moderate and no swap configured

Snapshot: CPU & Memory
![4](images/4.jpg)


![5](images/5.jpg)


![6](images/6.jpg)


**Disk / IO** 
df -h
du -sh /var/log

Observation: Root filesystem is only 12% utilized (17GB available), indicating ample disk capacity and no immediate risk of disk exhaustion. All tmpfs and boot partitions also show minimal usage.

/var/log is only 32MB, indicating logs are under control and not contributing to disk space issues.

 Snapshot: Disk & IO
 
![7](images/7.jpg)



**Network (2):** `ss -tulpn`/`netstat -tulpn`, `curl -I <service-endpoint>`/`ping`

* Snapshot: Network

![net1](images/net1.jpg)

![net2](images/net2.jpg)




**Logs (2):**  journalctl -u ssh -n 50
observation - no signs of service failure , no crashes or persistent SSH errors detected.

* snapshot Logs 

![log](images/log.jpg)



*  Quick findings
- SSH is working fine 
- CPU and memory is moderate 
- disk space is under control 
- no SSH errors detected
