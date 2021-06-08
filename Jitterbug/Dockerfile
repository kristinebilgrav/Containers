FROM ubuntu:16.04 
LABEL software="jitterbug"
RUN apt-get update
RUN apt-get -y install python3-pip git wget
RUN wget https://repo.continuum.io/miniconda/Miniconda2-latest-Linux-x86_64.sh


RUN pip install pysam==0.8.1 numpy
RUN pip install matplotlib matplotlib-venn
RUN pip install pybedtools psutil pandas memory_profiler 
RUN git clone https://github.com/elzbth/jitterbug.git


CMD ["jitterbug"]
