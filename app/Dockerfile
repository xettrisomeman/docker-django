#importing baseimage
FROM python:3-alpine 

#set working directory
WORKDIR /app

#set environment variables
#pythondontwritebytecode prvents python from wrting pyc files
#pythonnunbuffered prevents python from stdout and stinput
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONNUNBUFFERED 1

#install dependencies
RUN pip install --upgrade pip
COPY ./requirements.txt /app/requirements.txt
RUN pip install -r requirements.txt 

#copy project
COPY . /app


