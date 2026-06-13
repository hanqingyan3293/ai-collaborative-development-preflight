# MomoCrypt Preflight Record

## Idea

An open-source local file encryption app that disguises encrypted output as normal images, audio, and documents.

## Locked decisions

| Decision | Choice |
|---|---|
| Stack | Rust + Tauri + Vue |
| Security | Authenticated encryption required |
| Feature layer | Codebook obfuscation and disguise output |
| Plugins | WASM sandbox |
