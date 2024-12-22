FROM gcr.io/google-appengine/python:latest

WORKDIR /app

COPY requirements.txt ./
RUN pip install -r requirements.txt

COPY . .

ENTRYPOINT gunicorn -b :$PORT main:app
