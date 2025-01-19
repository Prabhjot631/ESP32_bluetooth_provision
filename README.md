# ESP32_bluetooth_provision

INTRODUCTION: 
In this documentation i am going to show you how to upload wifi SSID and PASSWORD to your esp32 using bluetooth app on your mobile phone and connect your
esp32 to the wifi router or internet.

THINGS NEEDED:
1. ESP32 WITH BLUETOOTH
2. WORKING MOBILE
3. COMPUTER/LAPTOP
4. WIFI ROUTER

STEP 1: Install vscode in your computer after installing the vscode go to left side panel and click on extensions from there search esp idf click on the first extension and click install. After installing click on express setting and it will be configured automatically.

Step 2: Now open the idf extension and after that click on advance and new than click on new project wizard. Now there will be some files in the left panel of vscode from there select main.c and rename it .cpp this will convert it into c++ file.

Step 3: Now you have to make code to turn wifi provision and bluetooth on esp32 i will attach the code in this file. This code needs a dependency to generate a qr code that dependacy can be downloaded from here: https://components.espressif.com/components/espressif/qrcode go to this side and copy the terminal command from the right side of the web page. For code to work you also need a jason.hpp file which can be download from here: https://github.com/nlohmann/json/tree/develop/single_include/nlohmann After this all coding part has been done now you only have to compile and upload code to the esp32.

step 4: Uploading code click on fire icon which is in the bottom of the vscode that will compile and upload code to esp32 from com port select appropriate com port for your esp32.

step 5: After uploading code you will see some output there will be a qr code which is important for wifi provision.

step 6: Download ble provision app from the app store and turn on bluetooth on your phone. Open the app and there will be only one button in app which is provision device click on the and scan that qr code which is displayed in vscode. after that it will ask for you ssid and password type it and than your esp32 will be automatically connected to the router. You will also see result in the vscode.
