# Get official Python runtime image
FROM python:2.7-slim

# Set working directory
WORKDIR /app

# Move local contents to /app
ADD . /app

# Install Python packages
RUN pip install --trusted-host pypi.python.org -r ./requirements.txt

# Expose port 80
EXPOSE 80

# Environment variables
ENV NAME World

# Run on container launch
CMD ["python", "app.py"]