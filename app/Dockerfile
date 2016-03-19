FROM ubuntu:latest
MAINTAINER cdagli
RUN apt-get update
# RUN apt-get -y install wget python
# RUN wget https://bootstrap.pypa.io/get-pip.py
RUN apt-get -y install python-pip python-dev build-essential supervisor
# Or use requirements.txt
ADD config/requirements.txt .
COPY config/supervisord.conf /etc/supervisor/supervisord.conf
RUN pip install -r requirements.txt
RUN /etc/init.d/supervisor stop
# RUN supervisord -c /etc/supervisor/supervisord.conf