# PiHole-HoneyPot
Steps i took turning my single board cpu into a honeypot.
Raspberry Pi Honeypot Lab

Overview

This project documents the steps I used to turn a Raspberry Pi into a basic cybersecurity honeypot lab. The goal of this project was to learn more about Linux administration, network monitoring, SSH security, attacker behavior, and log analysis in a safe home-lab environment.

A honeypot is a decoy system designed to attract unauthorized access attempts so activity can be logged, reviewed, and studied. This project helped me better understand how exposed systems are targeted and how defenders can monitor suspicious behavior.

Lab Goals

* Configure a Raspberry Pi as a Linux-based honeypot
* Monitor unauthorized login attempts
* Capture SSH activity and authentication logs
* Review attacker patterns such as brute-force attempts
* Practice Linux command-line administration
* Build hands-on cybersecurity experience for SOC and IT support roles

Hardware and Software Used

* Raspberry Pi
* Raspberry Pi OS / Linux
* SSH
* Terminal / Bash
* Router with local network access
* Log files located in /var/log/
* Optional tools:
    * Cowrie
    * Fail2Ban
    * UFW firewall
    * tcpdump
    * journalctl

Project Steps

1. Installed Raspberry Pi OS

I started by installing Raspberry Pi OS onto a microSD card and booting the Raspberry Pi. After the initial setup, I updated the system packages.
sudo apt update
sudo apt upgrade -y

Enabled SSH Access

Next, I enabled SSH so I could remotely access the Raspberry Pi from another machine on my network.
sudo raspi-config

