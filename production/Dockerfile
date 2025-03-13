FROM python:3.12

WORKDIR /tmp/

COPY . . 

RUN pip3 install -r requirements.txt

EXPOSE 8000

CMD ["gunicorn","-w","1","-b","0.0.0.0:8000","wsgi:app"]
