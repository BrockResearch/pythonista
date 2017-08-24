# Version: 1.0.0
FROM brockresearch/pinebox:3.6
MAINTAINER Brock Research 

RUN apk add python3=3.6.1-r2

RUN apk add py3-pip
RUN pip3 install --upgrade pip==9.0.1

# Add Virtual Environment to enable project-specific package installations.
RUN pip3 install virtualenv==15.1.0

# Common Tools

## Command Line Framework
RUN pip3 install cement==2.10.2

## BDD Framework
RUN pip3 install behave==1.2.5

## Project Scaffolding
RUN pip3 install pyscaffold==2.5.7

## Web Framework
RUN pip3 install flask==0.12.2

# Create projects directory under developer's home directory
WORKDIR /root
RUN mkdir -p /root/projects

# Setup VIM Python syntax highlighting
COPY vimrc /root/.vimrc

CMD ["/bin/sh"]