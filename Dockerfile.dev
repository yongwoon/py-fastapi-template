FROM python:3.12-slim

RUN mkdir -p /var/www

WORKDIR /var/www
COPY api .

RUN pip install --no-cache-dir fastapi uvicorn

EXPOSE 8000

# command to run the app using uvicorn.
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]