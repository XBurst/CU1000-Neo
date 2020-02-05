# Debian文件系统镜像
Debian9的文件系统镜像，ext4格式，使用7-Zip分卷压缩，包含apt、build-essential、htop、vim、wpasupplicant等常用软件包，并配置有384MiB的SWAP交换文件。  
  
## 解压缩镜像分卷压缩包
本文档将指导开发者解压缩Debian9的文件系统镜像分卷压缩包，文中默认开发者使用的是Debian或者类似Debian的操作系统。  

### 1. 安装7-Zip软件包
执行以下命令：  

>sudo apt install p7zip-full  

然后即可使用7z命令来对镜像的分卷压缩包进行解压缩。  

### 2. 解压缩分卷压缩包
执行以下命令：  

>7z x debian.7z.001  

然后即可得到解压缩后的镜像文件：debian9-20191227.ext4，可使用君正Cloner烧录工具将其烧录至目标板。  
  
***
  
# Debian rootfs image
Ext4 format rootfs image of Debian9, multi-volume compressed by 7-Zip, contains common software packages such as apt, build-essential, htop, vim, wpasupplicant, etc., and is configured with 384MiB SWAP file.  
  
## Extract image from 7z archives
This document will guide developers to extract the rootfs image of Debian9 from the multi-volume compressed 7z archives. In this document, it is by default that developers are using Debian or Debian-like operating systems.  

### 1. Install 7-Zip software package
Run the following command:  

>sudo apt install p7zip-full  

Now you can use the 7z command to extract the image from the multi-volume compressed 7z archives.  

### 2. Extract the image
Run the following command:  

>7z x debian.7z.001  

Then you can get the image file: debian9-20191227.ext4, this file can be burned to the target board by Ingenic Cloner burning tool.
