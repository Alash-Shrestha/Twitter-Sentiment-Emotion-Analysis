FROM python:3.10-alpine

EXPOSE 8000

WORKDIR /app 

RUN pip install Django textblob numpy tweepy pandas

COPY . /app/

EXPOSE 8000

CMD ["sh", "-c", "python manage.py makemigrations && python manage.py migrate && python manage.py runserver 0.0.0.0:8000"]