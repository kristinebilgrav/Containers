FROM kristinebilgrav/tiddit 
LABEL software="lumpy"
ENV PATH=/opt/anaconda/bin:${PATH}


RUN conda install -c bioconda pysam sambamba 
RUN conda install -c bioconda samblaster  lumpy-sv



