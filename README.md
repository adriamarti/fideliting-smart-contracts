# Fideliting Smart contracts

Fideliting is a customer loyalty system based on Blockchain that allows the association of businesses of different types and sizes in a single program.

The project was born during the completion of the BitBCN School Blockchain Program as part of the final project.

## Pre-Requisites

node v10.5.0 (npm v6.1.0)

## Steps to start working

0. Clone the repo and install all dependencies
```bash
git clone https://github.com/adriamarti/fideliting-smart-contracts.git
cd fideliting-smart-contracts
npm install
```

1. Install Truffle
```bash
npm install -g truffle
```

2. Start the Truffle console to compile, test and migrate
```bash
truffle develop
```

3. Once you have started the Truffle console you can compile, test and migrate just by typing
```bash
compile
test
migrate
```

4. To close the Truffle Console type
```bash
.exit
```

## Connect to Kaleido
> :closed_lock_with_key: To follow the next steps you have to get access to the Kaleido Account, send an email to adria.marti.blasco@gmail.com to get access into the Kaleido platform.

In Kaleido, select the node you want to connect to, then choose **+ Connect Node**.

1. Select **Native JSON/RPC**

2. Choose an application credential to use for this connection.

3. Choose the **Truffle Suite** connection type.

4. Copy the connection info from this panel into the respective variables inside of **truffle-config.js**. If you are using Quorum in this environment, ensure to uncomment the type: "quorum" property on your network object.
```javascript
const appCred = 'yourappcred';
const connectionURL = 'nodeConnectionURL';
```
```javascript
type: 'quorum' // Use this property for Quorum environments
```

5. Migrate your contracts to your Kaleido chain!
```bash
truffle migrate
```