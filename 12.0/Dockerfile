FROM odoo:12.0
MAINTAINER jokercharlie <cmonge@jackdevelopers.com>

USER root

RUN apt-get update -y && apt-get install apt-file -y && apt-file update -y && apt-get install -y python3-dev build-essential

RUN python3 -m pip install wheel

COPY requirements.txt requirements.txt

RUN python3 -m pip install -r requirements.txt