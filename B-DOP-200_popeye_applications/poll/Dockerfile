# Use the official Python image as the base image
FROM python:latest

# Set the working directory in the container to /app
WORKDIR /app

# Copy the requirements.txt file to the container
COPY requirements.txt .

# Install the dependencies using pip3
RUN pip3 install -r requirements.txt

# Copy the rest of the application code to the container
COPY . .

# Set the environment variable to let Flask know where the application is
ENV FLASK_APP=app.py

# Expose port 80
EXPOSE 80

# Start the application using the flask run command
CMD ["flask", "run", "--host=0.0.0.0", "--port=80"]