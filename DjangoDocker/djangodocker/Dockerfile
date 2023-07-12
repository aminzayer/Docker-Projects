FROM python:3.11.2
ENV PYTHONBUFFERED=1
WORKDIR /code
COPY requirements.txt .
RUN pipenv install -r requirements.txt
COPY . .
EXPOSE 8000
RUN pipenv shell
CMD ["python","manage.py","runserver"]
