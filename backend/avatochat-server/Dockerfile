FROM ubuntu:24.04
SHELL ["/bin/bash", "-c"]

ARG DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y liburing2

WORKDIR /workspace

# Must provoide conduwuit
COPY ./conduwuit ./conduwuit

CMD [ "./conduwuit" ]
