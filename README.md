# Transistor-Tester-AVR-Compiled-files-On-Windows
WinAVR Alternative, Compile  files On Windows Windows Subsystem for Linux (Ubunti Jammy)

While I share how I compiled, Karl-Heinz Kübbeler (kubi48) TransistorTester 1.13k and also Markus Reschke (madires) ComponentTester 1.51m, You may explore diffrent way's. Please feel free to share your way's and perhaps better way's.


How I Compiled files On Windows 11 Windows Subsystem for Linux (Ubunti Jammy)

How to install Linux on Windows with WSL  https://learn.microsoft.com/en-us/windows/wsl/install

After Installing you can access you linux drive with Windows Explorer. I created short cuts on my desktop
example   \\wsl.localhost\Ubuntu-22.04\home\carl\New-GM328A\ComponentTester-1.51m

![GM328A_Programing_Setup](https://github.com/carl1961/New-GM328A/assets/3056821/3a151028-bf4d-4c7c-a00e-a6f73a3b285a)


I did all the code working in Windows Explorer and only used linux to run (make) 
One issues is, always refrech Windows Explorer to update the files before coping them to your firmware uploader. I used 
the latest AVRDUDESS which is called version AVRDUDESS 2.6 on theier web site. I have a compiled copy here on github.

https://github.com/ZakKemble/AVRDUDESS    


I greated a GitHub and uploaded the files needed all unpacked and ready.


Karl-Heinz Kübbeler (kubi48) TransistorTester 1.13k    and also  Markus Reschke (madires) ComponentTester 1.51m

https://github.com/kubi48/TransistorTester-source

https://www.mikrocontroller.net/articles/AVR_Transistortester

https://github.com/madires/Transistortester-Warehouse

https://www.eevblog.com/forum/testgear/$20-lcr-esr-transistor-checker-project/
Great Reading here

https://github.com/madires/Transistortester-Warehouse/blob/master/Documentation/English/FAQ.Feliciano.pdf

https://github.com/madires/Transistortester-Warehouse/blob/master/Documentation/English/Mini-FAQ.indman.pdf

https://github.com/madires/Transistortester-Warehouse/blob/master/Documentation/English/Clone-Comparison-Chart.pdf



# Setting up System

sudo apt-get update

sudo apt-get install build-essential pkg-config git libusb-1.0-0-dev

sudo apt-get update

sudo apt-get install binutils gcc-avr avr-libc uisp avrdude

