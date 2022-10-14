# ESE-519-Lab-2-Setup-Guide
 **We will set up our Laptop/PC for Adafruit QT Py 2040 using the official C/C++ SDK. Afterward, we will compile and run example code like "Hello World".
**
##Machine Details
###OS:
###OS Version:
###Processor:
###Laptop Model:

##Installed Software List:

Arm GCC Compiler               :    https://developer.arm.com/downloads/-/gnu-rm
CMake Software                 :    https://cmake.org/download/
The C++ build tools for VS     :    https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2019
Python 3                       :    https://www.python.org/downloads/windows/
Git                            :    https://git-scm.com/download/win
Visual Studio Code             :    https://code.visualstudio.com/Download


##Resources:
The following resources were really helpful while setting up QT Py RP2040 in Windows 11

**The RP2040 Datasheet**
https://datasheets.raspberrypi.com/rp2040-datasheet.pdf

**Getting Started with Pico Guide**
https://datasheets.raspberrypi.com/pico/getting-started-with-pico.pdf

**Installing** 
https://www.youtube.com/watch?v=mUF9xjDtFfY

##Introduction to RP2040
The Datasheet is a good way to gain more knowledge about RP2040 if it's new for you. 
RP2040 is a high-performance microcontroller device. which is affordable with a price range of 4$ (Raspberry pi 2040 Pico) and 9.95$ (Adafruit QTPy 2040). For this setup, we will be using the Adafruit QTPy 2040. 
You can check out the prices using the following links:
Adafruit QTPy 2040:  https://www.adafruit.com/product/4900?gclid=CjwKCAjwkaSaBhA4EiwALBgQaOmjnHcdEo4q9H4MoJQDE_jhDx9zxB4jheQuGPh3GJivzcsChdSn-RoCLWMQAvD_BwE
Raspberry pi 2040 Pico: https://www.seeedstudio.com/Raspberry-Pi-Pico-p-4832.html?gclid=CjwKCAjwkaSaBhA4EiwALBgQaOLM-ngyliXnJmNtwO_3_M5T1HyQ3RY6-jMKIX6E3jxdE7TcRvVEFBoCEPsQAvD_BwE

*Key features of RP2040 are listed below:*
• Dual ARM Cortex-M0+ @ 133MHz
• In six independent banks 264kB on-chip SRAM 
• DMA controller
• AHB crossbar Fully-connected 
• 30 GPIO pins, 4 of which have analog inputs
• peripherals for Interpolator and integer divider
• Support for up to 16MB of off-chip Flash memory via a dedicated QSPI bus
• To generate core voltage On-chip programmable LDO 
• To generate core clocks and USB, 2 on-chip PLLs
• Peripherals: I2C controllers **2**, UARTs **2**, PWM channels **16**, SPI controllers **2**, PIO state machines **8**

##Setup Steps:

###Step 1 :
Download all the required files. For that, I followed Chapter **9.2 Building on MS Windows** of the Getting started with Pico Guide.

##Step 2 :
Downloading and Installing all the Software. I referred to the above-mentioned youtube video in the resources for the same. 
            So for this, the steps are as follows:
             1. Install Arm GCC Compiler using the following link or the link given above under installed software 
                https://developer.arm.com/downloads/-/gnu-rm
                
                Just open it, select preferred language and then install. 
                
                Before clicking Finish Installation at the end. Make sure that th option is also selected as by default ususally it's not. 
                
                
    

##Quirks encountered:
I first tried to install WSL, I even referred to Arnav Ganfhu work. But I was getting an error while installing WSL. The first error I got while installing was This action requires elevation. That can be resolved by using Command Prompt at the administrative level. Then I got a new error. I followed a few links to try to resolve it like:               
But as I was not able to Install WSL, I decided to use Windows and VS Code instead. 


##Tips:
