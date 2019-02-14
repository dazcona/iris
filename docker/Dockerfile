# Select a base image:

FROM tensorflow/tensorflow:latest-py3
#python:2.7
#python:3.7
#tensorflow/tensorflow:latest-gpu
#tensorflow/tensorflow:latest-gpu-py3
#tensorflow/tensorflow:latest-py3: python 3 + tensorflow + jupyter
#nvidia/cuda:8.0-cudnn5-devel


# Install OS packages (from requirements_os.txt):

ADD docker/requirements_os.txt .
RUN apt update -y && apt install -y $(cat requirements_os.txt|grep -v '#')


# Install Python packages (from requirements.txt):

ADD docker/requirements.txt .
RUN pip3 install -r requirements.txt
