FROM python:3.9

WORKDIR /app

COPY requirements.txt . [cite: 4093]

RUN pip install -r requirements.txt --no-cache-dir

COPY . . [cite: 4100]

CMD ["gunicorn", "kittygram_backend.wsgi:application", "--bind", "0:8000"]
