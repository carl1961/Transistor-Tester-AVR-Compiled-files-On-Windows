# Transistor-Tester-AVR-Compiled-files-On-Windows
WinAVR Alternative, Compile  files On Windows Windows Subsystem for Linux (Ubunti Jammy)  WSL2

While I share how I compiled, Karl-Heinz Kübbeler (kubi48) TransistorTester 1.13k and also Markus Reschke (madires) ComponentTester 1.51m, You may explore diffrent way's. Please feel free to share your way's and perhaps better way's.


# How to Compiled files On Windows 11 (10) Windows Subsystem for Linux (Ubunti Jammy)

How to install Linux on Windows with WSL  https://learn.microsoft.com/en-us/windows/wsl/install

After Installing you can access you linux drive with Windows Explorer. 
to get your folder in Windows Explorer   Open Windows Explorer and in address bar Type or paste 

\\wsl.localhost\Ubuntu-22.04\home
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/3b2a1827-d8cf-433f-851a-733fb2520d7f)

Click on your user name.

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/5a1bf84c-d15b-402b-bbc3-c9f6c75c6f13)


I created short cuts on my desktop
example   \\wsl.localhost\Ubuntu-22.04\home\carl\New-GM328A\ComponentTester-1.51m

right click your desktop click NEW and select " Shortcut

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/e7c87e9a-068f-4432-bd3a-b28f6365504d)

and paste your folder path click ok. Now you can get fast access to work with the Files and folders without all the learning to do this on Ubunti Linux. 

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/1bb7b9e7-19a8-49ff-a55c-2c3ea5a75cdb)

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/e0560164-a69c-4572-a61e-43576e131704)


I did all the code working in Windows Explorer , coping the files and folders to \\wsl.localhost\Ubuntu-22.04\home\carl\New-GM328A\ and only used linux to run (make) 
One issues is, always refrech Windows Explorer to update the files before coping them to your firmware uploader.

![GM328A_Programing_Setup](https://github.com/carl1961/New-GM328A/assets/3056821/3a151028-bf4d-4c7c-a00e-a6f73a3b285a)

I used the latest AVRDUDESS which is called version AVRDUDESS 2.6 on theier web site. I have a compiled copy here on github.

https://github.com/ZakKemble/AVRDUDESS    

Download your files needed and unpack them , I use 7-zip  https://7-zip.org/


# Karl-Heinz Kübbeler (kubi48) TransistorTester (1.13k)   

https://github.com/kubi48/TransistorTester-source

https://www.mikrocontroller.net/articles/AVR_Transistortester


# Markus Reschke (madires) ComponentTester (1.51m)

https://github.com/madires/Transistortester-Warehouse

# Great Reading here

https://www.mikrocontroller.net/topic/transistortester-avr?page=1

https://www.eevblog.com/forum/testgear/$20-lcr-esr-transistor-checker-project/

https://github.com/madires/Transistortester-Warehouse/blob/master/Documentation/English/FAQ.Feliciano.pdf

https://github.com/madires/Transistortester-Warehouse/blob/master/Documentation/English/Mini-FAQ.indman.pdf

https://github.com/madires/Transistortester-Warehouse/blob/master/Documentation/English/Clone-Comparison-Chart.pdf



# Setting up System

In windows search in task bar type u and click on Ubuntu-22.04

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/87053217-ff29-4ee4-b4eb-002163035401)

You get the Ubuntu console 

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/bf2a6ced-b046-462f-831c-f17921575cbc)

What's great here is windows copy and paste works in your Ubuntu, so you cand copy and paste these comands and not have to type them all out.
so copy and paste these next comands. I already have installed all these so your screen will be diffrent, you will most likly need to press Y for YES to update and install files.


sudo apt-get update

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/8295bdc1-2002-4404-8dd3-ad4cf77e1996)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/da4e0c17-4b8c-4f47-8c2c-e0f2fbc035e0)

