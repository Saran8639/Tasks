
FROM python:3.9-slim

COPY . .

RUN pip install flask

EXPOSE 5000

ENV FLASK_APP=app.py

CMD ["python", "app.py"]
