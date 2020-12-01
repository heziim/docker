FROM alpine:3.9

LABEL maintainer="hezi.im@gmail.com"

RUN apk update &&  apk add python3 py3-pip

RUN pip3 install --upgrade pip &&  pip3 install click==7.0 flask==1.0.2 itsdangerous==1.1.0 jinja2==2.10 markupsafe==1.1.1 werkzeug==0.14.1

COPY app.py /tmp

EXPOSE 5000

RUN chmod +x /tmp/app.py 

ENTRYPOINT ["python3","/tmp/app.py"]





