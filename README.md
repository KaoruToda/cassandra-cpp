cassandra-cpp
=============

Cassandra C++ library by thrift

Generated by thrift command with cassandra 1.2.1 and modified for FreeBSD.

- thrift 0.8.0
- cassandra 1.2.1

# How to build and install

Build and install.

    ./configure
    make
    sudo make install

Uninstall

    sudo make uninstall

# How to use

    clang++ foo.cpp -L/usr/local/lib -I/usr/local/include -lcassandracpp
