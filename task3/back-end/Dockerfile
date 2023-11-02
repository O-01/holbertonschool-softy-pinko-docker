# base image for container
FROM ubuntu:latest

# update apt
RUN apt-get update

# upgrade installed software
RUN apt-get upgrade -y

# install python3 + pip
RUN apt-get install -y python3 python3-pip

# install flask
RUN pip3 install flask

# install flask-cors
RUN pip3 install flask-cors

# working directory set to /app
WORKDIR /app

# copy local input contents to specified output location within container
COPY ./api.py /app/api.py

# run api using newly installed Python3
CMD [ "python3", "/app/api.py" ]
