# AiLang macOS Target

Official AiLang target package for macOS.

The target owns macOS `.app` packaging, local app launch, target diagnostics,
codesigning/notarization hooks, and macOS host library integration.

## Package

```text
packages/target-macos
```

## Status

Initial target repository scaffold. Package discovery is enabled; platform
tooling is intentionally explicit and currently fails with deterministic
not-yet-implemented diagnostics until the macOS implementation is moved in.
