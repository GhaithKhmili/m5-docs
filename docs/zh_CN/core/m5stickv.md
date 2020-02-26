# M5StickV {docsify-ignore-all}


<img src="assets\img\product_pics\core\minicore\m5stickv/m5stickv_01.jpg" width="30%" height="30%"><img src="assets\img\product_pics\core\minicore\m5stickv/m5stickv_02.jpg" width="30%" height="30%"><img src="assets\img\product_pics\core\minicore\m5stickv/m5stickv_07.jpg" width="30%" height="30%">


## 描述

**M5Stick-V RISC-V AI 摄像头**

**M5Stick-V**是一款搭载Kendryte K210的AIOT（AI + IOT）摄像头，集成双核64位RISC-V CPU和最先进的神经网络处理器边缘计算片上系统（SoC）
<br><br>
M5stickV AI 摄像头具备机器视觉能力，支持多种视觉识别能力的它（ 如实时获取被检测目标的大小与坐标 • 实时获取被检测目标的种类），并且能够在低功耗情况下进行卷积神经网络计算，因此M5StickV会是一个很好的零门槛机器视觉嵌入式解决方案
<br><br>
支持MicroPython开发环境，这使得你在使用M5stick-V上进行项目开发时，程序代码将会更加精简.
<br><br>
配备OmniVision OV7740图像传感器，采用OmniPixel®3-HS技术，提供相比同类最佳的低光灵敏度，是机器视觉项目的理想选择.

<br><br><br>
<img src="assets\img\product_pics\core\minicore\m5stickv/m5stickv_03.jpg" width="30%" height="30%">&nbsp;&nbsp;&nbsp;
<img src="assets\img\product_pics\core\minicore\m5stickv/m5stickv_06.jpg" width="30%" height="30%">&nbsp;&nbsp;&nbsp;
<img src="assets\img\product_pics\core\minicore\m5stickv/m5stickv_05.jpg" width="30%" height="30%"><br>



### 产品特性:
- 双核 64-bit RISC-V RV64IMAFDC (RV64GC) CPU / 400Mhz(Normal)
- 双精度 FPU
- 8MiB 64bit 片上 SRAM     
- 神经网络处理器（KPU） / 0.8Tops
- 可编程 IO 阵列 (FPIOA)
- 双硬件512点16位复数FFT
- SPI, I2C, UART, I2S, RTC, PWM, 定时器支持
- AES, SHA256 加速器
- 直接内存存取控制器  (DMAC)
- 支持 Micropython
- 固件加密支持
- 板载硬件资源:
    - Flash:  16M.
    - TFT:  ST7789. 135*240 IPS 1.14  SPI
    - 摄像头 :OV7740
    - PCM: MAX98357
    - 电源管理IC: AXP192
    - 按键:  Front and side.
    - 锂电池:  200mAh. 
    - 指示灯:  RGBW .
    - 外部存储:  TF card/Micro SD
    - 六轴IMU传感器:  MPU6886 
    - 接口:  GROVE.

   
### 包含

-  1x M5StickV
-  1x USB Type-C(100cm)

## 尺寸重量

- 包装尺寸:144mm x 44mm x 43mm
- 包装重量:82g


### SD卡测试

M5StickV目前并不能识别所有类型的SD卡，我们对一些常见的SD卡进行了测试，测试结果如下.

<img src="assets\img\product_pics\core\minicore\m5stickv/m5stickv_08.jpg" width="30%" height="30%">

