FROM debian:7.7

RUN apt-get update && \
	apt-get install -y \
    curl \
		debhelper \
    libasound2 \
    libxi6 \
    libxrender1\
    libxt6 \
    libxtst6 \
    lsb-release \
    unixodbc \
    unzip \
    zip

RUN git clone git://github.com/rraptorr/oracle-java8.git && \
  cd oracle-java8 && \
  ./prepare.sh && \
  dpkg-buildpackage -uc -us && \
  cd .. && \
  zip oracle-java8.zip *.deb
