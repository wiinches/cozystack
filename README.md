# CozyStack Installation Guide.
###### Disclaimer: CozyStack has been designed specifically for certain hardware sets. Meaning it was not meant to be a dynamic install, before you begin this installation please notice that within the provided scripts some  values will need to be assigned in order for this to work.

# Pre-Installation
Download RPM files needed to install needed services and dependencies.

Download Images: https://drive.google.com/open?id=0B2bFFRuLgR2JODNmLVhrdjQ0aDQ

Download Docker RPMs:
https://drive.google.com/drive/folders/0B2bFFRuLgR2JMWw2YWdzXzhueDg?usp=sharing

Download Extra RPMS:
https://drive.google.com/drive/folders/0B2bFFRuLgR2JWGc0dkRRaUlRRk0?usp=sharing

### Images
After downloading images from Google Drive move .docker files to "images" folder.

### Docker RPMs
After downloading docker RPMs from Google Drive move .rpm files to "docker" folder

### Extras
After downloading extra RPMs from Google Drive move .rpm files to "extras" folder.

# Install Guide

Copy "Application" folder to target server /tmp directory.
```
scp -r Application <username>@<serverIP>:/tmp/
```
ssh into target server.
```
ssh <username>@<serverIP>
```
Change Directory to /tmp/Application
```
cd /tmp/Application
```
Run Application server installation scripts
```
sudo bash ApplicationServer_deploy.sh
```

#### Post Installation

Verify docker images are running.
```
docker ps -a
```
