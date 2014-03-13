Java 8 is still a work in progress and so is this package. Things can
change anytime without any compatibility concerns.

Introduction
------------

Java 8 packages for Debian.

Supported Debian versions
-------------------------

So far packages were tested on following Debian versions:

- jessie i386/amd64
- wheezy i386/amd64

Packages are compatible with "official" Debian ones of Java 6, but
have a lower priority (use update-java-alternatives if you have Java 6
already installed).

I do not have resources to test packages on Ubuntu. However, if one
finds any problem on Ubuntu, feel free to report an issue and I will
try to resolve it.

Usage
-----

To create packages on your own:

- apt-get install dpkg-dev
- git clone git://github.com/rraptorr/oracle-java8.git
- cd oracle-java8
- Download jdk-8-fcs-bin-b132-linux-i586-04_mar_2014.tar or
  jdk-8-fcs-bin-b132-linux-x64-04_mar_2014.tar from
  <http://jdk8.java.net/download.html> (depending on your
  architecture)
- dpkg-buildpackage -uc -us
- install any missing packages that dpkg-buildpackage complains about
  and repeat

Legal
-----

Oracle does not permit to distribute repackaged binaries of Java, so
be advised that hosting any public repository with Java packages is
probably illegal (at least in some parts of the world).

On the other hand, this repository contains only scripts, that allows
one to repackage Oracle Java in Debian friendly way. No binaries are
or will be hosted.

Thanks
------

If this saved you some time you can thank me with some bitcoins:
1java8a15RHQPzyrSPMFTNnRvDohZa7Ui
