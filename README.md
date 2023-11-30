# Self Hosted, self contained www.ascii-middle-finger.com ASCII Middle Finger

![Docker Pulls](https://img.shields.io/docker/pulls/modem7/middle-finger) 
![Docker Image Size (tag)](https://img.shields.io/docker/image-size/modem7/middle-finger/latest) 
[![Build Status](https://drone.modem7.com/api/badges/modem7/docker-middle-finger/status.svg)](https://drone.modem7.com/modem7/docker-middle-finger)
[![GitHub last commit](https://img.shields.io/github/last-commit/modem7/docker-middle-finger)](https://github.com/modem7/docker-middle-finger)

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/modem7)

Image is based on Nginx alpine, and all the content is local to the container.

# Container Screenshot
## Single
![image](https://user-images.githubusercontent.com/4349962/157274069-6196f5cc-6c34-4cd7-bde8-e401cc257607.png)

## Dual
![image](https://user-images.githubusercontent.com/4349962/157416791-353edbf9-99c5-4295-aff8-e7f26fd208c9.png)

# Breaking change
Due to changing the image to nginxinc/nginx-unprivileged, the ports have changed from `80` to `8080`. 
Please update your files accordingly. 

# Configuration

```bash
version: "2.4"

services:

  middlefinger:
    image: modem7/middle-finger:latest
    container_name: MiddleFinger
    ports:
      - 8080:8080
```

# Tags
| Tag | Description |
| :----: | --- |
| latest | Single middle finger version |
| dual | Single + Dual middle finger version |
