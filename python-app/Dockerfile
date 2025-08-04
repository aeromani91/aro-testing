# Use the latest official Python image
FROM python:latest

# Set the working directory inside the container
WORKDIR /app

# Copy project files into the container
COPY python-app/requirements.txt .
COPY python-app/app.py .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port that the Flask app will run on
EXPOSE 8080

# Run the application
CMD ["python", "app.py"]
