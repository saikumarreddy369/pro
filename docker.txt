FROM python:3.9-slim

WORKDIR /app

COPY app.py .

# 👇 This installs Flask inside the container
RUN pip install flask

CMD ["python", "app.py"]