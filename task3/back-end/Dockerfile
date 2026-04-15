# Use the latest Ubuntu image as the base
FROM ubuntu:latest

# Update and upgrade
RUN apt-get update && apt-get upgrade -y

# Install Python and pip
RUN apt-get install -y python3 python3-pip

# REMOVE the environment restriction file
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Now pip will be allowed to install Flask globally

RUN pip3 install flask flask-cors

# Set working directory and copy the file
WORKDIR /app
COPY ./api.py /app/api.py

# Run the app
CMD ["python3", "api.py"]