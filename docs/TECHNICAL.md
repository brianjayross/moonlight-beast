# Technical Documentation

Comprehensive technical documentation for the Moonlight Beast NFT collection.

## Smart Contract

### Overview
The Moonlight Beast smart contract is an ERC-721 (NFT) implementation.

### Contract Details

| Property | Value |
|----------|-------|
| **Name** | Moonlight Beast |
| **Symbol** | MB |
| **Standard** | ERC-721 |
| **Chain** | [Ethereum/Polygon/etc] |
| **Address** | `0x...` |
| **Total Supply** | [Number] |

### Key Features

- **Minting:** Controlled minting with supply limits
- **Burning:** Holders can burn NFTs
- **Royalties:** Creator royalties on secondary sales
- **Metadata:** Dynamic URI management

## Token Standards

### ERC-721 Compliance
Moonlight Beast is fully compliant with ERC-721:
- Single token ownership
- Transfer capabilities
- Approval mechanisms

### ERC-2981 (Royalties)
Our contract implements ERC-2981 for royalty information with automatic royalty calculations.

## Deployment

### Networks

| Network | Address | Status |
|---------|---------|--------|
| Mainnet | `0x...` | ✅ Active |
| Testnet | `0x...` | ✅ Active |

## Metadata

### Structure
Each NFT has JSON metadata:

```json
{
  "name": "Moonlight Beast #1",
  "description": "A unique Moonlight Beast NFT",
  "image": "ipfs://...",
  "attributes": [
    {
      "trait_type": "Background",
      "value": "Moonlit Forest"
    }
  ]
}
```

### Storage
- **Format:** JSON
- **Hosting:** IPFS
- **Immutable:** Yes

## Development

### Setup
```bash
git clone https://github.com/brianjayross/moonlight-beast.git
cd moonlight-beast
npm install
```

### Testing
```bash
npm test
npm run test:coverage
```

### Linting
```bash
npm run lint
npm run lint:fix
```

## Security

- Smart contracts audited
- Non-upgradeable contract (immutable)
- Standard ERC-721 implementation
- No external dependencies

---

**Last Updated:** 2026-01-02  
**Version:** 1.0.0