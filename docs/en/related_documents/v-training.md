# V-Training {docsify-ignore-all}


<img src="assets\img\related_documents\v-training\v_training.webp" width="100%">

**[1. Burner Firmware](#Burner-Firmware)**

**[2. Insert SD Card](#Insert-SD-Card)**

**[3. Material Training](#Material-Training)**

**[4. Upload Data  to Cloud](#Upload-Data-to-Cloud)**

**[5. Download Model](#Download-Model)**

**[6. Run Recognition Program](#Run-Recognition-Program)**

**[7. Good Practice](#Good-Practice)**


## Burner Firmware

<h4><mark>Users who have already programmed the firmware should start directly from the Second step.</mark></h4>

### EasyLoader <span class="badge badge-secondary">optional</span>

<img src="https://m5stack.oss-cn-shenzhen.aliyuncs.com/image/EasyLoader_logo.webp" width="100px" style="margin-top:20px">

<a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/EasyLoader/M5Core/M5StickV/EasyLoader_M5StickV_1022_beta.exe"><button type="button" class="btn btn-primary">Download EasyLoader</button></a>

>1, EasyLoader is a consice and effictive firmware flashing tool, each product page will packed with a EasyLoader for users to flash product related application example. For those who need none-customized firmware, using EasyLoader can offer you a default firmware,(Only Windows computer supported)  

>2, After downloaded , double click to run the app,  connect the device to computer via USB cable, select the com port number, then click "Burn" to start it.

### Download Firmware <span class="badge badge-secondary">optional</span>

> EasyLoader is only Window-supported.  If you don't have a Windows computer or you would like to download specific file to flash , please use "Kflash, download firmware below "

<a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/M5StickV_Firmware_1022_beta.kfpkg"><button type="button" class="btn btn-primary">click to download firmware file</button></a>


>1, Select Kflash_GUI flash tool for your computer OS.

<div class="link">
 <h4><span>Kflash_GUI:</span></h4>
    <p>
    <a href="https://github.com/sipeed/kflash_gui/releases/download/v1.5.3/kflash_gui_v1.5.3_windows.7z" target="_blank" rel="noopener noreferrer"><img src="https://cdn.shopify.com/s/files/1/0056/7689/2250/files/windows_89cc6ea0-2a3c-4327-97e5-8f51f448c38b_icon.webp?v=1557026574" alt="">Windows</a>
    <a href="https://github.com/sipeed/kflash_gui/releases/download/v1.5.2/kflash_gui_v1.5.2_macOS.dmg" target="_blank" rel="noopener noreferrer"><img src="https://cdn.shopify.com/s/files/1/0056/7689/2250/files/mac_large.webp?v=1557026570" alt="">MacOS</a>
    <a href="https://github.com/sipeed/kflash_gui/releases/download/v1.5.3/kflash_gui_v1.5.3_linux.tar.xz" target="_blank" rel="noopener noreferrer"><img src="https://cdn.shopify.com/s/files/1/0056/7689/2250/files/linux_icon.webp?v=1557026584" alt="">Linux</a></p>
</div>

>2, Connect the device to computer via Type-C cable, double click to open the **Kflash_GUI** app, choose the right com port , developement board type, firmware file, baud rate, click download to start the process.

<img src="assets\img\getting_started_pics\m5stickv\kflash_gui_01.webp">

### Kflash

>3, For people who are used to use command line, Kflash could be an alternative option.[Click here for details](https://github.com/kendryte/kflash.py)

## Material Training

### boot code

> Material Training requires SD cards, users could downloade boot code zip files, unzip the files to SD card.(M5StickC only recognized certain type of SD card , [click to see the supported type](en/core/m5stickv?id=sd-card-test))

<a href="https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/VTraining-Client-VerA02B01.zip"><button type="button" class="btn btn-primary">Click here download boot zip</button></a>

<img src="assets\img\related_documents\v-training\1.webp" width="60%">

### Footage Shooting 

> Load the SD card before power on the device. SD card is used for saving the footage. Long press left button to power on, if the screen show a display  Training like below, means it entered shooting program. 

<img src="assets\img\related_documents\v-training\2.webp" width="60%">

> By default, the code provided 10 set of Class for you to shooting the training material, each class represent a recognition object. <mark>For better result, we recommend to shoot more than 3 Class (More than 3 recognition object )</mark>

>Navigate bar on top of the screen would display instant Class number and picture amount. Press HOME button to start  shooting, right side button is to switch between Classes.

<img src="assets\img\related_documents\v-training\3.webp" width="60%">

>During shooting, plase try to keep the shooting picture as close to the reality scene as possible, such as light intensity. Regars to the shooting distance,  better keep it just enough to fill the recgnition object into the screen, not much choas on the background.

<img src="assets\img\related_documents\v-training\4.webp" width="100%">

<mark>note：In order to reach a certain accuracy, each Class should contains at least 35 pictures, or the Could Training would give out a rejection</mark>

### Material Checking and Compress

>After finish the shooting, shut down the device, take out SD card, put the photos materials into "train" and "vaild" folder. Copy to your computer.

<img src="assets\img\related_documents\v-training\5.webp" width="60%">

> Inside folder "train","vaild", they share exact the same folder directory, when we switch Class, the program will generate the same folder (with a name of Class number) in both "train" and "vaild". The phtotos will placed either in "train" or "vaild",  underneath the coorespondent Class folder.

> Before we compress the package, we should check the photo and photo number, make sure for the same Class, the number of photos in the coorespondent Class Folder in  
<mark>"train" and "vaild"  should add up over 35. If any Class photos total amount were under 35, please either delete it or copy for back up. After finish the checking, let's compress the "train" and "vaild" to ZIP.
</mark>

## Upload Data to Cloud

>[Click to visit upload page](http://v-training.m5stack.com/)，type in your personal information（upload file should under 200MB, and had to be ZIP format）

<img src="assets\img\related_documents\v-training\6.webp" width="60%">

> After the Upload is done, file will enter request queue. At bottom left corner will show the current queue status.

<img src="assets\img\related_documents\v-training\7.webp" width="60%">

## Download Model

>After training accomplished, code file will sent to your personal e-mail, copy the download link to download the file to your computer.Unzip the file, copy it to SD card, keep the SD card in the M5StickV

<img src="assets\img\related_documents\v-training\8.webp" width="60%">

<img src="assets\img\related_documents\v-training\9.webp" width="60%">

## Run Recognition Program

>power on to run the progarm automatically.

<img src="assets\img\related_documents\v-training\10.webp" width="60%">

>Default program will do the recognition according to the order of the Class, and will display on the screen. Users can change the boot.py file to modify the display information.

<img src="assets\img\related_documents\v-training\11.webp" width="60%">


<style>

.link a{

    padding-left: 13%;

}

</style>


## Good Practice

>1.  If your Loss line looks like below, there is something wrong with your dataset, you need to either clear it up or add more pictures. If everything is OK, and adding more pictures does not help, our network structure may not good for solve your problem.

<img src="assets\img\related_documents\v-training\12.webp" >


<img src="assets\img\related_documents\v-training\13.webp" >

>2. If your Loss line looks like below, it seems the Convolutional Neural Network does not converge at all. There might be some serious problems in your data-set, check your data-set. If everything is OK, and adding more pictures does not help, our network structure may not good for solve your problem.

<img src="assets\img\related_documents\v-training\14.webp" >

>3.  If your Loss line looks like below, but recognition results are still not good, you might need to add more pictures and try again;
If everything is OK, and adding more pictures does not help, our network structure may not good for solve your problem.


<img src="assets\img\related_documents\v-training\15.webp" >

>4. If the results you get is not very ideal, you might want to try to add few more pictures and train again. Network may converge better this time.

### Common Errors(FAQ):

>1. “CONTENT: Number of Classes presented in Train and Vaild dataset is not equal.”
Or
“CONTENT: Train or Valid folder not found. If you are using the M5StickV software, make sure you reach enough image counts of 35 per class.”
Or
“CONTENT: Number of Classes presented in Train and Vaild dataset is not equal.”

Answer: Your zip file should looks like this:
Inside your zip file, you have two folder named train and valid(or vaild, is also ok)

<img src="assets\img\related_documents\v-training\16.webp" >

Inside each of the folder, You have several folders start named by class (class should only be a number from 1 to 10). The number of folders in your train and valid folder should be the same. And the name of the folder should follow each other and starting at 1. 

<img src="assets\img\related_documents\v-training\17.webp" >

>2. “CONTENT: Lake of Enough Valid Dataset, Only 16 pictures found, but you need 20 in total.”
Or
“CNTENT: Lake of Enough Train Dataset, Only 43 pictures found, but you need 45 in total.”

Answer: You don’t have enough pictures in your train or valid folder. You need to add more photos to them. Or you accidentally add an extra class.

>3. “CONTENT: Number of Classes should larger or equal to two.”

Answer: Sorry, we don’t support single class, you need to at least have two or more class folders in your valid and train folder. 

>4. “CONTENT: Unexpected error happened during checking dataset, cannot identify image file 'dataset_tmp/xxxxxxxx_dataset/train/2/1.webp'”

Answer: The system cannot read the image while processing it. You might need to replace this picture. 
