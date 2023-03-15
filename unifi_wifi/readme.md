unifi_wifi
Shows how to use Unifi UAP-PRO devices to extend wifi coverage in your home

Features:
You can define multiple wifi hotspot names (devices will connect via either name)
Get solid wifi coverage all over large home

Check status:
	pi@rpi-unifi-server:~ $ sudo systemctl status unifi

This email address is not registered in your UniFi Network application. 
Please ask the owner to do so, if possible. Otherwise, you must factory-reset your devices and adopt them with a new Network application. 
For the best network management experience, we recommend hosting your system with a UniFi OS Console.
Cloud console: $30/month

https://account.ui.com/login


Release notes: https://community.ui.com/releases/UniFi-Network-Application-7-3-83/88f5ff3f-4c13-45e2-b57e-ad04b4140528
https://help.ui.com/hc/en-us/articles/220066768-UniFi-How-to-Install-and-Update-via-APT-on-Debian-or-Ubuntu
	sudo apt-mark hold openjdk-11-*
Debian/Ubuntu specific
    For Debian/Ubuntu users installing via our repo, please update your APT source (see HERE). https://help.ui.com/hc/en-us/articles/220066768-UniFi-How-to-Install-and-Update-via-APT-on-Debian-or-Ubuntu
    We support MongoDB 3.6 since 5.13.10, older UniFi Network Application versions only support up to MongoDB 3.4.



Unifi Controller setup on Raspberry PI 3 B+
                Alternate: Unifi Cloud key (device that you can buy running Unifi Controller software)
Connect:
                ssh pi@10.0.0.9
                ssh pi@rpi-unifi-server
Setup:
Unifi Controller Software: this is required to run on a computer on the network and provision and control the access points
Unifi AP AC Pro: These are the WIFI access points. We have 4 of them spread throughout the church. connect with POE ethernet cable
POE Injector: Device has AC power input, Ethernet input (from switch), POE output (to Unifi AP)
POE Switch: New 8 port switch to send POE to all Unifi AP units
Raspbian buster lite (server version of Raspbian). Flash with Balena Etcher to 16 GB SD card
Default login: pi, raspberry
sudo raspi-config
                localization - US Standard. EN-US, English (US)
                change password
                Network options - hostname: RPI-UNIFI-SERVER
                enable SSH access
                                sudo systemctl enable ssh
                reboot
sudo apt update, sudo apt upgrade
setup static IP
                sudo nano /etc/dhcpd.conf
 
 

Install Unifi software tutorial:
                https://pimylifeup.com/rasberry-pi-unifi/
                sudo apt install openjdk-8-jre-headless
                Setup RNG for entropy
                                sudo apt install rng-tools
                                sudo nano /etc/default/rng-tools
                                HRNGDEVICE=/dev/hwrng
                                sudo systemctl restart rng-tools
                Install Unifi
                                echo 'deb https://www.ui.com/downloads/unifi/debian stable ubiquiti' | sudo tee /etc/apt/sources.list.d/100-ubnt-unifi.list
                                sudo wget -O /etc/apt/trusted.gpg.d/unifi-repo.gpg https://dl.ui.com/unifi/unifi-repo.gpg
                                sudo apt update
                                sudo apt install unifi
 
Connect with browser:
                https://10.0.0.9:8443



