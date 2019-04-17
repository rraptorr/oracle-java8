Please note that Java 8 reached its end of public updates and Oracle will not release any more updates after January 2019. For details please see https://www.oracle.com/technetwork/java/java-se-support-roadmap.html

Introduction
------------

Java 8 packages for Debian.

Supported Debian versions
-------------------------

So far packages were tested on following Debian versions:

- stretch i386/amd64
- jessie i386/amd64
- wheezy i386/amd64

I do not have resources to test packages on Ubuntu. However, if one
finds any problem on Ubuntu, feel free to report an issue and I will
try to resolve it.

Usage
-----

To create packages on your own:

- apt-get install debhelper
- git clone git://github.com/rraptorr/oracle-java8.git
- cd oracle-java8
- download jdk-8u211-linux-x64.tar.gz and jdk-8u211-linux-i586.tar.gz
- sh ./prepare.sh
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
