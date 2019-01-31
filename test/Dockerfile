FROM python:3.6
MAINTAINER Shota <>

RUN apt-get update
RUN apt-get upgrade -y
# RUN apt-get install git -y
RUN pip install numpy
RUN pip install matplotlib
RUN pip install scipy
RUN pip install pillow
# RUN pip install -q scipy
RUN pip install -q requests
 RUN pip install scikit-image
 RUN pip install --upgrade scikit-image

COPY jupyter_notebook_config.py /root/.jupyter/
