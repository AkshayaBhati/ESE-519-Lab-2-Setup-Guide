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
Git                            :    https://git-scm.com/download/win
CMake Software                 :    https://cmake.org/download/
Visual Studio Code             :    https://code.visualstudio.com/Download
Python 3                       :    https://www.python.org/downloads/windows/
The C++ build tools for VS     :    https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2019


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
                <img width="943" alt="1" src="https://user-images.githubusercontent.com/114259992/195955516-2d2c880b-1428-4400-812b-325c707c0276.png">
                Just open it, select preferred language and then install.
                <img width="371" alt="2" src="https://user-images.githubusercontent.com/114259992/195955618-06bc8ee8-8367-44e4-9a40-90870c4dcb44.png">
                Before clicking Finish Installation at the end. Make sure **Add Path to Environment Variables** option is also selected as by default ususally it's not. 
                <img width="373" alt="3" src="https://user-images.githubusercontent.com/114259992/195955586-e52447ce-ac57-4b60-8cbd-f27a397cc99c.png">

             2. Install Git using the following link or the link above
             
                <img width="791" alt="4" src="https://user-images.githubusercontent.com/114259992/195956083-44161144-1d06-4bf2-9e45-c487ac6508ff.png">
                
                Select where to Install Git, then change the deafault editor according to your preference. 
                
                <img width="362" alt="5" src="https://user-images.githubusercontent.com/114259992/195957404-a0967b3c-364a-41d6-99e4-a6e7e7d951ba.png">
                
                Then let Git decide the branch name for the inital branch in new repositories. Then choose the recommended option Git from the Command line and also 3rd party software. Then use all the default options like use the open SSL Library, Use MinTTY. Then use Checkout as-is, commit as-is option rather than the default so that no conversions are performed by Git while checking text files. 
                
                <img width="368" alt="6" src="https://user-images.githubusercontent.com/114259992/195957380-eb0608d4-d590-4c00-bd7b-d481172738ab.png">
                
                3. Install CMake 
 
    
##Quirks encountered:
I first tried to install WSL, I even referred to Arnav Ganfhu work. But I was getting an error while installing WSL. The first error I got while installing was This action requires elevation. That can be resolved by using Command Prompt at the administrative level. Then I got a new error. I followed a few links to try to resolve it like:               
But as I was not able to Install WSL, I decided to use Windows and VS Code instead. 


##Tips:
