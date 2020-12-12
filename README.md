# Running the Vegi Network

This network is based on the official "test-network" example by Hyperledger Fabric.
For more information, see [Using the Fabric test network](https://hyperledger-fabric.readthedocs.io/en/latest/test_network.html)

The network is first started with three organizations including one peer for each organization. Certificate Authorities are used for authorization and CouchDB is used to store the world state.

## Quickstart

1. First, you need to follow the instructions to [Install the Samples, Binaries and Docker Images](https://hyperledger-fabric.readthedocs.io/en/latest/install.html).
2. Navigate into the network-config folder:
```
cd ./network-config
```
3. Start the network:
```
./network.sh up
```
4. Create a channel (default name is set to "mychannel"):
```
./network.sh createChannel
```
5. Deploy the chaincode located in the chaincode folder:
```
./network.sh deployCC
```
The network is now ready to perform further actions. To add a fourth organization later on, run the following commands:
```
cd ./addOrg4
./addOrg4.sh up
```
To bring the network down again, navigate back into the network-config folder:
```
cd ../
./network.sh down
```
