
Linux basic (----2----)

: now you have installed Linux(UBUNTU) or using docker on your windows or mac to use Linux


\\\\\\FOLDER STRUCTURE \\\\\\\\  all the main folders in Linux and why we use them

root@ubuntu-dev:/# what does this mean

the user is the root it can be changed and only the root user is the administrative user and for other user some access are denied vice versa
Linux basic (----2----)

: now you have installed Linux(UBUNTU) or using docker on your windows or mac to use Linux


\\\\\\FOLDER STRUCTURE \\\\\\\\  all the main folders in Linux and why we use them

root@ubuntu-dev:/# what does this mean

the user is the root it can be changed and only the root user is the administrative user and for other user some access are denied vice versa

ubuntu is a host name which doesn't matter a lot only matters if you maintaining a lot of systems

/ is the path your currently in which is very important
       ---   a file system where a file needs to be created and for that to be created it need storage and the default path or  storage location is the /  you can create any number of folder               and file in that root path
       ---  if for example you have kaushal@ubuntu:~  the ~ is the home which is mainly /home/Kaushal which is the home directory which is mainly inside the root path which we discussed before which is the / when the user is root this comes by default when you create a user


: ls -ltr

  ---  ls is basically a list command  and the ls -ltr lists all the folder and file in that directory

\\\\\\ mainly the question is how does Linux know that ls is for list and mkdir is for making a new folder in the ls -ltr which shows all the files and folder in a folder there is a package which we have learnt last chapter which is already pre installed some times which makes the Linux understand that the command we type in the command line  interface which are setup in the Linux environment so as we read the layer of Linux it has system libraries and system utilities above kernel those are presen in the ls -ltr which are already predefined  

---if you using on virtual machine you need to type sudo su- to get into root user so you can access the ls -ltr

: FIRST FOLDER sbin (System binaries)
   -----binary files for administrative command  used to manage the system like example useradd this command helps in creating a user


:SECOOND FOLDER lib (Library)
   -----  these library as used by Linux kernel we dont use them kernel use it basically to make system calls with hardware


:THRID FOLDER boot
  -----  basically for booting/restarting Linux the machine it contains the folder which basically helps for restarting the Linux os such as commands or actions

: FOURTH FODLER BIN
 -----   sbin is for system binaries and bin is basically for user binaries this command access can be done for regular users aswell where as sbin is mainly allowed for the admin(root)so anybody has access  

:FIFTH FOLDER user
----- so mainly user directory has folder which consist of the folder such as sbin , bin lib etc as sbin is (user/sbin), bin (user/bin) where shortcuts are created for all of them

:SIXTh FOLDER srv(Server)
----- you can store important files and stuff on this folder so it can be used on the webserver and by default whichever you save normally goes into srv by default its empty

:SEVENTH FOLDER opt
----very important folder when you join a organization or a team you want to install a third party dependency like example a particular version of java we will use that folder called opt
opening opt using cd opt you create a folder such as mkdir custom-tools etc and place them inside and this is a common location for all the third party dependency you use this so the whole organization can use this directory and they dont need any authorization for opening and stuff (Mainly a common location) which is a common practice in Linux


:EIGHT FOLDER mount
----system administrator basically has task such as adding storage they should get the disk and temporarily add mount later we will read for disk management mainly to mount new volumes or disk

:NINTH folder media
----- just for adding files and stuff so such as mp4,mp3 etc

:TENTH FOLDER var
----- this folder is mainly used to store logfiles ,some library mainly for logfiles

so for example we install a webserver such as apache or http the logs of this server might log into the /var/log folder

:ELEVEN FOLDER Home
----is just a basic direct we normally add user etc it is self explanatory

:TWELVE folder data
----basically for storing data and we need to share that data you add that in data and you can restrict based on access

:You have a set of folder which have volatile files and folder basically not permanent such as proc(virtual file system),dev,sys  we will learn when we study script they are just temporary folder for now and tmp (temporary) every Linux has a time system which it deletes the temp directory every time in a set period of time


:FOLDER root


:FOLDER test basically a test folder


