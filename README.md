# BerlussimoSetup
The setup repo for berlussimo project

## Install Instruction 

### Installation of Debian 
Install Debian 9 e.g. in VM

be sure network is enabled 

minimum 16GB HDD must be available


#### These instructions assume that you are running Debian 9. After completing these instructions
you will have a basic installation with database and webserver.

https://www.debian.org/distrib/

debian-9.3.0-amd64-netinstall.iso  

graphical (debian desktop environment) installed with default system tools 

#### login as root
su 

#### install git
apt install git --yes

#### Download setup script 
cd /var/tmp/; git clone https://github.com/Igel18/BerlussimoSetup berlussimo

#### change execution permissions 
cd /var/tmp/berlussimo/ 

chmod -x setup.sh 

#### execute script 
bash setup.sh

-> you will be asked 2 times to set and a password for sql: typ 'berlussimo' to have no changes 
"install and setup database berlussimo with user root and password berlussimo"

-> you will be asked 4 times for the sql password. allways type 'berlussimo' 
"setup database query for berlussimo" 

-> you will be asked for really want to do this command (yes/no) type 'yes' 

### you should now be able to open http://<your_server>/ in your browser and login with
login: admin@berlussimo

password: password
