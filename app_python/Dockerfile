FROM python:3.11-slim

WORKDIR /app_python

RUN adduser --disabled-password user && chown -R user /app_python

USER user

COPY templates ./templates
COPY main.py requirements.txt app-test.py ./
RUN pip install --no-cache-dir -r requirements.txt
RUN mkdir /app/data && touch /app/data/visits.txt

EXPOSE 5000

CMD ["python", "main.py"]