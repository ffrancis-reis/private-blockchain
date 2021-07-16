# Private Blockchain Application

### Introduction

This project consists in a simple private blockchain to be familiared with some fundamentals concepts like block, blockchain, wallet, blockchain identity and prrof of existence. It is a REST API that expose some funcionalities regarding a private blockchain, one of Udacity's Blockchain Developer Nanodegree course projects.

### Getting Started

1. Clone this repository
2. Run it and test it out

### Dependencies

1. Install the [Bitcoin Core Test tool](https://bitcoin.org/en/full-node)
2. Install the [VS Code IDE](https://code.visualstudio.com/)
3. Install the [Node.js engine](https://nodejs.org/en/)
4. Install or use the [Postman](https://www.postman.com/) tool from web

**Important** The Bitcoin Core Test tool lets you test your apllications that have blockchain tech attached to it. It's advisable to check its documentation to get a better knowledge. I suggest adding the **prune** parameter on its configuration file **bitcoin.conf** so that it will not download the entire database chain associated with Bitcoin, because as of this day, it is more than 300GB of size.

### Instructions

1. Open up the project on your familiar IDE (like VS Code), and run the command below in the terminal to install the required dependencies:

```powershell
  npm install
```

2. Run it with the command below:

```powershell
  npm start
```

3. Then you can test the API endpoints with your familiar REST API requests tool like Postman. I've added an Insomnia collection file that contains all the requests from the API.

4. To request an ownership and test the requestOwnership request, you will need a valid bitcoin wallet address, that can be generated on the Bitcoin Core Testnet tool. On the testnet tool (v0.21.1) go to the Window menu, then Console option and run the command bellow to get a new address that is associated with private key (remember to test it with the Testnet tool/network of the Bitcoin Core software instead of the production one).

```powershell
  getnewaddress [address-name] legacy
```

5. To test the submitStar request, you will need to sign the message with your generated key. On the testnet tool (v0.21.1) go to the File menu, then Sign message. Insert the address, the message and the sign it to get resulting signature. Then you can use the signature to test the request.

### Output

At the very end you have been created a star, signed it with your bitcoin wallet and added into your private blockchain.

