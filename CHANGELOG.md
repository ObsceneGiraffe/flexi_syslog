# Changelog

# [Unreleased]

# [0.4.1] - 2022-01-23

* Added lints to the clippy script to avoid submitting debug code in future.
* Added doc comment to custom time format.
* Removed dbg! code.

# [0.4.0] - 2022-01-18

This release makes breaking changes to the API!

* Added a custom Formatter5424 that implements the timestamp correctly with 6 fractional digits.
* Added `time` crate to allow formatting timestamp correclty.
* Changed the `Builder::build` signiture to take a `flexi_syslog::Formatter5424`.

# [0.3.0] - 2022-01-18

This release makes breaking changes to the API!

* Changed the hard coded formatter to the syslog 5424 standard.
* Changed the `Builder::build` signiture to take a `syslog::Formatter5424`.

# [0.2.2] - 2021-12-30

* Added compiler lints
* Added more documentation
* Changed default_format fn to the documented format.

# [0.2.1] - 2021-12-30

* Changed example in the readme to a the working 0.2.0 `example/basic.rs`

# [0.2.0] - 2021-12-29

This release makes breaking changes to the API!

* Added `syslog` crate and `flexi-syslog` now publically depends on it.
* Added `syslog` implementation of `flexi-logger::LogWriter`.
* Removed libc implementation of `flexi-logger::LogWriter`.

# [0.1.0] - 2021-12-19

* Added `flexi-logger::LogWriter` targetting syslog through libc. 
