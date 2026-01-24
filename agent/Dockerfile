# Base image with Python
FROM python:3.11-slim

# Set working directory
WORKDIR /app

# Copy files
COPY . /app

# Install dependencies from agent/requirements.txt
RUN pip install --no-cache-dir -r /app/agent/requirements.txt



# Expose Flask port
EXPOSE 8001

# Prevent output buffering
ENV PYTHONUNBUFFERED=1
ENV PYTHONPATH=/app


# Run the app
CMD ["python", "agent/main.py"]
