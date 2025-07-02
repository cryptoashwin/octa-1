STEP BY STEP WALLET GENERATION GUIDE OF OCTRA { CODESPACE }

🔹 Step 1: Install Bun

curl -fsSL https://bun.sh/install | bash
source ~/.bashrc
bun --version

2. Open terminal in gitpod and install Python

sudo apt install python3 python3-pip python3-venv python3-dev -y

2. Run these commands :

git clone https://github.com/octra-labs/octra_pre_client.git
cd octra_pre_client
python3 -m venv venv
source venv/bin/activate # for windows use: venv\Scripts\activate
pip install -r requirements.txt
cp wallet.json.example wallet.json


3. Open wallet.json

nano wallet.json

4. Edit it (change placeholders to your wallet data):

{
  "priv": "private-key-here",
  "addr": "octxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "rpc": "https://octra.network"
}

5. Run to open frontend UI to make transaction

   ./run.sh
