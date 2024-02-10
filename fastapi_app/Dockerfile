FROM python:3.9.10

# copy all necessary files into the container
ADD . /app/

# go into work directory
WORKDIR /app

# Install all useful dependancies for good app running
RUN pip install --no-cache-dir -r requirements.txt

# Expose entry port
EXPOSE 8000

# Running api app command
CMD ["uvicorn", "api_app:app", "--host", "0.0.0.0", "--port", "8000"]
