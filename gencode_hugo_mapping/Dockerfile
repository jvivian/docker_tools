FROM ubuntu:14.04

RUN sudo apt-get update && sudo apt-get install -y python-dev python-pip
RUN sudo pip install pandas

RUN mkdir /opt/mapping
RUN mkdir /data

COPY attrs.tsv /opt/mapping/
COPY gencode_hugo_map.py /opt/mapping/

WORKDIR /data

ENTRYPOINT ["python", "/opt/mapping/gencode_hugo_map.py"]