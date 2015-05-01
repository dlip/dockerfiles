FROM       dlip/centos6-ansible-php
MAINTAINER Dane Lipscombe <dane@lipscombe.com.au>

ADD roles /var/playbooks/roles

RUN add-role dlip.apache

ENV LOG_FILE /var/log/httpd/*

RUN add-shutdown "service httpd stop"

RUN container-install

EXPOSE 80
EXPOSE 443
