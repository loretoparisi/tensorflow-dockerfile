FROM tensorflow/tensorflow:latest-gpu-py3

MAINTAINER Loreto Parisi loretoparisi@gmail.com

########################################  BASE SYSTEM
# set noninteractive installation
ARG DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y apt-utils
RUN apt-get install -y --no-install-recommends \
    build-essential \
    pkg-config \
    software-properties-common

######################################## PYTHON3.7
RUN add-apt-repository ppa:deadsnakes/ppa && \
    apt-get  update && \
    apt-get install -y python3.7

######################################## PIP3.7
RUN curl https://bootstrap.pypa.io/get-pip.py > get-pip.py && \
    python3.7 ./get-pip.py

# transfer-learning-conv-ai
ENV PYTHONPATH /usr/local/lib/python3.7

RUN pip3 install tensorflow-gpu
    
CMD ["bash"]
