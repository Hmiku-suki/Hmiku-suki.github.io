---
title: 'Associate Cloud Engineer Exam Guide'
date: 2021-01-19 13:39:39
tags: GCP
category: Cloud
---
此篇记录了Associate Cloud Engineer的官方Exam Guide。
<!-- more -->

## Associate Cloud Engineer
先来个链接  
<https://cloud.google.com/certification/guides/cloud-engineer>  

### Setting up a cloud solution environment
1. Setting up cloud projects and accounts.  
    Activities include:
    - Creating projects
    - Assigning users to predefined IAM roles within a project
    - Managing users in Cloud Identity (manually and automated)
    - Enabling APIs within projects
    - Provisioning one or more Stackdriver workspaces
2. Managing billing configuration.  
    Activities include:
    - Creating one or more billing accounts
    - Linking projects to a billing account
    - Establishing billing budgets and alerts
    - Setting up billing exports to estimate daily/monthly charges
3. Installing and configuring the command line interface (CLI), specifically the Cloud SDK (e.g., setting the default project).  

### Planning and configuring a cloud solution
1. Planning and estimating GCP product use using the Pricing Calculator
2. Planning and configuring compute resources. 
    Considerations include:
    - Selecting appropriate compute choices for a given workload (e.g., Compute Engine, Google Kubernetes Engine, App Engine, Cloud Run, Cloud Functions)
    - Using preemptible VMs and custom machine types as appropriate
3. Planning and configuring data storage options. 
    Considerations include:
    - Product choice (e.g., Cloud SQL, BigQuery, Cloud Spanner, Cloud Bigtable)
    - Choosing storage options (e.g., Standard, Nearline, Coldline, Archive)
4. Planning and configuring network resources. 
    Tasks include:
    - Differentiating load balancing options
    - Identifying resource locations in a network for availability
    - Configuring Cloud DNS  

### Deploying and implementing a cloud solution  
1. Deploying and implementing Compute Engine resources. 
    Tasks include:
    - Launching a compute instance using Cloud Console and Cloud SDK (gcloud) (e.g., assign disks, availability policy, SSH keys)
    - Creating an autoscaled managed instance group using an instance template
    - Generating/uploading a custom SSH key for instances
    - Configuring a VM for Stackdriver monitoring and logging
    - Assessing compute quotas and requesting increases
    - Installing the Stackdriver Agent for monitoring and logging
2. Deploying and implementing Google Kubernetes Engine resources. 
    Tasks include:
    - Deploying a Google Kubernetes Engine cluster
    - Deploying a container application to Google Kubernetes Engine using pods
    - Configuring Google Kubernetes Engine application monitoring and logging
3. Deploying and implementing App Engine, Cloud Run, and Cloud Functions resources. 
    Tasks include, where applicable:
    - Deploying an application, updating scaling configuration, versions, and traffic splitting
    - Deploying an application that receives Google Cloud events (e.g., Cloud Pub/Sub events, Cloud Storage object change notification events)
4. Deploying and implementing data solutions. 
    Tasks include:
    - Initializing data systems with products (e.g., Cloud SQL, Cloud Datastore, BigQuery, Cloud Spanner, Cloud Pub/Sub, Cloud Bigtable, Cloud Dataproc, Cloud Dataflow, Cloud Storage)
    - Loading data (e.g., command line upload, API transfer, import/export, load data from Cloud Storage, streaming data to Cloud Pub/Sub)
5. Deploying and implementing networking resources. 
    Tasks include:
    - Creating a VPC with subnets (e.g., custom-mode VPC, shared VPC)
    - Launching a Compute Engine instance with custom network configuration (e.g., internal-only IP address, Google private access, static external and private IP address, network tags)
    - Creating ingress and egress firewall rules for a VPC (e.g., IP subnets, tags, service accounts)
    - Creating a VPN between a Google VPC and an external network using Cloud VPN
    - Creating a load balancer to distribute application network traffic to an application (e.g., Global HTTP(S) load balancer, Global SSL Proxy load balancer, Global TCP Proxy load balancer, regional network load balancer, regional internal load balancer)
