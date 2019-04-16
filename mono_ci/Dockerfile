FROM mono:latest
MAINTAINER Paul Oosthuysen

RUN apt-get update && apt-get install curl bzip2 libfontconfig git -y && which ssh-agent || ( apt-get update -y && apt-get install openssh-client -y )

RUN curl -sL https://deb.nodesource.com/setup_11.x | bash - && apt-get install -y nodejs && npm install -g grunt-cli