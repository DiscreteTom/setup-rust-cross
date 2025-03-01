# Setup Rust Cross

![license](https://img.shields.io/github/license/DiscreteTom/setup-rust-cross?style=flat-square)
[![release](https://img.shields.io/github/v/release/DiscreteTom/setup-rust-cross?style=flat-square)](https://github.com/DiscreteTom/setup-rust-cross/releases/latest)

This GitHub Action sets up Rust toolchains and [cross-rs](https://github.com/cross-rs/cross) in your workflow.

## Usage

```yaml
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v4

      - name: Setup Rust toolchains and cross-rs
        uses: DiscreteTom/setup-rust-cross@v0.1.1

      - name: Build
        run: |
          cross build --target aarch64-unknown-linux-musl
```

## [CHANGELOG](./CHANGELOG.md)
