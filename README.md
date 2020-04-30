# Nginx server with Docker on your raspberry pi 3 

## First dowload Alpine Linux for armv7 or armhf
https://www.alpinelinux.org/downloads/

## Fast tutorial for instalation
https://pi3g.com/2018/10/24/alpine-linux-first-steps/

We have two docker-compose files in this repo. One is for nginx-proxy compatible with raspberrypi(arm) architecture.
The other file have a nginx-proxy for any pc.

Inside www folder put all your website files.

## How to
```
docker-compose <yourdockerfile.yml> up
```
