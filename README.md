# U-Boot源码
CU1000-Neo开发板的U-Boot源码。  
  
## 从源码编译U-Boot
本文档将指导开发者从源码编译U-Boot，文中默认开发者已正确配置相关的开发环境。  

### 1. 编译Nor Flash版本
执行以下命令：  

>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- distclean  
>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- cu1000-neo_uImage_sfc_nor  

将会生成目标文件：u-boot-with-spl.bin，该文件用于从Nor Flash存储介质启动。  

### 2. 编译eMMC版本
执行以下命令：  

>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- distclean  
>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- cu1000-neo_uImage_msc0  

将会生成目标文件：u-boot-with-spl-mbr-gpt.bin，该文件用于从eMMC存储介质启动。  
  
***
  
# U-Boot source code
U-Boot source code for the CU1000-Neo board.  
  
## Build U-Boot from source code
This document will guide developers to compile U-Boot from source code. In this document, it is by default that developers has configured the relevant development environment correctly.  

### 1. Build the Nor Flash version
Run the following commands:  

>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- distclean  
>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- cu1000-neo_uImage_sfc_nor  

This will generate target file: u-boot-with-spl.bin, this file is used for boot from Nor Flash storage media.  

### 2. Build the eMMC version
Run the following commands:  

>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- distclean  
>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- cu1000-neo_uImage_msc0  

This will generate target file: u-boot-with-spl-mbr-gpt.bin, this file is used for boot from eMMC storage media.
