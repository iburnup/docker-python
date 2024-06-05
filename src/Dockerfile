FROM python:3.10-bookworm


RUN apt-get update && apt-get install -y git python3-dev
RUN groupadd -r --gid 1000 pyuser && useradd --no-log-init -r -g pyuser --uid 1000 --no-create-home  pyuser    

COPY requirements.txt ./

RUN pip3 install --no-cache-dir -r requirements.txt

WORKDIR /usr/src/app