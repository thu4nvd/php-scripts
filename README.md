# php-scripts
Example of running docker to test code ( for each folder inside).

```
docker run -p 80:80 -p 443:443 --name php-cms -v /home/thuanvd/projects/php-scripts/SimpleCMS:/var/www/html/ -d eboraas/apache-php
docker run -it -d --name mysql01 -v ~/data/mysql/mysql01:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=123456 mysql:latest
docker run --name myadmin -d --link mysql01:db -p 8080:80 phpmyadmin/phpmyadmin
```
