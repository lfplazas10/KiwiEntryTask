# KiwiEntryTask

Entry task for the Kiwi Cloud Weekend.

Nginx server using SSL (with a self-signed certificate) runninig on a docker container.

## Requirements

Docker must be installed in order for this container to run, see [Install Docker](https://docs.docker.com/install/)

## Installation

Clone the docker image:
```
docker pull lfplazas10/docker-https:v1
```
Run it with:
```
docker run -p 443:443 -p 80:80 lfplazas10/docker-https:v1
```

### Alternative:

Clone this repo, navigate into the main directory and create the image by running:
```
docker build -t docker-https .
```

For running the image make sure to map your local ports to the container ports:
```
docker run -p 443:443 -p 80:80 docker-https
```

You should be able to access the page by going to:
<http://localhost>

## Credits

[Serve static files from docker via nginx - A basic example](https://www.linkedin.com/pulse/serve-static-files-from-docker-via-nginx-basic-example-arun-kumar/)

[Create A Local HTTPS Proxy Server](https://www.shanestillwell.com/2016/10/03/create-a-local-https-proxy-server/)

[Blacktie themes](https://blacktie.co/)
