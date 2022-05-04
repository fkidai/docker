FROM ubuntu:20.04

RUN apt-get update
RUN apt-get install -y python3 python3-pip curl

RUN apt-get install -y git sudo

#pip   jupyterもrequirements.txtに書いてあるのが前提
COPY ./jupyter_lab/build/requirements.txt /tmp
RUN pip3 install --no-cache-dir -r /tmp/requirements.txt

#これを設定しないPythonで日本語を扱えない
ENV PYTHONIOENCODING utf-8
ENV LANG C.UTF-8
ENV LC_ALL C.UTF-8
