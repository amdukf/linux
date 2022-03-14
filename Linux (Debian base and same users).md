for problem in instalation of apps => sudo apt-get install ubuntu-restricted-extras
***
for problem in tor => sudo killall tor
***
man => for getting information about a command
***
for shutdown pc , => shutdown -p time
***
for see that what is our package instalation name for remove it
or something like that , we can use =>>> apt list --installed | grep -i appname
***
for remove (uninstall) an app , we can use =>>>>>>>>>> apt-get remove a (ubuntu)
***
Run the command below to generate a list of all processes whose name comprises 
of the word apt, you will get a list inclusive of all apt or apt-get 
processes by using ps and grep commands together with a pipeline. =>> ps -A | grep apt
***
win + tab => for showing apps and go to another app easily .
backspace + alt => for speedup for erasing texts in terminal.
***
for deleting some files with each other in terminal , we should use rm filename*   ( for example we have 7 files that they first name is rapt , we type rm rapt* 
***
for recording screen , we use ctrl + alt + shift + R
for finishing the recording screen , we use that keys again
***
for solving wifi problem that doesnt work after using wifite , we can use => sudo airmon-ng stop wlp3s0 (wifi interface)
***
for showing the wifi interface , we should type => airmon-ng
***
for changing user password , we type => sudo passwd username that user
***
if we type (| less ) after any orders , it showd that order page by page in terminal.
for example , cat cpuinfo | less
***
when touchpad doesnt working , type =>
sudo rmmod psmouse
sudo modprobe psmouse proto=imps
***
for checking battery life and health , we can use 
/sys/class/power_supply/BAT0/
***
For this error on every distros , ( sudo rm /var/lib/apt/lists/lock ) , we should type 
sudo rm /var/cache/apt/archives/lock
sudo rm /var/lib/dpkg/lock
sudo dpkg --configure -a
***
for get out of base envirnment in anaconda , type
conda config --set auto_activate_base False
source ~/.bashrc
for getting in base mode =>
conda config --set auto_activate_base True
source ~/.bashrc
***
we can see Name of the distro that we using by => lsb_release -a
***
If we see that ifconfig command isnt working we have to install this package => net-tools
***
for install aps that have tar.xz in them , we should first 
tar xf file
./install that file
***
If we wanna to shutdown the bell of the terminal , we should uncomment "set the bell-style none" in /etc/inputrc
***
sudo apt install make cpp perl => for virtual machine
***