# liballoc

C binding of `libm` crate for x86 or x86_64 OS, using pure soft-float without SSE or AVX.

## Usage

Download the header file and lib from [releases](https://github.com/plos-clan/libm/releases/tag/release).

Link the library to your project.

## Build

Build directly to get the two target files:

```bash
cargo build --release
```

The production build will be in `target/<target>/release/` directory.

And use `cbindgen` to generate the header file:

```bash
cargo install cbindgen
cbindgen --output math.h
```
