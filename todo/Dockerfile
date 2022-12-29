# pull official base image
FROM python:3.9.6-alpine

# set work directory
WORKDIR /home/matrix/django_class_base_view/todo

# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

RUN apk update


# install dependencies
RUN pip install --upgrade pip
COPY ./requirements.txt .
RUN pip install -r requirements.txt

# copy project
COPY . .
