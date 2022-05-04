# Supply chain & data auditing


Summary
This project contains an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer.In this project, I have created a coffee supply chain solution on Ethereum using smart contracts with role and access to track and verify a product's end to end lifecycle.  The code for this project is in the `coffee-supply-chain/` folder.



ganache-cli accounts used here...
```
Contract Owner: accounts[0]  0x27d8d15cbc94527cadf5ec14b69519ae23288b95
Farmer: accounts[1]  0x018c2dabef4904ecbd7118350a0c54dbeae3549a
Distributor: accounts[2]  0xce5144391b4ab80668965f2cc4f2cc102380ef0a
Retailer: accounts[3]  0x460c31107dd048e34971e57da2f99f659add4f02
Consumer: accounts[4]  0xd37b7b8c62be2fdde8daa9816483aebdbd356088

  Contract: SupplyChain
    ✓ Testing smart contract function harvestItem() that allows a farmer to harvest coffee (108ms)
    ✓ Testing smart contract function processItem() that allows a farmer to process coffee (58ms)
    ✓ Testing smart contract function packItem() that allows a farmer to pack coffee (58ms)
    ✓ Testing smart contract function sellItem() that allows a farmer to sell coffee (55ms)
    ✓ Testing smart contract function buyItem() that allows a distributor to buy coffee (67ms)
    ✓ Testing smart contract function shipItem() that allows a distributor to ship coffee (66ms)
    ✓ Testing smart contract function receiveItem() that allows a retailer to mark coffee received (65ms)
    ✓ Testing smart contract function purchaseItem() that allows a consumer to purchase coffee (52ms)
    ✓ Testing smart contract function fetchItemBufferOne() that allows anyone to fetch item details from blockchain
    ✓ Testing smart contract function fetchItemBufferTwo() that allows anyone to fetch item details from blockchain


  10 passing (619ms)
```
UML Diagrams

Activity Diagram
![Activity Diagram](images/uml/activity_diagram.png)

Sequence Diagram
![Sequence Diagram](images/uml/sequence_diagram.png)

State Diagram
![State Diagram](images/uml/state_diagram.png)

Classes
![Classes Diagram](images/uml/class_diagram.png)

Libraries Write-up
Below are the dependencies in my `packages.json` file:
```json
"dependencies": {
    "truffle": "^5.1.51",
    "truffle-hdwallet-provider": "^1.0.17",
    "web3": "^1.3.0"
  }
```

Node version used is v12.22.6

### Library Usage:
- `truffle`: truffle is a  development environment, testing framework and asset pipeline for blockchains using the Ethereum Virtual Machine (EVM). I used `truffle` to deploy my smart contracts to the `Rinkeby` test network.


The Rinkeby contract address for this project is: `0xd35BbA5a1d3e32Ae44e8e9817f73bD6963c17464`
