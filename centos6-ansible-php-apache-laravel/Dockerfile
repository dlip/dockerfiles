FROM       dlip/centos6-ansible-php-apache
MAINTAINER Dane Lipscombe <dane@lipscombe.com.au>

ADD roles /var/playbooks/roles
RUN add-role dlip.laravel

RUN container-install
