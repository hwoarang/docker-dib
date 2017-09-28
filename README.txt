Docker image to build OPNFV XCI OS images using diskimage-builder

It's probably not very useful outside of an OPNFV XCI environment :)

The recommended way to use it

docker run --rm --privileged=true -e ONE_DISTRO=<opensuse|centos|ubuntu> -t -v `pwd`:`pwd` -w `pwd` hwoarang/docker-dib-xci '/usr/bin/do-build.sh'
