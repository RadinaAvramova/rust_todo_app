# Rust Yew Todo Application

# A simple Rust client side Todo App using the Yew Framework.  

### Running it

Clone or download this repository.

You need to have cargo-web installed as well as a suitable target for the Rust compiler to generate web output. 
By default cargo-web uses asmjs-unknown-emscripten. 

#### Rust stable

Install cargo-web and the asmjs and wasm32 emscripten targets as follows:

```
$ cargo install cargo-web
$ rustup target add asmjs-unknown-emscripten
$ rustup target add wasm32-unknown-emscripten
```

For normal Debug build run 
```
$ cargo web start
```

To run an optimised build instead of a debug build use:

```
$ cargo web start --target-webasm-emscripten=wasm32-unknown-emscripten --release
```

#### Rust nightly
If you are using rust nightly you can use the brand new `wasm32-unknown-unknown` target

```
$ cargo install cargo-web
$ rustup target add wasm32-unknown-unknown
$ cargo web start --target-webasm=wasm32-unknown-unknown
```


