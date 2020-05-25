# docker-Install-Script
this is the script that have worked for me always when trying to install docker on parrot security os 

# Steps to install docker 


```
$ git clone this repo
$ cd in docker-install-Script
$ sudo chmod +x DockerInstall.sh
$ sudo ./DockerInstall.sh
```

do not forget to run it as root to check after the system reboots if docker got installed fine
```
$ docker run hello-world
Hello from Docker!
```

# Steps for kali

just run this step by step or all at once and itll be good
```
sudo apt-get remove docker docker-engine docker.io
sudo apt-get update
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo apt-key fingerprint 0EBFCD88
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
xenial \
stable"

sudo apt-get update
sudo apt-get install docker-ce
sudo docker run hello-world
```
