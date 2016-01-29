FROM continuumio/anaconda

RUN mkdir /opt/mapping
RUN mkdir /data

COPY attrs.tsv /opt/mapping/
COPY gencode_hugo_map.py /opt/mapping/

WORKDIR /data

ENTRYPOINT ["python", "/opt/mapping/gencode_hugo_map.py"]