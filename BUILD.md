# Build Instructions for nullclaw (ARMv6)

This repository distributes a pre-compiled static binary of nullclaw, optimized for 32-bit ARMv6 Linux systems (e.g., Raspberry Pi Model B, Raspberry Pi Zero).

The binary was built from source using Zig 0.15.2 with the following exact command:

```bash
zig build \
  -Doptimize=ReleaseSmall \
  -Dtarget=arm-linux-gnueabihf \
  -Dcpu=arm1176jzf_s
