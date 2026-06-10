# Universal RLE Compressor

A simple, educational Run-Length Encoding (RLE) compression and decompression tool written in C.

The goal of this project is to create a **universal** and easy-to-understand compression library that can be used on PC and embedded systems (Like the Raspberry Pi Pico Game Boy).

## Features

- Lossless compression/decompression using RLE
- Works with any binary data (sprites, tilemaps, game assets, etc.)
- Very small and portable C code
- Separate compressor (PC) and decompressor (can run on Game Boy)
- Round-trip verified (compress → decompress = original data)

## Current Status

This is an early learning project. The compressor is functional and correct, but still basic. It works well on data with repeated bytes (e.g. simple backgrounds or large empty areas) and is a solid foundation for more advanced techniques later.

## How to Build

```bash
gcc main.c -o rle_test
./rle_test