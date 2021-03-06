# RustCrypto: Cipher Feedback Mode (CFB)

[![Crate][crate-image]][crate-link]
[![Docs][docs-image]][docs-link]
![Apache2/MIT licensed][license-image]
![Rust Version][rustc-image]
[![Build Status][build-image]][build-link]
[![HAZMAT][hazmat-image]][hazmat-link]

Generic [Cipher Feedback (CFB)][1] mode implementation as a
[self-synchronizing stream cipher][2].

[Documentation][docs-link]

<img alt="diagram" src="https://raw.githubusercontent.com/RustCrypto/meta/master/img/stream-ciphers/cfb.png" width="500px">

## ⚠️ Security Warning: [Hazmat!][hazmat-link]

This crate does not ensure ciphertexts are authentic (i.e. by using a MAC to
verify ciphertext integerity), which can lead to serious vulnerabilities
if used incorrectly!

No security audits of this crate have ever been performed, and it has not been
thoroughly assessed to ensure its operation is constant-time on common CPU
architectures.

USE AT YOUR OWN RISK!

## Minimum Supported Rust Version

Rust **1.41** or higher.

Minimum supported Rust version can be changed in the future, but it will be
done with a minor version bump.

## SemVer Policy

- All on-by-default features of this library are covered by SemVer
- MSRV is considered exempt from SemVer as noted above

## License

Licensed under either of:

 * [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
 * [MIT license](http://opensource.org/licenses/MIT)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
dual licensed as above, without any additional terms or conditions.

[//]: # (badges)

[crate-image]: https://img.shields.io/crates/v/cfb-mode.svg
[crate-link]: https://crates.io/crates/cfb-mode
[docs-image]: https://docs.rs/cfb-mode/badge.svg
[docs-link]: https://docs.rs/cfb-mode/
[license-image]: https://img.shields.io/badge/license-Apache2.0/MIT-blue.svg
[rustc-image]: https://img.shields.io/badge/rustc-1.41+-blue.svg
[hazmat-image]: https://img.shields.io/badge/crypto-hazmat%E2%9A%A0%EF%B8%8F-red.svg
[hazmat-link]: https://github.com/RustCrypto/meta/wiki/About-%22hazmat%22-crates
[build-image]: https://github.com/RustCrypto/stream-ciphers/workflows/cfb-mode/badge.svg?branch=master&event=push
[build-link]: https://github.com/RustCrypto/stream-ciphers/actions?query=workflow%3Acfb-mode

[//]: # (footnotes)

[1]: https://en.wikipedia.org/wiki/Block_cipher_mode_of_operation#CFB
[2]: https://en.wikipedia.org/wiki/Stream_cipher#Self-synchronizing_stream_ciphers