<table class="table_center">
   <tr style="font-weight:bold" >
      <td>品牌</td>
      <td>内存</td>
      <td>类型</td>
      <td>传输速度</td>
      <td>分区格式</td>
      <td>测试结果</td>
   </tr>
   <tr>
      <td>Kingston</td>
      <td>8G</td>
      <td>HC</td>
      <td>Class4</td>
      <td>FAT32</td>
      <td>OK</td>
   </tr>
   <tr>
      <td>Kingston</td>
      <td>16G</td>
      <td>HC</td>
      <td>Class10</td>
      <td>FAT32</td>
      <td>OK</td>
   </tr>
   <tr>
      <td>Kingston</td>
      <td>32G</td>
      <td>HC</td>
      <td>Class10</td>
      <td>FAT32</td>
      <td>NO</td>
   </tr>
   <tr>
      <td>Kingston</td>
      <td>64G</td>
      <td>XC</td>
      <td>Class10</td>
      <td>exFAT</td>
      <td>OK</td>
   </tr>
   <tr>
      <td>SanDisk</td>
      <td>16G</td>
      <td>HC</td>
      <td>Class10</td>
      <td>FAT32</td>
      <td>OK</td>
   </tr>
   <tr>
      <td>SanDisk</td>
      <td>32G</td>
      <td>HC</td>
      <td>Class10</td>
      <td>FAT32</td>
      <td>OK</td>
   </tr>
   <tr>
      <td>SanDisk</td>
      <td>64G</td>
      <td>XC</td>
      <td>Class10</td>
      <td>/</td>
      <td>NO</td>
   </tr>
   <tr>
      <td>SanDisk</td>
      <td>128G</td>
      <td>XC</td>
      <td>Class10</td>
      <td>/</td>
      <td>NO</td>
   </tr>
   <tr>
      <td>XIAKE</td>
      <td>16G</td>
      <td>HC</td>
      <td>Class10</td>
      <td>FAT32</td>
      <td>OK(紫色)</td>
   </tr>
   <tr>
      <td>XIAKE</td>
      <td>32G</td>
      <td>HC</td>
      <td>Class10</td>
      <td>FAT32</td>
      <td>OK</td>
   </tr>
   <tr>
      <td>XIAKE</td>
      <td>64G</td>
      <td>XC</td>
      <td>Class10</td>
      <td>/</td>
      <td>NO</td>
   </tr>
   <tr>
      <td>TURYE</td>
      <td>32G</td>
      <td>HC</td>
      <td>Class10</td>
      <td>/</td>
      <td>NO</td>
   </tr>
</table>



## EasyLoader

<img src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/image/EasyLoader_logo.png" width="100px" style="margin-top:20px">

<a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/EasyLoader/M5Core/M5StickV/EasyLoader_M5StickV_1022_beta.exe"><button type="button" class="btn btn-primary">点击下载EasyLoader</button></a>

>1.EasyLoader是一个简洁快速的程序烧录器，每一个产品页面里的EasyLoader都提供了一个与产品相关的案例程序.**(目前EasyLoader仅适用于Windows操作系统)**

>2.下载软件后，双击运行应用程序，将M5设备通过数据线连接至电脑,选择端口参数，点击 **"Burn"** 即可开始烧录


### 功能描述
#### 1.1   KENDRYTE K210 
Kendryte K210 是集成机器视觉能力的系统级芯片 (SoC)。使用台积电 (TSMC) 超低功耗的 28 纳米先进制程，具有双核 64 位处理器，拥有较好的功耗性能，稳定性与可靠性。该方案力求零门槛开发，可在最短时效部署于用户的产品中，赋予产品人工智能.<br><br>
- 具备机器视觉能力
- 更好的低功耗视觉处理速度与准确率 
- 具备卷积人工神经网络硬件加速器 KPU，可高性能进行卷积人工神经网络运算
- TSMC 28nm 先进制程，温度范围-40°C 到 125°C，稳定可靠
- 支持固件加密，难以使用普通方法破解 
- 独特的可编程 IO 阵列，使产品设计更加灵活
- 低电压，与相同处理能力的系统相比具有更低功耗
- 3.3V/1.8V 双电压支持，无需电平转换，节约成本

##### 1.1.1 CPU
本芯片搭载基于 RISC-V ISA 的双核心 64 位的高性能低功耗 CPU，具备以下特性：

- 核心数量：  双核处理器
- 处理器位宽:   64-bit CPU 400MHz
- 标称频率:   400MHz 
- 指令集扩展:  IMAFDC
- 浮点处理单元(FPU):  双精度
- 平台中断管理:  PLIC
- 本地中断管理:  CLINT
- 指令缓存:  32KiB x 2
- 数据缓存:  32KiB x 2
- 片上 SRAM:  8MiB


#### 1.2    OV7740
- 支持输出格式：RAW RGB和YUV
- 支持图像尺寸：VGA，QVGA，CIF或其他更小尺寸
- 支持太阳黑子消除
- 支持内部和外部帧同步
- 标准SCCB串行接口
- 数字视频端口（DVP）并行输出接口 
- 嵌入式一次性可编程（OTP）存储器
- 片上锁相环（PLL）
- 用于内核的嵌入式1.5 V稳压器

