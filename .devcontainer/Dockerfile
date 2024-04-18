FROM ubuntu:22.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt update
RUN apt upgrade -y
RUN apt install -y python3 python3-pip
RUN pip3 install --upgrade pip

# Install Git
RUN apt install -y git

# Install IVerilog and GTKWave
RUN apt install -y iverilog gtkwave

# Install Requirements
COPY ../test/requirements.txt requirements.txt
RUN pip3 install -r requirements.txt