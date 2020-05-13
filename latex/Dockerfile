FROM tianon/latex

RUN apt-get update && apt-get install -y \
    software-properties-common \
    fonts-firacode \
    && rm -rf /var/lib/apt/lists/*

RUN add-apt-repository "deb http://deb.debian.org/debian buster main contrib non-free" && \
    apt update && \
    apt install -y fonts-firacode