# Dockerfile for Frontend Service
FROM python:3.12-slim

#creating a working app directory
WORKDIR /app
# copying the app files to the container (main.py, requirements.txt)
COPY . .
# install dependecies
RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 5002

# because the app located in /app and the main.py is in app/src/main.py i need to specify the new location
CMD ["python", "src/main.py"]
