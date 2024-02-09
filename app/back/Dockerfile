# Use the official Python runtime as a parent image
FROM python:3

# Set the working directory in the container to /app/back
WORKDIR /app

# Copy the current directory contents into the container at /app/back
COPY . /app

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Make port 5000 available to the world outside this container
EXPOSE 5000

# Define environment variable
ENV NAME World

# Run the Python application on container startup
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]
