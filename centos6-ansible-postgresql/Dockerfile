FROM       dlip/centos6-ansible
MAINTAINER Dane Lipscombe <dane@lipscombe.com.au>

ADD roles /var/playbooks/roles

RUN add-role dlip.postgresql

ENV LOG_FILE /var/log/pgsql

RUN container-install

RUN add-shutdown "service postgresql-9.3 stop"

EXPOSE 5432
