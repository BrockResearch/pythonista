# Version: 1.0.0
FROM alpine:3.5
MAINTAINER Brock Research 

RUN apk add --no-cache \
    ca-certificates

RUN apk update

RUN apk add git=2.11.2-r0

RUN apk add python3=3.5.2-r9

RUN apk add py3-pip
RUN pip3 install --upgrade pip==9.0.1

# Add Virtual Environment to enable project-specific package installations.
RUN pip install virtualenv==15.1.0

# Common Tools

## Command Line Framework
RUN pip install cement==2.10.2

## BDD Framework
RUN pip install behave==1.2.5

## Project Scaffolding
RUN pip install pyscaffold==2.5.7

## Web Framework
RUN pip install flask==0.12.2

# Create projects directory under developer's home directory
WORKDIR /root
RUN mkdir -p /root/projects

CMD ["/bin/sh"]