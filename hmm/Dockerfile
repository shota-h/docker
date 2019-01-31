FROM python:3.6
MAINTAINER Shota <>

RUN pip install -q numpy
RUN pip install -q scipy
RUN pip install -q matplotlib
RUN pip install -q scikit-learn
RUN pip install -q pandas
RUN pip install -q hmmlearn
RUN pip install -q requests

COPY jupyter_notebook_config.py /root/.jupyter/
