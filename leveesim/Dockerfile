FROM  tensorflow/tensorflow:1.15.0-py3

COPY leveesim/requirements.txt /tmp/requirements.txt
RUN pip install -r /tmp/requirements.txt
RUN apt-get --yes install git
RUN pip install git+git://github.com/hill-a/stable-baselines.git@42c22908e6f2c366f06d84f434fb4ea2d04350cd