6. Deploying a solution using Cloud Marketplace. 
    Tasks include:
    - Browsing Cloud Marketplace catalog and viewing solution details
    - Deploying a Cloud Marketplace solution
7. Deploying application infrastructure using Cloud Deployment Manager. 
    Tasks include:
    - Developing Deployment Manager templates
    - Launching a Deployment Manager template  

### Ensuring successful operation of a cloud solution  
1. Managing Compute Engine resources. 
    Tasks include:
    - Managing a single VM instance (e.g., start, stop, edit configuration, or delete an instance)
    - SSH/RDP to the instance
    - Attaching a GPU to a new instance and installing CUDA libraries
    - Viewing current running VM inventory (instance IDs, details)
    - Working with snapshots (e.g., create a snapshot from a VM, view snapshots, delete a snapshot)
    - Working with images (e.g., create an image from a VM or a snapshot, view images, delete an image)
    - Working with instance groups (e.g., set autoscaling parameters, assign instance template, create an instance template, remove instance group)
    - Working with management interfaces (e.g., Cloud Console, Cloud Shell, GCloud SDK)
2. Managing Google Kubernetes Engine resources. 
    Tasks include:
    - Viewing current running cluster inventory (nodes, pods, services)
    - Browsing the container image repository and viewing container image details
    - Working with node pools (e.g., add, edit, or remove a node pool)
    - Working with pods (e.g., add, edit, or remove pods)
    - Working with services (e.g., add, edit, or remove a service)
    - Working with stateful applications (e.g. persistent volumes, stateful sets)
    - Working with management interfaces (e.g., Cloud Console, Cloud Shell, Cloud SDK)
3. Managing App Engine and Cloud Run resources. 
    Tasks include:
    - Adjusting application traffic splitting parameters
    - Setting scaling parameters for autoscaling instances
    - Working with management interfaces (e.g., Cloud Console, Cloud Shell, Cloud SDK)
4. Managing storage and database solutions. 
    Tasks include:
    - Moving objects between Cloud Storage buckets
    - Converting Cloud Storage buckets between storage classes
    - Setting object life cycle management policies for Cloud Storage buckets
    - Executing queries to retrieve data from data instances (e.g., Cloud SQL, BigQuery, Cloud Spanner, Cloud Datastore, Cloud Bigtable)
    - Estimating costs of a BigQuery query
    - Backing up and restoring data instances (e.g., Cloud SQL, Cloud Datastore)
    - Reviewing job status in Cloud Dataproc, Cloud Dataflow, or BigQuery
    - Working with management interfaces (e.g., Cloud Console, Cloud Shell, Cloud SDK)
5. Managing networking resources. 
    Tasks include:
    - Adding a subnet to an existing VPC
    - Expanding a subnet to have more IP addresses
    - Reserving static external or internal IP addresses
    - Working with management interfaces (e.g., Cloud Console, Cloud Shell, Cloud SDK)
6. Monitoring and logging. 
    Tasks include:
    - Creating Stackdriver alerts based on resource metrics
    - Creating Stackdriver custom metrics
    - Configuring log sinks to export logs to external systems (e.g., on-premises or BigQuery)
    - Viewing and filtering logs in Stackdriver
    - Viewing specific log message details in Stackdriver
    - Using cloud diagnostics to research an application issue (e.g., viewing Cloud Trace data, using Cloud Debug to view an application point-in-time)
    - Viewing Google Cloud Platform status
    - Working with management interfaces (e.g., Cloud Console, Cloud Shell, Cloud SDK)  

### Configuring access and security  
1. Managing identity and access management (IAM). 
    Tasks include:
    - Viewing IAM role assignments
    - Assigning IAM roles to accounts or Google Groups
    - Defining custom IAM roles
