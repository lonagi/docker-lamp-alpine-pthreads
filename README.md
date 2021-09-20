# docker-lamp-alpine-pthreads
Docker LAMP with PHP 7.3 ZTS using pthreads on Linux Alpine

### Install

Firstly install docker and exec next:

```sh
git clone https://github.com/lonagi/docker-lamp-alpine-pthreads
cd ./docker-lamp-alpine-pthreads
docker build -t docker-lamp-alpine-pthreads

```

### Run

```sh
docker run --name webserver-zts -p 80:80 -e MYSQL_ROOT_PASSWORD=password docker-lamp-alpine-pthreads

```

### phpmyadmin

URL - /phpmyadmin


### Copy files

```sh
docker cp /hostfile  (container_id):/(to_the_place_you_want_the_file_to_be)

```