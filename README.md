# Jenkins deployment on Docker

This project designed to implement and test the strategy of automating deployment of Jenkins (on 2 nodes)


## Basic setup

Ensure /data/jenkins/ directory is created and has the correct permissions.

- If you are using vagrant, the directory should be owned by vagrant. If you are logged in to an Ubuntu EC2 instance, then the ubuntu user should own the directory.
- If it needs to be created:
    - Run `sudo mkdir /data`
    - Run `sudo mkdir /data/jenkins`
    - Run `sudo chown 1000 /data/jenkins`


## Building Jenkins image


```
docker build -t oleggorj/jenkins:[version]
```



---
