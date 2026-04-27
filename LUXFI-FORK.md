# LUXFI-FORK

This is a luxfi-maintained fork of [BLAKE3-team/BLAKE3](https://github.com/BLAKE3-team/BLAKE3).

## Pin

* Upstream tag: `1.8.5`
* License: dual-licensed CC0-1.0 / Apache-2.0 (see `LICENSE` and
  `LICENSE_APACHE`)

## Why this fork exists

BLAKE3 is the canonical reference implementation. luxcpp/crypto/blake3
maintains a first-party C++ port (the port is independent of upstream code;
KAT vectors come from this fork). luxfi pins the upstream so test-vector
files cannot drift.

## Sync policy

* Track upstream tagged releases only.
* Pull tags into `sync/<tag>` branches. Re-run BLAKE3 KATs in
  luxcpp/crypto/blake3 against the new test vectors. Merge to `master` only
  when KATs pass.
* The BLAKE3 algorithm is final — any change to the spec is a hard stop.

## Maintainer

luxfi crypto team. Contact via the `luxfi/crypto` repo.
