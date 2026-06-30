# AiLang macOS Target

Official AiLang target package for macOS.

The target owns macOS `.app` packaging, local app launch, target diagnostics,
codesigning/notarization hooks, and macOS host library integration.

Current package release: `0.0.1-alpha.2`.

## Package

```text
packages/target-macos
```

## Status

Package discovery is enabled. The current alpha target package declares the
macOS target contract and delegates to the SDK's built-in macOS run/publish
path while the target-owned host library and signing pipeline are moved out of
the core toolchain.

Supported target identifiers:

```text
macos
apple-macos
darwin
```

Declared artifact types:

```text
app
dir
dmg
```

Declared options:

```text
arch
bundle-id
signing-identity
notarize
```

## Usage

```bash
ailang package restore
ailang run . --target macos
ailang publish . --target macos --target-option bundle-id=com.example.MyApp
```

Local `run` requires a macOS host. Packaging, signing, notarization, and host
library work remain target-owned responsibilities for this repository.
