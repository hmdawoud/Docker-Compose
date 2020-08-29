FROM python:3.8-alpine
WORKDIR /code
COPY requirements.txt /code/
RUN pip install -r requirements.txt
COPY scr/ /code/
ENV FLASK_APP server.py
EXPOSE 5000
CMD flask run --host=0.0.0.0
 