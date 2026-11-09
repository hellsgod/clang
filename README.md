# LLVM/Clang Builds

Unofficial, precompiled LLVM/Clang toolchains for Linux kernel development.

## About

These builds are compiled on my AMD Ryzen 9 9950X using [tc-build](https://github.com/ClangBuiltLinux/tc-build), with **PGO (Profile-Guided Optimization)** and **ThinLTO** enabled.

Build command:

```bash
./build-llvm.py --pgo kernel-defconfig --lto thin --targets X86 --distribution-profile kernel
```

The toolchain is primarily built for my personal use with my **linux-hC kernel**. I am simply sharing the same builds I use myself, without making additional changes or providing separate configurations.

The builds target **x86-64 Linux** and are intended for **Linux kernel compilation**.

**libclang is included** for Rust and Bindgen support.

New releases are planned approximately once a week, based on the latest available LLVM development sources.

## Scope & Support

- Builds are provided **as-is**, without warranty or support.
- No feature requests or custom build configurations.
- Only the X86 LLVM target is enabled.
- No builds for other architectures or use cases.
- Built on Arch Linux and intended for Arch Linux.
- Other Linux distributions are not tested or officially supported.
- Release frequency is not guaranteed.

## License

LLVM is licensed under the Apache License 2.0 License with LLVM Exceptions (`Apache-2.0 WITH LLVM-exception`).

This repository distributes unofficial, precompiled LLVM/Clang binaries built from the upstream LLVM project.

These builds are not affiliated with or endorsed by the LLVM Project.

Original source code: https://github.com/llvm/llvm-project

See the LICENSE file for the full license terms.
