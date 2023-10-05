FROM python:latest
COPY . /app
WORKDIR /app
RUN find wheels -name '*.whl' -print0 | xargs -0 pip install
ENV PYTHONUNBUFFERED 1
CMD ["python","server.py","34802","-b","0.0.0.0"]
