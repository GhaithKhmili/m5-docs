# Module GoPlus {docsify-ignore-all}

<img src="assets/img/product_pics/module/goplus/goplus_p1.jpg" width="30%" height="30%"> <img src="assets/img/product_pics/module/goplus/goplus_p2.jpg" width="30%" height="30%">



<!-- :memo:**[Description](#Description)**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:octocat:**[Example](#Example)**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:electric_plug:**[Schematic](#Schematic)**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;🛒**[Purchase](https://www.aliexpress.com/store/product/M5Stack-New-Arrival-PLUS-Module-Encoder-Module-with-MEGA328P-500mAh-Battery-ISP-IR-Transmitter-UART-GPIO/3226069_32949278724.html?spm=a2g1x.12024536.productList_5885013.pic_1)**-->

## 描述

**GoPlus** 是M5Stack堆叠模块系列中的一款，功能增强型模块.集成**MEGA328P**与**LV8548MC**电机驱动芯片.整合Module、Units功能（SERVO，PbHUB，IR）.

配备2通道直流电机驱动、4通道舵机驱动接口、红外收发器、3个扩展端口B（GPIO端口）.具备多种功能特性，能够帮助你快速搭建功能强大的电机应用.

<img src="assets/img/product_pics/module/goplus/goplus_p3.jpg" width="30%" height="30%"><img src="assets/img/product_pics/module/goplus/goplus_p4.jpg" width="30%" height="30%">


通信协议：IIC（0x61）.

### 产品特性

-  2x 直流电机驱动通道
-  4x 舵机驱动通道
-  IR 发射 & 接收
-  3x 拓展 PORT B
-  MEGA328P
-  LV8548MC
-  产品尺寸：54.2mm x 54.2mm x 12.8mm
-  产品重量：27.5g

### 套件清单

-  1x M5Stack GoPlus Module

## EasyLoader

<img src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/image/EasyLoader_logo.png" width="100px" style="margin-top:20px">

<a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/EasyLoader/Module/EasyLoader_GOPLUS.exe"><button type="button" class="btn btn-primary">点击下载EasyLoader</button></a>

>1.EasyLoader是一个简洁快速的程序烧录器，每一个产品页面里的EasyLoader都提供了一个与产品相关的案例程序，通过简单步骤将其烧录至主控，能够进行一系列的功能验证.**(目前EasyLoader仅适用于Windows操作系统)**

>2.下载软件后，双击运行应用程序，将M5设备通过数据线连接至电脑,选择端口参数，点击 **"Burn"** 即可开始烧录

!>3.EasyLoader烧录前需要安装有CP210X（USB驱动程序），[点击此处查看驱动安装教程](zh_CN/related_documents/M5Burner#安装串口驱动)

## 原理图

<img src="assets/img/product_pics/module/goplus/goplus_sch.jpg">


## 管脚映射

**Mega328 ISP**下载接口Pin脚定义

<img src="assets\img\product_pics\app\mega328_isp.png" width="30%" height="30%">


## 参考文档


- 协议手册 - **[I2C协议](https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/datasheet/module/GoPlus_I2C_Protocol%20operation%20instructions.pdf)**

- 数据手册 - **[LV8548MC](https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/datasheet/module/LV8548MC-D.PDF)**


## 案例程序

- 驱动固件 - **[GoPlus](https://github.com/m5stack/GoPlus/tree/master/src)**
- 测试程序 - **[GoPlus](https://github.com/m5stack/GoPlus/tree/master/test)**

### UIFLOW

<img src="assets/img/product_pics/module/goplus/goplus_p5.jpg">

- [点击此处，获取UIFlow](https://github.com/m5stack/M5-ProductExampleCodes/tree/master/Module/GOPLUS/UIFLOW). 

<script>

   var 购买链接 = 'https://m5stack.com/collections/m5-module/products/goplus-module';


   anchor_search(购买链接);
   scrollFunc();

</script>