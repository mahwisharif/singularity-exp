BootStrap: debootstrap
OSVersion: trusty
MirrorURL:  http://us.archive.ubuntu.com/ubuntu/

%runscript
    echo "This is what happens when you run the container..."
    lsb_release -a
    mkdir example
    cd example
    touch example.cpp
%post
    apt-get install -y software-properties-common
    add-apt-repository universe
    apt-get update
    apt-get install -y cowsay
    apt-get clean

%environment
    export PATH="$PATH:/usr/games"
    export LC_ALL=C
