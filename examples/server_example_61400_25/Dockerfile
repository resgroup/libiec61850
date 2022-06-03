FROM ubuntu:20.04

RUN  apt-get -y update \
     && apt-get -y autoremove \
     && apt-get clean \
     && apt-get install -y \
     gcc \
     make

WORKDIR app
COPY . .
RUN make examples

ENTRYPOINT ["/app/examples/server_example_61400_25/server_example_61400_25"]