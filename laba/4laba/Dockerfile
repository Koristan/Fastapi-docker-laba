
FROM python:3.10

WORKDIR /server

COPY server/req.txt .

RUN pip install --no-cache-dir -r req.txt

COPY . .

EXPOSE 8000

CMD ["python", "-m", "uvicorn", "server.main:app", "--host", "0.0.0.0", "--port", "8000"]