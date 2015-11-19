# Build Debian Java8 via Docker

Use docker to build Java8 Debian packages for Debian Wheezy (7.7)

    sudo docker build -t java8-deb .
    sudo docker run --rm -i java8-deb cat oracle-java8.zip > oracle-java8.zip
    sudo docker rmi java8-deb

Extract packages from `java8-deb.zip` and install them on your system

    sudo apt-get install java-common locales
    unzip oracle-java8.zip
    sudo dpkg -i oracle-java8-bin_8*.deb oracle-java8-fonts_8.*.deb oracle-java8-jre_8.*.deb
