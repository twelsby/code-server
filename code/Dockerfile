FROM codercom/code-server
USER root
RUN curl -fsSL https://deb.nodesource.com/setup_current.x | sudo -E bash - && \
    apt update && \
    apt dist-upgrade -y && \
    apt install -y \
      build-essential \
      cmake \
      gdb \
      libboost-all-dev \
      openssl \
      libssl-dev \
      pkg-config \
      nodejs && \
    curl https://sh.rustup.rs -sSf | bash -s -- -y && \
    . ~/.cargo/env && \
    cargo install wasm-pack cargo-generate
