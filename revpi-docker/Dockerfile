FROM arm32v7/debian:jessie

ADD ./repo /

RUN apt-get update && apt-get install -y --no-install-recommends \
  gnupg \
  dirmngr \
  && rm -rf /var/lib/apt/lists/*
  
CMD [ "bash" ]
