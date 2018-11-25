# Linux tips qxs
 - 以树状列出进程及子进程: `ps axwef` 
 -  改密码 `passwd`
 * 查看CPU: `lscpu` `nproc` 

**系统 uname -a               # 查看内核/操作系统/CPU信息    
 -
 head -n 1 /etc/issue   #
   查看操作系统版本     -
 cat /proc/cpuinfo      # 查看CPU信息     -
 hostname                # 查看计算机名
---- env                    # 查看环境变量

 
**资源**

 free -m                # 查看内存使用量和交换区使用量
 grep MemTotal /proc/meminfo   # 查看内存总量
 grep MemFree /proc/meminfo    # 查看空闲内存量
 uptime                 # 查看系统运行时间、用户数、负载
 cat /proc/loadavg      # 查看系统负载

**磁盘和分区**
 mount | column -t      # 查看挂接的分区状态
 fdisk -l               # 查看所有分区
 swapon -s              # 查看所有交换分区
 hdparm -i /dev/hda     # 查看磁盘参数(仅适用于IDE设备)
 dmesg | grep IDE       # 查看启动时IDE设备检测状况

**网络**
 - ifconfig               # 查看所有网络接口的属性    


**进程**
 ps -ef                 # 查看所有进程
 top                    # 实时显示进程状态
用户
 w                      # 查看活动用户
 id <用户名>            # 查看指定用户信息
 last                   # 查看用户登录日志
 cut -d: -f1 /etc/passwd   # 查看系统所有用户
 cut -d: -f1 /etc/group    # 查看系统所有组
 crontab -l             # 查看当前用户的计划任务
服务
 chkconfig --list       # 列出所有系统服务
 chkconfig --list | grep on    # 列出所有启动的系统服务
程序
 rpm -qa                # 查看所有安装的软件包




## touch file1 file2 file3
create 3 new empty files. 








# Cluster and HPC

### https://www.oreilly.com/library/view/high-performance-linux/0596005709/ch01.html


Centralized multiprocessors
- uniform memory access (UMA)/symmetric multiprocessors (SMP)
- nonuniform memory access (NUMA):
  -  each CPU maintains its own piece of memory
-  processor array
  -  a type of vector computer built with a collection of identical, synchronized processing elements. 

Cluster three elements:
- a collection of individual computers, 
- a network connecting those computers, and 
- software that enables a computer to share work among the other computers via the network.


Cluster structure
-  symmetric cluster 
  - each node can function as an individual computer
  - Cluster management and security can be more difficult. Workload distribution can become a problem, making it more difficult to achieve optimal performance.
- asymmetric architecture
- high level of security
- keep all customizations on head node 
- performance limitations imposed by the cluster head

I/O represents a particular challenge. It is often desirable to distribute a shared filesystem across a number of machines within the cluster to allow parallel access. 

Network design is another key issue. Examples include hyper-tree, hyper-cube, butterfly, and shuffle-exchange networks.

**High-availability clusters**, also called failover clusters, are often used in mission-critical applications. If you can't afford the lost business that will result from having your web server go down, you may want to implement it using a HA cluster.
**load-balancing cluster **is to provide better performance by dividing the work among multiple computers. 





