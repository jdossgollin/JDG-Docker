FROM mirisbowring/texlive_ctan_full:2019

RUN apt-get update && apt-get install -y \
    software-properties-common \
    fonts-font-awesome

RUN add-apt-repository "deb http://deb.debian.org/debian buster main contrib non-free" && \
    apt update && \
    apt install -y fonts-firacode \
    && rm -rf /var/lib/apt/lists/*