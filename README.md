# 🔄 Auto Bridge Bot (ETH sepolia ↔ Fhenix Helium)

<img width="1280" height="719" alt="image" src="https://github.com/user-attachments/assets/03e6f467-718d-448e-bb3d-1364fd384543" />

---

## 🚀 Features
- Randomized daily bridge (number of transactions, amount per bridge, and delay between swaps).
- Configurable RPC endpoint, wallet private key, and all randomization ranges via `.env`.
- Logs each bridge with timestamp and transaction hash.
- Loop runs continuously every days once started.

---

## 📦 Installation
Clone the repository and install dependencies:

```bash
git clone https://github.com/Kurisaitou/auto-daily-bridge-eth-sepolia-to-Fhenix-Testnet.git
```
```bash
cd auto-daily-bridge-eth-sepolia-to-Fhenix-Testnet
```
```bash
npm install
```

## ⚙️ Environment Setup
Create a .env file in the project root:
```bash
nano .env
```
Fill in your wallet details and randomization settings:
```bash
RPC_URL=https://ethereum-sepolia-rpc.publicnode.com
PRIVATE_KEY=your_privatekey

CHAIN_ID=11155111

MIN_TX_PER_DAY=3
MAX_TX_PER_DAY=5

MIN_AMOUNT_ETH=0.0001
MAX_AMOUNT_ETH=0.001

MIN_DELAY_SEC=30
MAX_DELAY_SEC=60

PRIORITY_FEE_GWEI=0.26

TIMEZONE_OFFSET_MIN=420
```

## ▶️ Running the Bot
To start the bot:
```bash
node index.js
```
What the bot does:

- Executes a random number of bridge daily (within your configured range).

- Randomizes bridge amount and delay between each transaction.

- Signs and sends transactions using your private key.

## 🔖 Tags
#eth #fhenix #swap #bot #crypto #web3 #automation #trading #dex #evm #airdrop #fhenix-helium #bridge #fhenix-testnet
