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


# RUN AFTER REBOOT (updated 2025-08-18)

---WINDOWS---

Via Docker CLI : docker run -it --rm --name windows -p 8006:8006 --device=/dev/kvm --device=/dev/net/tun --cap-add NET_ADMIN -v "${PWD:-.}/windows:/storage" --stop-timeout 120 dockurr/windows

Via Kubernetes : kubectl apply -f https://raw.githubusercontent.com/dockur/windows/refs/heads/master/kubernetes.yml

---Linux

Via Docker CLI : docker run -it --rm --name qemu -e "BOOT=alpine" -p 8006:8006 --device=/dev/kvm --device=/dev/net/tun --cap-add NET_ADMIN -v "${PWD:-.}/qemu:/storage" --stop-timeout 120 qemux/qemu

Via Kubernetes : kubectl apply -f https://raw.githubusercontent.com/qemus/qemu/refs/heads/master/kubernetes.yml

---MAC OS---

Via Docker CLI : docker run -it --rm --name macos -p 8006:8006 --device=/dev/kvm --device=/dev/net/tun --cap-add NET_ADMIN -v "${PWD:-.}/macos:/storage" --stop-timeout 120 dockurr/macos

Via Kubernetes : kubectl apply -f https://raw.githubusercontent.com/dockur/macos/refs/heads/master/kubernetes.yml


**replace the first 8006 with the specified ports.. **

Windows 7  : 10007

Windows 8e : 10008

Windows 10 : 10010

Windows 11 : 10011

Windows 2012 : 10012

Windows 2016 : 10016

Windows 2019 : 10019

Windows 2022 : 10022

Windows 2025 : 10025

MacOS 11 : 10511

MacOS 12 : 10512

MacOS 13 : 10513

MacOS 14 : 10514

MacOS 15 : 10515

Alma Linux : 10041

Alpine : 10042

CentOS : 10043

Debian : 10044

Fedora : 10045

Kali Linux : 10046

Linux Mint : 10047

Oracle Linux : 10048

Ubuntu : 10049

---Troubleshooting reboot---

1. If you get "docker: Error response from daemon: Conflict. The container name "/windows" is already in use by container "#container-name". You have to remove (or rename) that container to be able to reuse that name." copy the container name and do "docker run #container-name"

REPLACE "#container-name" with your containers real ID
