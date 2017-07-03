# FROM <name>:<version> - tells Docker what the image's base image should come from
FROM ubuntu:latest

# MAINTAINER <detail> - specifies the owner of the file
MAINTAINER Alex Escalante <mail@mail.com>

# COPY <local file> <image location> - copies a file in the same location in the Dockerfile
#  location and copies it onto the docker image file system.
COPY alpharetta /home

# ADD <file on local file OR URL> <image location> - copies a file in the same location in the
# Dockerfile OR URL specified and copies it onto the docker image file system. This ADD can also
# deal with tar files.
ADD copy_files.tar /home

# ENV <key> <value> - creates an environmental variable in the container to be ran.
# example: ENV http_proxy 10.132.140.23:80 will create an http proxy env set.
ENV demo_state true

# ARG <variable_name> - creates an variable within the Dockerfile that allows definition at
# build time. Example: ARG message, then in "docker run --build-arg message=yay will make the
# message varible have a value at execution
# ARG COMPLETED_MESSAGE

# CMD <bash command> - tells docker to run the following command from within the running 
# Docker container.
# CMD echo Hello World!!!
# CMD echo ${COMPLETED_MESSAGE}
