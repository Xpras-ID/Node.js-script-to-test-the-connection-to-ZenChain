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

Here’s how to **run and test** the Node.js code to check ZenChain Testnet connection:

---

### **1. Install Node.js (if not installed)**

* Check Node.js version:

  ```bash
  node -v
  ```
* If not installed, download from [https://nodejs.org](https://nodejs.org) and install.

---

### **2. Create a new project folder**

```bash
mkdir zenchain-test
cd zenchain-test
```

---

### **3. Initialize Node.js project**

```bash
npm init -y
```

This will create a `package.json`.

---

### **4. Install Ethers.js**

```bash
npm install ethers
```

---

### **5. Create the script file**

Create a file named `testConnection.js`:

```bash
nano testConnection.js
```

(or use VSCode, Notepad, etc.)
Paste the code:

```javascript
const { ethers } = require("ethers");

// Replace with ZenChain Testnet RPC URL
const ZENCHAIN_TESTNET_RPC = "https://zenchain-testnet.api.onfinality.io/public"; 

async function testConnection() {
    try {
        const provider = new ethers.JsonRpcProvider(https://zenchain-testnet.api.onfinality.io/public);

        const network = await provider.getNetwork();
        console.log("Connected to network:", network);

        const blockNumber = await provider.getBlockNumber();
        console.log("Latest Block Number:", blockNumber);
    } catch (error) {
        console.error("Connection failed:", error);
    }
}

testConnection();
```

---

### **6. Run the script**

```bash
node testConnection.js
```

---

### **Expected output (if connection works)**

```
Connected to network: { chainId: ..., name: ... }
Latest Block Number: 123456
```

---



