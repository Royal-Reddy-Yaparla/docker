FROM python:3.9.18-alpine3.19

EXPOSE 8080
ENV AMQP_USER=roboshop \
    AMQP_PASS=roboshop123

USER root
WORKDIR /app

# Copy requirements file
COPY requirements.txt /app/

# Update and install necessary packages
RUN apt-get update && apt-get install -y \
    python3-dev build-essential linux-headers-amd64 libpcre3-dev && \
    rm -rf /var/lib/apt/lists/*

# Install Python dependencies
RUN pip install -r requirements.txt

# Copy application files
COPY *.py /app/
COPY payment.ini /app/

# Default command
CMD ["python", "payment.py"]
