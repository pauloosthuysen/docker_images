FROM node:latest
MAINTAINER Paul Oosthuysen

RUN which ssh-agent || ( apt-get update -y && apt-get install openssh-client -y ) && npm install grunt-cli bower -g

ADD hosts tmp/
CMD cat /tmp/hosts >> /etc/hosts; nodejs