FROM ubuntu:22.04

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update && \
    apt-get install -y \
        build-essential \
        git \
        locales \
        ruby-full \
        zlib1g-dev


# Ruby Gem

RUN gem install bundler

ADD Gemfile /home/Gemfile
ADD Gemfile.lock /home/Gemfile.lock
WORKDIR /home
RUN ls /home
RUN ls
RUN bundle install

#

# RUN cd /home && echo "adsfasdf" && ls && bundle install



CMD ["jekyll", "serve", "--future", "--host", "0.0.0.0"]
# CMD ["bundle", "install", "&&", "jekyll", "server", "--future", "--host", "0.0.0.0"]
# CMD ["ls", "/home"]
# CMD ["jekyll", "serve", "--future", "--host", "0.0.0.0"]
