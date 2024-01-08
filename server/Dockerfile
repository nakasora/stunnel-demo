FROM ubuntu:latest
RUN apt-get update && apt-get install -y stunnel4
COPY ./stunnel-server.conf /etc/stunnel/stunnel.conf
COPY ./cert.pem /etc/stunnel/cert.pem
COPY ./key.pem /etc/stunnel/key.pem
CMD ["stunnel4"]
