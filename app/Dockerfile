FROM python:3-slim
MAINTANER Michalski Luc <michalski.luc@gmail.com>

RUN apt-get update \
    && apt-get install nano bash jq

WORKDIR /opt/service
COPY requirements.txt .

RUN pip3 install --upgrade pip \
    && pip3 install -r requirements.txt

COPY . .

CMD ["/bin/bash"]



