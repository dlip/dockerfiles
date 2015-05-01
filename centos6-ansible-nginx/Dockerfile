FROM       dlip/centos6-ansible
MAINTAINER Dane Lipscombe <dane@lipscombe.com.au>

ADD roles /var/playbooks/roles

RUN add-role dlip.nginx

RUN container-install

RUN add-service "tail -f /var/log/nginx/*.log"

EXPOSE 80
