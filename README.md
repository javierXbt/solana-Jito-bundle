# solana-Jito-bundle
Create token + Add Liquidity: The program allows you to enter desired amount of base tokens(COIN) and quote tokens(SOL), upon which it will create the liquidity pool. this uses JITO Bundles to add liquidity to your token and makes the first swap (first txn).

**TELEGRAM** for contact : [@solmerd](https://t.me/solmerd) | 

Price of tool is 10 SOL.

## Features

- **Token Deployment**: Automate the deployment of new tokens on the Solana blockchain.
- **Market Creation**: Easily create markets with a lower cost of 0.29 SOL instead of 3 SOL.
- **Multiple Wallet Operations**: Utilize different wallets to perform instant market operations programatically ( you can generate what ever number you want ).
- **Comprehensive Trading Strategies**: From simple sell orders to sophisticated strategies involving a percentage of the supply.
- **Liquidity Management**: Options to add and remove liquidity effectively.
- **Guaranteed First Buys**: First 3 buys of the coin will always be yours and completely undetected using different keypairs and fee payer.
- **Comprehensive Documentation**: Even if you have no code experience, you will still be able to deploy and snipe using the easy prompts and the documentation attached.
  

## Overview
This guide outlines the process for managing market creation and transactions using Solana Bundler.

Below are detailed instructions for setting up your environment and executing prompts in a sequential manner.

### Initial Setup

1. **Install Dependencies**
   ```bash
   npm install

2. **Configuration**
    
    - Modify `config.ts`:
      - It includes two keypairs:
        1. One for handling sinpe wallets .
        2. Another for creating the pool ( Dev Wallet ) .
      - These keypairs can be the same if desired.
    - Modify RPC URL with one faster ( prefered Private RCP paid verision )
    - Enter token name , symbol , supply ,logo 

3. **Run script**
   ```bash
   npx ts-node main.ts

## Script Functions

Execute these steps in sequential order. After executing each step, verify the transaction bundle has landed by checking the first included transaction on [Jito Explorer](https://explorer.jito.wtf/).

### A) Create Keypairs
Run this step as needed, not necessarily for every launch. Ensure the existent keypairs hold no SOL before proceeding because this will override them with new keypairs.

### B) Follow steps 
Execute steps all steps notified end of each steps . If a bundle does not land, re-execute the step with a higher tip. 

### C) Create Pool
Repeatedly invoke the pool creation & bundling function. Increasing the tip and repeated attempts are recommended due to Solana congestion at peak times.

### D) Sell Features
After the pool is live, proceed to either:
  - Wallet Manager 
  - You will find list of oprations to manage your sniped tokens and wallets.
  - wallet manager 
    ### Main Menu 
  -  List All Wallets Tokens and balances >
  -  Select wallet to sell >
  -  Sell  Wallets Tokens (Sell all  Wallets at once)  >
  -  Recover Wallet Sols (Recover all Wallets at once)  >
   -  Wallet Transfers MENU > >

### E) LP Removal
This step removes liquidity from the market(if LP tokens are not burned)

## Notes

- Ensure you maintain a minimal SOL balance in your fee wallet so you can cover all the network fees.
- Monitor each transaction bundle to confirm landing using the suggested link to the explorer before proceeding to the next step.
- Consider adjusting the tip to ensure transactions land promptly.

### Main Menu

```bash
Menu:
1. Create Keypairs 
2. Wallet Manager
3. Manage wallets and token Balance
4. send token from main wallet / sinpe wallet 
5. select wallet to sell 
4. Sell All Buyers wallet at once 
5. Sell % of Supply from each wallet 
6. Remove Liquidity
Type 'exit' to quit.
```

### Buyer UI
```
1. Mint token 
2. revoke Mint 
3. Create Market ID (0.29 SOL)
3. Create Pool Bundle
4. Snipe on first Transction
5. Simulate LP Buys (Get exact amounts)

