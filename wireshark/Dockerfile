FROM squareslab/manybugs:base

# necessary to link shared libraries
# https://ubuntuforums.org/showthread.php?t=975334
ENV LD_LIBRARY_PATH "/usr/local/lib:${LD_LIBRARY_PATH}"
ADD doc.patch /experiment/doc.patch

RUN sudo apt-get update && \
    sudo apt-get install --no-install-recommends -y \
                            automake \
                            autoconf \
                            libtool \
                            subversion \
                            pkg-config \
                            bison \
                            flex \
                            libgtk2.0-dev \
                            libpcap-dev \
                            libwww-perl
