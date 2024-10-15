FROM python:3.10-slim

WORKDIR /app

COPY code/requirements.txt /app/requirements.txt

RUN pip install --upgrade pip
RUN pip install --no-cache-dir -r requirements.txt

COPY code /app/code

EXPOSE 5000

CMD ["python", "code/src/app.py"]
