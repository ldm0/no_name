# A Demo of Rust using FFmpeg library with FFI

To build it:

0. Compile FFmpeg in Linux.

1. The `src/binding.rs` is generated with `rust-bindgen`. You'd better generate it with corresponding header file(`avformat.h` and `avcodec.h`) since the FFmpeg api changes overtime.

2. Put this folder into the same directory where `lib` and `include` folder compiled from FFmpeg is in.

3. Run with `bash run.sh` or `RUSTFLAGS=-Awarnings cargo run -- bear.mp4` Since the `src/binding.rs` is auto-gen and `src/main.rs` is ported from C, tons of warning about style will emits.

LICENSE:

I forget where I get the `bear.mp4`.... Expect from that. Everything is under WTFPL.
