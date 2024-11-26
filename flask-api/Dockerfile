# Use the Python base image
FROM python:3.13-slim

# Set the working directory
WORKDIR /app

# Copy dependencies and install them
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the source code
COPY . .

# Expose the application port
EXPOSE 5000

# Start the app
CMD ["python", "app.py"]

