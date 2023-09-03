# move_ubuntu
Move Ubuntu to another partition on the disk

1. Partition disk for /, /home and swap partitions. Program GParted.
2. Install the *Systemback* program. Repository and installation by link: https://github.com/BluewhaleRobot/systemback/tree/master
3. Copy existing partitions to new ones with Systemback
4. Boot from Ubuntu Live CD, delete old partitions (/, /home, and swap) of old Ubuntu, with the program GParted.
5. Install Boot Repair from PPA:
   
sudo add-apt-repository -y ppa:yannubuntu/boot-repair && sudo apt update && sudo apt install -y boot-repair && boot-repair

After installation, we will be greeted by a window with two items to choose from, as well as the “Advanced options” item: 

Recommended repair allows you to fix most of the most common boot problems.
6. Reboot
