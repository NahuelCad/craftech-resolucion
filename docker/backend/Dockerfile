FROM python:3.8.3

WORKDIR /app
ADD ./backend/requirements.txt /app/backend/


RUN pip install --upgrade pip

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        postgresql-client \
    && rm -rf /var/lib/apt/lists/*
RUN apt update
RUN apt-get install libpq-dev python3-dev

RUN pip install -r backend/requirements.txt

ADD ./docker /app/docker
ADD ./backend /app/backend