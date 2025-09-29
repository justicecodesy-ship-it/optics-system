# Base image
FROM python:3.13-slim
# Set work directory
WORKDIR /app
# Copy requirements
COPY requirements.txt .
# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt
# Copy backend code
COPY . .
# Run server
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
