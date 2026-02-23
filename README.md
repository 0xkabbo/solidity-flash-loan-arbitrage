# Solidity Flash Loan Arbitrage

A professional-grade smart contract template for executing Flash Loans on Aave V3. This repository provides the logic to borrow millions in liquidity, execute an arbitrage trade across decentralized exchanges (DEXs), and repay the loan in a single atomic transaction.

## Core Features
* **Aave V3 Integration**: Uses the `FlashLoanSimple` standard for optimized gas costs.
* **Uniswap V3 Swaps**: Pre-configured for exact-input swaps to capture price discrepancies.
* **Slippage Protection**: Professional-grade checks to ensure the transaction reverts if the trade is not profitable.
* **Flat Structure**: All logic contained within the root for easy deployment and verification.

## Prerequisites
* **Solidity**: ^0.8.10
* **Mock Tokens**: Use Goerli or Sepolia testnets for initial simulations.
* **Provider**: Access to an Ethereum or Polygon RPC.

## Usage
1. Deploy `FlashLoanArbitrage.sol` with the Aave Pool Addresses Provider.
2. Fund the contract with a small amount of tokens to cover the flash loan fee (0.05%).
3. Execute the `executeTrade` function with the target assets and amounts.
