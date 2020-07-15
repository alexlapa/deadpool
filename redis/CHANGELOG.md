# Change Log

## v0.?.?

* Import `redis` with `default-features = false`.
* Add `tokio-comp` default feature that enables [tokio](https://crates.io/crates/tokio) async runtime.
* Add `async-std-comp` feature that enables [async-std](https://crates.io/crates/async-std) async runtime.

## v0.6.0

* Update `redis` dependency to version `0.16.0`
* Re-export `redis` crate

## v0.5.2

* Update `redis` dependency to version `0.15.1`
* Add `#[derive(Clone)]` to `Config` struct
* Add `Connection` type alias

## v0.5.1

* Disable `default-features` for `deadpool` dependency

## v0.5.0

* Update `redis` dependency to version `0.14.0`
* Rename `query` to `query_async` to match API of `redis` crate
* Rename `execute` to `execute_async` to match API of `redis` crate
* Add support for `config` crate

## v0.4.1

* Add `PoolError` type alias

## v0.4.0

* Rename `Connection` to `ConnectionWrapper`
* Add `Connection` type alias

## v0.3.0

* Add pipeline support
* Add wrappers for `Cmd` and `Pipeline` to mimick the API of the `redis` crate
* Make recycling more robust by changing the `Manager::recycle` to a non
  consuming API.
* Add proper connection using the `PING` command

## v0.2.0

* First release
