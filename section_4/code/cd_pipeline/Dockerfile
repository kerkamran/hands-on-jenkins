# base image
#FROM alpine:3.7
FROM python:3.6-alpine

# Install python 3 and pip
#RUN apk add --no-cache python

# Install Python modules needed by the Python app
RUN pip3 install Flask

# Copy files required for the app to run
COPY app.py /usr/src/app/
COPY templates/index.html /usr/src/app/templates/

# Tell the port number the container should expose
EXPOSE 5000

# Run the application
CMD ["python3", "/usr/src/app/app.py"]
