# MyToken-SmartContract
# 🪙 MyToken (MTK)

MyToken is a simple ERC-20-like token written in Solidity for learning and demonstration purposes. It includes basic functionality such as transferring tokens and checking balances.

## 📄 Overview

- **Name**: MyToken  
- **Symbol**: MTK  
- **Decimals**: 18  
- **Total Supply**: 1,000,000,000 MTK  
- **Standard**: ERC-20 Inspired (Not fully ERC-20 compliant, lacks `approve/transferFrom`)

---

## 🧠 Features

- Token supply is fixed at deployment.
- The deployer owns the entire initial supply.
- Users can transfer tokens to other addresses.
- Anyone can check balances using the `balanceOf` function.
- Emits a `Transfer` event on successful token transfer.

---

## 🚀 Getting Started

### 1. Deploy with Remix
- Open [Remix IDE](https://remix.ethereum.org/)
- Paste the contract in a `.sol` file.
- Compile with Solidity ^0.8.0
- Deploy using **Remix VM** or **Injected Provider (Metamask)**

### 2. Interact with Contract
- Use `transfer(address, amount)` to send tokens.
- Use `balanceOf(address)` to check token balances.
- Monitor events via Remix logs or frontend integration.

---

## 🔧 Functions

| Function | Description |
|----------|-------------|
| `constructor()` | Initializes total supply to contract owner. |
| `transfer(address recipient, uint256 amount)` | Transfers `amount` tokens to `recipient`. |
| `balanceOf(address account)` | Returns the balance of a specific address. |

---

## 📦 Example

```solidity
// Send 100 tokens to another user
token.transfer(0xAbC123..., 100 * 10**18);
