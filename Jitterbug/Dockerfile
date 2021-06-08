FROM ubuntu:16.04 
LABEL software="jitterbug"
RUN apt-get update
RUN apt-get -y install pip git
RUN pip install pysam==0.8.1 numpy
RUN pip install matplotlib matplotlib-venn
RUN pip install pybedtools psutil pandas memory_profiler 
RUN git clone https://github.com/elzbth/jitterbug.git


CMD ["jitterbug"]
