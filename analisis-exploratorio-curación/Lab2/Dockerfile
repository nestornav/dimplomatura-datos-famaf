# Use an official Python runtime as a parent image
FROM jupyter/scipy-notebook

# Set the working directory to /app
WORKDIR /app

COPY requirements.txt /app/

# Install any needed packages specified in requirements.txt
RUN pip install -r requirements.txt && python -m spacy download es_core_news_sm

# Copy the app code and dependencies file into the container at /app
COPY . /app/

# Make port 80 available to the world outside this container
EXPOSE 80

