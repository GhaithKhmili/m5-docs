# Arduino IDE Development{docsify-ignore-all}


1. [Install Arduino-IDE](#Install-Arduino-IDE)

2. [Install ESP32 Board](#Install-ESP32-Board)

3. [Install M5Stack Library](#Install-M5Stack-Library)

4. [Install USB Driver](#Install-USB-Driver)

5. [ArduinoAPI](#ArduinoAPI)

## Install Arduino-IDE


>[Click here to visit Arduino's official website](https://www.arduino.cc/en/Main/Software),Select the installation package for your own operating system to download.


<img src="assets/img/related_documents/Arduino_IDE/Arduino_install.webp">


## Install ESP32 Board

>1.Open up Arduino IDE, navigate to `File`->`Peferences`->`Settings`

<img src="assets/img/related_documents/Arduino_IDE/Arduino_1.webp">

>2.Copy the following ESP32 Boards Manager url to `Additional Boards Manager URLs:`

**https://dl.espressif.com/dl/package_esp32_index.json**

<img src="assets/img/related_documents/Arduino_IDE/Arduino_2.webp">

>3.Navigate to `Tools`->`Board:`->`Boards Manager...`

<img src="assets/img/related_documents/Arduino_IDE/Arduino_3.webp">

>4.Search `ESP32` in the pop-up window, find it and  click `Install`

<img src="assets/img/related_documents/Arduino_IDE/Arduino_4.webp">

>5.select `Tools`->`Board:`->`ESP32`

<img src="assets/img/related_documents/Arduino_IDE/Arduino_5.webp">

## Install M5Stack Library

>Different hardware devices, with different case libraries, please choose to download according to the device you use..Open Arduino IDE, then Select `Sketch`->`Include Library`->`Manage Libraries...`

<img src="assets/img/related_documents/Arduino_IDE/Arduino_6.webp">

### For M5Core and M5Stick

?>Search `M5Stack`  , find it and click `Install`

<img src="assets/img/related_documents/Arduino_IDE/Arduino_7.webp">

### For M5Stick-C

?>Search `M5StickC` , find it and click `Install`

<img src="assets/img/related_documents/Arduino_IDE/Arduino_8.webp">

## Install USB Driver

>1.Click on the CP210X driver for your operating system below to download.

<div class="link">

 <h4><span>CP210X Driver:</span></h4>
    <p>
    <a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/drivers/CP210x_VCP_Windows.zip" target="_blank" rel="noopener noreferrer"><img src="https://cdn.shopify.com/s/files/1/0056/7689/2250/files/windows_89cc6ea0-2a3c-4327-97e5-8f51f448c38b_icon.webp?v=1557026574" alt="">Windows</a>
    <a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/drivers/CP210x_VCP_MacOS.zip" target="_blank" rel="noopener noreferrer"><img src="https://cdn.shopify.com/s/files/1/0056/7689/2250/files/mac_large.webp?v=1557026570" alt="">MacOS</a>
    <a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/drivers/CP210x_VCP_Linux.zip" target="_blank" rel="noopener noreferrer"><img src="https://cdn.shopify.com/s/files/1/0056/7689/2250/files/linux_icon.webp?v=1557026584" alt="">Linux</a>
    </p>
</div>



### For Windows

>Unzip the downloaded driver package, select the installer for your operating system, and double-click to install.

<img src="assets/img/related_documents/Arduino_IDE/CP210X_WIN.webp">


### For Mac

>Unzip the downloaded driver package, install the program, double-click the image file to start the installation..

<img src="assets/img/related_documents/Arduino_IDE/CP210X_MAC.webp">

# ArduinoAPI

## M5Core

|||
|:---:|:---:|
|**[System](en/api/system)** | **[Speaker](en/api/speaker)** |
|**[LCD](en/api/lcd)** | **[Button](en/api/button)** |
|**[IMU Sensor(MPU9250)](en/api/mpu9250)** | **[TF Card](en/api/tf)** |
|**[Power](en/api/power)** |**[I/O](en/api/gpio)** |
|**[I2C Communication](en/api/commutil)** | **[WIFI](en/api/wifi)**|
|**[Timer](en/api/ticker)**|


## M5StickC

|||
|:---:|:---:|
|**[System](en/api/system_m5stickc)** | **[Power Management(AXP192)](en/api/axp192_m5stickc)** |
|**[TFT Screen](en/api/lcd_m5stickc)** | **[IMU(SH200Q)](en/api/sh200q_m5stickc)** |
|**[RTC](en/api/rtc)**|



<style>

.link a{

    padding-left: 13%;

}

</style>s