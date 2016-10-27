FROM ruby:2.3

RUN apt-get update -qq \
  && apt-get install -y --no-install-recommends \
    libxml2-dev \
    libxslt1-dev \
    nodejs \
  && rm -rf /var/lib/apt/lists/*

RUN gem install rails -v 5.0 --no-ri --no-rdoc

WORKDIR /usr/src/app

CMD /bin/bash
