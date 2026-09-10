# Usage

The README covers the basics. This page collects the
longer examples and the notes that did not fit up front.

## Basic

```bash
./target/release/byteview src/*.rs
cat README.md | ./target/release/byteview
```

## Notes

- Zero dependencies outside std
- Parallel over files with std threads
