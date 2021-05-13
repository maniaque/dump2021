FROM python:3.7-alpine

ADD ./app/requirements.txt /requirements.txt
RUN pip install -r /requirements.txt

COPY ./app /app/

EXPOSE 80

WORKDIR /app
ENV FLASK_APP=pytime

CMD [ "flask", "run", "--host=0.0.0.0", "--port=80" ]

