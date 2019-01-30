FROM ruby:2.6.0
ENV LANG C.UTF-8

RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs

RUN mkdir /usr/src/app
ENV APP_ROOT /usr/src/app
WORKDIR /usr/src/app

COPY ./app /usr/src/app

EXPOSE 3000