##### 1.2.1 规格
- 阵列尺寸：656 x 488
- 电源： - 内核：1.5VDC±5％ - 模拟：3.3V±5％ -  I / O：1.7~3.47V
- 温度范围： - 工作：-30°C至70°C  - 稳定图像：0°C至50°C
- 输出格式： -  8/10位原始RGB数据 -  8位YUV
- 镜头尺寸：1/5"
- 输入时钟频率：6~27 MHz
- 最大图像传输速率：VGA（640x480）：60 fps  -  QVGA（320 x 240）：120 fp
- 灵敏度：6800 mV /（Lux-sec）
- 最大曝光间隔：502 x tROW
- 像素尺寸：4.2μm×4.2μm
- 图像面积：2755.2μm×2049.6μm
- 封装/管芯尺寸： -  CSP3：4185μm×4345 μm-COB：4200μm×4360μm


#### 1.3    MAX98357
- 单电源工作(2.5V至5.5V)
- 3.2W输出功率：4Ω，5V
- 2.4mA静态电流
- 92% 效率(RL = 8Ω,POUT = 1W)
- 22.8µVRMS输出噪声(AV = 15dB)
- 1kHz时，0.015% THD+N
- 无需MCLK
- 8kHz至96kHz采样速率 
- 支持左声道、右声道以及(左声道/2 + 右声道/2)输出
- 成熟的边沿速率控制可使D类放大器输出无需滤波
- 1kHz下，具有77dB PSRR
- 低RF敏感度，可抑制GSM发射的TDMA噪声
- 喀嗒声抑制电路

#### 1.4    AXP192
- 工作电压: 2.9V - 6.3V(AMR：-0.3V~15V)
- 可配置的智能电源选择系统
- 自适应USB或AC适配器输入的电流和电压限制
- 内部理想二极管的电阻低于100mΩ

#### 1.5    MPU6886

##### 1.5.1陀螺仪功能
MPU-6886中的三轴MEMS陀螺仪具有多种功能：
- 数字输出X，Y和Z轴角速率传感器（陀螺仪），用户可编程满量程范围为±250 dps，±500 dps，±1000 dps和±2000 dps，集成16- 位ADC
- 数字可编程低通滤波器
- 低功率陀螺仪操作
- 工厂校准的灵敏度比例因子
- 镜头尺寸：1/5“
- 自我测试

##### 1.5.2 加速度计功能
MPU-6886中的三轴MEMS加速度计包括多种功能：
- 数字输出X，Y和Z轴加速度计，可编程满量程范围为±2g，±4g，±8g和±16g，集成16位ADC
- 用户可编程中断
- 唤醒动作中断，用于应用处理器的低功耗操作
- 自我测试


## 应用/ M5Stick-V可以做什么？
- 面部识别/检测
- 物体检测/分类
- 实时获取目标的大小和坐标
- 实时获取检测到的目标类型
- 形状识别
- 视频/显示
- 游戏模拟器


## 案例程序

-  **Example** [Code](https://docs.m5stack.com/#/zh_CN/related_documents/M5StickV-Maixpy)


## 相关链接

-  **Web page** - [sipeed](https://maixpy.sipeed.com/en/)
-  **Quick Start Guide** - [M5StickV Guide](https://docs.m5stack.com/#/en/quick_start/m5stickv/m5stickv_quick_start)
-  **Github** - [API](https://github.com/sipeed/MaixPy/tree/master/projects/maixpy_m5stickv)

-  **数据手册**

    - [MPU6886](https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/datasheet/core/MPU-6886-000193%2Bv1.1_GHIC_en.pdf)
    - [SH200Q](https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/datasheet/core/SH200Q_en.pdf)

## 原理图

<img src="assets\img\product_pics\core\minicore\m5stickv/m5stickv_04.jpg" width="30%" height="30%">

<script>

   var purchase_link = 'https://m5stack.com/collections/m5-core/products/stickv';

   var quickstart_link = 'https://docs.m5stack.com/#/zh_CN/quick_start/m5stickv/m5stickv_quick_start';

   anchor_search(purchase_link,quickstart_link);
   scrollFunc();

</script>