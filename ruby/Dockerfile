FROM komljen/ubuntu
MAINTAINER Alen Komljen <alen.komljen@live.com>

ENV PATH /usr/local/rvm/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
ENV RUBY_VERSION 1.9.3

RUN curl -sL https://get.rvm.io | bash -s stable
RUN rvm requirements
RUN rvm install ruby-$RUBY_VERSION
RUN /bin/bash -l -c 'rvm use $RUBY_VERSION --default'
