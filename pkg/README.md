# Image Effects

This is a mini project to learn about `webassembly` with the help of `rust` language. The concept is image processing

## Rust Tools

  1. `rustup` - a tool for managing different versions of rust
  2. `rustc`  - a tool for compiling rust code
  3. `cargo`  - a tool for managing rust packages and projects

## How to create a new project?

  1. Binary Project - Executable Program

  ```bash
cargo init
  ```

  2. Library Project - Dependency for other Programs

  ```bash
cargo init --lib
  ```

## Installing dependent node packages

  1. webpack

```bash
npm install -D webpack webpack-cli webpack-dev-server
```

  2. [HTML Webpack Plugin](https://www.npmjs.com/package/html-webpack-plugin)

```bash
npm install -D html-webpack-plugin
```

  3. [wasm-pack](https://rustwasm.github.io/wasm-pack/)

      * [wasm-pack npm package](https://www.npmjs.com/package/@wasm-tool/wasm-pack-plugin)

```bash
npm install -D @wasm-tool/wasm-pack-plugin
```

  4. Add [wasm-bindgen](https://crates.io/crates/wasm-bindgen) to `.toml` file

```
wasm-bindgen = "0.2.78"
```

  5. Add [web-sys](https://crates.io/crates/web-sys) to `.toml` file under `dependencies.web-sys` table. This is to export JS functions into rust. We're importing `console.log`

```
version = "0.3.55"
features = ["console"]
```

  6. Add [base64](https://crates.io/crates/base64) to `.toml` file

```
base64 = "0.13.0"
```

  7. Add [image](https://crates.io/crates/image) to `.toml` file

```
image = "0.23.14"
```

## How to run this app?

```bash
npm run serve
```

### VSC extensions

  - [Even Better TOML](https://marketplace.visualstudio.com/items?itemName=tamasfe.even-better-toml)
  - [Rust](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust)

### Resources

  * [Rust Package registry](https://crates.io/)
  * [Rustup Book](https://rust-lang.github.io/rustup/)
  * [Awesome WebAssembly Languages](https://github.com/appcypher/awesome-wasm-langs)
  * [Primitive Data Types in Rust](https://www.codingame.com/playgrounds/365/getting-started-with-rust/primitive-data-types)
  * [Operators and Symbols](https://doc.rust-lang.org/book/appendix-02-operators.html)
  * [Enum image::DynamicImage](https://docs.rs/image/0.19.0/image/enum.DynamicImage.html)