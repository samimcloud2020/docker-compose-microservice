FROM python:3.6-slim

WORKDIR /app

COPY . /app
  
RUN apt-get update && apt-get install

RUN apt-get install -y \
  dos2unix \
  libpq-dev \
  libmariadb-dev-compat \
  libmariadb-dev \
  gcc \
  && apt-get clean

RUN pip3 install -r requirements.txt




EXPOSE 5000

CMD ["python3","app.py"]
