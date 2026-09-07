<div align="center">

# ciphr

### Encryption, done right.

A modern, developer-friendly encryption CLI with an interactive terminal UI. No bloated GUIs, no confusing flags — just clean, simple encryption from your terminal.

</div>

---

## What is ciphr?

ciphr is a command-line encryption tool built for developers who want the power of public-key encryption without the nightmare of GPG or tools like Kleopatra.

It handles key generation, file encryption, decryption, and signing — all through a clean interactive terminal UI that doesn't require reading a manual to use.

We think encryption tools should be:

- Approachable without being dumbed down
- Clear about what they're doing at every step
- Fast to use once you know the basics
- Trustworthy — built on proven cryptographic libraries, not custom crypto

## Features

- **Interactive terminal UI** — navigate ciphr through a clean, keyboard-driven interface
- **Key generation** — generate public/private keypairs in seconds
- **Encrypt & decrypt** — encrypt files or text for a recipient using their public key
- **Sign & verify** — sign files to prove authenticity, verify signatures from others
- **Key management** — import, export, list and delete keys from your local keyring
- **Readable output** — errors and results in plain English, no cryptic exit codes

## Installation

```bash
npm install -g ciphr
```

## Usage

Launch the interactive UI:

```bash
ciphr
```

Or use commands directly:

```bash
ciphr keygen
ciphr encrypt secret.txt --recipient keys/recipient.pub
ciphr decrypt secret.txt.ciphr --key keys/my.priv
ciphr sign document.txt --key keys/my.priv
ciphr verify document.txt --sig document.txt.sig --key keys/sender.pub
ciphr keys list
```

## Philosophy

> Encryption shouldn't require an expert to use.

ciphr doesn't implement its own cryptography. It is built on top of proven, audited libraries so you get the security of established standards with an interface that actually makes sense.

The goal is to make encryption something developers reach for naturally — not something they avoid because the tooling is too painful.

## Get involved

Pull requests are welcome. If you have an idea, found a bug, or want to contribute, open a PR or get in touch:

**joshuaorpen@tutanota.de**

---

<div align="center">

**Encryption, done right.**
<br />
<a href="https://github.com/tinkrd-labs/ciphr">github.com/tinkrd-labs/ciphr</a>

</div>
