FROM ubuntu:14.04

RUN \
  apt-get update && \
  apt-get -y upgrade && \
  apt-get install -y python wget

RUN \
  cd /opt && \
  wget http://nodejs.org/dist/v0.10.28/node-v0.10.28-linux-x64.tar.gz && \
  tar xvf node-v0.10.28-linux-x64.tar.gz && \
  mv node-v0.10.28-linux-x64 node && \
  rm -f node-v0.10.28-linux-x64.tar.gz && \
  cd /usr/local/bin && \
  ln -s /opt/node/bin/* .

CMD ["/bin/bash"]