2. Managing service accounts. 
    Tasks include:
    - Managing service accounts with limited privileges
    - Assigning a service account to VM instances
    - Granting access to a service account in another project
3. Viewing audit logs for project and managed services.


## 中文版见这里

### 设置云解决方案环境
1. 设置云项目和帐户  
    Activities include:
    - 创建项目
    - 将用户分配给项目中的预定义IAM角色
    - 在Cloud Identity中管理用户(手动和自动)
    - 在项目中启用API
    - 设置一个或多个Stackdriver工作区
2. 管理计费配置  
    Activities include:
    - 创建一个或多个计费帐户
    - 将项目链接到计费帐户
    - 建立帐单预算和警告
    - 设置结算出口以估算每日/每月费用
3. 安装和配置命令行界面(CLI)，尤其是Cloud SDK(例如，设置默认项目)   

### 规划和配置云解决方案
1. 使用价格计算器规划和估计GCP产品的使用情况
2. 规划和配置计算资源  
    Considerations include:
    - 为给定的工作负载选择适当的计算选项 (e.g., Compute Engine, Google Kubernetes Engine, App Engine, Cloud Run, Cloud Functions)
    - 适当使用preemptible VMs和自定义机器类型
3. 规划和配置数据存储选项  
    Considerations include:
    - 产品选择 (e.g., Cloud SQL, BigQuery, Cloud Spanner, Cloud Bigtable)
    - 选择存储选项 (e.g., Standard, Nearline, Coldline, Archive)
4. 规划和配置网络资源  
    Tasks include:
    - 区分负载均衡选项
    - 识别网络中的资源位置以提高可用性
    - 配置云DNS  

### 部署和实施云解决方案  
1. 部署和实施Compute Engine资源  
    Tasks include:
    - 使用Cloud Console和Cloud SDK(gcloud)启动计算实例 (e.g., assign disks, availability policy, SSH keys)
    - 使用实例模板创建自动缩放的托管实例组
    - 为实例生成/上传自定义SSH密钥
    - 配置VM以进行Stackdriver监视和记录
    - 评估计算配额并请求增加
    - 安装Stackdriver Agent进行监视和日志记录
2. 部署和实施Google Kubernetes Engine资源  
    Tasks include:
    - 部署Google Kubernetes Engine集群
    - 使用pods将容器应用程序部署到Google Kubernetes Engine
    - 配置Google Kubernetes Engine应用程序监视和日志记录
3. 部署和实施App Engine，Cloud Run和Cloud Functions资源  
    Tasks include, where applicable:
    - 部署应用程序，更新扩展配置，版本和流量分割
    - 部署接收Google Cloud事件的应用程序 (e.g., Cloud Pub/Sub events, Cloud Storage object change notification events)
4. 部署和实施数据解决方案  
    Tasks include:
    - 使用产品初始化数据系统 (e.g., Cloud SQL, Cloud Datastore, BigQuery, Cloud Spanner, Cloud Pub/Sub, Cloud Bigtable, Cloud Dataproc, Cloud Dataflow, Cloud Storage)
    - Loading data (e.g., command line upload, API transfer, import/export, load data from Cloud Storage, streaming data to Cloud Pub/Sub)
5. 部署和实施网络资源  
    Tasks include:
    - 使用子网创建VPC (e.g., custom-mode VPC, shared VPC)
    - 使用自定义网络配置启动Compute Engine实例 (e.g., internal-only IP address, Google private access, static external and private IP address, network tags)
    - 为VPC创建入口和出口防火墙规则 (e.g., IP subnets, tags, service accounts)
    - 使用Cloud VPN在Google VPC和外部网络之间创建VPN
    - 使用负载均衡器将应用程序网络流量分配给应用程序 (e.g., Global HTTP(S) load balancer, Global SSL Proxy load balancer, Global TCP Proxy load balancer, regional network load balancer, regional internal load balancer)
6. 使用云市场部署解决方案  
    Tasks include:
    - 浏览Cloud Marketplace目录并查看解决方案详细信息
    - 部署Cloud Marketplace解决方案
