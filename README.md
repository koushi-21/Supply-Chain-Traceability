# Decentralized Supply Chain Traceability System

A cloud-hosted blockchain application that simulates secure and transparent supply chain operations using Ethereum smart contracts.

## 🚀 Project Overview

This project demonstrates a decentralized supply chain system where users can:
- Assign and manage roles (e.g., Supplier, Manufacturer, Distributor)
- Order and manufacture materials
- Track every transaction through a local blockchain (Ganache)

Users interact with the system through a browser connected to MetaMask, enabling secure transaction signing and blockchain integration.

## 🌐 Hosted Environment

- **Cloud Platform**: Microsoft Azure (Linux VM)
- **Blockchain Network**: Ganache (local Ethereum blockchain)
- **Frontend Access**: Via the Azure VM's public IP (e.g., `http://<your-vm-ip>:<port>`)
- **Wallet Integration**: MetaMask

## 🛠️ Tech Stack

- **Frontend**: HTML, JavaScript
- **Backend**: Node.js (Express)
- **Blockchain**: Solidity smart contracts deployed on Ganache
- **Deployment**: Azure Virtual Machine

## 📦 Features

- Role-based access for supply chain participants
- Smart contract-based operations (Order, Manufacture, Ship)
- MetaMask prompts for every blockchain interaction
- Real-time tracking of material flow with immutable records

## 🧪 How to Use

1. Clone the project using `git clone`
2. Run cmd in the project directory. Enter the command `npm install -g truffle`
3. To install dependencies, enter `npm i`
4. Open Ganache and make sure you have the default RPC server address and the Network ID as HTTP://127.0.0.1:7545 and 5777 respectively. In case they are different, make sure to modify it as per your requirements in turffle-config.js file.
5. Run `truffle migrate` on your CMD. This will deploy the smart contract to the Blockchain.
6. Open your browser and download the MetaMask extension. Import one of the accounts from your Ganache Workspace.
7. To run the DApp, open folder "client" with `cd client` on your terminal.
8. Install all the packages in package.json file through `npm i` and install web3 with `npm install -save web3`. Note: This step is to be done in your-project-dir/client/ on your terminal.
9. Run the app with `npm start`. This should launch your node server.
10. On your MetaMask extension, make sure you are connected to your local Ganache network instead of Ethereum Mainnet. You can do that by clicking on "Add network" and entering the following:
      Network Name: _Anything works_
      New RPC URL: HTTP://127.0.0.1:7545
      Chain ID: 1337
      Currency Symbol: ETH
Click save and connect your MetaMask wallet to this test network.
11. In case there are any issues after this step, run `truffle migrate --reset` and then `truffle migrate` followed by `npm start`.

You can make this cloud deployable by following the same steps on a VM in Azure and use the public IP of the VM to connect to the blockchain system from your device(s) via the internet.


## 📄 Outcomes

- Cloud-hosted, user-accessible blockchain server
- Real-time supply chain simulation with smart contracts
- Transparent and secure transaction logging

## 🔐 Security Note
All operations are executed through MetaMask, ensuring user-side key management and secure signing of blockchain transactions.

## 👨‍💻 Authors

- Koushik Panchadarla, Kanuri Manikrishna Kaushik

---
