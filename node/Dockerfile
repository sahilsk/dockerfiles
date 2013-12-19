FROM ubuntu
MAINTAINER Kimbro Staken

RUN apt-get install -y python-software-properties python
RUN add-apt-repository ppa:chris-lea/node.js
RUN echo "deb http://us.archive.ubuntu.com/ubuntu/ precise universe" >> /etc/apt/sources.list
RUN apt-get -y update

# TOOLS
RUN apt-get install -y -q curl git make wget vim nano build-essential g++

## NODE
RUN apt-get install -y -q nodejs

RUN git clone https://github.com/sahilsk/dockworker.git	/home/dockworker
RUN cd /home/dockworker && npm install

EXPOSE 80
WORKDIR /home/dockworker

CMD ["node", "index.js"]