FROM  --platform=linux/amd64 odoo:15.0
MAINTAINER jokercharlie <cmonge@jackdevelopers.com>

USER root

RUN apt-get update -y && apt-get install -y  python3-pip

RUN python3 -m pip install --upgrade pip


RUN python3 -m pip install wheel

COPY server.py server.py

RUN rm -rf /usr/lib/python3/dist-packages/odoo/service/server.py && mv server.py /usr/lib/python3/dist-packages/odoo/service

COPY requirements.txt requirements.txt

RUN python3 -m pip install -r requirements.txt
