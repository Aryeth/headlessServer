# Headless rpi webserver / website hosting at home

## Note that this guide is currently in the writings :neckbeard:

This repo pretty much explains how to create a web hosting server on a raspberry pi, using swisscom's dynamic DNS (DDNS) config, and an Infomaniak domain.
This guide is divided in 5 parts :
Note that this guide is currently in the writings :neckbeard:
  - [Configurating rpi and ssh](#configurating-rpi-and-ssh)
  - [Apache installation](#apache-installation)
  - [Your first webpage](#your-first-webpage)
  - [Opening your ports](#opening-your-ports)
  - [Swisscom's DDNS config](#swisscoms-ddns-config)

Enjoy the guide !

## Configurating rpi and ssh
---
First things first : we're going to need to set up your raspberry pi.
For this build, I used raspberry pi's imager that you can find on their [website](https://www.raspberrypi.com/software/).
I used for this project the Lite 32-bit OS, because I do not feel that there is a need for any GUI when using the computer in a headless mode.
Using the imager, you can already define a ssh username and password in the advanced options:
![advanced options of the raspberry pi imager, showing the ssh parameter](assets/images/sshImager.png)
You can also modify the Wifi settings there, but I prefer using direct ethernet connection.
You now should be able to ssh into your machine when you will connect it to the ethernet cable and power it up.
To find the raspberry pi ip, you can use [nmap](https://nmap.org/). This [tutorial](https://vitux.com/find-devices-connected-to-your-network-with-nmap/) can help you if you never used this tool too.
![Nmap scan report showing the raspberry pi ip (hidden by a red rectangle)](assets/images/terminal.png)
The output should look something like this, and your ip should be where the red rectangle is.
To now (finally) ssh into your soon-to-be server, you will need to type in your terminal (using linux here, follow [this](https://jarrodstech.net/how-to-raspberry-pi-ssh-on-windows-10/) for windows) : `ssh [your username]@[raspberry ip]`. You will then be asked for your password, and you should be able to login to something that looks like this :
![raspberry pi login prompt and welcome message](assets/images/connected.png)
Congratz ! You're now connected onto your headless raspberry pi :)
## Apache installation


## Your first webpage
To put up your first webpage on your website, you can use this [example page](assets/examplePage.html), or feel free to create your own.
## Opening your ports

## Swisscom's DDNS config
