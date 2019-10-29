# lnmp
lnmp docker-compose.yml
1. docker, docker-compose required
2. create custom net app_net with command `docker network create app_net`
3. create runtime dir `../lnmp_runtime/mysql-data`  `../lnmp_runtime/logs/php-fpm`  `../lnmp_runtime/logs/nginx`
4. create code dir `../www`   
3. use command `docker-compose up` to start all containers
