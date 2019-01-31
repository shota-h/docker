FROM tensorflow/tensorflow:latest-gpu-py3
MAINTAINER Shota <>

RUN apt-get update
RUN apt-get install -y vim less
RUN pip install --upgrade pip
RUN apt-get install -y language-pack-ja-base language-pack-ja
ENV LANG=ja_JP.UTF-8

RUN pip install -q numpy
RUN pip install -q scipy
RUN pip install -q matplotlib
RUN pip install -q seaborn
RUN pip install -q scikit-learn
RUN pip install -q scikit-image
RUN pip install -q pandas
RUN pip install -q hmmlearn
RUN pip install -q keras==2.1.5
RUN pip install -q pyclustering
RUN pip install -q h5py
RUN pip install -q requests

COPY jupyter_notebook_config.py /root/.jupyter/
