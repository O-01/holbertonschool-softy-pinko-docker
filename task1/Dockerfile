# base image for container
FROM ubuntu:latest

# update apt/upgrade installed software/install python3 + pip/install flask
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y python3 python3-pip
RUN pip3 install flask

# working directory set to /app
WORKDIR /app

# copy local input contents to specified output location within container
COPY ./api.py /app/api.py

# run api using newly installed Python3
CMD [ "python3", "/app/api.py" ]
