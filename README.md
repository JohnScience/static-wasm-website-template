# Template for basic static Rust-powered website

This is a template for a basic static website powered by Rust programming language. It uses only the essential, code-generated JavaScript, which delegates all the heavy lifting to the WebAssembly module compiled from Rust.

## Pre-requisites

- Rust toolchain.
- [`cargo make`].
- [`wasm-pack`].
- [`http-server`] or any other web server of your choice.

## Building

```console
cargo make build-front
```

## Running

In order to run the website, you need to host the created `build` directory with a local web server. Without a server, the website will not work due to the same-origin policy.

If you choose to use [`http-server`], you can run it with the following command

```console
http-server ./build
```

and then it will be available at <http://127.0.0.1:7878/index.html>.

For more information, see `http-server --help`.

## Cloning

```console
git clone 
```

[`cargo make`]: https://crates.io/crates/cargo-make
[`wasm-pack`]: https://rustwasm.github.io/wasm-pack/installer/
[`http-server`]: https://crates.io/crates/http-server
