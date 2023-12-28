FROM python:3.9.18-slim

WORKDIR /opt/api

COPY ./compose/entrypoint /entrypoint
COPY ./compose/api/start /start
COPY . /opt/api/

EXPOSE 8000

RUN pip install -r requirements.txt

ENTRYPOINT [ "/entrypoint" ]
