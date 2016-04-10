FROM rocker/r-base

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

ONBUILD COPY . /usr/src/app
ONBUILD RUN Rscript -e 1 --args --bootstrap-packrat
