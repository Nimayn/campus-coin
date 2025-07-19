Setup Instructions
Clone the repository:
git clone https://github.com/ash-047/CampusCoins-Blockchain-Project.git
cd CampusCoins-Blockchain-Project
Install dependencies:
npm install truffle -g  # If truffle is not installed globally
npm install ganache
pip install flask
pip install web3
Start Ganache:
Launch Ganache and create a workspace with desirable number of accounts.
Start/run the workspace and make sure it is running on port 7545
Deploy the smart contract:
truffle compile
truffle migrate --reset
This will automatically set up the roles for all accounts.

To manually set up the roles, you can run the following command:

truffle exec setup_roles.js
And to verify the assigned roles, run the following command:

truffle exec check_roles.js
Update the contract address:
python deploy.py
Start the Flask application:
python app.py
