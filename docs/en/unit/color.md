# COLOR {docsify-ignore-all}

<img src="assets/img/product_pics/unit/M5GO_Unit_color.png" width="30%" height="30%">



## Description

**COLOR** is color recognition unit integrated **TCS3472**. Like its namesake, **COLOR** is able to detect color value and return RGB data to the host.

**Identify color principle:**

In the TCS3472, a 3*4 array of filtered photodiodes and a 16 bit analog-to-digital converters are embedded. Of the 12 photodiodes, 3 have red filters, 3 have green filters, 3 have blue filters and 3 have no filter(clear).

<img src="assets/img/product_pics/unit/color/unit_color_07.png">

When detecting the color of an object, TCS3472 returns data from four channels: red(R), green(G), blue(B) and clear(C)(non-filtered). The response from the red, green and blue channels (RGB) can be used to determine a particular source’s chromaticity coordinates (x, y).

<img src="assets/img/product_pics/unit/color/unit_color_04.png">

Chromaticity Calculation Process Overview:

<img src="assets/img/product_pics/unit/color/unit_color_05.png">

When we get coordinates (x, y), please reference the below figure so as to get the recommended color.

<img src="assets/img/product_pics/unit/color/unit_color_06.png">

This Unit communicates with the M5Core via the GROVE A interface(I2C). Address is 0x29.

## Product Features

- Detection range: -40℃~85℃
- GROVE interface, support [UIFlow](http://flow.m5stack.com) and [Arduino](http://www.arduino.cc)
- Two Lego-compatible holes
- Product Size：32.2mm x 24.2mm x 8.2mm
- Product weight：3.9g

## Include

- 1x COLOR Unit
- 1x Grove Cable

## Applications

- Product Color Verification
- Color tracking robot

## Related Link

-  **Datasheet** - [TCS3472](https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/datasheet/unit/TCS3472_en.pdf)

## EasyLoader

<img src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/image/EasyLoader_logo.png" width="100px" style="margin-top:20px">

<a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/EasyLoader/Unit/EasyLoader_Color.exe"><button type="button" class="btn btn-primary">click to download EasyLoader</button></a>

>1.EasyLoader is a simple and fast program burner. Every product page in EasyLoader provides a product-related case program. It can be burned to the master through simple steps, and a series of function verification can be performed. .

>2. After downloading the software, double-click to run the application, connect the M5 device to the computer through the data cable, select the port parameters, click **"Burn"** to start burning. (**For M5StickC burning, please Set the baud rate to 750000 or 115200**)

?>3. Currently EasyLoader is only suitable for Windows operating system, compatible with M5 system adopts ESP32 as the control core host. Before installing for M5Core, you need to install CP210X driver (you do not need to install with M5StickC as controller)[Click here to view the driver installation tutorial](en/related_documents/M5Burner#install-usb-driver)

## Example

### 1. Arduino IDE

*The code below is incomplete. To get the complete code, please click [here](https://github.com/m5stack/M5-ProductExampleCodes/tree/master/Unit/COLOR/Arduino).*

```arduino
/*
  Color test
    hardware: M5Stack

  please install the Adfruit TCS34725 library first ...
*/
#include <Wire.h>
#include <M5Stack.h>
#include "Adafruit_TCS34725.h"

// declaration
uint16_t clear, red, green, blue;
#define commonAnode true // set to false if using a common cathode LED

// new a object
Adafruit_TCS34725 tcs;
tcs = Adafruit_TCS34725(TCS34725_INTEGRATIONTIME_50MS,TCS34725_GAIN_4X);

// initialization
M5.begin(true, false, false);
tcs.begin();
tcs.setIntegrationTime(TCS34725_INTEGRATIONTIME_154MS);
tcs.setGain(TCS34725_GAIN_4X);

// read data
tcs.getRawData(&red, &green, &blue, &clear);
```

After burnt this example, PC serial terminal will print original value RGBC(red, green, blue, clear).

<img src="assets/img/product_pics/unit/unit_example/COLOR/example_unit_color_result_01.png">

### 2. UIFlow

*If you want the complete code, please click [here](https://github.com/m5stack/M5-ProductExampleCodes/tree/master/Unit/COLOR/UIFlow).*

<img src="assets/img/product_pics/unit/color/color.png">

## Schematic

<img src="assets/img/product_pics/unit/color_sch.JPG">

### PinMap

<table>
 <tr><td>M5Core(GROVE A)</td><td>GPIO22</td><td>GPIO21</td><td>5V</td><td>GND</td></tr>
 <tr><td>COLOR Unit</td><td>SCL</td><td>SDA</td><td>5V</td><td>GND</td></tr>
</table>

## Video

**COLOR Case - 01**

<video class="video_size" controls>
    <source src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/video/Blog/Twitch201902/Color%20Unit.mp4" type="video/mp4">
</video>

<script>

   var purchase_link = 'https://m5stack.com/collections/m5-unit/products/color-unit';

   anchor_search(purchase_link);
   scrollFunc();

</script>