# Linux内核源码
CU1000-Neo开发板的Linux内核源码。  
  
## 从源码编译Linux内核
本文档将指导开发者从源码编译Linux内核，文中默认开发者已正确配置相关的开发环境。  

### 编译Linux内核的uImage镜像
执行以下命令：  

>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- distclean  
>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- cu1000-neo_defconfig  
>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- uImage  

将会生成目标文件：arch/mips/boot/uImage.gz，可使用君正cloner烧录工具将其烧录至目标板。  
  
***
  
# Linux Kernel source code
Linux Kernel source code for the CU1000-Neo board.  
  
## Build Linux Kernel from source code
This document will guide developers to compile Linux Kernel from source code. In this document, it is by default that developers has configured the relevant development environment correctly.  

### Build uImage of Linux Kernel
Run the following commands:  

>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- distclean  
>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- cu1000-neo_defconfig  
>make ARCH=mips CROSS_COMPILE=mips-linux-gnu- uImage  

This will generate target file: arch/mips/boot/uImage.gz, this file can be burned to the target board by Ingenic cloner burning tool.
