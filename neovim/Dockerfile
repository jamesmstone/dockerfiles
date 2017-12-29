FROM alpine:edge
ENV PATH "/root/bin:$PATH"
ENV CMAKE_EXTRA_FLAGS=-DENABLE_JEMALLOC=OFF
RUN echo "http://dl-cdn.alpinelinux.org/alpine/edge/testing" >> /etc/apk/repositories && \
    apk add --update-cache --virtual build-deps --no-cache \
    curl \
    autoconf \
    automake \
    cmake \
    g++ \
    libtool \
    libuv \
    linux-headers \
    lua5.3-dev \
    m4 \
    make \
    unzip \
    libtermkey-dev \
    lua-sec \
    git \
    libtermkey \
    unibilium \
    libgcc  && \
    git clone --depth=1 https://github.com/neovim/libvterm.git && \
    cd libvterm && \
    make && \
    make install && \
    cd ../ && rm -rf libvterm && \
    git clone --depth=1 https://github.com/neovim/neovim.git nvim && \
    cd nvim && \
    make CMAKE_BUILD_TYPE=Release && \
    make install && \
    cd .. && \
    rm -rf nvim && \
echo "would be nice to remove build-deps" #    apk del build-deps

ENTRYPOINT nvim
