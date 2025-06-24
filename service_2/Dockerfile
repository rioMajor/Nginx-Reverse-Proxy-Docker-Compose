# Use an official Python base image
FROM python:3.10-slim

# Set the working directory in the container
WORKDIR /app

# Copy the app files into the container
COPY . .

# Install Flask
RUN pip install --no-cache-dir flask

# Expose the port the app runs on
EXPOSE 8002

# Run the app
CMD ["python", "app.py"]
