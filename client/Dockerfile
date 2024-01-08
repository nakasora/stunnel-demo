FROM ubuntu:latest
RUN apt-get update && apt-get install -y stunnel4
COPY ./stunnel-client.conf /etc/stunnel/stunnel.conf
CMD ["stunnel4"]
