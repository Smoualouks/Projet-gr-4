FROM python:3.8-slim-buster

RUN apt-get update
RUN apt-get install -y curl

WORKDIR /app

COPY requirements.txt .
RUN pip3 install -r requirements.txt

COPY . .

CMD ["python", "app.py"]
