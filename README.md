# 交叉编译工具链
君正交叉编译工具链r3.2.1版，基于Binutils-2.25、GCC-5.2、Glibc-2.22以及UClibc-0.9.33，支持君正MXU和MXU2指令集。  
  
## 部署工具链
本文档将指导开发者部署并测试交叉编译工具链，文中默认工具链存放路径为“~/CU1000-Neo/toolchain”。  

### 1. 设置环境变量
执行以下命令：  

>export PATH=~/CU1000-Neo/toolchain/bin:$PATH  

然后即可使用mips-linux-gnu-gcc和mips-linux-gnu-g++来编译程序。  

### 2. 测试工具链
创建helloworld.c文件，内容如下： 

```
#include <stdio.h>
int main(void)
{
    printf("Hello world!\n");
    return 0;
}
```

然后执行以下命令：  

>mips-linux-gnu-gcc -O2 -o helloworld helloworld.c  

如果能正常完成编译，则说明工具链可以正常使用。  
  
***
  
# Cross-compile toolchain
Ingenic cross-compile toolchain r3.2.1 version, based on Binutils-2.25, GCC-5.2, Glibc-2.22 and UClibc-0.9.33, supports Ingenic MXU and MXU2 instruction set.  
  
## Deploy the toolchain
This document will guide developers to deploy and test the cross-compile toolchain. In this document, it is by default that the storage path of the toolchain is "~/CU1000-Neo/toolchain".  

### 1. Set PATH environment variable
Run the following command:  

>export PATH=~/CU1000-Neo/toolchain/bin:$PATH  

Now you can use the mips-linux-gnu-gcc and mips-linux-gnu-g++ to compile programs.  

### 2. Test the toolchain
Create a helloworld.c file with the following contains:  

```
#include <stdio.h>
int main(void)
{
    printf("Hello world!\n");
    return 0;
}
```

Then build it:  

>mips-linux-gnu-gcc -O2 -o helloworld helloworld.c  

If helloworld can be built correctly, it shows that the toolchain has been deployed properly and can be used normally.
