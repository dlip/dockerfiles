FROM       resin/rpi-raspbian:wheezy
MAINTAINER Dane Lipscombe <dane@lipscombe.com.au>

RUN apt-get update && apt-get install -y --no-install-recommends\
    python python-yaml python-jinja2 python-httplib2 python-keyczar python-paramiko python-setuptools python-pkg-resources python-pip

RUN apt-get install -y --no-install-recommends\
    tar git netcat

RUN pip install ansible

ADD scripts/ /usr/local/bin

ADD docker.yml /var/playbooks/docker.yml

RUN mkdir /var/playbooks/host_vars

ENV LOG_FILE /dev/null

#service announcements
EXPOSE 9811

CMD ["container-boot"]
