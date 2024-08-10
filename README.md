<p align="center">
  <img src="https://user-images.githubusercontent.com/80714882/234116124-5bbd7e92-5432-42f2-bb0e-574ed005aee8.png" width="75%" height="75%">
</p>


<p align="center">
   <img src="https://img.shields.io/badge/ESPRESSIF-ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white" >
   <img src="https://img.shields.io/badge/FreeRTOS-4bbb4f?style=for-the-badge">
   <img src="https://img.shields.io/badge/LICENSE-MIT-green?style=for-the-badge" >
</p>








# Home-Automation-Using-ESP32
Welcome to my Home Automation project using ESP32! This repository contains the code and documentation for building a fully-connected smart home system. With this project, you'll be able to control your home appliances using a smartphone or computer, as well as manual buttons.
ESP32 based 4 Channel IOT Home Automation using ESPRAINMAKER Application. Can be controlled using Physical switch as well as virtual buttons on the ESPRAINMAKER app. Works with or without internet connection using Manual Switches and WiFi connectivity with real time device status on the app.

## About Smart Home Automation

When we think of home automation we generally visualize switching on/off some buttons, temperature monitoring, etc.

> It is not smart automation in true sense

- To achieve true home automation Real Time Operating System (RTOS) is integrated in the system which can perform multiple things simultaneously.
- The system is smart enough to automatically trigger actions based on certain events happening in real time.
## Features
- Control using physical switches
- Control using ESPRAIAMAKER APP
- Get Real Time Device Status in the APP
- Works Online or Offline
- Works with Manual Switch and WiFi simultaneously.
- You can also add a timer to control the relays automatically with the pre-defined time.
- The method used for controlling are voice controlled with Google Assistant, Amazon Alexa, EspRainmaker App and Manual switches.
## Overview Of the project
  The entire system is powered by a 5V Adaptor/charger (Micro-type). After receiving user commands over the internet. ESP 32 process these instructions to operate these loads accordingly and display the system status on a smart phone display. Thus, this system allows for efficient home automation over the internet. In this we have used an ESP Rainmaker application for controlling the home appliances all over the world. The method used for controlling are voice controlled with Google Assistant, Amazon Alexa, and manual switches. If the ESP32 connected with Wi-Fi then it can also monitor the real-time feedback of the relays in the ESP Rainmaker app. If the Wi-Fi is available then ESP32 will automatically connect with the Wi-Fi.. If there is no internet available still it can control the relay module from the manual switches.
  ## Requirement Specification
  This project consists of two parts Software and Hardware. Software part refers to the designing algorithms, coding and compilation. It also includes development of user interface. Hardware refers to the development of the device itself including circuit construction, printed circuit board etching and soldering process
## Hardware Requirements
| S.NO. | Components             | Quantity |
|-------|------------------------|----------|
| 1     | ESP 32                 | 1        |
| 2     | 4 Channel Relay Module | 1        |
| 3     | Hi-link                | 1        |
| 4     | Zero PCB               | 1        |
| 5     | Switches               | 4        |
| 6     | Board                  | 1        |
| 7     | Male pin headers       | 1        |
| 9     | Female pin headers     | 1        |
| 10    | USB cables             | 1        |
## Software Requirments
-	**ARDUINO IDE:** is an open-source prototyping platform enabling users to create interactive electronic objects. Arduino IDE software is used to compile the code contains a text editor for writing code, a message area, a text console, a toolbar with buttons for common functions and a series of menus. It connects to the Arduino hardware to upload programs and communicate with them. 

-	**ESP RAINMAKER APPLICATION:** was designed for the Internet of Things. It can control hardware remotely, it can display sensor data, it can store data, visualize it, etc. the prototype primarily uses ESP Rainmaker application to sense commands from user to the hardware over wireless network.

-	**GOOGLE ASSISTANT:** is a system software present on the android phone. It interprets the voice commands by the user to turn on or off an appliances

-	**AMAZON ALEXA:** Alexa Voice Service is the intelligent voice control service that powers the device, Amazon Echo. Alexa uses natural language processing techniques trained by the developers. The voice service can be triggered using the keyword “Alexa”. As mentioned earlier, the skill/application that I have developed can be triggered using the voice command, “Alexa, Turn the lights on”. Once Alexa is triggered, it runs a script on the cloud, which in-turn runs a subroutine on an ESP 32 to Switch on the light. Once computation is done in the ESP 32, it sends the confirmation back to Alexa. Only the essential information is sent to Alexa which passes it on back to the user

  -	### Schematic

Components can be assembled and connected as shown in the schematic.

<p align="center">
	<img src="https://github.com/parikshitpagare/smart-home-automation-rtos/assets/80714882/7b1ebb97-7876-485a-b43b-686890d2b0f5" width="80%" height="80%">
</p>

### How to connect ESP32 with Arduino IDE?

- Download and install the Arduino IDE
- Install the ESP32 Library at `File -> Preference -> Additional Boards Manager URLs:` https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json
- Then in the `Tools -> Board Manager` -> search for ESP32 and install

### Libraries 

Certain libraries are required for proper functioning of the microcontroller and interfaced components.

- [Bluetooth Serial]((https://github.com/espressif/arduino-esp32/tree/master/libraries/ESP32))
- [Wire](https://github.com/esp8266/Arduino/blob/master/libraries/Wire/)
- [DHT](https://github.com/adafruit/DHT-sensor-library)
- [Adafruit_SSD1306](https://github.com/adafruit/Adafruit_SSD1306)
- [Adafruit_GFX](https://github.com/adafruit/Adafruit-GFX-Library)
- [Ticker](https://github.com/espressif/arduino-esp32/tree/master/libraries/Ticker)