7. 使用Cloud Deployment Manager部署应用程序基础架构  
    Tasks include:
    - 开发Deployment Manager模板
    - 启动Deployment Manager模板  

### 确保云解决方案的成功运行  
1. 管理Compute Engine资源  
    Tasks include:
    - 管理单个VM实例 (e.g., start, stop, edit configuration, or delete an instance)
    - SSH/RDP连接到实例
    - 将GPU附加到新实例并安装CUDA库
    - 查看当前正在运行的VM清单 (instance IDs, details)
    - 使用快照 (e.g., create a snapshot from a VM, view snapshots, delete a snapshot)
    - 使用镜像 (e.g., create an image from a VM or a snapshot, view images, delete an image)
    - 使用实例组 (e.g., set autoscaling parameters, assign instance template, create an instance template, remove instance group)
    - 使用管理接口 (e.g., Cloud Console, Cloud Shell, GCloud SDK)
2. 管理Google Kubernetes Engine资源  
    Tasks include:
    - 查看当前运行的集群清单 (nodes, pods, services)
    - 浏览容器镜像存储库并查看容器镜像详细信息
    - 使用节点池 (e.g., add, edit, or remove a node pool)
    - 使用pods (e.g., add, edit, or remove pods)
    - 使用服务 (e.g., add, edit, or remove a service)
    - 使用有状态的应用程序 (e.g. persistent volumes, stateful sets)
    - 使用管理接口 (e.g., Cloud Console, Cloud Shell, Cloud SDK)
3. 管理App Engine和Cloud Run资源  
    Tasks include:
    - 调整应用程序流量分割参数
    - 设置自动缩放实例的缩放参数
    - 使用管理接口 (e.g., Cloud Console, Cloud Shell, Cloud SDK)
4. 管理存储和数据库解决方案  
    Tasks include:
    - 在Cloud Storage存储桶之间移动对象
    - 在存储类别之间转换Cloud Storage存储桶
    - 设置Cloud Storage存储桶的对象生命周期管理策略
    - 执行查询从数据实例中检索数据 (e.g., Cloud SQL, BigQuery, Cloud Spanner, Cloud Datastore, Cloud Bigtable)
    - 估算BigQuery查询的费用
    - 备份和还原数据实例 (e.g., Cloud SQL, Cloud Datastore)
    - 在Cloud Dataproc，Cloud Dataflow或BigQuery中查看作业状态
    - 使用管理接口 (e.g., Cloud Console, Cloud Shell, Cloud SDK)
5. 管理网络资源  
    Tasks include:
    - 将子网添加到现有VPC
    - 扩展子网以拥有更多IP地址
    - 保留静态外部或内部IP地址
    - 使用管理接口 (e.g., Cloud Console, Cloud Shell, Cloud SDK)
6. 监视和日志记录  
    Tasks include:
    - 根据资源指标创建Stackdriver警报
    - 创建Stackdriver自定义指标
    - 配置日志接收器并将日志导出到外部系统 (e.g., on-premises or BigQuery)
    - 在Stackdriver中查看和过滤日志
    - 在Stackdriver中查看特定的日志消息的详细信息
    - 使用云诊断来分析应用程序问题 (e.g., viewing Cloud Trace data, using Cloud Debug to view an application point-in-time)
    - 查看Google Cloud Platform状态
    - 使用管理接口 (e.g., Cloud Console, Cloud Shell, Cloud SDK)  

### 配置访问和安全性  
1. 管理身份和访问管理(IAM)  
    Tasks include:
    - 查看IAM角色分配
    - 将IAM角色分配给帐户或Google组
    - 定义自定义IAM角色
2. 管理服务帐户  
    Tasks include:
    - 以有限的权限管理服务帐户
    - 为VM实例分配服务帐号
    - 授予对另一个项目中的服务帐户的访问权限
3. 查看项目和托管服务的审核日志