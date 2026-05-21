FROM ubuntu:latest
WORKDIR /app
RUN apt-get update\
	&& apt-get upgrade -y\
	&& apt-get install -y python3 python3-pip\
	&& pip install --no-cache-dir --break-system-packages flask
COPY ./api.py api.py
CMD ["python3", "api.py"]
