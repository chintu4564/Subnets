## Subnet

This project consists of two Solidity smart contracts, `ERC20` and `Vault`, aimed at providing functionalities for managing ERC-20 tokens and a vault system for depositing and withdrawing tokens.

### ERC20 Contract

The `ERC20` contract is a basic implementation of the ERC-20 token standard. It includes functionalities such as:

- Minting new tokens.
- Burning tokens.
- Transferring tokens between addresses.
- Approving allowances for spending tokens on behalf of another address.

#### Contract Details:

- **Total Supply:** Tracks the total supply of the token.
- **BalanceOf:** A mapping to keep track of token balances for each address.
- **Allowance:** A mapping to keep track of approved allowances for spending tokens.
- **Name, Symbol, Decimals:** Metadata for the token.
- **Events:** Emit events for transfers and approvals.

### Vault Contract

The `Vault` contract is designed to allow users to deposit and withdraw ERC-20 tokens while minting and burning shares representing ownership within the vault. This enables users to interact with the vault without needing to handle specific token amounts.

#### Contract Details:

- **Token:** An immutable reference to the ERC-20 token contract.
- **Total Supply:** Tracks the total supply of shares representing ownership within the vault.
- **BalanceOf:** A mapping to keep track of shares owned by each address.
- **Deposit:** Function to deposit tokens into the vault, minting shares proportional to the deposited amount.
- **Withdraw:** Function to withdraw tokens from the vault, burning shares proportional to the withdrawn amount.

### How to Use

1. **Deploy Contracts:**
   - Deploy the `ERC20` contract first, providing necessary parameters like name, symbol, and decimals.
   - Deploy the `Vault` contract, passing the address of the deployed ERC20 contract.

2. **Interact with ERC20:**
   - Mint new tokens using the `mint` function.
   - Burn tokens using the `burn` function.
   - Transfer tokens between addresses using the `transfer` function.
   - Approve allowances for spending tokens using the `approve` function.

3. **Interact with Vault:**
   - Deposit tokens into the vault using the `deposit` function.
   - Withdraw tokens from the vault using the `withdraw` function.

## Author 

Choshith reddy 

chintubasha186@gmail.com
