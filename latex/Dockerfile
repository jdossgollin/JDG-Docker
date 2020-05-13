FROM debian:stretch-slim

RUN apt-get update && apt-get install -y \
    biber \
    latexmk \
    make \
    texlive-full \
    software-properties-common \
    fonts-font-awesome \
    && rm -rf /var/lib/apt/lists/*

RUN add-apt-repository "deb http://deb.debian.org/debian buster main contrib non-free" && \
    apt update && \
    apt install -y fonts-firacode \
    && rm -rf /var/lib/apt/lists/*