FROM odoo:14.0
MAINTAINER jokercharlie <cmonge@jackdevelopers.com>

USER root

RUN apt-get update -y && apt-get install -y  python3-pip

RUN python3 -m pip install --upgrade pip


RUN python3 -m pip install wheel

COPY requirements.txt requirements.txt

RUN python3 -m pip install -r requirements.txt
