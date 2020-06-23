FROM python:3.7.1

COPY ./app /srv/www/app
WORKDIR /srv/www/app

ENV DEBIAN_FRONTEND noninteractive
ENV DEBIAN_FRONTEND newt

RUN apt-get update && \
    apt-get -yq install openssl && \
    apt-get -yq install ca-certificates

RUN pip install -r requirements.txt