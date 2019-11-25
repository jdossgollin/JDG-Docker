FROM  tensorflow/tensorflow:1.15.0-py3

COPY leveesim/requirements.txt /tmp/requirements.txt
RUN pip install -r /tmp/requirements.txt
RUN apt-get --yes install git
RUN pip install https://github.com/hill-a/stable-baselines/archive/e315ebecbfd26225522a2e63a6bbd440c1df7f01.zip &&\
    pip install https://github.com/jdossgollin/leveesim/archive/ce61df0e637bbc0020f744fcd3ed88e20e0e0f66.zip