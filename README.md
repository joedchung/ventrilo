# Minimal docker image for running Ventrilo

- Built on [baseimage-docker](http://phusion.github.io/baseimage-docker/)
- Sets codec to Speex for mac client compatibiity

To run, publish Ventrilo's port ( 3784 ) for both tcp and udp. For example:

    docker pull mightyjoec/ventrilo-github:latest
    docker run -d -p 3784:3784 -p 3784:3784/udp mightyjoec/ventrilo-github
