Here’s a simple **Node.js** script to test the connection to **ZenChain Testnet** (assuming it works like an EVM-compatible chain, similar to Ethereum):

```javascript
const { ethers } = require("ethers");

// ZenChain Testnet RPC URL
const ZENCHAIN_TESTNET_RPC = "https://zenchain-testnet.api.onfinality.io/public"; 

async function testConnection() {
    try {
        // Create a provider
        const provider = new ethers.JsonRpcProvider(https://zenchain-testnet.api.onfinality.io/public);

        // Get network details
        const network = await provider.getNetwork();
        console.log("Connected to network:", network);

        // Get latest block number
        const blockNumber = await provider.getBlockNumber();
        console.log("Latest Block Number:", blockNumber);
    } catch (error) {
        console.error("Connection failed:", error);
    }
}

testConnection();
```

### Steps to Run

1. **Initialize project & install dependencies**

   ```bash
   mkdir zenchain-test
   cd zenchain-test
   npm init -y
   npm install ethers
   ```
2. **Save code** (e.g., `testConnection.js`)
3. **Run**

   ```bash
   node testConnection.js
   ```

Do you also want me to **add account creation & balance check** (like Ethereum wallet test)?
