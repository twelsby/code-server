FROM codercom/code-server
USER root
RUN apt update && \
    apt dist-upgrade -y && \
    apt install -y \
      build-essential \
      cmake \
      gdb \
      libboost-all-dev && \
    curl https://sh.rustup.rs -sSf | sh -s -y
