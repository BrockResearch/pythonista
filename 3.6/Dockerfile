# Version: 1.0.0
FROM alpine:3.6
MAINTAINER Brock Research 

RUN apk add --no-cache \
    ca-certificates

RUN apk update

RUN apk add git=2.13.0-r0

RUN apk add python3=3.6.1-r2

RUN apk add py3-pip
RUN pip3 install --upgrade pip==9.0.1

# Add Virtual Environment to enable project-specific package installations.
RUN pip3 install virtualenv==15.1.0

CMD ["/bin/sh"]