# Indroduction

The Automatic Windows/Linux Installer is made for Windows 11 and all of the Debian Linux based OS

To set it up, select your OS's Folder

(RUQUIRES LINUX MINT, DEBIAN, UBUNTU, DOZIANOS, OR WINDOWS 11)

------------------------Windows 11

Install Docker Desktop 

Open Command prompt (in your OS's folder)

Run "docker compose up -d"

-----------------------Debian Linux 

sudo su

sudo apt update -y && sudo apt upgrade -y

sudo apt install docker.io docker-compose

mkdir dockercom

cd dockercom

vim docker-compose.yml

-Copy your code from your yml file

----------------------Debian Online

sudo su

sudo apt update -y && sudo apt upgrade -y

cd ~

mkdir dockercom

cd dockercom

wget https://github.com/joshuadjteam/Automatic-Windows-Docker-Installer/releases/download/Docker/AutoDocker.zip

unzip AutoDocker.zip

apt install docker.io

apt install docker.io docker-compose

cd AutoDocker

sudo apt-get install python3-pip

python3 -m pip install setuptools --break-system-packages

##### If your OS has a space, do start it with a ' and end it with a '

docker-compose -f docker-compose.yml up -d

##### Now enjoy, access your VM by the port, read readme.txt in the zip file for the ports

----------------------Access Your VM

Read README for ports
