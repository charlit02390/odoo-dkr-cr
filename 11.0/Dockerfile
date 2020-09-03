FROM odoo:11.0
MAINTAINER jokercharlie <cmonge@jackdevelopers.com>

USER root

RUN python3 -m pip install wheel

COPY requirements.txt requirements.txt

RUN python3 -m pip install -r requirements.txt