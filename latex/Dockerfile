FROM tianon/latex

# Install Fira Sans font
RUN apt-get update \
    && apt-get install -y \
    fonts-font-awesome \
    unzip \
    wget

RUN wget https://github.com/bBoxType/FiraSans/archive/master.zip -O fira.zip \
    && unzip fira.zip -d FiraSans-master \
    && rm fira.zip \
    && mkdir -p /usr/share/fonts/opentype/fira \
    && find FiraSans-master/ -name "*.otf" -exec cp {} /usr/share/fonts/opentype/fira/ \; \
    && mkdir -p /usr/share/fonts/truetype/fira \
    && find FiraSans-master/ -name "*.ttf" -exec cp {} /usr/share/fonts/truetype/fira/ \; \
    && rm -rf fira