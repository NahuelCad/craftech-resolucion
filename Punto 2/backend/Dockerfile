  
FROM python:3.8.3
ENV PYTHONUNBUFFERED 1
WORKDIR /backend
COPY requirements.txt requirements.txt

RUN pip install --upgrade pip

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        postgresql-client \
    && rm -rf /var/lib/apt/lists/*
RUN apt update
RUN apt-get install libpq-dev python3-dev gcc -y
RUN export PATH=/usr/lib/postgresql/X.Y/bin/:$PATH
RUN apt-get install graphviz graphviz-dev -y

RUN pip3 install -r requirements.txt
COPY . .