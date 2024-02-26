# Install Base Image
FROM alpine:3.14

# Install rust
RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

# Add wasm target
RUN rustup target add wasm32-unknown-unknown

# Install wasm-pack for testing
RUN curl https://rustwasm.github.io/wasm-pack/installer/init.sh -sSf | sh

# Install trunk
RUN cargo install --git https://github.com/trunk-rs/trunk trunk



