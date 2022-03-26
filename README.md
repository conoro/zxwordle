# ZX Wordle
The core Wordle game implemented in C for the ZX Spectrum in 2022 to celebrate 40 years since the launch on April 23rd 1982.

My blogpost about it [is here](https://conoroneill.net/2022/03/26/celebrating-40-years-of-sinclair-zx-spectrum-with-zx-wordle/).

It has the answers for Wordle 272 to 1010 built-in, so it will keep you happy until March 2024. Lots of RAM still available if you want to add even more.

It's obviously missing features like stats/streaks etc unless someone wants to implement saving to tape/DivMMC.

## Building it yourself
It was created using [Z88DK](https://github.com/z88dk/z88dk/). I haven't written C in over 20 years so the code is rubbish. Feel free to improve.

Compile with:

```bash
  zcc +zx -vn -startup=1 -clib=sdcc_iy zxwordle.c -o zxwordle -create-app
```

## Porting
It's all pretty much stdin/stdout including the colour blocks which are just Spectrum INVERSE blocks. So should be trivial to port it to other 8-bit Micros.

 Copyright Conor O'Neill 2022 (conor@conoroneill.com)
 LICENSE: Apache-2.0
 