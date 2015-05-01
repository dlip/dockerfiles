FROM       dlip/centos6-ansible
MAINTAINER Dane Lipscombe <dane@lipscombe.com.au>

ADD roles /var/playbooks/roles

RUN add-role dlip.remi
RUN add-role dlip.php

RUN container-install
