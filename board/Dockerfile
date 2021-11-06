FROM python:3.9.1

WORKDIR /board

ENV PYTHONPATH /board
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

COPY . /board
RUN pip install -r requirements.txt
RUN cd /board

EXPOSE 9001

CMD [ "python", "manage.py", "runserver", "--port", "9001"  ]
