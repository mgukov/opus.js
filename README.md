# Opus Recorder

A javascript library to encode/decode audio in Opus format. Audio encoded and decoded using libopus v1.1.4. Audio resampling is performed by speexDSP 1.2RC3. 
Encoded and muxed audio will be returned as typedArray.

### Usage

---------
### Building from sources

Prebuilt sources are included in the dist folder. However below are instructions if you want to build them yourself. Opus and speex are compiled without SIMD optimizations. Performace is significantly worse with SIMD optimizations enabled.

[Install EMScripten](https://kripken.github.io/emscripten-site/docs/getting_started/downloads.html)

Install autoconf, automake, libtool and pckconfig.
On Mac you can do this using [MacPorts](https://www.macports.org/install.php)
`sudo port install automake autoconf libtool pkgconfig`

Make the dependencies using command `make`!
