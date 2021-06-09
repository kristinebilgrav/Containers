FROM ubuntu:16.04
LABEL software="STEAK"
ENV PATH=/opt/anaconda/bin:${PATH}
RUN apt-get update
RUN apt-get -y install git wget python3-pip gcc libboost-all-dev mpi bedtools
RUN git clone https://github.com/applevir/STEAK.git
RUN cd STEAK/ &&  make
