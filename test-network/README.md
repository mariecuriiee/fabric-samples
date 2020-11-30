## Running the minimal test network

This is a minimal example of the official fabric-samples test-network. 
This repository includes the following modifications:
- all files that were not necessary to run the test-network were deleted
- default database was set to CouchDB
- default chaincode language was set to javascript (as the only available chaincode is in javascript in this repo); therefore, all lines/files associated with different languages were deleted
- default authentication uses CAs and not cryptogen; therefore, all lines/files associated with cryptogen were deleted

Steps to start and use the network:

1. Download the binaries: [Install the Samples, Binaries and Docker Images](https://hyperledger-fabric.readthedocs.io/en/latest/install.html)

2. Start the network: `./network.sh up`

3. Create a channel: `./network.sh createChannel`

4. Deploy the javascript chaincode: `./network.sh deployCC`

5. Perform further steps to interact with the network. More details: [Using the Fabric test network](https://hyperledger-fabric.readthedocs.io/en/release-2.2/test_network.html)

6. Bring down the network: `./network.sh down`
