FROM python:3.9

WORKDIR /app

COPY requirements.txt .
RUN pip install -r requirements.txt
RUN pip install psycopg2-binary
RUN pip install flask-cors


COPY . .

CMD ["flask", "run", "--host=0.0.0.0"]