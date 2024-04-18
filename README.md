# TransferUSDCBasic Contract

## Overview
The TransferUSDCBasic contract enables the cross-chain transfer of USDC (USD Coin) tokens from the Avalanche Fuji testnet to the Ethereum Sepolia testnet using Chainlink's Cross-Chain Interoperability Protocol (CCIP). It provides a simple and secure mechanism for transferring USDC tokens between different blockchain networks.

## Getting Started
To use the TransferUSDCBasic contract, follow these steps:
1. Deploy the contract on the Avalanche Fuji testnet.
2. Ensure that the contract owner has sufficient LINK tokens and USDC tokens for transaction fees and transfers, respectively.
3. Specify the recipient address and the amount of USDC tokens to transfer.
4. Call the `transferUsdcToSepolia` function to initiate the cross-chain transfer.
5. Monitor the event logs for confirmation of the token transfer.

## Contract Details
- **Owner:** The address that deployed the contract.
- **CCIP Router:** The address of the CCIP router contract.
- **LINK Token Address:** The address of the LINK token contract on the Avalanche Fuji testnet.
- **USDC Token Address:** The address of the USDC token contract on the Avalanche Fuji testnet.
- **Destination Chain Selector:** The identifier for the Ethereum Sepolia testnet.
- **Fee Calculation:** The contract calculates and approves the required LINK token fees for the cross-chain transfer.

## Functions
- `transferUsdcToSepolia`: Initiates the cross-chain transfer of USDC tokens to the Ethereum Sepolia testnet.
- `allowanceUsdc`: Retrieves the current allowance of USDC tokens approved for the contract.
- `balancesOf`: Retrieves the LINK and USDC token balances of an account.
- `withdrawToken`: Allows the contract owner to withdraw remaining token balances.

## Security Considerations
- **Hardcoded Values:** The contract uses hardcoded values for clarity and demonstration purposes. Do not use this code in production without proper auditing and modifications.
- **Access Control:** Only the contract owner can withdraw remaining token balances.

