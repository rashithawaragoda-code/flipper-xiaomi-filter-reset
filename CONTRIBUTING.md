# Contributing

Thanks for your interest in improving Xiaomi Filter Reset!

## Ground rules

- **Conventional Commits.** Prefix messages with `feat:`, `fix:`, `docs:`, `test:`,
  `chore:`, `ci:`, `refactor:`, etc. Example: `fix: verify counter page after write`.
- **English** for code, comments, and documentation.
- Keep changes focused; one logical change per PR.

## Development setup

```sh
python3 -m pip install --user ufbt   # micro Flipper Build Tool
ufbt                                 # build the FAP (downloads the SDK on first run)
```

## Before you open a PR

Run all of the following and make sure they pass:

```sh
make -C test test    # host unit tests (also enforces the strict warning set)
ufbt                 # the FAP must build clean
ufbt lint            # formatting must be clean
```

If you change formatting-affecting code, run `ufbt format` to apply the project's
`.clang-format`.

## Where things go

- Pure, testable logic (crypto, memory map, parsing) → `src/core/`. It must **not**
  include firmware headers, and **must** come with a host test in `test/`.
- NFC/tag interaction → `src/nfc/`.
- UI → `scenes/`.

See [`CLAUDE.md`](./CLAUDE.md) for architecture and the hardware-verified protocol
facts, and [`docs/protocol.md`](./docs/protocol.md) for the reverse-engineering
details.

## Testing on hardware

CI cannot exercise the NFC stack. If you touch `src/nfc/` or scene navigation, please
test on a real Flipper against a real Xiaomi filter and describe the result in your PR.

## Reporting compatibility

If you reset (or fail to reset) a filter, an issue noting the purifier model and the
on-tag product code shown by the app (e.g. `AP11`) helps grow the compatibility list.
