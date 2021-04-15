BootStrap:debootstrap 
OSVersion: xenial
MirrorURL:  http://us.archive.ubuntu.com/ubuntu/

%runscript
    echo "going to set up and install - please wait"
    echo "This is what happens when you run the container..."
    lsb_release -a
    echo "checking cmake version..."
    cmake --version
    echo "checking make version..."
    make --version
    echo "checking gcc version..."
    gcc --version
    echo "checking clang version..."
    clang --version
    echo "checking bison version..."
    bison --version
    echo "checking clang version"
%post
    apt update
    apt install -y software-properties-common
    add-apt-repository universe
    apt -y install sudo 
    apt -y install build-essential curl git man wget vim autoconf libtool bison flex cmake clang-3.8 libelf-dev libboost-all-dev libdwarf-dev zlib1g-dev libtbb-dev binutils-dev libiberty-dev
    apt -y install python
    apt clean
%help

%test
 
%environment
