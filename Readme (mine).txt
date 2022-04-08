1) First, you should already have npm installed. Then, you can run the following, both to install and upgrade Yarn:

npm install --global yarn


2) Check that Yarn is installed by running:

yarn --version

(			If it gives an error:
	i) Run this: Set-ExecutionPolicy –Scope CurrentUser
	ii) Give 'RemoteSigned' as the 'ExecutionPolicy'
	iii) Then run this: Set-ExecutionPolicy -ExecutionPolicy RemoteSigned
)


3) Run 'yarn start'

--------------------------------------------------------------------------------

QUICK START

1) Install all dependencies:

yarn install


2) Rename '.env.example' to '.env' in the main folder and provide your 'appId' and 'serverUrl' from your Moralis server.
(Here is a related document to start a Moralis server:

https://docs.moralis.io/moralis-dapp/getting-started/create-a-moralis-dapp
)


3) Locate the 'MoralisDappProvider' in src/providers/MoralisDappProvider/MoralisDappProvider.js and paste the deployed marketplace smart contract address and ABI.


4) Sync the 'MarketItemCreated' event /src/contracts/marketplaceBoilerplate.sol contract with your Moralis Server, making the tableName MarketItems.


5) Run your App:

yarn start