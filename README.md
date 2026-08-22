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
- **RAM** : 1 GB available memory 
- **Storage** : 2 GB available disk space 
- **Browser** : Chrome , Firefox , Edge 

### Recommended
- **CPU:** Quad-core (2.4 GHz or faster)
- **RAM:** 2 GB available memory
- **Storage:** 10 GB available disk space
- **Browser:** Latest Chrome, Firefox, Edge

---

## Network Requirements 🌐
- **Internet connection:** Required for initial download and updates.
- **Required Host Ports:** 

  + Peer-to-Peer: 4003~4001
  + Frontend: 3000
  + Backend: 3001~3005

## Additional Notes 💡

- **Self-contained executable:** No Node.js runtime installation required.
- **No external dependencies:** All necessary libraries are bundled with the application.
- **Cross-platform:** Binaries are provided for Windows and Linux (64-bit).

---

## API 🔍
Collection of useful API endpoints for developers. 

### Public Explorer 

- When using `node.1stbase.org` ommit the ports for queries, e.g `node.1stbase.org/api/explorer/stats/circulatingSupply`
- `node.1stbase.org/explorer/transactions/txid` - GUI link for transactions (Instead of raw JSON)

### Network Statistics
- `GET localhost:3000/api/explorer/stats/overview` - Get network overview statistics
- `GET localhost:3001/api/explorer/stats/circulatingSupply` - Get circulating supply (Non-satoshi decimal value)

### Blocks
- `GET localhost:3000/api/explorer/blocks` - Get recent blocks
- `GET localhost:3000/api/explorer/blocks/latest` - Get the latest block
- `GET localhost:3000/api/explorer/blocks/:blockHash` - Get details for a specific block
- `GET localhost:3000/api/explorer/blocks/:blockHash/transactions` - Get transactions for a specific block

### Transactions
- `GET localhost:3000/api/explorer/transactions` - Get recent transactions
- `GET localhost:3000/api/explorer/transactions/latest` - Get the latest transactions
- `GET localhost:3000/api/explorer/transactions/:txid` - Get details for a specific transaction



### Addresses
- `GET localhost:3000/api/explorer/addresses/:address/transactions` - Get recent transaction history for an address
- `GET localhost:3000/api/explorer/addresses/:address/transactions/?page=XX&size=XX&exclude=inputs,outputs` - Get transaction history for an address in pages, 500 max per page, optional to exclude UTXOs for smaller payload.
- `GET localhost:3000/api/explorer/addresses/:address/aggregates` - Get aggregated data for an address
- `GET localhost:3000/api/explorer/addresses/:address/utxos` - Get unspent transaction outputs for an address

________________________________________________________________________________________________________________________________________________________________________________________________________

Copyright © 2026 1stBase (PTY) LTD. All rights reserved, except where third-party open-source components are licensed under their respective licenses.

This repository contains proprietary, closed-source software and confidential intellectual property belonging to 1stBase (PTY) LTD, including proprietary black-box software, blockchain logic, smart-contract logic, on-chain application logic, custom artwork, logos, and documentation.

Unauthorized copying, modification, distribution, deployment, reverse engineering, or commercial use of the Company’s proprietary components is strictly prohibited without prior written consent.

Third-party open-source dependencies included in this repository remain subject to their respective licenses. See THIRD_PARTY_NOTICES.md and the applicable LICENSE files. Nothing in this notice limits rights granted under those third-party licenses.

The 1stBase name, logos, and custom artwork are proprietary and may be protected by copyright, trademark, passing-off/unfair-competition, and other applicable laws. No license is granted to use them.

Governed by the laws of South Africa.





