# php-scripts
Example of running docker to test code ( for each folder inside).

docker run -p 80:80 -p 443:443 --name php-cms -v /home/thuanvd/projects/php-scripts/SimpleCMS:/var/www/html/ -d eboraas/apache-php