sudo apt-get install build-essential pkg-config git libusb-1.0-0-dev

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/1b2729be-5d2f-4ebf-889d-7331316fa614)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/8a06a3b8-4730-4033-9496-0ebb6f96565c)

# Installing AVR

sudo apt-get update

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/323f9bac-2d5c-4b11-8994-26da69f136e9)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/18c4e6a1-5e66-422a-a5fd-b3973760c9b3)


sudo apt-get install binutils gcc-avr avr-libc uisp avrdude


![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/22a2df0c-e2d2-426c-8bba-35b276cf2c46)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/620a637e-081d-4598-9bce-e2651e84b5bd)

# Downgrading AVR  
sudo apt-get purge gcc-avr

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/b4964c1d-ece2-4938-af6a-9e37f46d6518)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/48d34581-5e9c-4686-8c76-3d8186eabb69)

# gcc-avr 5.4.0

sudo apt-get install binutils gcc-avr 5.4.0

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/b0b4e24e-f323-4a33-9777-05d529904b94)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/419526eb-bb0b-4e5e-89d5-f602941e26a0)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/25cc9cf7-fddd-40a4-9b6a-842e219df3cd)

avr-gcc --version

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/9441051e-6252-41ea-bfa6-c48472c45df0)

sudo apt-get install binutils   avr-libc uisp avrdude


![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/b9f1dcf9-2d06-4c95-a428-d4942cbb6536)


# Compiling TransistorTester (1.13k)

From windows download Karl-Heinz Kübbeler (kubi48) TransistorTester files from  https://github.com/kubi48/TransistorTester-source

Click on Code and then Download Zip to your prefered folder.

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/19be4bf4-1d54-4ad0-8b34-e446846b5c94)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/02f65adf-dcd7-4551-ba93-c6b02d2cfb86)

Unzip (unpack) TransistorTester-source-master.zip I use 7-zip for tar files

You can double click  TransistorTester-source-master.zip to Unzip ZIP file with Windows or right click Zip file and move mouse pointer to 7-zip 
then to right to  Extrack to "TransistorTester-source-master\"  (win 10) with windows 11 you need to right click, select Show more options and 
then move mouse pointer to 7-zip then to right to  Extrack to "TransistorTester-source-master\"

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/0b067522-6c5b-4e0a-bff4-fde5cf80e32c)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/f1db04c6-1364-4564-866d-647aae0652b3)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/f727475b-84b1-482c-a5a9-8bf59f0c235a)

Go to Your unzipped TransistorTester-source-master folder then right click copy trunk folder to your Ubuntu home (username) folder 

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/b8dbc0a8-df33-4f3f-a929-a06e33e8d73a)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/874dc0f0-7c88-44a6-8029-4e29686bc6dc)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/42cb26fb-370e-4160-a940-8bebc041554c)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/1ea9c21f-c96a-4367-8829-ca753892d122)

go to your Ubuntu trunk folder (we or still using Windows Explorer)
make changes to your prefered Makefile  ( Do not mess with Makefile in trunk main folder , use the Makefile in prefered firmware folder 
ex: mega328_color_kit folder

I edit with Notepad++  https://notepad-plus-plus.org/

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/17b4c531-27e6-44ae-a4aa-cafe551fd01f)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/7d64623c-bbf4-497d-aa15-f2bf1545e11c)

After your done making your changes Go to your Ubuntu Command prompt , or Start Ubuntu 

copy paste this ( or type it out)

cd  ~/trunk/mega328_color_kit (or your prefered folder)

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/0b2dad27-4809-4bf4-bffd-40f1204f014f)


then type 

make  

![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/148654d4-e5f4-4fda-9905-1139cc86028c)
![image](https://github.com/carl1961/Transistor-Tester-AVR-Compiled-files-On-Windows/assets/3056821/f3957547-1e03-4812-8e14-9346173d76f4)


























