# docker-webmin-rpi
Docker container running Webmin on latest Ubuntu to arm64v8 architecture. For Raspberry Pi 3 and 4.

## Building the image
```
sudo git clone https://github.com/jpeant/docker-webmin-rpi.git
cd docker-webmin-rpi
sudo docker build -t jpeant/webmin .
```

## Running the container
```
docker run -d -p 10000:10000 jpeant/webmin
```

Log into webmin and manage your server
```
http://hostname.or.ip:10000
(root:password)
```

SSL has been switched off but can be switched back on by editing the Dockerfile.
