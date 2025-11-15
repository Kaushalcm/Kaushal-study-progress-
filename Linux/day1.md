Linux basics (----1----)

lesson 1  FUNDAMENTALS

:  Operating system  why operating system  mainly first we have hardware which is the physical components which consist of cpu or monitor ,
  mother board and are there two main aspects which needs communication with the hardware which are users such as us and apps which we give commands to the cpu we user interact with hardware to create file etc or even manage the resources of hardware , but both are not directly capable of interacting with the hardware to interact with the hardware we eiter need a graphic user interface or command line interface which is not given by the hardware soo we need operating system which helps in this process which it maintains
   - process management
   -  memory management
   - device management
   - network management

So if an app need to talk to a hardware it goes through the operating system then the system allocates the required hardware components to the program to make it run so thats the reason we need operating system
-----Software interact with the hardware through operating system -----

above the operating system the layer which helps interaction btwn apps and operating sytem are gui(Graphic user interface),cli(command line interface)  

For gui example is windows,cli is Linux

\\\\\\DEFINATION- INTERMEDIATE SOFTWARE LAYER WHICH ACTS AS BRIDGE BETWEEN THE SOFTWARE AND HARDWARE AND DOES ALL THE MANAGMENT  \\\\\\



: Structure of Linux and what does Linux kernel do !!!

Mainly the kernel does the most work such as memory,device,network,process management so most of the heavy lifting top of that there are some layers like system library or packages  on top of that there is the -----command line interface(SHELL) -----


: what is Linux distribution !!

as Linux is open source so many companies use the copy of the open source Linux they add more feature, commands or wrapper and provide as -----UBUNTU and REDHAT etc -----


: LINUX SETUP

---Install WSL its a subsystem just go to command shell and type wsl --install   and restart and then go to command line and type wsl and ubuntu will be running ---


: package manager

how to install application on Linux or packages this Linux distrubutors such as ubuntu add package managers to help u deploy dependency or upgrade to new version delete them such as python , java or maintain them  for ubuntu it is -----APT-----

first use the command \

apt update

then

apt install python3
