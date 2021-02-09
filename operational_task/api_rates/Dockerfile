FROM python:latest
LABEL maintainer="Eugene Papkou"
COPY operational-task-git/rates/ .
EXPOSE 3000
RUN DEBIAN_FRONTEND=noninteractive apt-get update && apt-get install -y python-pip && \
    pip install -U gunicorn && \
    pip install -Ur requirements.txt
CMD [ "gunicorn", "-b", ":3000", "wsgi"]