FROM python:3.6-slim

WORKDIR /app

COPY . /app
RUN apt install build-essential libpq-dev python3-dev

RUN pip3 install -r requirements.txt




EXPOSE 5000

CMD ["python3","app.py"]
