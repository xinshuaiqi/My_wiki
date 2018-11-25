<<<<<<< HEAD
[TOC]



#﻿EC2

Amazon Elastic Compute Cloud (Amazon EC2) 是一种提供可调节计算容量的 Web 服务 – 简单来说，就是 Amazon 数据中心里的服务器 – 您可以使用它来构建和托管您的软件系统。

### [On-Demand](https://aws.amazon.com/ec2/pricing/on-demand/) 按需

### [Spot Instances](https://aws.amazon.com/ec2/spot/)

### [Reserved Instances](https://aws.amazon.com/ec2/pricing/reserved-instances/)

### [Dedicated Hosts](https://aws.amazon.com/ec2/dedicated-hosts/)

###  







# Amazon Elastic Container Registry (Amazon ECR) 

是一项完全托管的 Docker 容器注册表服务，可让开发人员轻松存储、管理和部署 Docker 容器映像。
=======


>>>>>>> 27fa53e3a1b88d0181fe4f3289c2d573d44bd050

# AWS from LinuxAcademy

 * [AWS concept](https://www.youtube.com/watch?v=LKStwibxbR0&index=1&list=PLv2a_5pNAko2Jl4Ks7V428ttvy-Fj4NKU)
	 * VPC: virtual private cloud
 * [AWS Essentials](https://www.youtube.com/watch?v=BDBvHOaaKHo&list=PLv2a_5pNAko0Mijc6mnv04xeOut443Wnk)
 * [Google Cloud Platform (GCP) for AWS user](https://www.youtube.com/watch?v=IotvQOfdPnA&list=PLv2a_5pNAko1E-W-vjl9SSzDyOljP0-AX)
 * [Project Omega Interactive guide link](http://bit.ly/2guw5gY)




# S3 
* S3 class
	* standard
	* Reduced Redundancy Storage
	* S3-IA
	* Glacier (Archive
* create life-cycle role
* permissions； public sharing
* Versioning


# IAM: Identity and access management
user and group: police and roles
* roles (allow instant (EC2) to access other service (S3) )

# VPC
* Internet GateWay (IGW): like a 路由器
* Route table: provide IP
* NACLs (Network access control lists) ： like a firewall
* subnet <-> Route table
	* public can access internet
	* private can NOT access internet

# RDS w
ith DynamoDB
* RDS:
	* MySQL; Microsoft SQL; PostgreSQL 
* resizeable capacity

* SSH tunning

# SNS 
* simple notification service
	* publishers
	* subscribers

# HPC
https://aws.amazon.com/cn/hpc/?nc1=f_dr

# ﻿EC2

Amazon Elastic Compute Cloud (Amazon EC2) 是一种提供可调节计算容量的 Web 服务 – 简单来说，就是 Amazon 数据中心里的服务器 – 您可以使用它来构建和托管您的软件系统。



# Amazon Elastic Container Registry (Amazon ECR) 

是一项完全托管的 Docker 容器注册表服务，可让开发人员轻松存储、管理和部署 Docker 容器映像。



# Amazon Elastic Container Service (Amazon ECS)

 是一项高度可扩展的快速容器管理服务，可轻松运行、停止和管理 Amazon EC2 实例群集上的 Docker 容器。

- to run, stop, and manage Docker containers on a cluster



# CLI

# batch 

https://docs.aws.amazon.com/zh_cn/cli/latest/reference/batch/index.html

- job submit
- cancel
- queue
- 



Lambda function

https://docs.aws.amazon.com/zh_cn/lambda/latest/dg/python-programming-model.html

YouTube introhttps://articles.extension.org/plant_breeding_genomics

https://www.youtube.com/watch?v=fSUEk6iMW88&index=1&list=PLzvRQMJ9HDiSQMe68cti8cupI0mzLk1Gc





# IAM (Identity and Access Management)

https://aws.amazon.com/cn/iam/


<<<<<<< HEAD



# AWS from LinuxAcademy

 * [AWS concept](https://www.youtube.com/watch?v=LKStwibxbR0&index=1&list=PLv2a_5pNAko2Jl4Ks7V428ttvy-Fj4NKU)
	 * VPC: virtual private cloud
 * [AWS Essentials](https://www.youtube.com/watch?v=BDBvHOaaKHo&list=PLv2a_5pNAko0Mijc6mnv04xeOut443Wnk)
 * [Google Cloud Platform (GCP) for AWS user](https://www.youtube.com/watch?v=IotvQOfdPnA&list=PLv2a_5pNAko1E-W-vjl9SSzDyOljP0-AX)
 * [Project Omega Interactive guide link](http://bit.ly/2guw5gY)




### S3 
* S3 class
	* standard
	* Reduced Redundancy Storage
	* S3-IA
	* Glacier (Archive
* create life-cycle role
* permissions； public sharing
* Versioning
```
aws s3 ls s3://
aws s3 cp --sse AES256


```

### IAM: Identity and access management
user and group: police and roles
* roles (allow instant (EC2) to access other service (S3) )

### VPC
* Internet GateWay (IGW): like a 路由器
* Route table: provide IP
* NACLs (Network access control lists) ： like a firewall
* subnet <-> Route table
	* public can access internet
	* private can NOT access internet

### RDS w
ith DynamoDB
* RDS:
	* MySQL; Microsoft SQL; PostgreSQL 
* resizeable capacity

* SSH tunning

### SNS 
* simple notification service
	* publishers
	* subscribers

### HPC
https://aws.amazon.com/cn/hpc/?nc1=f_dr





# Cost

EC2: 

| t2.2xlarge  | 8             | 变量 | 32 GiB  | 仅限 EBS          | 每小时 0.3712 USD  |
| ----------- | ------------- | ---- | ------- | ----------------- | ------------------ |
| m5.2xlarge  | 8             | 31   | 32 GiB  | 仅限 EBS          | 每小时 0.384 USD   |
| m4.2xlarge  | 8             | 26   | 32 GiB  | 仅限 EBS          | 每小时 0.40 USD    |
| c5.2xlarge  | 8             | 34   | 16 GiB  | 仅限 EBS          | 每小时 0.34 USD    |
| r5.2xlarge  | 8             | 38   | 64 GiB  | 仅限 EBS          | 每小时 0.504 USD   |
| r5d.2xlarge | 8             | 38   | 64 GiB  | 1 个 300 NVMe SSD | 每小时 0.576 USD   |
| i3.2xlarge  | 8             | 27   | 61 GiB  | 1 x 1900 NVMe SSD | 每小时 0.624 USD   |
| d2.2xlarge  | 8             | 28   | 61 GiB  | 6 x 2000 HDD      | 每小时 1.38 USD    |
| m4.16xlarge | 64            | 188  | 256 GiB | 仅限 EBS          | 每小时 3.20 USD    |
| c4.8xlarge  | $1.591 每小时 |      |         |                   | $1.508 每小时 预留 |
| c4.8xlarge  | 36            | 132  | 60 GiB  | 仅限 EBS          | 每小时 1.591 USD   |
| r4.16xlarge | 64            | 195  | 488 GiB | 仅限 EBS          | 每小时 4.256 USD   |
| d2.8xlarge  | 36            | 116  | 244 GiB | 24 x 2000 HDD     | 每小时 5.52 USD    |

0.4 * 24 * 7 = $67 /week

$9.6 / day

https://aws.amazon.com/cn/ec2/pricing/on-demand/

https://aws.amazon.com/cn/ec2/pricing/reserved-instances/pricing/



EFS

1T ~ $300
=======
>>>>>>> 27fa53e3a1b88d0181fe4f3289c2d573d44bd050
