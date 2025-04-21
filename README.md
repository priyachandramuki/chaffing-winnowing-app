🕵️‍♀️ Cyber Sieve: Chaffing & Winnowing Web App with Hybrid Encryption

Cyber Sieve is a hacker-themed Flask web app that lets users hide and extract secret messages using **Chaffing & Winnowing** powered by AES + RSA hybrid encryption.

🔐 Built with:
- Flask (Python)
- Hybrid Encryption (AES + RSA)
- File support for `.txt`, `.pdf`, `.png`, `.docx`, audio/video
- Sleek hacker-style UI with dashboard layout

🚀 Features
- 🔒 Encrypt secret messages using a secret key and RSA public key
- 🧩 Chaff file generation for data camouflage
- 🔍 Winnow the real message using RSA private key and keyinfo
- 📁 Supports multi-format files
- 💡 Built for stealth, security, and fun

🛠️ How to Use

1. Chaffing:
   - Upload a file
   - Enter a secret message
   - Upload the receiver’s public key
   - Get a `.keyinfo` file and a chaffed binary file

2. Winnowing:
   - Upload the chaffed file and the `.keyinfo` file
   - Upload your private key
   - Extract the original hidden message

Local Setup

git clone git@github.com:priyachandramuki/chaffing-winnowing-app.git
cd chaffing-winnowing-app
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
python app.py
