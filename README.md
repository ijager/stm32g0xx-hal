# `stm32g0xx-hal`

*Warning*: Work in progress.

_stm32g0xx-hal_ contains a multi device hardware abstraction on top of the
peripheral access API for the STMicro STM32G0 series microcontrollers. The
selection of the MCU is done by feature gates, typically specified by board
support crates.

## Usage

This crate will eventually contain support for multiple microcontrollers in the
stm32g0 family. Which specific microcontroller you want to build for has to be
specified with a feature, for example `stm32g070`.

### Building an Example

If you are compiling the crate on its own for development or running examples, 
specify your microcontroller on the command line. For example:

```
cargo build --example blinky --features stm32g07x
```

### Using as a Dependency

When using this crate as a dependency in your project, the microcontroller can 
be specified as part of the `Cargo.toml` definition.

```
[dependencies]
stm32g0xx-hal = "0.0.3"
```

## Documentation

The documentation can be found at [docs.rs](https://docs.rs/stm32g0xx-hal/).

## License

Licensed under either of

- Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or
  http://www.apache.org/licenses/LICENSE-2.0)
- MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
dual licensed as above, without any additional terms or conditions.
