#os 
FROM python:3.11-alpine 

# this enables logs to be displayed in container terminal immediately
ENV PYTHONUNBUFFERED=1

# directory
WORKDIR /django 

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

#copy everythong in src to current directory
COPY . .


CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]