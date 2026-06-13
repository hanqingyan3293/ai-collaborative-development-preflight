# MomoCrypt Preflight Record

## Idea

Build an open-source local file encryption app. Encrypted output can be disguised as normal images, audio, and documents. It should support plugins and portable builds.

## Locked decisions

| Decision | Choice |
|---|---|
| Project type | Cross-platform desktop app |
| Stack | Rust + Tauri + Vue |
| Security layer | Authenticated encryption required |
| Feature layer | Codebook obfuscation and disguise output |
| Plugins | WASM sandbox |
| Release | Portable build |

## Risks

- Custom encryption must not replace modern cryptography.
- Disguised files may be damaged after recompression or editing.
- Plugins must be sandboxed.
- Wrong passwords must not reveal plaintext.
