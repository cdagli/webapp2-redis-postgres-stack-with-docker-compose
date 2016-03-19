FROM ubuntu:latest
MAINTAINER cdagli
RUN apt-get update
# RUN apt-get -y install wget python
# RUN wget https://bootstrap.pypa.io/get-pip.py
RUN apt-get -y install python-pip python-dev build-essential 
# Or use requirements.txt
ADD requirements.txt .
RUN pip install -r requirements.txt
