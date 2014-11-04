FROM kiyohara/docker-sshd

MAINTAINER Tomokazu Kiyohara <tomokazu.kiyohara@gmail.com>

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get -y update
RUN apt-get -y install ruby
RUN apt-get -y install ruby-dev
RUN apt-get -y install make
RUN apt-get -y install libssl-dev

RUN apt-get -y install git
RUN gem install --no-ri --no-rdoc rake
RUN gem install --no-ri --no-rdoc bundler

CMD [ "/usr/bin/supervisord" ]
