# Raspberry Pi Build/Usage Instructions

All of this sample code will build on a Raspberry Pi, which can then be used
as an inexpensive print server or as part of an automated test framework.  All
of the commands in this file assume you are using the Raspbian OS.


## Prerequisites

Run the following command to install the core software you'll need to build and
use all of the ippsample code:

    sudo apt-get install build-essential autoconf avahi-daemon avahi-utils \
        cura-engine libavahi-client-dev libnss-mdns libpam-dev libssl-dev \
        zlib1g-dev

Prerequisites for just 2D printing:

    sudo apt-get install build-essential autoconf avahi-daemon avahi-utils \
        libavahi-client-dev libnss-mdns libpam-dev libssl-dev zlib1g-dev

Prerequisites for just 3D printing:

    sudo apt-get install build-essential autoconf avahi-daemon avahi-utils \
        cura-engine libavahi-client-dev libnss-mdns libpam-dev libssl-dev \
        zlib1g-dev


## Building the IPP Sample Code

If you haven't already done so, you can download the latested IPP sample sources
with Git using:

    git clone --recurse-submodules https://github.com/istopwg/ippsample.git

Then, from the ippsample source directory, run the following commands to
build and install everything:

    ./configure
    make
    sudo make install


## Using the IPP Server

The `sample-configs` directory contains sample configuration directories for
`ippserver` to do different things.

> Work in progress here...
