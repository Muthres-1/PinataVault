# PinataVault

**PinataVault** is a decentralized file storage application leveraging **Ethereum** and **IPFS (via Pinata)** for secure and immutable file uploads. With PinataVault, users can upload, share, and view files securely while ensuring data integrity through blockchain technology.

---

## Features

- **Decentralized Storage**: Files are uploaded to IPFS via Pinata.
- **Secure Sharing**: Users can share file access with other Ethereum addresses.
- **Blockchain Integration**: Ethereum smart contract ensures access control and file integrity.
- **User-Friendly Interface**: Intuitive React-based UI for uploading and managing files.
- **Metamask Integration**: Seamlessly connects with Ethereum wallets.

---

## Tech Stack

- **Frontend**: React.js, Axios
- **Blockchain**: Ethereum, Solidity
- **File Storage**: IPFS (via Pinata)
- **Web3 Provider**: Ethers.js
- **Smart Contract**: `Upload.sol`

---

### Installation & Setup
## 1. Uninstall Previous Hardhat Version (If Installed)
      npm uninstall hardhat
## 2. Install Specific Hardhat Version
      npm install --save-dev hardhat@2.12.4 `
## 3. Initialize Hardhat
      npx hardhat
## 4. Install Hardhat Toolbox
      npm install --save-dev "hardhat@^2.12.4" "@nomicfoundation/hardhat-toolbox@^2.0.0"
## 5. Create React App for Client
      npm install create-react-app
      npx create-react-app client
      cd client
## 6. Install Additional Dependencies
      npm install --save-dev ajv@^7
## 7. Start the Development Server
      npm start
      
###Deployment
##1. Deploy Smart Contracts
##2. Ensure the blockchain is running locally. Use the following command to deploy the smart contracts:
      npx hardhat run --network localhost scripts/deploy.js

###Note:
     If the terminal running the blockchain is closed, the blockchain will be destroyed.

###Important Notes
     Pinata API Key
     Ensure the API key is active and not exhausted.
     Do not set the max_uses limit for the API key to avoid unexpected restrictions during uploads.


### Prerequisites
1. Node.js installed on your system.
2. Metamask browser extension.
3. Pinata account with API key and secret.

---

## Usage

1. **Connect Your Wallet**  
   Open the application and connect your Ethereum wallet using Metamask.

2. **Upload a File**  
   - Use the "Choose Image" button to select an image from your system.  
   - Click "Upload File" to pin your file to IPFS via Pinata.  
   - Your file's IPFS hash will be stored securely in the blockchain.

3. **Share File Access**  
   - Click the "Share" button to open the sharing modal.  
   - Enter the Ethereum address you wish to share access with and click "Share."  
   - You can view all addresses with access in the dropdown menu.

4. **View Files**  
   - Enter your Ethereum address or any shared address in the "Enter Address" field.  
   - Click "Get Data" to view the images associated with the address.

---

## Smart Contract Details

**Upload.sol** provides:  
- **File Storage:** Stores file hashes securely on IPFS using Pinata.  
- **Access Control:** Allows file owners to share access with specific Ethereum addresses.  
- **Data Retrieval:** Fetches stored file hashes based on user or shared permissions.

---


## License

This project is licensed under the [MIT License](./LICENSE). Please see the LICENSE file for details.

---

## Acknowledgments

- **[Pinata](https://www.pinata.cloud/):** For enabling efficient IPFS integration.  
- **[Ethereum](https://ethereum.org/):** For providing the blockchain infrastructure.  
- **[Metamask](https://metamask.io/):** For seamless wallet connectivity.  
