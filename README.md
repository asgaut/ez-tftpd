# ez-tftpd

A simple tftp server utility, written in Rust.

## Features

- Easy to use: by default serves the files in the current directory
- Multiplatform support - compatible with Linux, MacOS and Windows
- Use it from the command line

## Usage

Just run the executable to serve the files the current directory.

## Building

If desired, you can build ez-tftpd yourself.
You will need a working `Rust` and `Cargo` setup.
[Rustup](https://rustup.rs/) is the simplest way to set this up on either Windows, Mac or Linux.

Once the prerequisites have been installed, compilation on your native platform is done by running the following in a terminal:
```
cargo build --release
```

Building for Windows under Linux using [cross](https://github.com/cross-rs/cross):
```
cross build --release --target x86_64-pc-windows-gnu
```