FROM arm32v7/debian:jessie 

ADD ./repo /

RUN apt-get update \
  && chmod +x /usr/bin/piSerial \
  && chmod +x /usr/bin/revpi-config \
  && chmod +x /opt/vc/bin/vcgencmd

CMD [ "bash" ]