FROM python:3.11-slim-buster
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
CMD ["gunicorn", "amazoo.wsgi:application", "--bind", "0.0.0.0:8000"]