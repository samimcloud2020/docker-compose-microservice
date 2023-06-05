FROM python:3.6-slim

WORKDIR /app

COPY . /app

RUN pip3 install -r requirements.txt
RUN apt-get install build-dep python-psycopg2
RUN pip3 install psycopg2-binary 



EXPOSE 5000

CMD ["python3","app.py"]
