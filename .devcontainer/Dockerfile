FROM mcr.microsoft.com/devcontainers/rust:1-1-bullseye

# Add wasm target
RUN rustup target add wasm32-unknown-unknown

# Install wasm-pack for testing
RUN curl https://rustwasm.github.io/wasm-pack/installer/init.sh -sSf | sh

# Install binstall
RUN curl -L --proto '=https' --tlsv1.2 -sSf https://raw.githubusercontent.com/cargo-bins/cargo-binstall/main/install-from-binstall-release.sh | bash

# Use Binstall to install trunk
RUN cargo binstall --no-confirm trunk



