FROM python:2.7-slim

RUN apt-get update && apt-get install -y python-dev gcc --no-install-recommends apt-utils

RUN apt-get install -y curl 

RUN pip install --upgrade && pip install -U setuptools && pip install uwsgi

COPY requirements.txt /tmp/

RUN pip install -r /tmp/requirements.txt

RUN apt-get remove -y --purge python-dev gcc
