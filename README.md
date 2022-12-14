# ESE-519-Lab-2-Setup-Guide
 **We will set up our Laptop/PC for Adafruit QT Py 2040 using the official C/C++ SDK. Afterward, we will compile and run example code like "Hello World"**
## Machine Details
#### OS: Windows
#### OS Version: Windows 11 64-bit (x64-based Processor) 
#### Processor: 11th Gen Intel(R) Core(TM) i5-1135G7 @ 2.40GHz   2.42 GHz
#### Laptop Model: HP Pavilion Laptop 14-dv0xxx 

## Installed Software List:

Arm GCC Compiler              :    https://developer.arm.com/downloads/-/gnu-rm/  <br>
Git                           :    https://git-scm.com/download/win/ <br >
CMake Software                :    https://cmake.org/download/ <br >
Visual Studio Code            :    https://code.visualstudio.com/Download/ <br >
Python 3                      :    https://www.python.org/downloads/windows/ <br >
The C++ build tools for VS    :    https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2019 <br />
Putty                         :    https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html <br />
C/C++ MinGW Compiler          :    https://www.mingw-w64.org/downloads/ <br>


## Resources:
The following resources were really helpful while setting up QT Py RP2040 in Windows 11

**The RP2040 Datasheet**
https://datasheets.raspberrypi.com/rp2040-datasheet.pdf

**Getting Started with Pico Guide**
https://datasheets.raspberrypi.com/pico/getting-started-with-pico.pdf

**pico-examples Repository**
https://github.com/raspberrypi/pico-examples

**pico-sdk Repository**
https://github.com/raspberrypi/pico-sdk

## Introduction to RP2040
The Datasheet is a good way to gain more knowledge about RP2040 if it's new for you. <br> 
RP2040 is a high-performance microcontroller device. which is affordable with a price range of 4$ (Raspberry pi 2040 Pico) and 9.95$ (Adafruit QT Py 2040). For this setup, we will be using the Adafruit QT Py 2040. <br>

You can check out the prices using the following links:

Adafruit QTPy 2040:  https://www.adafruit.com/product/4900?gclid=CjwKCAjwkaSaBhA4EiwALBgQaOmjnHcdEo4q9H4MoJQDE_jhDx9zxB4jheQuGPh3GJivzcsChdSn-RoCLWMQAvD_BwE <br>

Raspberry pi 2040 Pico: https://www.seeedstudio.com/Raspberry-Pi-Pico-p-4832.html?gclid=CjwKCAjwkaSaBhA4EiwALBgQaOLM-ngyliXnJmNtwO_3_M5T1HyQ3RY6-jMKIX6E3jxdE7TcRvVEFBoCEPsQAvD_BwE <br>

*Key features of RP2040 are listed below:* <br>

??? Dual ARM Cortex-M0+ @ 133MHz <br>
??? In six independent banks 264kB on-chip SRAM <br>
??? DMA controller <br>
??? AHB crossbar Fully-connected <br> 
??? 30 GPIO pins, 4 of which have analog inputs <br>
??? peripherals for Interpolator and integer divider <br>
??? Support for up to 16MB of off-chip Flash memory via a dedicated QSPI bus <br>
??? To generate core voltage On-chip programmable LDO <br>
??? To generate core clocks and USB, 2 on-chip PLLs <br>
??? Peripherals: I2C controllers **2**, UARTs **2**, PWM channels **16**, SPI controllers **2**, PIO state machines **8** <br>

## Setup Steps:

