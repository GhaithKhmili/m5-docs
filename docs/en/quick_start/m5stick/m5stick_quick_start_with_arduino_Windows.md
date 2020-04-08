# M5Stick Quick Start - Arduino Win {docsify-ignore-all}

<img src="assets/img/getting_started_pics/m5stick/stick_01.webp"><img src="assets/img/getting_started_pics/m5stick/stick_06.webp">

## Table of Contents

**[1. Install Arduino IDE](#_1-install-Arduino-IDE)**

**[2. Install USB to Serial Driver](#_2-Install-USB-to-Serial-Driver)**

**[3. Install ESP32 Boards Manager](#_3-Install-ESP32-Boards-Manager)**

**[4. Install M5Stack Library](#_4-Install-M5Stack-Library)**

**[5. Install U8g2 Library](#_5-Install-U8g2-Library)**

**[6. Example](#_6-Example)**

## 1. Install Arduino IDE

<!-- *注意：如果已经安装了 IDE，请直接从[步骤 2](#_2-安装串口驱动) 开始。* -->

Open up your browser, and visit Arduino official website https://www.arduino.cc/en/Main/Software

#### (1) click `Windows ZIP file for non admin install` to download `Arduino IDE`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/arduino_cc_package.webp">

#### (2) click `JUST DOWNLOAD`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/arduino_cc_package_02.webp">

#### (3) To install IDE, double click Arduino executable file. Keep the default selection throughout this process, including the installation path.

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/select_arduino_install_path.webp">

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/install_arduino_2.webp">

## 2. Install USB to Serial Driver

>1.Click the link on the right to download the CP210X driver.. <a class="link" style="padding-left: 20%" href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/drivers/CP210x_VCP_Windows.zip" target="_blank" rel="noopener noreferrer"><img src="https://cdn.shopify.com/s/files/1/0056/7689/2250/files/windows_89cc6ea0-2a3c-4327-97e5-8f51f448c38b_icon.webp?v=1557026574" alt="">Windows</a>

#### (2) Based on your Windows operating system type, select the corresponding driver installation package

* 32-bit  `CP210xVCPInstaller_x86_vx.x.x.x.exe`

* 64-bit  `CP210xVCPInstaller_x64_vx.x.x.x.exe`

<img src="assets/img/getting_started_pics/establish_serial_connection/windows_install_usb_driver01.webp">

#### (3) double click the executable file to install.

<img src="assets/img/getting_started_pics/establish_serial_connection/windows_install_usb_driver02.webp">

<img src="assets/img/getting_started_pics/establish_serial_connection/windows_install_usb_driver03.webp">

#### (4) Check the serial port number `COMx`

Check identified COM port list in the `Windows Device Manager`:

Connect the Core to the computer via a USB Type-C cable, open `Windows Device Manager`, click `Ports(COM & LPT)` if you see this `SiLicon Labs CP210x USB to UART Bridge(COMx) `, means the driver installation succeed and your PC is allowed to communicate with M5.

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/check_serial_port_01.webp">

## 3. Install ESP32 Boards Manager

#### (1) Open up Arduino IDE, navigate to `File`->`Peferences`->`Settings`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/quick_start_arduino_win_01.webp">

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/quick_start_arduino_win_02.webp">

#### (2) Copy the following ESP32 Boards Manager url to `Additional Boards Manager URLs:` , hit `OK`.

*ESP32 Boards Manager url: https://dl.espressif.com/dl/package_esp32_index.json*

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/quick_start_arduino_win_03.webp">

#### (3) Navigate to `Tools`->`Board:`->`Boards Manager...`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/quick_start_arduino_win_04.webp">

#### (4) Search `ESP32` at `Boards Manager` window, find it and  click `Install`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/quick_start_arduino_win_05.webp">

## 4. Install M5Stack Library

#### (1) Open Arduino IDE, then Select `Sketch`->`Include Library`->`Manage Libraries...`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/install_m5stack_lib_01.webp">

#### (2)  Search `M5Stack`  , find it and click `Install`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/install_m5stack_lib_02.webp">

## 5. Install U8g2 Library

#### (1) Open Arduino IDE, and navigate to  `Sketch`->`Include Library`->`Manage Libraries...`, search `U8g2` and install this library.

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_m5stick/install_u8g2.webp">

## 6. Example

Now that everything is ready to go, you can select a demo from the `Example` list, before that, let's do some configuration on the IDE. 

Make sure you have M5Stick connected to your computer via USB

#### (1) Select the correct board name and serial device name

Select `Tools -> Boards -> M5Stack-Core-ESP32` 

Choose the right port number at  `Tools -> Ports ->`.

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/mac/quick_start_arduino_mac_10.webp">

#### (2) Select an example

Click `File-> Examples`. Here are some test demo in `M5Stack`->`Stick`

Let's try an example inside Basics. Name `FactoryTest` 

<img src="assets/img/getting_started_pics/m5stick/m5stick_quick_start_arduino_mac_01.webp">

Click `Upload`, to flash the code to the device. Once it's done, reset the device, The screen will display "Hello World!"

**The button located at the bottom left is the power button, single-click to  reboot. To enter deep sleep mode, double click this button**
