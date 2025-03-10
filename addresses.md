# Whitelist Configuration for TLB MintPumpFun

## Overview

The `addresses.json` file allows collection creators to enable and manage a whitelist (WL) for minting. This gives you full control over who can mint and how many items each address can mint.

### Example `addresses.json` File

```json
{
  "whitelistEnabled": true,
  "maxMintsPerAddress": 2,
  "addressOverrides": {
    "bc1qdxr9fwgv4q2f6p2e3q8yg3tzegvr33pn8wzcv9": 1
  },
  "addresses": [
    "bc1qdxr9fwgv4q2f6p2e3q8yg3tzegvr33pn8wzcv9",
    "bc1q39rqt7cerl7xept3wjwdern8kt0cwh69akxph2",
    "bc1q330fqr66c6ph4wnv8gd2e6gqpc0h73rtvw0hem"
  ]
}
```

## How It Works

- **`whitelistEnabled`**: If `true`, only addresses in the whitelist can mint. If `false`, the minting is open to everyone.
- **`maxMintsPerAddress`**: This sets a default maximum number of mints per address.
- **`addressOverrides`**: Allows you to set specific mint limits for individual addresses. If an address is listed here, its minting limit overrides the default `maxMintsPerAddress`.
- **`addresses`**: This is the list of addresses that are allowed to mint if `whitelistEnabled` is `true`.

## Customization & Flexibility

1. **Disable Whitelist**  
   - If you want to allow anyone to mint, simply set:
   
   ```json
   "whitelistEnabled": false
   ```

2. **Change Minting Limits**  
   - If you want each address to mint up to 5 NFTs, modify:
   
   ```json
   "maxMintsPerAddress": 5
   ```

3. **Set Custom Limits Per Address**  
   - If you want to allow a specific address to mint only 1 NFT while others can mint 3, modify:
   
   ```json
   "maxMintsPerAddress": 3,
   "addressOverrides": {
     "bc1qdxr9fwgv4q2f6p2e3q8yg3tzegvr33pn8wzcv9": 1
   }
   ```

4. **Adding More Addresses**  
   - Simply append them to the `addresses` array:
   
   ```json
   "addresses": [
     "bc1qexample1...",
     "bc1qexample2...",
     "bc1qexample3..."
   ]
   ```

## How It Works in the Minting Process

When a user connects their wallet:
- If the whitelist is enabled, the system checks if their address is in the list.
- If their address is found, it checks how many times they have minted and enforces the limits accordingly.
- If their address is not in the list and `whitelistEnabled` is `true`, they won’t be able to mint.

## Best Practices

- **Always test** your whitelist configuration before making it live.
- **Ensure addresses are correctly formatted** to avoid rejection during minting.
- **Use `addressOverrides` wisely** for special allocations without affecting the general limit.

---

By using `addresses.json`, you can create an exclusive minting experience, reward early supporters, or control supply effectively. 🚀
Feel free to reach out for help or if any issue arises !
