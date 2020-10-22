---
title: "Home Lab - Part 1 - OS Install"
date: 2020-10-19T01:55:22+02:00
draft: true
description: "Building my personal home lab"
keywords: "lab, development, os, centos 8"
---

After setting up my workstation in a totally different way (building my own immutable OS in a GitHub based repository based on Fedora Silverblue 31)  which i will describe in another post it is time to setup a server based device development use-cases.

The first thing is to make a choice for an Operation System for this prototype of a home lab.

For this i have chosen to use CentOS 8.2 <sup>[1](#footnote1)</sup>, mostly because in daily life, i work with Red Hat based stuff. I have used Ubuntu and other Debian OS'es in the past but i keep comming back to Red Hat. I think because it was my first encounter (Red Hat 7.1 the old one with 10 floppy disks of data) with Linux in my student years.
Beside that the stuff i want to try out is als more in this corner. I could have chosen for Fedora as server OS because it has the latest features but i am afraid this can be to bleedy edgie.

## Feautures
- DNF is the default package manager though yum can also be used.
- Network configuration will be controlled by Network Manager (nmcli & nmtui) as network scripts are removed.
- Podman utility to manage containers
- Introduction of two new packages repositories: BaseOS and AppStream
- Cockpit available as default server management tool
- Wayland is the default display server (not going the use on this server system)
- Iptables are replaced by nftables
- Linux Kernel 4.18
- PHP 7.2, Python 3.6, Ansible 2.8, VIM 8.0 and Squid 4

## Prerequisites
- Download [CentOS-8.2.2004-x86_64-minimal.iso](http://linux.cs.uu.nl/centos/8.2.2004/isos/x86_64/CentOS-8.2.2004-x86_64-minimal.iso)
- Create a bootable instance of CentOS 8 USB drive. 

### Footnotes

<a name="footnote1">1</a>: CentOS is a free and open source operating system derived from the sources of Red Hat Enterprise Linux (RHEL). CentOS (Community Enterprise Operating System) is a community-supported distribution of Linux. 