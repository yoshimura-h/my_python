FROM nvidia/cuda:10.2-devel-ubuntu18.04

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y python3 python3-pip libgl1-mesa-dev

RUN pip3 install --upgrade pip
RUN pip3 install --upgrade setuptools

RUN mkdir -p /root/src
COPY requirements.txt /root/src

WORKDIR /root/src
RUN pip3 install -r requirements.txt
