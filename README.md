# TLA+ tools: pinned copies

This repository holds unchanged copies of TLA+ tools builds (`tla2tools.jar`), one build per release. Orchestra Works publishes it.

## Why it exists

The TLA+ project publishes its main line as the `v1.8.0` pre-release on GitHub. The project rebuilds that file in place, so its download address does not always return the same file. A tool that checks the jar by SHA-256 needs one file that never changes. Each release here is one such file.

## What each release holds

- `tla2tools.jar`: the jar exactly as the TLA+ project published it. Nothing is added, removed or rebuilt.
- `tla2tools.jar.sha256`: its SHA-256 checksum.
- The release notes name the source address, the TLA+ commit the jar was built from, the build time, and the date of the copy.

Check a download before you run it:

```
sha256sum -c tla2tools.jar.sha256
```

## Source and license

The TLA+ tools come from <https://github.com/tlaplus/tlaplus>. They are under the MIT License, which is in `LICENSE`. This repository is not part of the TLA+ project, and the TLA+ project does not endorse it.

To use a new build, publish a new release. Do not replace a file in an existing release.
