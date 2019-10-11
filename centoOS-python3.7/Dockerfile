FROM centos:centos7

RUN yum -y update \
    && yum -y install \
    epel-release \
    gcc \
    openssl-devel　\
    bzip2-devel　\
    libffi-devel　\
    git \
    vim \
    which \
    wget \
    make \
    zlib \
    zlib-devel \
    libffi-devel \
    && yum clean all

RUN wget https://www.python.org/ftp/python/3.7.3/Python-3.7.3.tgz \
    && tar xzf Python-3.7.3.tgz \
    && cd Python-3.7.3 \
    && ./configure --enable-optimizations \
    && make altinstall \
    && rm ../Python-3.7.3.tgz

WORKDIR /root
CMD ["/bin/bash"]
