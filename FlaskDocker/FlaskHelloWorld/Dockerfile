# Use the official Python image as the base image
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the dependencies file to the working directory
COPY requirements.txt .

# Install FastAPI and Uvicorn
RUN pip install -r requirements.txt

# Copy the entire project to the working directory
COPY . .

# Expose port 8000 for the FastAPI app
EXPOSE 5050

# Command to run the FastAPI app using Uvicorn
CMD ["python", "app.py"]