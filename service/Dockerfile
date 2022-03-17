FROM python:3.9-slim-buster

RUN mkdir /app
COPY main.py run.sh requirements.txt model.bin /app/

WORKDIR /app

RUN pip install --upgrade pip && pip install -r requirements.txt
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8080"]
