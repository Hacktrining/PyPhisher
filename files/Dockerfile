# Dockerfile

# Author       : A Mohan
# Github       : https://github.com/Hacktrining
# Instagram    : https://www.instagram.com/alone__rider__rc_390/
# Email        : mohan63025@gmail.com
# Date         : 25-08-2021
# Main Language: Python

# Download and import main images

# Operating system
FROM debian:latest
# Main package
FROM python:3

# Author info
LABEL MAINTAINER="https://github.com/Hacktrining/PyPhisher"

# Working directory
WORKDIR /PyPhisher/
# Add files 
ADD . /PyPhisher

# Installing other packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install python3-pip php openssh-client -y
RUN pip3 install -r files/requirements.txt --break-system-packages
RUN apt-get clean

# Main command
CMD ["python3", "pyphisher.py", "--noupdate"]

## Wanna run it own? Try following commnads:

## "sudo docker build . -t Hacktrining/pyphisher:latest", "sudo docker run --rm -it Hacktrining/pyphisher:latest"

## "sudo docker pull Hacktrining/pyphisher", "sudo docker run --rm -it Hacktrining/pyphisher"
