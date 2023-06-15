FROM tiangolo/uvicorn-gunicorn-fastapi:python3.8
WORKDIR /app
COPY . .
COPY ./requirements.txt /requirements.txt

RUN pip install -r /requirements.txt

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]
