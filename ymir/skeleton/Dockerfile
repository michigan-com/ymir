FROM ubuntu:14.04
MAINTAINER Eric Bower neurosnap@gmail.com

RUN apt-get update && apt-get install -y wget
RUN wget -P /tmp https://apt.puppetlabs.com/puppetlabs-release-trusty.deb
RUN dpkg -i /tmp/puppetlabs-release-trusty.deb

RUN apt-get update && apt-get install -y puppet
RUN apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

CMD ["bash"]