### Step 1 :
Downloading and Installing all the Software. For that, I referred to Chapter **9.2 Building on MS Windows** of the Getting started with Pico Guide available in the resources. 
So for this, the steps are as follows: 
  1. Install Arm GCC Compiler using the following link or the link given above under installed software <br>
     https://developer.arm.com/downloads/-/gnu-rm <br>
  
     Just open it, select your preferred language, and then install it.<br>
                
      <img width="371" alt="2" src="https://user-images.githubusercontent.com/114259992/195955618-06bc8ee8-8367-44e4-9a40-90870c4dcb44.png">
                
     Before clicking Finish Installation at the end. Make sure the **Add Path to Environment Variables** option is also selected by default usually it's not.<br>
                
      <img width="373" alt="3" src="https://user-images.githubusercontent.com/114259992/195955586-e52447ce-ac57-4b60-8cbd-f27a397cc99c.png">
                
  2. Install Git using the following link or the link above <br>
                   
     Select where to Install Git, then change the default editor according to your preference. 
                
      <img width="362" alt="5" src="https://user-images.githubusercontent.com/114259992/195957404-a0967b3c-364a-41d6-99e4-a6e7e7d951ba.png">
                
     Then let Git decide the branch name for the initial branch in new repositories. Then choose the recommended option Git from the Command line and also 3rd party software. Then use all the default options like use the open SSL Library, Use MinTTY. Then use the Checkout as-is, commit as-is option rather than the default so that no conversions are performed by Git while checking text files. <br> 
                
      <img width="368" alt="6" src="https://user-images.githubusercontent.com/114259992/195957380-eb0608d4-d590-4c00-bd7b-d481172738ab.png">
                
  3. Install CMake <br>
                 
     Add CMake for the system path for all users rest let it be the same as the default. <br>
                
      <img width="380" alt="8" src="https://user-images.githubusercontent.com/114259992/195958057-5ce84d2e-6571-43d9-8132-3ee02e4f0c6a.png">
                
  4. Install Visual Studio Code if you don't already have it <br>
                
  5. Install Python 3 by downloading the python installer <br>
                  
     Select the option **Add Python 3.11 to PATH** <br>
                  
      <img width="486" alt="11" src="https://user-images.githubusercontent.com/114259992/195958775-395a66c5-fa0a-4217-b483-d49facc1c0e6.png">
                  
  6. Install The C++ build tools for VS <br>
  
     Scroll to the bottom to find the option to download it. <br>
      
      <img width="899" alt="13" src="https://user-images.githubusercontent.com/114259992/195959258-5fcddf71-0b2f-44c5-8755-471552083a9b.png">
                  
     Select the C++ Build tools option while installing and then install it. <br>
                  
      <img width="704" alt="14" src="https://user-images.githubusercontent.com/114259992/195959346-98425072-0fc0-4b43-8b55-ba36edaa858c.png">

  7. Install Putty from this site as given in the link above. <br>
                  
      <img width="940" alt="12" src="https://user-images.githubusercontent.com/114259992/195959013-a8bc813d-14e1-4b03-adef-31cd21d1e857.png">
  
  8. Install C/C++ MinGW Compiler using the link given in the resources

### Step 2 :

Now we have to clone the pico-sdk and the pico-examples git respositories as given in the resources.<br>
To do that we will perform the following instructions in command prompt: <br>
1. We will create a folder named pico using **mkdir pico**
2. Then we will clone the pico-sdk Repository in this pico folder.

``` 
    mkdir pico  
    cd pico 
    git clone -b master https://github.com/raspberrypi/pico-sdk.git
    cd pico-sdk
    git submodule update --init
```
3. Then we will clone pico-examples Repository

```
    cd .. 
    git clone -b master https://github.com/raspberrypi/pico-examples.git
```

### Step 3: built the Hello World file

 1. In windows path we will add PICO_SDK_PATH. To do so we need to search Edit Environmental Variables. Then we will **add the path** as given below:
    
  <img width="435" alt="15" src="https://user-images.githubusercontent.com/114259992/195966047-96fa4f21-cc43-4e7d-a37e-f158abcb682b.png">
  
 2. We will use the following command to generate CMake Files 

```
     cd pico-examples
     mkdir build
     cd build
     cmake .. -G 'MinGW Makefiles'
```
 3. Now we will build hello_world to get a .uf2 file 
```
     cd hello_world/usb
     mingw32-make -j6
```

### Step 4: Run in PuTTY

1. After step 3, a .uf2 file will be created. We need to drag the .uf2 file in the RP2040 folder called **RP1-RP2 (E:)** <br>
2. Open device manager to check the Port, if the **Ports** option is not available. Go to **view** and then **show hidden devices**.<br>
3. Check the port, here it's **COM7** <br>

  <img width="571" alt="device manager" src="https://user-images.githubusercontent.com/114259992/195964556-fe7a210d-5fac-459d-a794-307248509ee9.png"> <br>
  
3. Now we will run the code through PuTTY so that we can see the output in the terminal. So we need to change the serial line according to our device manager. Here it's **COM7** <br>

  <img width="334" alt="putty" src="https://user-images.githubusercontent.com/114259992/195964959-4f2b02ab-8ae7-4b5a-b133-01005ae7f6c4.png">

5. You can see the output **Hello World** as follows:  <br>
    
  <img width="494" alt="Hello World" src="https://user-images.githubusercontent.com/114259992/195965076-a76f2aa2-6450-43cf-82bb-2f2554ea2c1e.png">

### Quirks encountered:
I first tried to install WSL. But I was getting the following error while installing WSL

```
Installing: Virtual Machine Platform
An unrecoverable error occurred during installation. Component: 'Virtual Machine Platform' Error Code: 0x80073701
The referenced assembly could not be found.
```

### Tips:
I would recommend using Windows and VS code. 
