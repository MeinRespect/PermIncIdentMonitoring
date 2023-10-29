# Use an official Python runtime as a parent image
FROM python:3.9-slim

# Set environment variables for your app
ENV APP_PORT 8000

# Create and set the working directory inside the container
WORKDIR /

# Copy the current directory contents into the container at /app
COPY . /

# Install any necessary dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port your app will run on
EXPOSE 8000

# Define the command to run your application using uvicorn
CMD ["uvicorn", "app:app", "--host", "0.0.0.0", "--port", "8000"]
