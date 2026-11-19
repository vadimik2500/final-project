FROM python:3.9-slim
RUN apt-get update && apt-get install -y libpq-dev gcc && rm -rf /var/lib/apt/lists/*
WORKDIR /app
RUN pip install psycopg2-binary
COPY app.py .
EXPOSE 8000
CMD ["python", "app.py"]

