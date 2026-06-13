# MomoCrypt Development Specification

## Overview

A local file encryption and disguise-output tool.

## Core flow

Original file → authenticated encryption → codebook obfuscation → disguised output.

## Disguise formats

- PNG
- JPG
- WAV
- DOCX
- log text
- color palette

## Acceptance criteria

- Decrypted file hash matches the original.
- Wrong password cannot decrypt.
- Disguised files open in normal software.
