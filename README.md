# byteview

Learning Rust by rewriting coreutils, one tool at a time

Built for my own use; public in case it helps someone.

## What it does

- Reads stdin or multiple files
- Parallel over files with std threads
- Counts lines, words and bytes like wc
- Zero dependencies outside std

## How to use

```bash
./target/release/byteview src/*.rs
cat README.md | ./target/release/byteview
```

## Install

```bash
cargo build --release
```

## Project structure

```text
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── faq.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── src/
│   └── main.rs
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── Cargo.toml
└── SECURITY.md
```

## Development

```bash
cargo build
cargo clippy -- -D warnings
```

## Changelog

- `0.1.1` - fix edge case in argument parsing
- `0.1.0` - first working version
