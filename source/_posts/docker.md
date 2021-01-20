---
title: docker
date: 2021-01-08 13:39:39
tags: linux
category: Tool
---
此篇记录了那些常用的docker命令
<!-- more -->
删除镜像  
`docker rmi -f (image-name/image-id)`  
删除为none的镜像  
`docker rmi $(docker images | grep "none" | awk '{print $3}')`  
查看docker镜像  
`docker ps`  
进入到容器的命令行  
`docker exec -it container_id /bin/bash`  