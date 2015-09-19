FROM       dlip/raspbian-ansible
MAINTAINER Dane Lipscombe <dane@lipscombe.com.au>

ADD roles /var/playbooks/roles

RUN add-role dlip.plex

RUN container-install

RUN add-shutdown "service plexmediaserver stop"
