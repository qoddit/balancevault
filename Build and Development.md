# Build and Development

Balance uses CMake and C17, with OpenSSL 3, CURL, Threads, and ncurses/curses dependencies in the available CMake configuration.

## macOS (Homebrew)
```bash
brew install cmake openssl@3 curl
OPENSSL_PREFIX="$(brew --prefix openssl@3)"
cmake -S . -B build -DCMAKE_BUILD_TYPE=Release \
  -DOPENSSL_ROOT_DIR="$OPENSSL_PREFIX" \
  -DOPENSSL_INCLUDE_DIR="$OPENSSL_PREFIX/include" \
  -DOPENSSL_CRYPTO_LIBRARY="$OPENSSL_PREFIX/lib/libcrypto.dylib"
cmake --build build --target balance -j
```

If CMake cannot find OpenSSL, inspect `brew --prefix openssl@3` and configure the paths accordingly. Delete `build/` when switching between operating systems or architectures to avoid stale binaries.

## Linux
Install compiler/build tools, CMake, ncurses development headers, OpenSSL 3 development files, and libcurl development files; then configure and build with CMake.

## Related files
- [[CMakeLists.txt]]
- [[BUILD.md]]
- [[ci.yml]]
- [[CONTRIBUTING.md]]
- [[VERSIONING.md]]
