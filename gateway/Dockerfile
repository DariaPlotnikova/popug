FROM python:3.9.1

WORKDIR /gateway

ENV PYTHONPATH /gateway
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

COPY . /gateway
RUN pip install -r requirements.txt
RUN cd /gateway

EXPOSE 8000

CMD [ "python", "manage.py", "runserver" ]
