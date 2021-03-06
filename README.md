# gl-rs

[![Build Status](https://travis-ci.org/bjz/gl-rs.svg?branch=master)](https://travis-ci.org/bjz/gl-rs)

## Overview

The following crates are contained in this repository:

### [gl](https://github.com/bjz/gl-rs/tree/master/gl)

[![Version](https://img.shields.io/crates/v/gl.svg)](https://crates.io/crates/gl) [![License](https://img.shields.io/crates/l/gl.svg)](https://github.com/bjz/gl-rs/blob/master/LICENSE) [![Downloads](https://img.shields.io/crates/d/gl.svg)](https://crates.io/crates/gl)

An OpenGL function pointer loader for the Rust Programming Language.

```toml
[dependencies]
gl = "0.5.2"
```

### [gl_generator](https://github.com/bjz/gl-rs/tree/master/gl_generator)

[![Version](https://img.shields.io/crates/v/gl_generator.svg)](https://crates.io/crates/gl_generator) [![License](https://img.shields.io/crates/l/gl_generator.svg)](https://github.com/bjz/gl-rs/blob/master/LICENSE) [![Downloads](https://img.shields.io/crates/d/gl_generator.svg)](https://crates.io/crates/gl_generator)

Code generators for creating bindings to the Khronos OpenGL APIs.

```toml
[build-dependencies]
gl_generator = "0.4.2"
```

### [khronos_api](https://github.com/bjz/gl-rs/tree/master/khronos_api)

[![Version](https://img.shields.io/crates/v/khronos_api.svg)](https://crates.io/crates/khronos_api) [![License](https://img.shields.io/crates/l/khronos_api.svg)](https://github.com/bjz/gl-rs/blob/master/LICENSE) [![Downloads](https://img.shields.io/crates/d/khronos_api.svg)](https://crates.io/crates/khronos_api)

The Khronos XML API Registry, exposed as byte string constants.

```toml
[build-dependencies]
khronos_api = "1.0.0"
```

## Compiling from source

`khronos_api` uses a git submodule. You will need to initialize it before building:

```sh
git submodule update --init
```

A batch cargo script is provided at `bin/cargo`. [See the script](https://github.com/bjz/gl-rs/blob/master/bin/cargo)
for some example usages.
