FROM       dlip/centos6-ansible
MAINTAINER Dane Lipscombe <dane@lipscombe.com.au>

ADD roles /var/playbooks/roles

RUN add-role dlip.logstash-forwarder

#ENV LOG_FILE /var/log/pgsql

RUN container-install

RUN add-shutdown "service logstash-forwarder stop"

EXPOSE 5432
