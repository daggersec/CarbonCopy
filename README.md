# CarbonCopy
A tool which creates a spoofed certificate of any online website and signs an Executable for AV Evasion. Works for both Windows and Linux

![Screenshot](Usage.jpg)

## Prerequisites

In order to use it on Linux, please execute commands below:
```shell
apt-get install osslsigncode
pip3 install pyopenssl
```

Windows will also require signtool.exe installed. Included in the zip file.
Alternatively install directly from MS:

---begin signtool install---
1. Download the .iso file from https://developer.microsoft.com/en-us/windows/downloads/windows-10-sdk (current download link is 
http://go.microsoft.com/fwlink/p/?LinkID=2022797) The .exe download will not work, since it's an online installer that pulls down its dependencies at runtime.
2. Unpack the .iso with a tool such as 7-zip.
3. Install the Installers/Windows SDK Signing Tools-x86_en-us.msi file - it's only 388 KiB large. For reference, it pulls in its files from the following .cab files, so these are also needed for a standalone install:
    3.1 4c3ef4b2b1dc72149f979f4243d2accf.cab (339 KiB)
    3.2 685f3d4691f444bc382762d603a99afc.cab (1002 KiB)
    3.3 e5c4b31ff9997ac5603f4f28cd7df602.cab (389 KiB)
    3.4 e98fa5eb5fee6ce17a7a69d585870b7c.cab (1.2 MiB)
4. You will now have the signtool.exe file and companions in C:\Program Files (x86)\Windows Kits\10\bin\10.0.17763.0\x64 (replace x64 with x86, arm or arm64 if you need it for another CPU architecture.)
---end signtool install---
