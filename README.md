<p align="center">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/613943/213103585-33c79982-617d-4f81-a949-3335b465129a.png">
     <img src="https://user-images.githubusercontent.com/613943/213103583-4399e224-841f-462a-887d-6427f7af7376.png" width="90px">
   </picture>
</p>

---
<img width="320" alt="image" align="right" src="https://user-images.githubusercontent.com/613943/213217673-e58c873a-9219-4a33-8487-620a07210206.png">

**Gõkey** - A Vietnamese input method editor.

- :zap: Excellent performance (Gen Z translation: Blazing fast!)
- :crab: Written completely in Rust.
- :keyboard: Supported both Telex and VNI input method.
- :sparkles: Focused on typing experience and features that you will use.

## About

This is my attempt to build an input method editor using only Rust. It's not the first, and definitely not the last.

The goal is to create an input method editor that enable users to type Vietnamese text on the computer using
either VNI or TELEX method. Other than that, no other features are planned.

## How to install

Currently, since we are still at an early development stage, no pre-built binaries are provided.

But the source code can be compiled easily:

1. Get the latest stable version of the Rust compiler ([see here](https://rustup.rs/))
2. Install the [cargo-bundle](https://github.com/burtonageo/cargo-bundle) extension, this is necessary for bundling macOS apps
3. Checkout the source code of the **gõkey** project
   ```
   git clone https://github.com/huytd/goxkey && cd goxkey
   ```
4. Run the bundle command:

   ```
   cargo bundle
   ```

After that, you'll find the `Gõ Key.app` file in the `target/debug/bundle` folder.

## Dependencies

- [core-foundation](https://crates.io/crates/core-foundation), [core-graphics](https://crates.io/crates/core-graphics): for event handling on macOS
- [vi-rs](https://github.com/zerox-dg/vi-rs): the Vietnamese Input Engine
