# rusty_time

> **This repository has moved.** `rusty_time` now lives at
> [`crates/rusty_time`](https://github.com/Rusty-Mill/rusty_mill/tree/main/crates/rusty_time)
> in the [`rusty_mill`](https://github.com/Rusty-Mill/rusty_mill) monorepo, with full commit
> history preserved. This repository is kept for historical reference and is no longer
> developed; please open issues and pull requests against `rusty_mill` instead.

A `#![no_std]` + `alloc` sovereign `Date`, `Time`, `DateTime`, RFC 3339/ISO-8601
parser/formatter, and timezone-offset calculation crate for the **Rusty Mill**
ecosystem — a dependency-free alternative to crates like `time` and `chrono` for
consumers that don't want them.

## Status
Active — @baileyrd.

## Getting started
```bash
git clone https://github.com/baileyrd/rusty_time
cd rusty_time
cargo build
cargo test
```

`rusty_std` is a pinned `git` dependency (see `Cargo.toml`), so no sibling checkout
is needed — `cargo build` resolves it on its own, including as a `git` dependency of
some other crate.

## Architecture
See [ARCHITECTURE.md](./ARCHITECTURE.md) for boundaries, key decisions, and data flow.

## Development
```bash
cargo test              # unit tests
cargo clippy --all-targets -- -D warnings
cargo fmt --check
```

## Contributing
See [CONTRIBUTING.md](./CONTRIBUTING.md).

## Security
See [SECURITY.md](./SECURITY.md) to report a vulnerability.

## License
MIT OR Apache-2.0 (see `Cargo.toml`).
