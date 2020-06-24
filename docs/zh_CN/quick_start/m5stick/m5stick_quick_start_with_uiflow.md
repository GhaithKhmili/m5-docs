# M5Stick 快速上手 - UIFlow {docsify-ignore-all}

<img src="assets/img/getting_started_pics/m5stick/stick_01.webp"><img src="assets/img/getting_started_pics/m5stick/stick_06.webp">

1. **[更新固件](#更新固件)**

2. **[开关机操作](#开关机操作)**

3. **[编程环境配置](#编程环境配置)**

    - **[Step1. 设置WIFI](#step1-设置wifi)**

    - **[Step2. 设置API Key](#step2-设置api-key)**

4. **[例程](#例程)**

5. **[相关视频](#相关视频)**

6. **[UIFlow 教程](https://m5stack.github.io/UIFlow_doc/cn/index.html)**

## 更新固件

>将stick更新到最新固件版本，以获得更棒的体验

*如果需要更新或自行烧录固件的话，请点击[这里](zh_CN/related_documents/M5Burner)*

<img src="assets/img/getting_started_pics/m5stick/stick_03.webp">

## 开关机操作

>位于机身左侧下方的按键是电源键，单击为开机，运行时再次按下为复位，如需休眠则需快速按下电源键两次

>除了电源键以外，stick还提供了另一个A按键可供您编程使用

<img src="assets/img/getting_started_pics/m5stick/stick_02.webp" width="300" height="300">

## 编程环境配置

### Step1. 设置WIFI

#### 注意

配置的WIFI的信息内容不允许使用中文及特殊符号.

首次开机时，会默认进入配置页面，stick的屏幕上显示了**热点的名称（SSID）**，以及**网络配置的地址（192.168.4.1）**

这时候可以使用手机连接这个热点，待连接成功后，使用浏览器输入网络配置地址，进入WIFI配置页面，输入个人WIFI的信息，点击保存，等待连接成功

<img src="assets/img/getting_started_pics/m5stick/stick_04.webp">

### Step2. 设置API Key

配置WIFI成功后stick会自动进行重启，并进入编程模式，当屏幕显示“Done”，则表示已经成功连接上了网络，访问[flow.m5stack.com](http://flow.m5stack.com/)进入编程UIFlow编程页面

点击屏幕右上角的菜单中的设置按钮，填写stick屏幕上显示的**API Key**，点击保存，开始编程吧！

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_m5stick/uiflow_setting.webp">

<img src="assets/img/getting_started_pics/m5stick/stick_05.webp">

## 操作补充

>如果下载了程序，那么每次开机都会默认运行，如果想要重新运行或下载程序，那么需要在重启出现Logo时单击按键A，再次进入编程模式

<img src="assets/img/getting_started_pics/m5stack_core/get_started_with_m5stick/uiflow_download.webp" width="50%" height="50%">

>如果想要配置新的WIFI，那么需要在重启出现Logo时，长按按键A一秒以上后松开，进入配置页面

>如果错过了操作时间，可以单击复位按钮，重启再次操作

## 例程

>点击下载[例程](https://github.com/m5stack/M5-ProductExampleCodes/tree/master/Core/M5Stick/UIFlow)，并在UIFlow中打开例程，下载例程到stick中。效果：白色方块会在屏幕上来回滚动

<img src="assets/img/product_pics/core/minicore/m5stick/example/example_core_m5stick_02.png" width=50% height=50%><img src="assets/img/product_pics/core/minicore/m5stick/example/example_core_m5stick_03.png" width=50% height=50%>


## 相关视频

**UIFlow 的简单介绍**

<video width="500" height="315" controls>
    <source src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/video/%E6%95%99%E7%A8%8B/UIFlow%20Tutorials/A3%20-%20UIflow%E7%AE%80%E4%BB%8B.mp4" type="video/mp4">
</video>

**UIFlow 的快速指南 (Mac & Linux)**

<video width="500" height="315" controls>
    <source src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/video/LukeVideo/Getting%20started%20with%20UI%20flow%20(Mac_Linux).mp4" type="video/mp4">
</video>
