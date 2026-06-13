# MomoCrypt Development Specification

## Overview

MomoCrypt is a local file encryption and disguised-output tool. It protects real data with authenticated encryption, then applies custom codebook obfuscation and carrier formats.

## Core flow

```text
Original file
↓
Compression
↓
Authenticated encryption
↓
Codebook obfuscation
↓
Disguised output
```

## Technology stack

- Rust
- Tauri
- Vue
- TypeScript
- WASM plugin sandbox

## Disguise formats

- PNG
- JPG
- WAV
- DOCX
- TXT
- LOG
- CSS color palette

## Modules

| Module | Responsibility |
|---|---|
| CryptoCore | Standard encryption |
| MomoCipher | Codebook obfuscation |
| CarrierFormats | Disguise formats |
| PluginRuntime | Plugin sandbox |
| UI | User interface |
| History | History records |

## Acceptance criteria

- Decrypted file hash matches the original.
- Wrong password cannot decrypt.
- Disguised files open in normal software.
- Plugins cannot access master keys.
- Logs contain no sensitive information.
