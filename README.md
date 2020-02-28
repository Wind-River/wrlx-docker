# Overview

A small docker image built from [Wind River Linux LTS18](https://github.com/WindRiver-Labs/wrlinux-x), it is based on glibc and busybox, can be expanded by package manager opkg. It supports a lot of most commonly used packages, such as mariadb, apache2, gcc and so on. And busybox can be replaced by related tools easily.

# Project License

GPL-2.0

# Prerequisite

## External dependencies

docker

## Other Prerequisites

None

# Installation

Use like you would any other base image

```dockerfile
FROM %%IMAGE%%:10.18.0011
RUN opkg update
RUN opkg install python3-django
```

This example has a virtual image size of 92.6MB.

# Legal Notices

All product names, logos, and brands are property of their respective owners. All company, product and service names used in this software are for identification purposes only. Wind River is a registered trademark of Wind River Systems, Inc. Linux is a registered trademark owned by Linus Torvalds.

Disclaimer of Warranty / No Support: Wind River does not provide support and maintenance services for this software, under Wind River's standard Software Support and Maintenance Agreement or otherwise. Unless required by applicable law, Wind River provides the software (and each contributor provides its contribution) on an "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, either express or implied, including, without limitation, any warranties of TITLE, NONINFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the software and assume any risks associated with your exercise of permissions under the license.
