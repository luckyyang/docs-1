---
slug: /sdk.erc20mintable
title: Erc20Mintable class
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## Erc20Mintable class

Mint ERC20 Tokens

**Signature:**

```typescript
export declare class Erc20Mintable implements DetectableFeature
```

**Implements:** DetectableFeature

## Remarks

Token minting functionality that handles unit parsing for you.

## Example

```javascript
const contract = await sdk.getContract("{{contract_address}}");
await contract.nft.mint.to(walletAddress, nftMetadata);
```

## Constructors

| Constructor                                                                   | Modifiers | Description                                                       |
| ----------------------------------------------------------------------------- | --------- | ----------------------------------------------------------------- |
| [(constructor)(erc20, contractWrapper)](./sdk.erc20mintable._constructor_.md) |           | Constructs a new instance of the <code>Erc20Mintable</code> class |

## Properties

| Property                                          | Modifiers | Type                                                               | Description                         |
| ------------------------------------------------- | --------- | ------------------------------------------------------------------ | ----------------------------------- |
| [batch](./sdk.erc20mintable.batch.md)             |           | [Erc20BatchMintable](./sdk.erc20batchmintable.md) &#124; undefined | Batch mint Tokens to many addresses |
| [featureName](./sdk.erc20mintable.featurename.md) |           | "ERC20Mintable"                                                    |                                     |

## Methods

| Method                                      | Modifiers | Description |
| ------------------------------------------- | --------- | ----------- |
| [to(to, amount)](./sdk.erc20mintable.to.md) |           | Mint Tokens |
