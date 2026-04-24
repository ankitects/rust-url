# percent-encoding-iri

Same API as [`percent-encoding`](https://crates.io/crates/percent-encoding) from [rust-url](https://github.com/servo/rust-url), published on crates.io under this name so projects can depend on a **distinct package** while optionally enabling **IRI-style** behaviour (UTF-8 non-ASCII octets are not forced to percent-encode when the `iri` feature is on).

```toml
percent-encoding-iri = { version = "2.3.2", features = ["iri"] }
```

In Rust, import as **`percent_encoding`** (library name), for example:

```rust
use percent_encoding::{utf8_percent_encode, AsciiSet, CONTROLS};
```

Without the `iri` feature, encoding matches the stock WHATWG-style rule.

Source: <https://github.com/ankitects/rust-url>
