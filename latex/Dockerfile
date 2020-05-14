FROM debian:testing

RUN apt-get update -q && apt-get install -qy \
    # some auxiliary tools
    wget \
    git \
    make \
    sudo \
    pandoc \
    pandoc-citeproc \
    fig2dev \
    python3-pygments \
    fonts-font-awesome \
    software-properties-common && \
    add-apt-repository "deb http://deb.debian.org/debian buster main contrib non-free" && \
    apt update && \
    apt install -y fonts-firacode && \
    apt-get --purge remove -y .\*-doc$ && \
    apt-get clean -y && \
    apt-get autoremove && \
    rm -rf /var/lib/apt/lists/*

# Install TexLive with scheme-basic
RUN wget http://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz; \
    mkdir /install-tl-unx; \
    tar -xf install-tl-unx.tar.gz -C /install-tl-unx --strip-components=1; \
    echo "selected_scheme scheme-basic" >> /install-tl-unx/texlive.profile; \
    /install-tl-unx/install-tl -profile /install-tl-unx/texlive.profile; \
    rm -r /install-tl-unx; \
    rm install-tl-unx.tar.gz && \
    tlmgr update --self; \
    tlmgr install scheme-full; \
    tlmgr update --all

