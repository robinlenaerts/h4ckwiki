# PHP Coding Server
## Intoduction
This project is a first PoC of a Dockerized PHP coding server. It allows for in-browser editing of PHP files and directly watching it's changes on a web server.

## Usage
Install Docker on your server (obviously :D).

> Be aware that this project is made for the amd64 architecture by default.

Download the `docker-compose.yml` and `Dockerfile-php-apache` files.
Change the credentials in the `docker-compose.yml` file.
Execute `docker compose up -d` in the directory containing the downloaded files.
Now you can access the following resources via your web browser:
- <your server IP>:9443 -> Code Server web interface
- <your server IP>:9080 -> PHP enabled Apache web server
- <your server IP>:9081 -> PHPMyAdmin web interface
