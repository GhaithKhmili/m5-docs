# M5GO IoT Starter Kit {docsify-ignore-all}

<img src="assets/img/product_pics/core/m5go/m5go_01.png" alt="gray_02" width="250" height="250"> <img src="assets/img/product_pics/core/m5go/m5go_02.webp" alt="gray_02" width="250" height="250"> <img src="assets/img/product_pics/core/m5go/m5go_03.png" alt="gray_04" width="250" height="250">

* * *

:memo:**[描述](#描述)**&nbsp;&nbsp;&nbsp;:bulb:**[上手指南](zh_CN/quick_start/m5core/m5stack_core_quick_start)**&nbsp;&nbsp;&nbsp;:octocat:**[例程](https://github.com/m5stack/M5Stack/tree/master/examples/Basics)**&nbsp;&nbsp;&nbsp;:electric_plug:**[原理图](https://github.com/m5stack/M5-Schematic/blob/master/Core/Basic/M5-Core-Schematic(20171206).pdf)**&nbsp;&nbsp;&nbsp;🛒**[购买链接](https://m5stack.com/collections/m5-core/products/m5go-iot-starter-kit-stem-education)**&nbsp;&nbsp;&nbsp;:clapper:**[相关视频](#相关视频)**

## 描述

**M5GO IoT Kit** 是 M5Stack 开发套件系列中的一款，面向 STEM 教育的开发套件.除了主机M5GO之外，套件内还包含了 6 个不同的功能Unit,以及一些乐高积木等配件.M5GO除了硬件资源之外，还拥有丰富的教学视频、教科书、技术文档与资源.针对各年龄段的学生，在STEM教育方面发挥重要作用.

提供线上版本的 WebIDE UIFlow 编程平台，通过网络推送程序的方式，让学生切身体会物联网的强大.支持多种编程方式，帮助学生逐步由图形化编程进阶到对实际代码的理解.

作为一款专为STEM教育而设计套件.M5GO想要做到的是使学生在获得知识的同时，收获乐趣，收获那份将自己的创意一步一步转换为现实的荣誉感.让学生可以自由的探索工程世界，制作自己的物联网产品，并将精彩的创意融入到现实生活中.

**注意：** 

新生产的M5Core更换了显示效果与可视角更加优质的屏幕，因此与旧版的Arduino库产生了一些兼容性问题，使用旧版程序库进行屏幕驱动时会产生反色显示的现象，您可以打开Arduino的库管理选项将您的M5Stack库升级至最新版本（0.2.8以后）来解决这个问题.

<img src="assets\img\product_pics\core\basic\lib_01.jpg" width="40%">
<br><br><br>
<img src="assets\img\product_pics\core\basic\lib_02.jpg" width="40%">

## 产品特性

- 5V 直流电源
- USB Type-C
- 基于ESP32开发
- 16 MByte flash
- BMM150 + MPU6886
- 扬声器，按键x3，LCD屏幕（320 * 240），电源/复位按键x1
- 2.4G天线：Proant 440
- TF卡插槽（最大可拓展16GB）
- 可拓展的引脚与接口
- Grove 接口
- M-Bus总线母座 & 引脚
- 开发平台 [UIFlow](http://flow.m5stack.com), [MicroPython](http://micropython.org/), [Arduino](http://www.arduino.cc)


### ESP32特性

- 240 MHz双核Tensilica LX6微控制器，性能达到 600 DMIPS
- 集成520 KB SRAM
- 集成的802.11b/g/n HT40 Wi-Fi收发器，基带，堆栈和LWIP
- 集成双模蓝牙（经典和BLE）
- 霍尔传感器
- 10x 电容触摸功能接口
- 32 kHz晶体振荡器
- 每个GPIO引脚都支持PWM/定时器 输入/输出
- SDIO master/salve 50MHz
- 支持SD卡接口


### M5GO底座

[点击查看详情参数](zh_CN/base/m5go_bottom)


<a href="#zh_CN/related_documents/M5Burner"><button type="button" class="btn btn-primary">查看固件烧录教程</button></a>

## 外设的管脚映射

#### 主板管脚

**LCD 屏幕 & TF 卡**

*LCD像素：320x240*
*TF卡最大支持16GB*

<table>
 <tr><td>ESP32 Chip</td><td>GPIO23</td><td>GPIO19</td><td>GPIO18</td><td>GPIO14</td><td>GPIO27</td><td>GPIO33</td><td>GPIO32</td><td>GPIO4</td></tr>
 <tr><td>ILI9342C</td><td>MOSI/MISO</td><td>/</td><td>CLK</td><td>CS</td><td>DC</td><td>RST</td><td>BL</td><td> </td></tr>
 <tr><td>TF卡</td><td>MOSI</td><td>MISO</td><td>CLK</td><td> </td><td> </td><td> </td><td> </td><td>CS</td></tr>
</table>

**按键 & 喇叭**

<table>
 <tr><td>ESP32 Chip</td><td>GPIO39</td><td>GPIO38</td><td>GPIO37</td><td>GPIO25</td></tr>
 <tr><td>按键引脚</td><td>BUTTON A</td><td>BUTTON B</td><td>BUTTON C</td></tr>
 <tr><td>喇叭</td><td> </td><td> </td><td> </td><td>喇叭引脚</td></tr>
</table>

**GROVE 接口 A & IP5306**

*电源管理芯片 (IP5306) 是定制 I2C 版本，它的 I2C 地址是 0x75。点击[这里](https://github.com/m5stack/M5-Schematic/blob/master/Core/IIC_IP5306_REG_V1.4.pdf)查看 IP5306 的寄存器手册。*

<table>
 <tr><td>ESP32 Chip</td><td>GPIO22</td><td>GPIO21</td><td>5V</td><td>GND</td></tr>
 <tr><td>GROVE A</td><td>SCL</td><td>SDA</td><td>5V</td><td>GND</td></tr>
 <tr><td>IP5306</td><td>SCL</td><td>SDA</td><td>5V</td><td>GND</td></tr>
</table>


**IP5306充/放电，电压参数**

<table>
   <tr style="font-weight:bold;text-align:center" >
      <td>充电</td>
      <td><td>
      <td>放电</td>
   </tr>
   <tr>
      <td>0.00 ~ 3.40V -> 0%</td>
      <td><td>
      <td>4.20 ~ 4.07V -> 100%</td>
   </tr>
   <tr>
      <td>3.40 ~ 3.61V -> 25%</td>
      <td><td>
      <td>4.07 ~ 3.81V -> 75%</td>
   </tr>
   <tr>
      <td>3.61 ~ 3.88V -> 50%</td>
      <td><td>
      <td>3.81 ~ 3.55V -> 50%</td>
   </tr>
   <tr>
      <td>3.88 ~ 4.12V -> 75%</td>
      <td><td>
      <td>3.55 ~ 3.33V -> 25%</td>
   </tr>
   <tr>
      <td>4.12 ~   /   -> 100%</td>
      <td><td>
      <td>3.33 ~ 0.00V -> 0%</td>
   </tr>
</table>

**6-Axis IMU Sensor MPU6886**

*MPU6886 I2C address 0x68*

<table>
 <tr><td>ESP32 Chip</td><td>GPIO22</td><td>GPIO21</td><td>5V</td><td>GND</td></tr>
 <tr><td>MPU6886</td><td>SCL</td><td>SDA</td><td>5V</td><td>GND</td></tr>
</table>

**3-Axis Geomagnetic Sensor BMM150**

*BMM150 I2C address 0x10*

<table>
 <tr><td>ESP32 Chip</td><td>GPIO22</td><td>GPIO21</td><td>5V</td><td>GND</td></tr>
 <tr><td>BMM150</td><td>SCL</td><td>SDA</td><td>5V</td><td>GND</td></tr>
</table>

#### M5GO 底座管脚

**GROVE 接口 B**

<table>
 <tr><td>ESP32 Chip</td><td>GPIO36</td><td>GPIO26</td><td>5V</td><td>GND</td></tr>
 <tr><td>GROVE B</td><td>GPIO36</td><td>GPIO26</td><td>5V</td><td>GND</td></tr>
</table>

**GROVE 接口 C**

<table>
 <tr><td>ESP32 Chip</td><td>GPIO16</td><td>GPIO17</td><td>5V</td><td>GND</td></tr>
 <tr><td>GROVE C</td><td>RXD</td><td>TXD</td><td>5V</td><td>GND</td></tr>
</table>

**LED 灯条 & 麦克风 MIC**

<table>
 <tr><td>ESP32 Chip</td><td>GPIO15</td><td>GPIO34</td><td>GPIO25</td></tr>
 <tr><td>LED灯条</td><td>SIG管脚</td><td> </td><td> </td></tr>
 <tr><td>麦克风MIC</td><td> </td><td>MIC管脚</td><td> </td></tr>
</table>

## 参数

<table>
   <tr style="font-weight:bold">
      <td>主控资源</td>
      <td>参数</td>
   </tr>
   <tr>
      <td>ESP32</td>
      <td>240MHz dual core, 600 DMIPS, 520KB SRAM, Wi-Fi, dual mode Bluetooth</td>
   </tr>
   <tr>
      <td>Flash闪存</td>
      <td>16MB Flash</td>
   </tr>
   <tr>
      <td>输入电压</td>
      <td>5V @ 500mA</td>
   </tr>
   <tr>
      <td>接口</td>
      <td>TypeC x 1, GROVE(I2C+I/0+UART) x 1</td>
   </tr>
   <tr>
      <td>IPS屏幕</td>
      <td>2 inch, 320x240 Colorful TFT LCD, ILI9342C</td>
   </tr>
   <tr>
      <td>喇叭</td>
      <td>1W-0928</td>
   </tr>
      <tr>
      <td>麦克风</td>
      <td>MEMS Analog BSE3729 Microphone</td>
   </tr>
   <tr>
      <td>LED</td>
      <td>SK6812 3535 RGB LED x 10</td>
   </tr>
   <tr>
      <td>MEMS</td>
      <td>BMM150 + MPU6886</td>
   </tr>
   <tr>
      <td>电池</td>
      <td>500 mAh @ 3.7V, inside  vb</td>
   </tr>
   <tr>
      <td>工作温度</td>
      <td>32°F to 104°F ( 0°C to 40°C )</td>
   </tr>
   <tr>
      <td>尺寸</td>
      <td>54 x 54 x 21 mm</td>
   </tr>
   <tr>
      <td>外壳材质</td>
      <td>Plastic ( PC )</td>
   </tr>
</table>



**<mark>Notice2：M5PORT 说明 </mark>**
*不同颜色的GROVE端口分别代表不同的功能.红色的PortA（21/22），为默认的I2C协议接口，黑色的PortB（26/36）, 支持DA/AD转换与信号总线通信.蓝色的PortC（16/17）, 支持Uart串口通信.在使用Unit进行功能拓展的时候，只需要匹配二者的端口的颜色，相应的进行连接即可正常使用.不仅提供简洁的硬件连接方式，还支持引脚的重映射.PortA（红色）被作为信号总线连接至是ESP32的GPIO21/22 ，没有AD通道转换方案，因此不能用作模拟输入使用.

- ADC1(8 通道 GPIO 32-39)
- ADC2(10 通道 GPIO 0，2，4，12-15，25-27)

使用AD读取功能:
1，使用杜邦线连接机身侧面的能够AD转换的引脚.
2，堆叠一个M5GO底座，使用其提供PortB.
3，使用PbHUB连接至PortA，拓展出6个PortB.
有关引脚分配和引脚重映射的更多信息，请查阅[ESP32数据手册](https://www.espressif.com/sites/default/files/documentation/esp32_datasheet_cn.pdf)


## 包含

-  1x M5GO
-  6x Units(ENV, IR, RGB, PIR, ANGLE, HUB)
-  4x LEGO积木
-  12x LEGO连接件
-  4x GROVE线
-  1x Type-C USB(20cm)
-  1x 使用手册

## 相关链接

- **数据手册**

    - [ESP32](https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/datasheet/core/esp32_datasheet_cn.pdf)
    - [MPU6886](https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/datasheet/core/MPU-6886-000193%2Bv1.1_GHIC_en.pdf)
    - [BMM150](https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/datasheet/core/BMM150_datasheet_en.pdf)

- **寄存器手册** 

    - [IP5306](https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/datasheet/core/IIC_IP5306_REG_V1.4_cn.pdf)

## 版本变更

<div class="table-wrapper">
    <table class="fl-table">
        <thead>
        <tr>
            <th>上市日期</th>
            <th>产品变动</th>
        </tr>
        </thead>    
        <tbody>
        <tr>
            <td>2018.4</td>
            <td>首次发售</td>
        </tr>
        <tr>
            <td>2019.6</td>
            <td>MPU9250变更为MPU6886+BMM150</td>
        </tr>
        <tr>
            <td>2019.7</td>
            <td>TN屏幕变更为IPS屏幕</td>
        </tr>
        <tr>
            <td>2019.11</td>
            <td>电池容量600mAh变更为500mAh</td>
        </tr>
        <tbody>
    </table>
</div>

## 相关视频

- **m5stack 的简介**

<video class="video_size" controls>
    <source src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/video/LukeVideo/m5stack%E7%AE%80%E4%BB%8B%EF%BC%88%E4%B8%AD%E6%96%87%EF%BC%89.mp4" type="video/mp4">
</video>

<script>

   var purchase_link = 'https://m5stack.com/collections/m5-core/products/basic-core-iot-development-kit';

   var quickstart_link = 'https://m5stack.com/collections/m5-core/products/basic-core-iot-development-kit';

   anchor_search(purchase_link,quickstart_link);
   scrollFunc();

</script>