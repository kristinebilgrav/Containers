FROM ubuntu:16.04 
LABEL software="TIDDIT"
ENV PATH=/opt/anaconda/bin:${PATH}
RUN apt-get update
RUN apt-get -y install cmake git wget python3-pip
RUN wget https://repo.continuum.io/miniconda/Miniconda2-latest-Linux-x86_64.sh
RUN chmod 700 ./Miniconda2-latest-Linux-x86_64.sh
RUN bash ./Miniconda2-latest-Linux-x86_64.sh -b -p /opt/anaconda/

RUN export PATH=/opt/anaconda/bin:${PATH}

RUN conda config --add channels defaults 
RUN conda config --add channels conda-forge
RUN conda config --add channels bioconda

RUN conda install -c bioconda samtools
RUN pip install numpy cython

#RUN git clone https://github.com/SciLifeLab/TIDDIT.git
RUN conda install tiddit
#RUN cd /TIDDIT
#RUN ./INSTALL.sh

CMD ["tiddit"]


