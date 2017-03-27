FROM centos:7

RUN ["rpm", "-ivh", "http://dl.fedoraproject.org/pub/epel/7/x86_64/e/epel-release-7-9.noarch.rpm"]
RUN ["rpm", "--import", "http://rpms.famillecollet.com/RPM-GPG-KEY-remi"]
RUN ["rpm",  "-ivh", "http://rpms.famillecollet.com/enterprise/remi-release-7.rpm"]
RUN ["yum", "-y", "update", "remi-release"]

RUN ["yum", "-y", "--enablerepo=remi-php71", "install", "php", "php-fpm", "php-gmp", "php-mbstring", "php-mcrypt", "php-opcache"]
