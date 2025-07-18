# Luci-App-Subconverter

## Based On

This project is based on the following open-source projects:

* [Subweb](https://github.com/stilleshan/subweb)
* [Subconverter](https://github.com/tindy2013/subconverter)

## Overview

A luci-app for subweb and subconverter on OpenWRT

# Screenshot

![subconverter](./img/subconverter.png)
![prefini](./img/prefini.png)
![subweb](./img/subweb.png)
## Features

* Supports amd64 and arm64 devices only
* Tested on official OpenWRT 23.0.5 and LEDE R23.4.1/R20.4.8, should be compatible with all amd64 and arm64 devices running OpenWRT

## System Requirements

* Disk space: approximately 8MB
* Memory: 512MB recommended, 256MB may be sufficient without other resource-intensive services

## Security Notice

**WARNING:** SUBCONVERTER AND SUBWEB HAVE NO PASSWORD PROTECTION. FOR SECURITY REASONS, DO NOT EXPOSE THEM TO THE PUBLIC INTERNET.
<br>

### To generate the `subconverter` binary  from trusted sources, follow the steps below:

[UPX 4.2.4](https://github.com/upx/upx/releases/download/v4.2.4/upx-4.2.4-win64.zip)
<br>
[Subconverter 0.9.0](https://github.com/tindy2013/subconverter/releases/download/v0.9.0/subconverter_aarch64.tar.gz)
```powershell
.\upx.exe -9 --lzma .\subconverter
```
If you still don't trust the provided binary file, you can compile your ipk with your own `subconverter` binary.
<br>

## Todo List

* ~Optimize disk usage further~
* Add password protection for enhanced security
* ~Implement configuration editing capabilities~
* ~Add crontab to schedule start and stop~
