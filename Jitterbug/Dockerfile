FROM ubuntu:16.04 
LABEL software="jitterbug"

ENV PATH=/opt/anaconda/bin:${PATH}

RUN apt-get update
RUN apt-get -y install python3-pip git wget
RUN wget https://repo.continuum.io/miniconda/Miniconda2-latest-Linux-x86_64.sh
RUN chmod 700 ./Miniconda2-latest-Linux-x86_64.sh
RUN bash ./Miniconda2-latest-Linux-x86_64.sh -b -p /opt/anaconda/

RUN export PATH=/opt/anaconda/bin:${PATH}

RUN conda config --add channels defaults conda-forge bioconda

RUN pip install pysam==0.8.1 numpy
RUN pip install matplotlib matplotlib-venn
RUN pip install pybedtools psutil pandas memory_profiler 
RUN git clone https://github.com/elzbth/jitterbug.git


CMD ["jitterbug"]
