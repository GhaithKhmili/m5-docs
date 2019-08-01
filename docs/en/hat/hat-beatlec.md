# BeatleC {docsify-ignore-all}

<img src="assets\img\product_pics\hat\beatlec_hat\beatlec_hat_01.jpg" width="30%" height="30%">


:memo:**[Description](#Description)**&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/image/EasyLoader_logo-min.jpg">**[EasyLoader](#EasyLoader)**


## Description

Ever wanted to build your robotic car with tiny body and smooth control? Here comes the BeatleC, features a dual-driver and 7 RGB LEDs, extreme concise design and ESP32-Based, makes it the handiest and full-function small robotic car ever. 

It is consist of two parts, the M5StickC controller and BeatleC base. On the base, we have two DC geared motor driven by STM32F030.  The two parts are connected through the top slot on StickC. 
The body of the robotic car is inclined because the wheels we put on front and back are different sizes as you can see from the pictures. 
Besides, a power switch is placed at the front. 

<img src="assets\img\product_pics\hat\beatlec_hat\beatlec_hat_02.jpg" width="50%" height="30%">

## Product Feature

- Small Robotic Car
- ESP32 based (Wi-Fi and Bluetooth available)
- Wireless controllable
- Dual-Driver
- 7x RGB LEDs 
- Built-in battery: base (80ma), M5StickC (80ma).
- Concise design
- Smooth control
- Size: 70mm*50mm*32mm
- Front-wheel diameter: 25mm ⌀
- Back-wheel diameter:14mm  ⌀


## Applications

- Remote Motor control 
- Wireless Robotic control

## EasyLoader

<img src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/image/EasyLoader_logo.png" width="100px" style="margin-top:20px">

<a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/EasyLoader/HAT/BeatleC/EasyLoader_BeatleC.exe"><button type="button" class="btn btn-primary">click to download EasyLoader</button></a>

>1.EasyLoader is a simple and fast program burner. Every product page in EasyLoader provides a product-related case program. It can be burned to the master through simple steps, and a series of function verification can be performed.(**Currently EasyLoader is only available for Windows OS**)

>2. After downloading the software, double-click to run the application, connect the M5 device to the computer through the data cable, select the port parameters, click **"Burn"** to start burning. (**For M5StickC burning, please Set the baud rate to 750000 or 115200**)


## Operation Steps

### How to set up BeatleC
- Connect M5StickC to the beatleC Base by Pin header.
- Press reset button to turn on M5StickC.
- Check the hardware reflection: 
  - 7 leds at Base will light up in turns for 3 times.
  - Press button A, the Front wheel will rotate forward and backward for 500ms.
- Use your phone or computer to Wi-Fi Scan, search and connect the ssid name start with "beatle" plus mac address displayed on the screen.  
- Then open a Browser and type in ```192.168.4.1/ctl```. Control page should show up after the page was loaded.

### Control Page

<img src="assets\img\product_pics\hat\beatlec_hat\beatlec_hat_03.png" width="40%" height="30%">

- Push upwards the control bar to speed up the wheel and push down to slow down.
- There are four color bolcks at the bottom. The colorful blocks are used to turn on all RGB LEDs at the bottom to the specified color. Block with black will turn off the light.


## Code

### 1. Arduino IDE

*To get complete code, please click [here](https://github.com/m5stack/M5-ProductExampleCodes/tree/master/Hat/beatleC/stickc/Arduino).*


## Video

<video width="500" height="500" controls>
    <source src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/video/Product_example_video/HAT/BeatleC_01.mp4" type="video/mp4">
</video>

<video width="500" height="500" controls>
    <source src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/video/Product_example_video/HAT/BeatleC_02.mp4" type="video/mp4">
</video>