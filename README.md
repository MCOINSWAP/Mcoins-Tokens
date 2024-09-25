# Mcoins Tokens

## Adding Your Token to Tokens-list.json

This guide explains how to add your token to the `Tokens-list.json` file by forking this repository.

### Steps to Add Your Token

1. **Fork the Repository**
   - Click the "Fork" button on the top right of the [Mcoins-Tokens](https://github.com/MCOINSWAP/Mcoins-Tokens) repository page.

2. **Clone the Forked Repository**
   ```bash
   git clone https://github.com/MCOINSWAP/Mcoins-Tokens.git

```bash
{
  "chainId": polygon.id,
  "symbol": "YOUR_SYMBOL",
  "name": "YOUR_TOKEN_NAME",
  "address": "YOUR_TOKEN_ADDRESS",
  "logoURI": "/images/tokens/YOUR_LOGO.svg",
  "decimals": YOUR_DECIMALS
}

```
```bash
git add Tokens-list.json
git commit -m "Add YOUR_TOKEN_NAME token"

git push origin main
```
### Create a Pull Request
```bash
Go back to the original repository and create a pull request from your fork.
Important Notes

Ensure that the token details are accurate.
Follow the existing format in Tokens-list.json for consistency.
Thank you for contributing!
```


# Mcoins Team Update Listing Page  [Mcoins Listing](https://mcoins.xyz/listing/)


