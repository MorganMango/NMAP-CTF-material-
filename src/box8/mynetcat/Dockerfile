FROM debian:latest

RUN apt-get update && \
    apt-get install -y ncat

CMD ["nc", "-l", "-p", "1234"]
