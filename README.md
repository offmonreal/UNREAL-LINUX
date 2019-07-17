# UNREAL-LINUX

#ПУТЬ /etc/apt/sources.list  
deb http://deb.debian.org/debian/ stretch main contrib non-free  
deb-src http://deb.debian.org/debian/ stretch main contrib non-free  
deb http://deb.debian.org/debian/ stretch-updates main contrib non-free  
deb-src http://deb.debian.org/debian/ stretch-updates main contrib non-free  
deb http://security.debian.org/debian-security/ stretch/updates main contrib non-free  
deb-src http://security.debian.org/debian-security/ stretch/updates main contrib non-free  

#Начало
apt update  
apt upgrade  

#Система
apt-get install net-tools curl htop iftop sshfs cryptsetup p7zip-full p7zip-rar unrar nmap zip curl gettext apt-transport-https 

#Система PC  
apt-get install geany jmtpfs libunwind8 terminator xarchiver  

#Система PC драйвера (нужна перезагрузка) (список всех устройств lspci -nn)  
apt-get install firmware-linux-nonfree wireless-tools pulseaudio firmware-iwlwifi software-properties-common  

#Nvidia (нужна перезагрузка)  
apt install nvidia-driver  

#Разработка C++  
apt install git-all g++ gcc clang cmake gdb build-essential libssl-dev valgrind xterm md5deep  


#ОФФ ДОКИ  
https://docs.unrealengine.com/en-US/Platforms/Linux/BeginnerLinuxDeveloper/SettingUpAnUnrealWorkflow/index.html  

#Связать аккаунты  

#Скачать исхожники  
git clone https://github.com/EpicGames/UnrealEngine.git  

#Сборка  
./Setup.sh  
./GenerateProjectFiles.sh  
make  

#Запуск  
/home/maxim/ue/UnrealEngine/Engine/Binaries/Linux/UE4Editor  
