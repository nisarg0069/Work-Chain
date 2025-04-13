# Blockchain-Based Freelance Platform

A decentralized application (DApp) that connects freelancers with clients through secure blockchain technology, smart contracts, and transparent payments.

## 🚀 Features

- **Blockchain Integration**: Secure transactions using Ethereum smart contracts
- **Two User Roles**: Register as either a client or freelancer
- **Task Management**: Create, accept, complete, and review tasks
- **Decentralized Payments**: Escrow payments released only upon task completion
- **Reputation System**: Build verifiable work history on the blockchain
- **MetaMask Integration**: Connect your Ethereum wallet for seamless transactions

## 📋 Prerequisites

- Python 3.8+
- Flask and Flask extensions
- Ganache (local Ethereum blockchain)
- MetaMask browser extension
- Solidity 0.8.0

## 🔧 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/blockchain-freelance.git
   cd blockchain-freelance
   ```

2. Install required packages:
   ```bash
   pip install flask flask-sqlalchemy flask-login web3 pycryptodome solcx
   ```

3. Install Solidity compiler:
   ```python
   from solcx import install_solc
   install_solc('0.8.0')
   ```

4. Setup your local blockchain environment:
   - Install and launch Ganache
   - Configure it to run on port 7545 with Chain ID 1337

5. Configure MetaMask:
   - Connect MetaMask to Ganache network (http://127.0.0.1:7545)
   - Use Chain ID: 1337
   - Import accounts from Ganache using private keys

## 🏃‍♂️ Running the Application

1. Initialize the database:
   ```bash
   flask shell
   >>> from main import db
   >>> db.create_all()
   >>> exit()
   ```

2. Start the application:
   ```bash
   python main.py
   ```

3. Access the application at `http://127.0.0.1:5000`

## 📱 Usage Guide

### For Clients
1. Register as a client
2. Connect your MetaMask wallet
3. Create tasks with detailed descriptions, budgets, and deadlines
4. Deploy smart contracts when a freelancer accepts your task
5. Release payment when satisfied with delivered work
6. Leave reviews for freelancers

### For Freelancers
1. Register as a freelancer
2. Connect your MetaMask wallet
3. Browse and accept available tasks
4. Submit completed work
5. Receive payment directly to your wallet upon client approval
6. Build reputation through positive reviews

## 💰 Smart Contract Integration

The platform uses Ethereum smart contracts to:
- Hold funds in escrow until work is approved
- Automatically release payments to freelancers upon client approval
- Track all transactions and task status changes in the blockchain
- Provide complete transparency and immutability

## 🔄 Blockchain Workflow

1. Client creates a task
2. Client deploys a smart contract with the task budget
3. Freelancer accepts the task
4. Freelancer completes the work and marks it as done
5. Client approves the work and releases payment
6. Smart contract transfers funds to the freelancer
7. All actions are recorded on the blockchain

## 📝 Notes

- The platform uses a simplified blockchain implementation for demonstration
- For production, you would deploy to a testnet or mainnet
- Contract gas costs are not optimized for this demo version

## ⚠️ Troubleshooting

- If MetaMask transactions don't appear in Ganache, ensure Chain IDs match (1337)
- Reset your MetaMask account if transactions are stuck
- Make sure you're using the correct network in MetaMask
- Check that Ganache is running before starting the application

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.
