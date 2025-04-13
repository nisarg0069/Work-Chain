💼 WorkChain – A Blockchain-Based Freelance Platform

WorkChain is a decentralized freelance platform built using blockchain technology to ensure fairness, transparency, and security for both clients and freelancers.

This project was developed during a hackathon by Exception Squad (LDCE) to address common issues in freelancing like delayed payments, lack of trust, and centralized dispute resolution.

---

🚀 Features

- Smart contract-based escrow system for secure task payments
- Decentralized dispute resolution without third parties
- Immutable rating and review system stored on-chain
- Automatic payment release after deadline expiry
- Separate dashboards for clients and freelancers

---

🛠️ Tech Stack

Backend:
- Python 3.8+
- Flask (API and app logic)
- Flask-SQLAlchemy (ORM)
- Flask-Login (User authentication)
- Web3.py (Ethereum interaction)
- SQLite (for development)

Frontend:
- HTML, CSS, JavaScript
- Bootstrap 5, jQuery
- MetaMask (Wallet integration)

Blockchain:
- Solidity 0.8.0 (Smart contracts)
- Ganache (Local blockchain)
- Web3.js
- py-solc-x (Solidity compiler)

---

🧪 How It Works

1. Users register and log in using email and MetaMask
2. Clients create tasks and deposit funds in escrow
3. Freelancers accept tasks and begin work
4. Upon completion, clients approve the task or funds auto-release
5. Both users leave a rating stored on the blockchain

---

📂 Project Structure

work-chain/
├── contracts/           → Solidity smart contracts
├── templates/           → HTML templates for Flask
├── static/              → CSS, JavaScript, and assets
├── app/                 → Flask backend (routes and logic)
│   ├── auth/            → Login and registration logic
│   └── dashboard/       → Task and user logic
├── main.py              → App entry point
├── requirements.txt     → Python dependencies
└── README.md            → Project info

---

🔧 Setup Instructions

1. Clone the repository

   git clone https://github.com/your-username/work-chain.git
   cd work-chain

2. Install dependencies

   pip install -r requirements.txt

3. Make sure Ganache is running and MetaMask is connected

4. Start the Flask app

   python main.py

5. Open the app in your browser at http://127.0.0.1:5000

---

🎯 Future Enhancements

- Move to public Ethereum testnet or Polygon
- Add community-based dispute resolution
- Introduce milestone-based payments
- Implement trust score system for freelancers

---

👥 Team: Exception Squad – LDCE

Nisarg Dave  
Mugdha Bhangale  
Tisha Varma  
Kirtan Patel

---

📜 License

MIT License

---

“We don’t promise trust — we encode it.”
