# Setup Rust Cross

![license](https://img.shields.io/github/license/DiscreteTom/setup-rust-cross?style=flat-square)
[![release](https://img.shields.io/github/v/release/DiscreteTom/setup-rust-cross?style=flat-square)](https://github.com/DiscreteTom/setup-rust-cross/releases/latest)

This GitHub Action sets up Rust toolchains and [cross-rs](https://github.com/cross-rs/cross) in your workflow.

## Usage

```yaml
steps:
  - uses: actions/checkout@v4

  - uses: DiscreteTom/setup-rust-cross@v0.1.0

  - name: Build for target
    run: cross build --target x86_64-unknown-linux-gnu
```

## [CHANGELOG](./CHANGELOG.md)
