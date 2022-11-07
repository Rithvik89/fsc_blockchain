# fsc_blockchain
Food supply chain Monitoring on a blockchain network

# Prerequisites :

1.Clone the Entire Repo.
2.If working with windows install WSL and start working in virtual linux environment.
3.Install Nodejs and golang and npm(latest versions).
4.Install docker and docker compose.

# Step 1:
SetUp Block-chain network

1. cd to test_network.
2. execute command ./network.sh up -ca (node peers, orderer, certificate authorities starts running)
3. execute command ./network.sh createChannel (channel with default name myChannel gets created)

# Step 2:
Deploy chain-code(smart contract) on peers and channel

1. execute command ./network.sh deployCC -ccn basic -ccp ../asset-transfer-basic/chaincode-go -ccl go

# Step 3:
Start Application server

1. Open a new tab in terminal.
2. cd to asset-transfer-basic/application-javascript.
3. Run npm install and node app.js to start app server.


Official Docs:
https://hyperledger-fabric.readthedocs.io/en/release-2.2/
