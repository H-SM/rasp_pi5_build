# rasp_pi5_build

This is a list of commandd that I used over to make a good build for the PI 5 (w/ docker, ssh, ros2) over *unbuntu server 24.04.1 (noble) 

[unbuntu noble](https://releases.ubuntu.com/noble/)

## basic updates 

```
sudo apt update
sudo apt upgrade
sudo apt-get update
sudo apt-get upgrade

sudo install network-manager curl ca-certificates
```

dont forget to setup wlan0 for wifi here is a tut - [tut](https://www.youtube.com/watch?v=s4ZDlV3tIuM)

## raspi config 

```
sudo apt update 

sudo apt install raspi-config

sudo raspi-config
```

## docker 

```
curl -sSL https://get.docker.com | sh

sudo usermod -aG docker $USER

logout

groups

docker run hello-world
```

more on docker with pi 5 - [here](https://pimylifeup.com/raspberry-pi-docker/)
## ssh 

```
sudo apt-get update
sudo apt-get install openssh-server
sudo ufw allow 22
# do the above on both the server and client

nmcli device show
```
here is how to setup your ssh over the rasp pi 5 - [refer](https://www.raspberrypi.com/documentation/computers/remote-access.html#connect-to-an-ssh-server)

## ROS2 - 

refer to get the unbuntu source for it - [refer](https://docs.ros.org/en/jazzy/Installation/Alternatives/Ubuntu-Development-Setup.html) 

You could even go for the deb version if you like. 

`Thats it hf with the raspberry PI 5 :D` 