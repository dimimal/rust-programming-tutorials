# Rust Programming Tutorials

A collection of small Rust tutorial projects and examples to help you learn the language by doing. Each folder contains a tiny Cargo project (or example) demonstrating a core Rust concept.

## Contents

- `hello-world/` — very small programs (including a simple `helloworld` and `guessing_game`).
- `hello_cargo/` — demonstrates creating and building a Cargo package.
- `ownership/` — examples that explain Rust's ownership model.
- `programming_concepts/` — subfolders for control flow, datatypes, functions, etc.
- `structs/` — examples showing structs and associated methods.

## Getting started

Prerequisites
- Rust toolchain (install via rustup): https://rustup.rs
- Recommended: `cargo`, `rustc`, and `rust-analyzer` for editor support.

Quick commands

Build a crate (from the crate folder):

```bash
cd hello_cargo
cargo build

# run the binary
cargo run
```

Build and run the guessing game example:

```bash
cd hello-world/guessing_game
cargo run
```

Build all workspace crates (simple approach using find):

```bash
# from the repo root
find . -maxdepth 3 -type f -name Cargo.toml -execdir cargo build \;
```

Run tests (where present):

```bash
cd path/to/crate
cargo test
```

## Project structure and notes

This repository is intentionally organized as individual small projects so you can open a single folder in your editor and focus on a single topic. Each subfolder contains a `Cargo.toml` and a `src/main.rs` unless the folder is purely an example.

IDE / Editor recommendations

- Visual Studio Code with the `rust-analyzer` extension.
- Install `rustfmt` and `clippy` for formatting and linting:

```bash
rustup component add rustfmt clippy
```

Contributing

Contributions and pull requests are welcome. Suggested small ways to contribute:

- Add more small examples and short comments explaining tricky parts.
- Add exercises or small challenges with solutions under an `exercises/` folder.
- Improve README or per-project READMEs with usage notes.

License

This repository is provided under the MIT license by default. If you want a different license, update this file and add a `LICENSE` file.

---

If you want, I can:

- Commit this `README.md` and finish the initial commit for the repo, or
- Create a richer README with per-crate example commands and badges.

Tell me which you prefer and I will proceed.
