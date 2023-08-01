## Abstract
The thesis explores the potential of integrating blockchain technology with the real estate 
sector to develop Web 3.0. The aim of this integration is to create a decentralized and 
transparent platform for real estate transactions that can improve efficiency, security, and trust 
in the sector. Multiple transactions, various unofficial fees, needless bureaucracy, the 
intervention of unqualified intermediaries, a lack of transparency, and other issues make it 
difficult to acquire land in Vietnam. According to studies, digitization might help Vietnam's 
land management system and solve these acquisition problems. Last but not least, however, 
mongoDBly offered a distinct conceptual digital framework for land purchase. The majority 
of recent land research evaluates blockchain technology as a viable remedy for these 
difficulties in Vietnam's land purchase procedure. In research paper concludes by system the 
potential of integrating blockchain technology with the real estate sector to develop Web 3.0. 
It also highlights the challenges and limitations of implementing blockchain technology in the 
real estate sector and suggests future research directions to overcome these challenges.
Web 3.0.
<p align="center">DEVELOPING WEB 3.0 BY INTEGRATING BLOCKCHAIN TECHNOLOGY WITH THE REAL ESTATE SECTOR.
</p>
<p align="center">
   <img src="https://i.ibb.co/yfGgNxr/web3-0.png">
</p>
## Features

- Seperate Portal for SuperAdmin and Admin.
- Quick Check for owners to view and verify their ownership.
- Search for properties based on survey number.
- Make your land available for sale with the ease of a click.
- Send and Receive Requests to purchase land.
- Buy approved property after making a deal with the owner.

## How to Run?

### Prerequisites:

<a style="color: red !important" href="https://nodejs.org/en/download/">`node js`</a>
<a href="https://www.trufflesuite.com/docs/truffle/getting-started/installation">`truffle`</a>
<a href="https://metamask.io/download">`MetaMask`</a>
<a href="https://www.trufflesuite.com/docs/truffle/getting-started/installation">`ganache`</a> (not mandatory)

1. Fire up the terminal and run the following command to clone the project.
```cmd
git clone https://github.com/
```
2. cd into client folder and run `npm install`
3. run npm start to view the frontend application on `localhost:3000`
```cmd
cd client
npm install
npm start
```
4. Repeat the same in server folder after creating a .env file with MONGOURI='/*Your mongodb URI*/'
```cmd
cd server
npm install
npm start
```
5. Now it's time to start the blockchain.
6. (If you are using ganache, then skip this) Change your truffle config file to run on port 8545 instead of 7545
7. cd into root directory and run `truffle develop`
8. This should create some test accounts and specify their private keys used to import in MetaMask later.
9. Within the truffle console run `compile` and then `migrate`
```cmd
truffle
>truffle compile
>truffle migrate
```
9. Make sure you run `migrate --reset` whenever you change the smart contract
10. (If you are NOT using ganache, then skip this) Open Metamask and create a Custom RPC on port 7545
11. Import the accounts using private key
12. Change the address /client/src/App.js#L74 ">here</a> to the address of your preferred SuperAdmin
13. Login from SuperAdmin and register Admins
14. Done! The land registry system is up and running!!
