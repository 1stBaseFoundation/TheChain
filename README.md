# All-In-One Node ✅

## Overview
A compact, self-contained node distribution containing the first binaries for the blockchain — ready to run without external runtime dependencies.

---

## Quick Start 
1. Download the binary for your OS extract and run **1stbase**.
2. Linux troubleshoot permissions: file ~ `chmod +x 1stbase`, directory ~ `chmod -R 755 1stBase_Linux_v1.x.x`

---

## System Requirements 🔧

### Minimum 
Windows/Linux

- **Operating System** : Windows 8/ 10 / 11 (64-bit) | Ubuntu 18.04+, CentOS 7+, Debian 9+ (64-bit) |
- **CPU** : Dual-core (2.0 GHz or faster) 
- **RAM** : 2 GB available memory 
- **Storage** : 2 GB available disk space 
- **Browser** : Chrome , Firefox , Edge 

### Recommended
- **CPU:** Quad-core (2.4 GHz or faster)
- **RAM:** 4 GB available memory
- **Storage:** 10 GB available disk space
- **Browser:** Latest Chrome, Firefox, Edge

---

## Network Requirements 🌐
- **Internet connection:** Required for initial download and updates.
- **Port access:** Peer-to-Peer ~ 4003~4001

> ⚠️ App automatically requests firewall permission on Windows, Linux may require custom rules.



## Additional Notes 💡
- **Self-contained executable:** No Node.js runtime installation required.
- **No external dependencies:** All necessary libraries are bundled with the application.
- **Cross-platform:** Binaries are provided for Windows and Linux (64-bit).

---

## Explorer API - Port 3003 🔍
Dedicated service for blockchain exploration and data indexing.

### Network Statistics
- `GET /api/explorer/stats/overview` - Get network overview statistics

### Blocks
- `GET /api/explorer/blocks` - Get recent blocks
- `GET /api/explorer/blocks/latest` - Get the latest block
- `GET /api/explorer/blocks/:blockHash` - Get details for a specific block
- `GET /api/explorer/blocks/:blockHash/transactions` - Get transactions for a specific block

### Transactions
- `GET /api/explorer/transactions` - Get recent transactions
- `GET /api/explorer/transactions/latest` - Get the latest transactions
- `GET /api/explorer/transactions/:txid` - Get details for a specific transaction

### Addresses
- `GET /api/explorer/addresses/:address/transactions` - Get recent transaction history for an address
- `GET /api/explorer/addresses/:address/transactions/?page=XX` - Get transaction history for an address in pages of 10~11
- `GET /api/explorer/addresses/:address/aggregates` - Get aggregated data for an address
- `GET /api/explorer/addresses/:address/utxos` - Get unspent transaction outputs for an address

---







