# Contributing to Cardpeek

Thank you for your interest in contributing! Here is how to get started.

## Reporting bugs

Please open a GitHub issue. Include:
- Your operating system and version
- Steps to reproduce the problem
- Any error output or logs

## Building from source

### Linux (Debian/Ubuntu)

Install dependencies:

```sh
sudo apt install autoconf make libglib2.0-dev libglib2.0-bin \
    libgtk-3-dev libgdk-pixbuf2.0-dev liblua5.2-dev \
    libcurl4-openssl-dev libssl-dev libpcsclite-dev libreadline-dev
```

Build:

```sh
autoreconf --install
./configure
make
```

### Windows (MSYS2 / MinGW-w64 64-bit)

See [`doc/build-windows.md`](doc/build-windows.md) for the full Windows build guide.

> **Note:** Produced Windows binaries may not run correctly yet.
> See [issue #1](https://github.com/ipamo/cardpeek/issues/1).

## Submitting changes

1. Fork the repository and create a branch from `master`.
2. Make your changes with clear, focused commits.
3. Ensure the code compiles without warnings on Linux (the CI will check this automatically).
4. Open a pull request against `master` with a clear description of the change.

## Code style

- C source files use tabs for indentation.
- Keep lines reasonably short (the project follows `-Wall -pedantic` gcc flags).
- Follow the existing style in each file.

## License

By submitting a pull request you agree that your contributions will be licensed under the [GNU General Public License v3](COPYING), with the OpenSSL linking exception that applies to the rest of the project.
