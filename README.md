Project BrainWalletBasic (BWB)
Welcome to Project BrainWalletBasic (BWB), a project aimed at helping individuals recover lost Bitcoin wallets through brute-force methods using mnemonics and wallet address generation. This tool allows users to either use the BlockCypher API to check wallet balances or the Bitcoin Core version (coming soon).

Features:
Generates Bitcoin wallet addresses using mnemonics from the BIP-39 wordlist.
Validates wallet balances using the BlockCypher API.
Bitcoin Core integration (coming soon) to avoid API rate limits.
Customizable rate limits: 1000 Requests Per Day, 100 Requests Per Hour, and 3 Requests Per Second.
Saves mnemonics with non-zero balances for review.
Installation
Dependencies
Before running the tool, make sure the following dependencies are installed:

Python 3.7+
bip32utils - For generating Bitcoin addresses from the seed.
requests - For making API calls to the BlockCypher API.
tqdm - For displaying progress bars.
You can install the required Python packages by running:

bash
Copy code
pip install bip32utils requests tqdm
Usage
Clone the repository:
bash
Copy code
git clone https://github.com/YourRepo/BrainWalletBasic.git
Navigate to the project directory:
bash
Copy code
cd BrainWalletBasic
Run the Python script:
bash
Copy code
python brainwalletbasic.py
Enter your BlockCypher API token when prompted.
API Limits:
1000 Requests Per Day
100 Requests Per Hour
3 Requests Per Second
The script adheres to these limits automatically, preventing rate-limit issues.

Coming Soon:
Bitcoin Core Integration: Avoid API limits entirely by checking balances using a local Bitcoin Core node.
Project Structure:
brainwalletbasic.py: Main script for generating mnemonics, deriving wallet addresses, and checking balances.
used_mnemonics.txt: File that keeps track of mnemonics already used to prevent duplication.
bip39.txt: BIP-39 wordlist used for generating mnemonics.
intro_logo.py: Script that displays an intro screen with the BWB logo when the project is run.
Contributing
We are actively looking for contributors to improve the code and help us with the goal of recovering a lost wallet. If you'd like to contribute, feel free to submit a pull request or open an issue.

License
This project is licensed under the MIT License. Feel free to use, modify, and distribute this code as needed.

