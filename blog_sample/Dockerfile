# Set the base image to use
FROM python:3.10

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements file to the working directory
#COPY ../../Downloads/Web-Blog-python/requirements.txt .

# Install any needed packages specified in requirements.txt

COPY . .
# Copy the rest of the application code to the working directory
#COPY ../../Downloads/Web-Blog-python .

# Copy the TAR archive to the working directory
# RUN tar -xf My_SAMPLE.tar


# Extract the contents of the TAR archive


COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

# Set the command to run the application
CMD [ "python3", "main.py" ]
