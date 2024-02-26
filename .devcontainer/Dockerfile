# Install Base Image
FROM rust:latest as builder

# Add wasm target
RUN rustup target add wasm32-unknown-unknown

# Install wasm-pack for testing
RUN curl https://rustwasm.github.io/wasm-pack/installer/init.sh -sSf | sh

# Install trunk
RUN cargo install --git https://github.com/trunk-rs/trunk trunk



