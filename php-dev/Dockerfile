FROM centos:7

RUN ["rpm", "-ivh", "http://dl.fedoraproject.org/pub/epel/7/x86_64/e/epel-release-7-9.noarch.rpm"]
#RUN ["rpm", "-ivh", "epel-release-7-9.noarch.rpm"]
RUN ["yum", "-y", "update", "epel-release"]

RUN ["rpm", "--import", "http://rpms.famillecollet.com/RPM-GPG-KEY-remi"]
RUN ["rpm",  "-ivh", "http://rpms.famillecollet.com/enterprise/remi-release-7.rpm"]
RUN ["yum", "-y", "update", "remi-release"]

RUN ["yum", "-y", "--enablerepo=remi-php71epel"]
RUN ["yum", "-y", "install", "php-fpm", "php-gd", "php-gmp", "php-mbstring", "php-mcrypt", "php-opcache", "php-pdo", "php-pear-MDB2-Driver-mysqli", "php-pecl-memcached", "php-pecl-msgpack", "php-xml"]
