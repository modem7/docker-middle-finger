# Self Hosted, self contained www.ascii-middle-finger.com ASCII Middle Finger

![Docker Pulls](https://img.shields.io/docker/pulls/modem7/middle-finger) 
![Docker Image Size (tag)](https://img.shields.io/docker/image-size/modem7/middle-finger/latest) 
[![Build Status](https://drone.modem7.com/api/badges/modem7/docker-middle-finger/status.svg)](https://drone.modem7.com/modem7/docker-middle-finger)
[![GitHub last commit](https://img.shields.io/github/last-commit/modem7/docker-middle-finger)](https://github.com/modem7/docker-middle-finger)

Image is based on Nginx alpine, and all the content is local to the container.

# Container Screenshot
## Single
![image](https://user-images.githubusercontent.com/4349962/157274069-6196f5cc-6c34-4cd7-bde8-e401cc257607.png)

## Dual
![image](https://user-images.githubusercontent.com/4349962/157303682-41cd407b-3160-4517-aa60-a112bc95b895.png)

# Configuration

```bash
version: "2.4"

services:

  middlefinger:
    image: modem7/middle-finger:latest
    container_name: MiddleFinger
    ports:
      - 80:80
```

# Tags
| Tag | Description |
| :----: | --- |
| latest | Single middle finger version |
| dual | Single + Dual middle finger version |
