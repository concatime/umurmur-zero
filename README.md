# _Purely_ static μMurmur
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg?longCache=true&style=flat-square)](//github.com/semantic-release/semantic-release)
[![ISC License](https://img.shields.io/badge/license-ISC-brightgreen.svg?longCache=true&style=flat-square)](//www.isc.org/downloads/software-support-policy/isc-license/)
[![Build Status](https://travis-ci.org/concatime/umurmur-zero.svg?branch=master)](//travis-ci.org/concatime/umurmur-zero)

Package | Version | Latest available
:------:|---------|-
Musl    | 1.1.20  | [![](https://repology.org/badge/latest-versions/musl.svg)](//git.musl-libc.org/cgit/musl/tree/WHATSNEW)
LibreSSL| 2.9.0   | [![](https://repology.org/badge/latest-versions/libressl.svg)](//raw.githubusercontent.com/libressl-portable/portable/master/ChangeLog)
Protobuf| 3.6.1.3 | [![](https://repology.org/badge/latest-versions/protobuf.svg)](//raw.githubusercontent.com/protocolbuffers/protobuf/master/CHANGES.txt)

By default, jemalloc is now disabled since it causes boilerplate.

The script (`nginx-zero`) requires:
 - gcc or clang>=3.5 (otherwise, `ld: cannot find -l-user-{start,end}`)
 - tar (+gzip)
 - git
 - make
 - cmake
 - patch

To clone:
`git clone --recurse-submodules -j8 https://github.com/concatime/umurmur-zero.git`

To install, download the release file called `umurmur.tar.gz`, and then
`sudo tar xf nginx.tar.gz -C/opt`

### Notes (for me)
In `deps/jemalloc/.gitignore`, I need to manually remove `configure`.
