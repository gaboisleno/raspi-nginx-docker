# Nginx server with Docker on your raspberry pi 3 

## First dowload Alpine Linux for armv7 or armhf
https://www.alpinelinux.org/downloads/

## Fast tutorial for instalation
https://pi3g.com/2018/10/24/alpine-linux-first-steps/

Download from https://alpinelinux.org/downloads/ – look under the Raspberry Pi heading
We recommend to use the armhf build, not the aarch64 one. As of writing this the most recent Alpine release is 3.8.1.

Remember, the Raspberry Pi needs a FAT partition as the first partition to boot properly!

Copy the contents of the directory to the SD card’s FAT partition

Enable root login over SSH:
```nano /etc/ssh/sshd_config```
```PermitRootLogin yes```
```service sshd restart```

## Docker
We have two docker-compose files in this repo. One is for nginx-proxy compatible with raspberrypi(arm) architecture.
The other file have a nginx-proxy for any pc.

Inside www folder put all your website files.

## How to
```
docker-compose <yourdockerfile.yml> up
```
