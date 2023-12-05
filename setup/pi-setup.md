local instructions on the installations of raspbian

1:
* https://www.raspberrypi.com/software/
* download the Pi OS installer

* run the isntaller on the sd card

* use raspbain lite install.

* boot raspbian using the screen pi for now. i think the boot is entirely contained on the raspi

## 2: create new user
* `sudo adduser disco`
* prompt password
* add disco to the sudoers
* `sudo adduser disco sudo`

## 3: enable ssh, set the hostname
`sudo raspi-config`
3 Interfate Options
* P2 SSH
* enable
* agree and stuff

* `sudo hostname -b disco-pi`

## 4: ssh into machine.
* hook up ethernet wire to system.
* `ssh disco@disco-pi`
* prompt for password
* now you are in!!!

## 5: remove the default pi user
* `sudo deluser pi`

## update system software
* `sudo apt-get update`
* `sudo apt-get install -y docker vim python3-pip`


## 6: enable other login setup



## ?: more setup
* /etc/motd
* replace with the motd file in this directory
