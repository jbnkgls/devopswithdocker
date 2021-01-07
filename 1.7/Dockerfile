FROM ubuntu:16.04
WORKDIR /mydir
COPY script.sh .
RUN chmod +x ./script.sh
RUN apt update
RUN apt install -y curl
ENTRYPOINT ["/bin/sh"]
CMD ["./script.sh"]

