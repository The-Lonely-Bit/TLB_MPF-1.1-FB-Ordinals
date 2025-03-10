# TLB MintPumpFun v1.1

## How to Submit Your Collection

For your collection to function correctly on TLB MintPumpFun, you must submit a complete metadata file along with the required files (images and JSON files).

### Required Metadata Format

Your collection metadata must follow this JSON structure:

```json
{
    "collectionName": "Order Of The L Bit",
    "description": "A set of Exclusive TLB membership Emblems that showcase the strength and resilience of the holder, recognizing their contribution to the TLB project. Fueled with incentives and utility, these emblems redefine the power of ownership on the blockchain.",
    "twitter": "https://x.com/fractal_tlb",
    "floorPrice": "0.00000546 BTC",
    "Deployer": "bc1qcagueggs2snz8uvh92qfffglu3hzqxmwvus45h",
    "WL": false,
    "Mintable": true,
    "items": [
        {
            "id": 1,
            "name": "L_Bit#1",
            "image": "1.png",
            "minted": false,
            "inscriptionId": "",
            "price": 546
        },
        {
            "id": 2,
            "name": "L_Bit#2",
            "image": "2.png",
            "minted": false,
            "inscriptionId": "",
            "price": 546,
            "minting": false
        },
        {
            "id": 3,
            "name": "L_Bit#3",
            "image": "3.png",
            "minted": false,
            "inscriptionId": "",
            "price": 546
        }
    ]
}
```

**Important Notes:**

- **Price is in Satoshis (sats)** – Ensure the `"price"` field is defined in sats.
- **File Submission Required** – In addition to the metadata JSON, all associated files (e.g., NFT images such as `1.png`, `2.png`, etc.) must be submitted.
- **Fractal Bitcoin Compatibility** – This format is designed to work seamlessly on Fractal Bitcoin.

---

## Including Optional Attributes

To enable additional details when an ordinal is expanded, you can optionally add an `"attributes"` array for each item. These attributes will be displayed below the main content when a user clicks “Expand” on an ordinal.

For example:

```json
{
    "collectionName": "Order Of The L Bit",
    "description": "A set of Exclusive TLB membership Emblems that showcase the strength and resilience of the holder, recognizing their contribution to the TLB project. Fueled with incentives and utility, these emblems redefine the power of ownership on the blockchain.",
    "twitter": "https://x.com/fractal_tlb",
    "floorPrice": "0.00000546 BTC",
    "Deployer": "bc1qcagueggs2snz8uvh92qfffglu3hzqxmwvus45h",
    "WL": false,
    "Mintable": true,
    "items": [
        {
            "id": 1,
            "name": "L_Bit#1",
            "image": "1.png",
            "attributes": [
                {
                  "trait_type": "Origin",
                  "value": "Hydrora"
                },
                {
                  "trait_type": "Element",
                  "value": "Water"
                },
                {
                  "trait_type": "Class",
                  "value": "Guardian"
                },
                {
                  "trait_type": "Rarity",
                  "value": "Legendary"
                }
            ],
            "minted": false,
            "inscriptionId": "",
            "price": 546
        },
        {
            "id": 2,
            "name": "L_Bit#2",
            "image": "2.png",
            "attributes": [
                {
                  "trait_type": "Origin",
                  "value": "Hydrora"
                },
                {
                  "trait_type": "Element",
                  "value": "Water"
                },
                {
                  "trait_type": "Class",
                  "value": "Guardian"
                },
                {
                  "trait_type": "Rarity",
                  "value": "Rare"
                }
            ],
            "minted": false,
            "inscriptionId": "",
            "price": 546,
            "minting": false
        },
    ]
}
```

**Note:**  
- The `"attributes"` field is optional. Items without this field will simply not display an attributes section when expanded.
- Each attribute should have a `"trait_type"` (for example, "Origin" or "Rarity") and a corresponding `"value"`.

---

## Additional Resources

For further details on preparing and submitting your collection, please refer to the following guides:


- **[Design README](design.md)**  
  Learn how to create or edit your `design.json` file to customize your minting page, or choose from our provided templates.

- **[Addresses README](addresses.md)**  
  Instructions on how to manage whitelist (WL) features using the `addresses.json` file.

---

## Join the Challenge

Embrace the challenge, mint your Ordinals fairly, and take full control of your digital assets. With **TLB MintPumpFun** on **Fractal Bitcoin**, you get a truly transparent and decentralized minting experience with ultra-low fees and complete fairness.

[**Get Started Now**](https://thelonelybit.org/TLB_MintPumpFun/)

