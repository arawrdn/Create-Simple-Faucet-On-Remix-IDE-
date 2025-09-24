# Create-Simple-Faucet-On-Remix-IDE-
Simple Faucet On # Base Token Faucet

This repository contains a simple ERC20 token faucet smart contract that can be deployed on the **Base Network** using Remix IDE. Users can claim tokens once per defined period (e.g., 24 hours).

---

## 1. Open Remix IDE

- Go to [https://remix.ethereum.org](https://remix.ethereum.org)  
- Connect your wallet (e.g., MetaMask) to Base Testnet/Mainnet.

---

## 2. Create Contract File

- File path: `contracts/Faucet.sol`  
- Paste the smart contract code from `Faucet.sol`.

---

## 3. Compile Contract

- Solidity compiler: **0.8.20**  
- Enable optimization (optional)  
- Click **Compile Faucet.sol**  

> Ensure there are no compilation errors.

---

## 4. Deploy Contract

- Environment: **Injected Web3**  
- Network: Base Testnet/Mainnet  
- Constructor parameter: ERC20 token address (the token to drip)  
- Click **Deploy** and confirm in your wallet

---

## 5. Interact with Contract

### Claim Tokens
- `claim()` → Users can claim faucet tokens once per wait period (default 24h)

### Admin Functions
- `setDripAmount(amount)` → Set how many tokens are given per claim  
- `setWaitTime(seconds)` → Set claim cooldown period  
- `withdrawTokens(amount)` → Owner can withdraw tokens from the faucet

---

## Notes

- Faucet requires enough token balance in the contract to function  
- Each wallet can claim **only once per period**  
- For testing, you can deploy a test ERC20 token first

