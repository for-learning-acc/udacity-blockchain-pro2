# Submission Infomation

* Truffle v5.5.26 and OpenZeppelin v2.3.0
* ERC-721 Token Name: StarNotaryService
* ERC-721 Token Symbol: SNS
* Token Address on Rinkeby Network: 0x336D58753d23bB48657EE819bD0271aE0E367af1

# Setup
## Dependencies

1. **Node and NPM** installed - NPM is distributed with [Node.js](https://www.npmjs.com/get-npm)
```bash
# Check Node version
node -v
# Check NPM version
npm -v
```

2. **Truffle v5.X.X** - A development framework for Ethereum. 
```bash
# Unsinstall any previous version
npm uninstall -g truffle
# Install
npm install -g truffle
# Specify a particular version
npm install -g truffle@5.0.2
# Verify the version
truffle version
```

3. **Metamask: 5.3.1**


4. [Ganache](https://www.trufflesuite.com/ganache) - Make sure that Ganache and Truffle configuration file have the same port.


5. **Other mandatory packages**:
```bash
cd app
# install packages
npm install --save  openzeppelin-solidity@2.3
npm install --save  @truffle/hdwallet-provider
npm install webpack-dev-server -g
npm install web3
```


### Run the application
1. Clean the frontend 
```bash
cd app
# Remove the node_modules  
# remove packages
rm -rf node_modules
# clean cache
npm cache clean
rm package-lock.json
# initialize npm (you can accept defaults)
npm init
# install all modules listed as dependencies in package.json
npm install
```

2. Start Truffle by running
```bash
# For starting the development console
truffle develop
# truffle console

# For compiling the contract, inside the development console, run:
compile

# For migrating the contract to the locally running Ethereum network, inside the development console
migrate --reset

# For running unit tests the contract, inside the development console, run:
test
```

3. Frontend - Once you are ready to start your frontend, run the following from the app folder:
```bash
cd app
npm run dev
```