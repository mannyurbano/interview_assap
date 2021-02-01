# your code goes here ...
FROM python:3.7.5-alpine

# Set the application directory
WORKDIR /src

# Copy requirements.txt
COPY ./src/requirements.txt requirements.txt

# Install our requirements.txt
RUN pip install -r requirements.txt

# Expose required port
EXPOSE 8000
