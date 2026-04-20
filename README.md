# Mcoins Tokens

The McoinSwap token list — fetched automatically by [McoinSwap](https://mcoins.xyz) on every page load. Adding your token here makes it appear in the swap interface across all supported chains.

---

## Token Format

Each token is a JSON object in the array. Use **numeric chain IDs** — not variable names.

```json
{ "chainId": 56, "symbol": "YOUR_SYMBOL", "name": "Your Token Name", "address": "0xYOUR_CONTRACT_ADDRESS", "logoURI": "https://your-logo-url.png", "decimals": 18 }
```

### Chain IDs

| Chain | chainId |
|---|---|
| BNB Smart Chain | `56` |
| Polygon | `137` |
| Base | `8453` |
| PulseChain | `369` |

### Notes
- `address` must be the token's contract address as a string
- For native coins with no contract (BNB, ETH, PLS, POL) use `null` as the address
- `decimals` is almost always `18` — check your token contract if unsure
- `logoURI` should be a direct image URL (PNG, SVG, or WebP)

---

## How to Add Your Token

### 1. Fork the Repository
Click **Fork** on the top right of the [Mcoins-Tokens](https://github.com/MCOINSWAP/Mcoins-Tokens) repository.

### 2. Clone Your Fork
```bash
git clone https://github.com/YOUR_USERNAME/Mcoins-Tokens.git
```

### 3. Edit `tokens-list`
Open the file and add your token entry to the JSON array:

```json
[
  ...existing tokens...,
  { "chainId": 56, "symbol": "MYTOKEN", "name": "My Token", "address": "0xABC123...", "logoURI": "https://mysite.com/logo.png", "decimals": 18 }
]
```

### 4. Commit and Push
```bash
git add tokens-list
git commit -m "Add MYTOKEN on BSC"
git push origin main
```

### 5. Open a Pull Request
Go back to the original repository and open a pull request from your fork. The Mcoins team will review and merge it.

---

## Important Notes
- Make sure the contract address is correct — wrong addresses cannot be swapped
- The file must remain valid JSON (no comments, no trailing commas)
- One token per chain entry — if your token exists on multiple chains, add one line per chain with the correct `chainId` and `address` for each

---

## Mcoins Team Direct Listing

Prefer a faster review? Submit via the official listing page:
**[mcoins.xyz/listing](https://mcoins.xyz/listing/)**
