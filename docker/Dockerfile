FROM python:3.9-slim

RUN apt-get update && \
    apt-get install -y --no-install-recommends procps && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

RUN python -m pip install --upgrade pip --no-cache-dir

COPY ./requirements.txt /requirements.txt
RUN pip3 install -r /requirements.txt
