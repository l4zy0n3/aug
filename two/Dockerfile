FROM python:alpine
WORKDIR /app
COPY . /app
RUN pip install -r requirements.txt
CMD ["python", "hello.py"]
EXPOSE 8080