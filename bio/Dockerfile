FROM python:2.7
MAINTAINER Shota <>

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install git -y
RUN pip install numpy
RUN pip install matplotlib
RUN pip install scipy
RUN pip install pillow
# RUN pip install -q scipy
RUN pip install -q requests
RUN apt-get install build-essential -y
RUN pip install cython==0.23
# RUN cython -V
RUN git clone https://github.com/scikit-image/scikit-image.git
WORKDIR /scikit-image/
RUN ls
RUN pip install -r requirements.txt
RUN pip install .
WORKDIR /scikit-image/

# RUN pip install --upgrade scikit-image
# RUN pip install -q scikit-image==0.14.1
# RUN ls
# RUN pip install -e git+https://github.com/scikit-image/scikit-image.git#egg=Someproject
RUN pip install -e .
# RUN git pull
RUN python setup.py build_ext -i

COPY jupyter_notebook_config.py /root/.jupyter/
