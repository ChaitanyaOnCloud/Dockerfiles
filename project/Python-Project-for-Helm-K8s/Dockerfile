# Use official Python 3.10 image as base
FROM python:3.10

# Set working directory
WORKDIR /myapp

# Copy only requirements first to leverage Docker cache
COPY requirements.txt /myapp/

# Install dependencies
RUN python -m pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application code
COPY . /myapp

# Expose Flask default port
EXPOSE 5000

# Command to run the app
CMD ["python", "main.py"]

