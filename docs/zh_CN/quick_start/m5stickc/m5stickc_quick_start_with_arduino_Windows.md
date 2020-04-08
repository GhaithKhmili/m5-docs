# M5StickC 上手指南 - Arduino Win{docsify-ignore-all}

<img src="assets/img/getting_started_pics/m5stickc/m5stickc_06.webp">

## 目录

**[1. 安装 Arduino IDE](#_1-安装-Arduino-IDE)**

**[2. 安装 ESP32 的板管理](#_2-安装-ESP32-的板管理)**

**[3. 安装 M5StickC 的库](#_3-安装-M5StickC-的库)**

**[4. 示例](#_4-示例)**

**[5. 视频教程](#_5-相关视频)**

## 1. 安装 Arduino IDE

<!-- *注意：如果已经安装了 IDE，请直接从[步骤 2](#_2-安装串口驱动) 开始。* -->

浏览器打开 Arduino 官网 https://www.arduino.cc/en/Main/Software

#### (1) 点击选择安装包 `Windows ZIP file for non admin install`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/arduino_cc_package.webp">

#### (2) 选择 `JUST DOWNLOAD`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/arduino_cc_package_02.webp">

#### (3) 双击下载好的 IDE 可执行文件，全过程保持默认的选择，包括安装路径也是默认。

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/select_arduino_install_path.webp">

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/install_arduino_2.webp">

## 2. 安装 ESP32 的板管理

#### (1) 打开 IDE，选择 `文件`->`首选项`->`设置`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/quick_start_arduino_win_01_cn.webp">

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/quick_start_arduino_win_02_cn.webp">

#### (2) 复制下面的 ESP32 板管理网址到 `附加开发板管理器:` 中

*ESP32 的板管理网址是这个：https://dl.espressif.com/dl/package_esp32_index.json*

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/quick_start_arduino_win_03_cn.webp">

#### (3) 选择 `工具`->`开发板:`->`开发板管理器...`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/quick_start_arduino_win_04_cn.webp">

#### (4) 在新弹出的对话框中，输入并搜索 `ESP32`，点击`安装`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/quick_start_arduino_win_05_cn.webp">

## 3. 安装 M5StickC 的库

#### (1) 打开 Arduino IDE, 然后选择 `项目`->`加载库`->`库管理...`

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_arduino_m5core/windows/install_m5stack_lib_01_cn.webp">

#### (2) 搜索 `M5StickC` 并安装，如下图所示

<img src="assets/img/getting_started_pics/m5stickc/m5stickc_quick_start_10.webp">

## 4. 示例

这部分是为了验证现在您是否能通过 Arduino IDE 对 M5StickC 编程。

#### (1) 查看串口号

打开`设备管理器`

<img src="assets/img/getting_started_pics/m5stickc/m5stickc_quick_start_06.webp">

因为 M5StickC 的串口驱动芯片免驱动安装类型，所以用 Tpye-C USB 线连接 M5StickC 和电脑，`设备管理器`就会新出现一个串口号

<img src="assets/img/getting_started_pics/m5stickc/m5stickc_quick_start_05.webp">

#### (2) 运行一个示例程序，比如 `FactoryTest.ino`

打开 Arduino IDE，并选择正确的串口号。这个串口号其实就是连接 M5StickC 的串口号，注意不要选错

* <font color="red">选择开发板 ( Board ): ESP32 Pico Kit</font>

* <font color="red">选择波特率 ( Upload Speed ): 115200bps 或 1.5Mbps</font>

* <font color="red">选择串口号 ( Port )：COM31</font> ( 我现在与 M5StickC 相连的串口就是 `COM31`，所以我应该选择 `COM31` )

<img src="assets/img/getting_started_pics/m5stickc/m5stickc_quick_start_08.webp">

选择 `M5StickC` -> `Basics` -> `FactoryTest.ino`

<img src="assets/img/getting_started_pics/m5stickc/m5stickc_quick_start_04.webp">

点击上传

<img src="assets/img/getting_started_pics/m5stickc/m5stickc_quick_start_09.webp">

<!-- **现象: 按下按键 A 之后，屏幕显示 "Hello World! Exist"**

**单击电源键开机，双击电源键休眠。** -->

<!-- ?> *如果您想升级Arduino-M5Stack库的话，请移步阅读这篇文档[如何升级Arduino-M5Stack库](zh_CN/related_documents/upgrade_m5stack_lib).* -->

## 5. 相关视频

- Arduino 中开发 M5StickC 的视频教程

<video width="500" height="315" controls>
    <source src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/video/%E6%95%99%E7%A8%8B/StickC/StickC%20Arduino%20Tutorial_cn.mp4" type="video/mp4">
</video>
