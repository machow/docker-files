FROM rocker/rstudio

RUN install2.r --error RCurl

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

ONBUILD COPY . /usr/src/app
ONBUILD RUN Rscript --no-save -e 1 --args --bootstrap-packrat
