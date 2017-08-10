# Version: 1.0.0
FROM alpine:3.5
MAINTAINER Brock Research 

RUN apk add --no-cache \
    ca-certificates

RUN apk update

RUN apk add git=2.11.2-r0

RUN apk add python3=3.5.2-r9

RUN apk add py3-pip
RUN pip install --upgrade pip==9.0.1

# Add Virtual Environment to enable project-specific package installations.
RUN pip install virtualenv==15.1.0

# Create projects directory under developer's home directory
WORKDIR /root
RUN mkdir -p /root/projects

CMD ["/bin/sh"]