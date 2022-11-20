FROM library/rust:1.65.0-bullseye

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        mingw-w64 \
        cmake && \
    rm -rf /var/lib/apt/lists/*

RUN rustup target add i686-pc-windows-gnu x86_64-pc-windows-gnu
