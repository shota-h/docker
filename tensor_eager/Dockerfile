FROM tensorflow/tensorflow:nightly-gpu-py3
MAINTAINER Shota <>

RUN pip install -q h5py
RUN pip install -q requests

COPY jupyter_notebook_config.py /root/.jupyter/