:FOLDER run
----- run basically stores the run time data of the processes if any runtime data is there it is stored in run directory


:FOLDER ETC (MOST IMP)
-----  it has many system configuration file its like the c folder in windows mainly the files in etc we can use to modify and configure our system



Something called as path on the Linux this will tells the Linux when somebody write something on the command it basically check in all the folder within that path

ubuntu is a host name which doesn't matter a lot only matters if you maintaining a lot of systems

/ is the path your currently in which is very important
       ---   a file system where a file needs to be created and for that to be created it need storage and the default path or  storage location is the /  you can create any number of folder               and file in that root path
       ---  if for example you have kaushal@ubuntu:~  the ~ is the home which is mainly /home/Kaushal which is the home directory which is mainly inside the root path which we discussed before which is the / when the user is root this comes by default when you create a user


: ls -ltr

  ---  ls is basically a list command  and the ls -ltr lists all the folder and file in that directory

\\\\\\ mainly the question is how does Linux know that ls is for list and mkdir is for making a new folder in the ls -ltr which shows all the files and folder in a folder there is a package which we have learnt last chapter which is already pre installed some times which makes the Linux understand that the command we type in the command line  interface which are setup in the Linux environment so as we read the layer of Linux it has system libraries and system utilities above kernel those are presen in the ls -ltr which are already predefined  

---if you using on virtual machine you need to type sudo su- to get into root user so you can access the ls -ltr

: FIRST FOLDER sbin (System binaries)
   -----binary files for administrative command  used to manage the system like example useradd this command helps in creating a user


:SECOOND FOLDER lib (Library)
   -----  these library as used by Linux kernel we dont use them kernel use it basically to make system calls with hardware


:THRID FOLDER boot
  -----  basically for booting/restarting Linux the machine it contains the folder which basically helps for restarting the Linux os such as commands or actions

: FOURTH FODLER BIN
 -----   sbin is for system binaries and bin is basically for user binaries this command access can be done for regular users aswell where as sbin is mainly allowed for the admin(root)so anybody has access  

:FIFTH FOLDER user
----- so mainly user directory has folder which consist of the folder such as sbin , bin lib etc as sbin is (user/sbin), bin (user/bin) where shortcuts are created for all of them

:SIXTh FOLDER srv(Server)
----- you can store important files and stuff on this folder so it can be used on the webserver and by default whichever you save normally goes into srv by default its empty

:SEVENTH FOLDER opt
----very important folder when you join a organization or a team you want to install a third party dependency like example a particular version of java we will use that folder called opt
opening opt using cd opt you create a folder such as mkdir custom-tools etc and place them inside and this is a common location for all the third party dependency you use this so the whole organization can use this directory and they dont need any authorization for opening and stuff (Mainly a common location) which is a common practice in Linux


:EIGHT FOLDER mount
----system administrator basically has task such as adding storage they should get the disk and temporarily add mount later we will read for disk management mainly to mount new volumes or disk

:NINTH folder media
----- just for adding files and stuff so such as mp4,mp3 etc

:TENTH FOLDER var
----- this folder is mainly used to store logfiles ,some library mainly for logfiles

so for example we install a webserver such as apache or http the logs of this server might log into the /var/log folder

:ELEVEN FOLDER Home
----is just a basic direct we normally add user etc it is self explanatory

:TWELVE folder data
----basically for storing data and we need to share that data you add that in data and you can restrict based on access

:You have a set of folder which have volatile files and folder basically not permanent such as proc(virtual file system),dev,sys  we will learn when we study script they are just temporary folder for now and tmp (temporary) every Linux has a time system which it deletes the temp directory every time in a set period of time


:FOLDER root


:FOLDER test basically a test folder


:FOLDER run
----- run basically stores the run time data of the processes if any runtime data is there it is stored in run directory


:FOLDER ETC (MOST IMP)
-----  it has many system configuration file its like the c folder in windows mainly the files in etc we can use to modify and configure our system



Something called as path on the Linux this will tells the Linux when somebody write something on the command it basically check in all the folder within that path
