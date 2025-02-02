---
slug: /IRoyalty
title: IRoyalty
hide_title: true
displayed_sidebar: contracts
---

# IRoyalty

## Methods

### getDefaultRoyaltyInfo

```solidity
function getDefaultRoyaltyInfo() external view returns (address, uint16)
```

_Returns the royalty recipient and fee bps._

#### Returns

| Name | Type    | Description |
| ---- | ------- | ----------- |
| \_0  | address | undefined   |
| \_1  | uint16  | undefined   |

### getRoyaltyInfoForToken

```solidity
function getRoyaltyInfoForToken(uint256 tokenId) external view returns (address, uint16)
```

_Returns the royalty recipient for a particular token Id._

#### Parameters

| Name    | Type    | Description |
| ------- | ------- | ----------- |
| tokenId | uint256 | undefined   |

#### Returns

| Name | Type    | Description |
| ---- | ------- | ----------- |
| \_0  | address | undefined   |
| \_1  | uint16  | undefined   |

### royaltyInfo

```solidity
function royaltyInfo(uint256 tokenId, uint256 salePrice) external view returns (address receiver, uint256 royaltyAmount)
```

_Returns how much royalty is owed and to whom, based on a sale price that may be denominated in any unit of exchange. The royalty amount is denominated and should be payed in that same unit of exchange._

#### Parameters

| Name      | Type    | Description |
| --------- | ------- | ----------- |
| tokenId   | uint256 | undefined   |
| salePrice | uint256 | undefined   |

#### Returns

| Name          | Type    | Description |
| ------------- | ------- | ----------- |
| receiver      | address | undefined   |
| royaltyAmount | uint256 | undefined   |

### setDefaultRoyaltyInfo

```solidity
function setDefaultRoyaltyInfo(address _royaltyRecipient, uint256 _royaltyBps) external nonpayable
```

_Lets a module admin update the royalty bps and recipient._

#### Parameters

| Name               | Type    | Description |
| ------------------ | ------- | ----------- |
| \_royaltyRecipient | address | undefined   |
| \_royaltyBps       | uint256 | undefined   |

### setRoyaltyInfoForToken

```solidity
function setRoyaltyInfoForToken(uint256 tokenId, address recipient, uint256 bps) external nonpayable
```

_Lets a module admin set the royalty recipient for a particular token Id._

#### Parameters

| Name      | Type    | Description |
| --------- | ------- | ----------- |
| tokenId   | uint256 | undefined   |
| recipient | address | undefined   |
| bps       | uint256 | undefined   |

## Events

### DefaultRoyalty

```solidity
event DefaultRoyalty(address newRoyaltyRecipient, uint256 newRoyaltyBps)
```

_Emitted when royalty info is updated._

#### Parameters

| Name                | Type    | Description |
| ------------------- | ------- | ----------- |
| newRoyaltyRecipient | address | undefined   |
| newRoyaltyBps       | uint256 | undefined   |

### RoyaltyForToken

```solidity
event RoyaltyForToken(uint256 indexed tokenId, address royaltyRecipient, uint256 royaltyBps)
```

_Emitted when royalty recipient for tokenId is set_

#### Parameters

| Name              | Type    | Description |
| ----------------- | ------- | ----------- |
| tokenId `indexed` | uint256 | undefined   |
| royaltyRecipient  | address | undefined   |
| royaltyBps        | uint256 | undefined   |
