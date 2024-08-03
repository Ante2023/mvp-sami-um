
FROM python:3.9-slim

WORKDIR /src

COPY requirements.txt .

RUN apt-get update && apt-get install -y net-tools

RUN pip install --no-cache-dir -r requirements.txt

COPY flaskapp.py .

CMD [ "python", "flaskapp.py" ]
