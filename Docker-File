FROM python:3.9-alpine

WORKDIR /app

COPY techtrends/ .

RUN pip install --no-cache-dir -r requirements.txt

RUN python ./init_db.py

EXPOSE 3111

CMD [ "python", "./app.py" ]
