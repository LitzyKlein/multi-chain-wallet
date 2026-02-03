# Multi-Chain Wallet Address Generator (Pure C)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## Overview

This is a **standalone Windows tool** written in **pure C**, using only  
[`libsecp256k1`](https://github.com/bitcoin-core/secp256k1) for elliptic curve operations.

It generates wallet addresses for multiple blockchains **directly from BIP39 mnemonic phrases**:

- **Ethereum**
- **Binance Smart Chain (BSC)**
- **Polygon (MATIC)**

This repository provides **precompiled binaries** for demonstration and interview purposes —  
no compilation required.

---

## Included Files

| File | Description |
|------|-------------|
| `mnemonicToAddress.exe` | Main executable |
| `libsecp256k1-5.dll` | Required ECC library |
| `README.md` | Project documentation |

> **Note:** Source code is  not included in this repository.

---

## Usage

1. Place `mnemonicToAddress.exe` and `libsecp256k1.dll` in the same folder.
2. Open a terminal in that folder.
3. Run:

Example:
```bat
mnemonicToAddress.exe "abandon abandon abandon abandon abandon abandon abandon abandon abandon abandon abandon about"
<div></div>
Sample Output:

0x9858EfFD232B4033E47d90003D41EC34EcaEda94


Features

✔️ Pure C implementation

✔️ Uses only libsecp256k1

✔️ Multi-chain address derivation

Ethereum / BSC / Polygon

✔️ Supports 12 / 15 / 24-word BIP39 mnemonics

✔️ Ethereum EIP-55 checksum

✔️ Ready-to-run executable (no build steps)


Security Notes

⚠️ Do NOT use real wallet mnemonics containing actual funds.
⚠️ This tool is for demonstration and interview purposes only.
✔️ You may safely use test mnemonics for evaluation.


License

This project is released under the MIT License.
