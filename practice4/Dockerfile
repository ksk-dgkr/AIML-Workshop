FROM python:3.8.10

WORKDIR /app

COPY requirements.txt requirements.txt

RUN pip install -r requirements.txt

COPY ./myfirstnn.pickle /app/myfirstnn.pickle

COPY ./src /app/src

CMD ["python", "./src/app.py"]

#docker build command --> docker build -t myapp:v1.0 .
#run command --> docker run -p 8410:8410 myapp:v1.0
#inside container --> docker exec -it 24e06e2f36b9 /bin/bash

#docker push gkaushika/ai_workshop8:v1.0