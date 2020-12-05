***

### CE Smart Home - LA-WF3 Wifi Plug (TYWE2S)
Simple and compact Wifi Plug, based in ESP8266, internal module Tuya TYWE2S


***

_esptool log:_
_Wifi module is an: TYWE2S:_
_Detecting chip type... ESP8266_
_Chip is ESP8285_
_Features: WiFi, Embedded._

Model purchased:
https://www.costco.ca/Wi-Fi-Smart-Plug%2C-2-pack.product.100417575.html 24.99 CAD$

### Product 

![Package](https://raw.githubusercontent.com/willngton/Smarth_Plug_LA_WF3/master/LA_WF3_01.png)
![Internal](https://raw.githubusercontent.com/willngton/Smarth_Plug_LA_WF3/master/LA_WF3_02.png)
![Internal](https://raw.githubusercontent.com/willngton/Smarth_Plug_LA_WF3/master/LA_WF3_03.png)


### OTA Flash

Successfully flashed to Tasmota 8.1.0.2 using [Tuya-Convert](https://github.com/ct-Open-Source/tuya-convert) [v2.4.4](https://github.com/ct-Open-Source/tuya-convert/releases/tag/v2.4.4), then upgraded to 9.1.0. Devices purchased 2019, no official firmware updates applied. 

### Flashing
GPIO0 Needs to be grounded in order to get into flashing mode.
1. erase_flash
2. flash tasmota_minimal
3. flash tasmota_full

![PCB Diagram](https://raw.githubusercontent.com/willngton/Smarth_Plug_LA_WF3/master/LA_WF3_08.png)
![PCB](https://raw.githubusercontent.com/willngton/Smarth_Plug_LA_WF3/master/LA_WF3_05.png)
![Pins](https://raw.githubusercontent.com/willngton/Smarth_Plug_LA_WF3/master/LA_WF3_04.png)

### Module Configuration

Template:
```
{"NAME":"LA-WF3","GPIO":[0,0,0,0,544,320,0,0,224,32,0,0,0,0],"FLAG":0,"BASE":18}
```

* GPIO4 = Blue LED
* GPIO5 = Red LED (Note the LED is a single bi-color LED; doesn't appear possible to have both red and blue at the same time)
* GPIO12 = Relay
* GPIO13 = Button

![Tasmota 9.1.0 module configuration](https://i.imgur.com/UFj8O40.png)

<details>
  <summary>Tasmota 6.2.1</summary>
  
  ![Tasmota 6.2.1 module configuration](https://raw.githubusercontent.com/willngton/Smarth_Plug_LA_WF3/master/LA_WF3_06.png)
</details>



