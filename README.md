# Freeboard in a container
* Added freeboard-mqtt plugin
* Alpine Linux with nginx, so it's teeeeny!

[![Microbadger](https://images.microbadger.com/badges/image/akbennett/freeboard-docker.svg)](http://microbadger.com/images/akbennett/freeboard-docker "Image size")
[![Docker Stars](https://img.shields.io/docker/stars/akbennett/freeboard-docker.svg?maxAge=86400)](https://hub.docker.com/r/akbennett/freeboard-docker/)
[![Docker Pulls](https://img.shields.io/docker/pulls/akbennett/freeboard-docker.svg?maxAge=86400)](https://hub.docker.com/r/akbennett/freeboard-docker/)


### How to use this image with default widgets

```
docker run --name myfreeboard -p 8081:80 -v $PWD/dashboard-private.json:/usr/share/nginx/html/dashboard.json -d freeboard
```

This will expose an installation of Freeboard and load the dashboard.json http://localhost:8081/?load=dashboard.json

*If you didn't modify dashboard.json to point to your devices and your cloudmqtt credentials you can modify these using the dashboard*

### Configure Cloudmqtt server datasource(s)
![Datasource](/datasource.png)

### Configure widgets
![Widget](/widget.png)

### View widgets
![Dashboard](/dashboard.png)
