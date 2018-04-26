# KiwiEntryTask

Entry task for the Kiwi Cloud Weekend.

Nginx server using SSL (with a self-signed certificate) runninig on a docker container.

## Requirements

Docker must be installed in order for this container to run, see [Install Docker](https://docs.docker.com/install/)

## Installation

Once you clone this repo, navigate into the main directory and create the container by running:
```
docker build -t docker-https .
```

For running the container make sure to map your local ports to the container ports:
```
docker run -p 443:443 -p 80:80 docker-https
```

## Credits

[Serve static files from docker via nginx - A basic example](https://www.linkedin.com/pulse/serve-static-files-from-docker-via-nginx-basic-example-arun-kumar/)

[Create A Local HTTPS Proxy Server](https://www.shanestillwell.com/2016/10/03/create-a-local-https-proxy-server/)

