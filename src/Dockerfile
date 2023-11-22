

FROM python:3-slim-buster

RUN apt-get update && apt-get install -y git

COPY requirements.txt ./

RUN pip3 install --no-cache-dir -r requirements.txt

WORKDIR /usr/src/app
