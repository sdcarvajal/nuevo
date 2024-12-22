FROM gcr.io/google-appengine/python:3.7

WORKDIR /app

COPY requirements.txt ./
RUN pip install -r requirements.txt

COPY . .

ENTRYPOINT gunicorn -b :$PORT main:app
