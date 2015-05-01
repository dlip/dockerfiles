FROM       dlip/centos6-ansible
MAINTAINER Dane Lipscombe <dane@lipscombe.com.au>

ADD roles /var/playbooks/roles

RUN add-role dlip.nfs

RUN container-install

RUN add-shutdown "service nfs stop"
RUN add-shutdown "service rpcbind stop"

EXPOSE 111/tcp 111/udp 2049/tcp 2049/udp 892/tcp 892/udp
