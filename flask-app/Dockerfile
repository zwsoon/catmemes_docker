# specifying our base image
FROM python:3

# set a directory for the app
WORKDIR /usr/src/app

# copy all the files to the container
COPY . .

# install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# The next thing we need to specify is the port number that needs to be exposed. 
# Since our flask app is running on port 5000, that's what we'll indicate.
Expose 5000

CMD ["python","./app.py"]