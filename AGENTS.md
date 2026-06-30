# macOS Target Agents

This repository owns the official AiLang macOS target package.

## Ownership

macOS owns platform packaging, `.app` bundle integration, app menu wiring,
codesigning/notarization tooling, native run/doctor/flash behavior where
applicable, and macOS host library integration.

It does not own AiLang language semantics, AiVM evaluation semantics, AiVectra
UI semantics, or package semantics.

## Verification

```bash
./scripts/validate-target.sh
```
