FROM ubuntu:xenial

# china timezone
RUN echo "Asia/Shanghai" > /etc/timezone

# install compiler, dependencies, tools , dnsmasq
RUN apt-get update && apt-get install -y \
    build-essential wget xz-utils libgnutls28-dev \
    libev-dev libwrap0-dev libpam0g-dev liblz4-dev libseccomp-dev libreadline-dev \
    libnl-route-3-dev libkrb5-dev liboath-dev libprotobuf-c0-dev libtalloc-dev \
    libhttp-parser-dev libpcl1-dev libopts25-dev autogen pkg-config nettle-dev \
    protobuf-c-compiler gnutls-bin gperf liblockfile-bin nuttcp lcov iptables \
    unzip dnsmasq libuid-wrapper libnss-wrapper libsocket-wrapper gss-ntlmssp libpam-oath \
    && rm -rf /var/lib/apt/lists/*