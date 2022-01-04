FROM python:3.6 as builder
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

FROM builder
ADD . /obmovies
WORKDIR /obmovies
EXPOSE 5000
CMD ["python", "run.py"]
