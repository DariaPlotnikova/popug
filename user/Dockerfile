FROM python:3.9.1

WORKDIR /user

ENV PYTHONPATH /user
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

COPY . /user
RUN pip install -r requirements.txt
RUN cd /user

EXPOSE 9000

CMD [ "python", "manage.py", "runserver", "--port", "9000" ]
