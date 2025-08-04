# Use the latest official Python image
FROM python:latest

# Set the working directory inside the container
##WORKDIR /app

RUN pwd && ls -ltr

# Copy project files into the container
COPY requirements.txt .
COPY app.py .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port that the Flask app will run on
EXPOSE 5000

# Run the application
CMD ["python", "app.py"]
