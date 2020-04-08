# Arduino IDE 环境搭建{docsify-ignore-all}


1. [安装Arduino-IDE](#安装Arduino-IDE)

2. [安装ESP32的板管理](#安装ESP32的板管理)

3. [安装M5Stack的库](#安装M5Stack的库)

4. [安装串口驱动](#安装串口驱动)

5. [ArduinoAPI](#ArduinoAPI)

## 安装Arduino-IDE


>[点击此处访问 Arduino 官网](https://www.arduino.cc/en/Main/Software),选择对应自己操作系统的安装包进行下载.


<img src="assets/img/related_documents/Arduino_IDE/Arduino_install.webp">


## 安装ESP32的板管理

>1.打开 Arduino IDE，选择 `文件`->`首选项`->`设置`

<img src="assets/img/related_documents/Arduino_IDE/Arduino_1.webp">

>2.复制下方的 ESP32 板管理网址到 `附加开发板管理器:` 中

**https://dl.espressif.com/dl/package_esp32_index.json**

<img src="assets/img/related_documents/Arduino_IDE/Arduino_2.webp">

>3.选择 `工具`->`开发板:`->`开发板管理器...`

<img src="assets/img/related_documents/Arduino_IDE/Arduino_3.webp">

>4.在新弹出的对话框中，输入并搜索 `ESP32`，点击`安装`（若出现搜索失败的情况，可以尝试重启Arduino程序）


<img src="assets/img/related_documents/Arduino_IDE/Arduino_4.webp">

>5.选择 `工具`->`开发板:`->`ESP32`

<img src="assets/img/related_documents/Arduino_IDE/Arduino_5.webp">

## 安装M5Stack的库

>不同的硬件设备，有着不同的案例程序库，请根据你所使用的设备选择下载.打开 Arduino IDE, 然后选择 `项目`->`加载库`->`库管理...`

<img src="assets/img/related_documents/Arduino_IDE/Arduino_6.webp">

### For M5Core and M5Stick

?>搜索 `M5Stack` 并安装，如下图所示

<img src="assets/img/related_documents/Arduino_IDE/Arduino_7.webp">

### For M5Stick-C

?>搜索 `M5StickC` 并安装，如下图所示

<img src="assets/img/related_documents/Arduino_IDE/Arduino_8.webp">

## 安装串口驱动

>1.点击下方对应自己操作系统的CP210X驱动程序 进行下载.

<div class="link">

 <h4><span>CP210X Driver:</span></h4>
    <p>
    <a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/drivers/CP210x_VCP_Windows.zip" target="_blank" rel="noopener noreferrer"><img src="https://cdn.shopify.com/s/files/1/0056/7689/2250/files/windows_89cc6ea0-2a3c-4327-97e5-8f51f448c38b_icon.webp?v=1557026574" alt="">Windows</a>
    <a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/drivers/CP210x_VCP_MacOS.zip" target="_blank" rel="noopener noreferrer"><img src="https://cdn.shopify.com/s/files/1/0056/7689/2250/files/mac_large.webp?v=1557026570" alt="">MacOS</a>
    <a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/drivers/CP210x_VCP_Linux.zip" target="_blank" rel="noopener noreferrer"><img src="https://cdn.shopify.com/s/files/1/0056/7689/2250/files/linux_icon.webp?v=1557026584" alt="">Linux</a>
    </p>
</div>



### For Windows

>将下载好的驱动压缩包解压，选择对应您操作系统的安装程序，双击安装.

<img src="assets/img/related_documents/Arduino_IDE/CP210X_WIN.webp">


### For Mac

>将下载好的驱动压缩包解压，安装程序，双击镜像文件开始安装.

<img src="assets/img/related_documents/Arduino_IDE/CP210X_MAC.webp">


## ArduinoAPI

### M5Core

|||
|:---:|:---:|
|**[System](zh_CN/api/system)** | **[喇叭](zh_CN/api/speaker)** |
|**[LCD 屏](zh_CN/api/lcd)** | **[按键](zh_CN/api/button)** |
|**[MPU9250](zh_CN/api/mpu9250)** | **[TF 卡](zh_CN/api/tf)** |
|**[电源管理](zh_CN/api/power)** |**[I/O](zh_CN/api/gpio)** |
|**[I2C](zh_CN/api/commutil)** |**[EEPROM](zh_CN/api/eeprom)**|
|**[WIFI](zh_CN/api/wifi)**|

<!-- <table>
    <tr>
        <th align="center"><a href="#/zh_CN/api/system">System</a></th>
        <th align="center"><a href="#/zh_CN/api/speaker">喇叭</a></th>
        <th align="center"><a href="#/zh_CN/api/speaker">LCD 屏幕</a></th>
        <th align="center"><a href="#/zh_CN/api/speaker">按键</a></th>
    </tr>
    <tr>
        <th align="center"><a href="#/zh_CN/api/system">Power</a></th>
        <th align="center"><a href="#/zh_CN/api/speaker">TF 卡</a></th>
        <th align="center"><a href="#/zh_CN/api/speaker">姿态传感器 (MPU9250)</a></th>
        <th align="center"><a href="#/zh_CN/api/speaker"> </a></th>
    </tr>
</table> -->

### M5StickC

<!-- |||
|:---:|:---:|
|**[System](zh_CN/api/system)** | **[喇叭](zh_CN/api/speaker)** |
|**[LCD 屏](zh_CN/api/lcd)** | **[按键](zh_CN/api/button)** |
|**[MPU9250](zh_CN/api/mpu9250)** | **[TF 卡](zh_CN/api/tf)** |
|**[Power](zh_CN/api/power)** | -->

|||
|:---:|:---:|
|**[System](zh_CN/api/system_m5stickc)** | **[AXP192](zh_CN/api/axp192_m5stickc)** |
|**[TFT 屏](zh_CN/api/lcd_m5stickc)** | **[SH200Q](zh_CN/api/sh200q_m5stickc)** |
|**[RTC](zh_CN/api/rtc)**|

<!-- |**[麦克风](zh_CN/api/spm1423_m5stickc)** | **[LED](zh_CN/api/led_m5stickc)** |

|**[按键](zh_CN/api/buttom_m5stickc)** | **[红外发射](zh_CN/api/led_m5stickc)** | -->



<!-- <div class="table-wrapper">
    <table class="fl-table">
        <thead>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
            <th>Header 3</th>
            <th>Header 4</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>1</td>
            <td>Content</td>
            <td>Content</td>
            <td>Content</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Content</td>
            <td>Content</td>
            <td>Content</td>
        </tr>
        <tr>
            <td>3</td>
            <td>Content</td>
            <td>Content</td>
            <td>Content</td>
        </tr>
        <tbody>
    </table>
</div> -->


<style>

.link a{

    padding-left: 13%;

}

</style>