# Changelog

All notable changes to bootstrap will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [Non-breaking changes since the last major version]

- Add a changelog for x.py [#76626](https://github.com/rust-lang/rust/pull/76626)
- Optionally, download LLVM from CI on Linux and NixOS
  + [#76439](https://github.com/rust-lang/rust/pull/76349)
  + [#76667](https://github.com/rust-lang/rust/pull/76667)
  + [#76708](https://github.com/rust-lang/rust/pull/76708)
- Distribute rustc sources as part of `rustc-dev` [#76856](https://github.com/rust-lang/rust/pull/76856)
- Make the default stage for x.py configurable [#76625](https://github.com/rust-lang/rust/pull/76625)
- Add a dedicated debug-logging option [#76588](https://github.com/rust-lang/rust/pull/76588)
- Add sample defaults for x.py [#76628](https://github.com/rust-lang/rust/pull/76628)
- Add `--keep-stage-std`, which behaves like `keep-stage` but allows the stage
  0 compiler artifacts (i.e., stage1/bin/rustc) to be rebuilt if changed
  [#77120](https://github.com/rust-lang/rust/pull/77120).


## [Version 0] - 2020-09-11

This is the first changelog entry, and it does not attempt to be an exhaustive list of features in x.py.
Instead, this documents the changes to bootstrap in the past 2 months.

- Improve defaults in `x.py` [#73964](https://github.com/rust-lang/rust/pull/73964)
  (see [blog post] for details)
- Set `ninja = true` by default [#74922](https://github.com/rust-lang/rust/pull/74922)
- Avoid trying to inversely cross-compile for build triple from host triples [#76415](https://github.com/rust-lang/rust/pull/76415)
- Allow blessing expect-tests in tools [#75975](https://github.com/rust-lang/rust/pull/75975)
- `x.py check` checks tests/examples/benches [#76258](https://github.com/rust-lang/rust/pull/76258)
- Fix `rust.use-lld` when linker is not set [#76326](https://github.com/rust-lang/rust/pull/76326)
- Build tests with LLD if `use-lld = true` was passed [#76378](https://github.com/rust-lang/rust/pull/76378)

[blog post]: https://blog.rust-lang.org/inside-rust/2020/08/30/changes-to-x-py-defaults.html
