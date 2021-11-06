FROM python:3.9.1

WORKDIR /app

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

COPY . /app
RUN pip install -r requirements.txt
RUN cd /app

CMD [ "python", "manage.py", "runserver", "--port", "9002" ]
