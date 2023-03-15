# M2 Domain Service
## Project description
M2 Domain is a Blockcahain base domain service build on Polygon Pos chain, that help individual, organisation to register their domain name on the smart contract and own it. It allows suers to register a domain name and associate it with a digital asset as NFT which is a digital representation of the domain name created insted of a long complex address.
The domain is mapped such that only the owner of the domain can have access to the editing feature, except a full ownership has been transfer to another user.
## Contract Structure
The Domains contract inherits from ERC721URIStorage, which is an OpenZeppelin library contract that implements the ERC721 interface for non-fungible tokens with a URI-based metadata extension.

## State Variables
### The contract has several state variables:

1. `owner`: the address of the contract owner, who has the ability to withdraw funds from the contract.
2. `_tokenIds`: a Counters.Counter object that is used to keep track of the current token ID when minting new tokens.
3. `names`: a mapping of token IDs to domain names.
4. `records`: a mapping of domain names to records.
5. `domains`: a mapping of domain names to owner addresses.
6. `tld`: a string representing the top-level domain for all registered domains.
7. `SVG_PART_ONE`: a string containing SVG data for a graphical representation of the domain name.
## Functions
### The contract has several functions:

1. `constructor`: sets the contract owner and top-level domain.
2. `register`: allows a user to register a domain name by minting a new token with the given name.
3. `setRecord`: allows the owner of a domain to set the record associated with the domain.
4. `getRecord`: allows anyone to retrieve the record associated with a domain.
5. `transfer`: allows the owner of a domain to transfer ownership of the domain to another Ethereum address
6. `getDomainOwner`: allows anyone to retrieve the owner address associated with a domain.
7. `tokenURI`: overrides the tokenURI function from the ERC721URIStorage contract to return metadata for a given token ID.
## Modifiers
### The contract has two modifiers:
In addition, the contract includes several modifiers for access control:

1. `onlyOwner`: restricts access to functions that can only be called by the contract owner (specified in the owner variable)
2. `isAuthorized`: restricts access to functions that can only be called by the owner of a particular domain
3. `unregistered`: can be applied to functions that require a domain name that has not already been registered.
## Libraries
### The contract imports two external libraries:

1. `Base64`: contains functions for encoding and decoding base64 strings.
2. `StringUtils`: contains string manipulation functions.
## Conclusion
## Technologies used
1. React
2. TelwinCss
3. Hardhat
4. Metamask
5. Quicknode end point
6. Solidity
7. Openzepelin
8. Polygon testscan
9. Mumbai Testnet
10. ERC721

## How to use

1. Go to [https://domain-serviceon-polygon.vercel.app/](https://domain-serviceon-polygon.vercel.app/)
2. Click on Connect wallet to connect your wallet and switch to mumbai
3. Enter the domain you want to mint, provide the Domain description, and click 'mint' to continue
4. Your domain will show as the recent mint domain on the dashboard
5. Click on the Domain to see your digital representation of the domain on opensea testnet

## Dapp Before wallet connect
![before connecting your wallet](https://user-images.githubusercontent.com/41795852/225465406-bc931491-3d26-443f-bbc4-6d6980517515.PNG)

## Wallect connected
![after wallet connect](https://user-images.githubusercontent.com/41795852/225465507-8779d711-278e-45fb-98ac-5673ccd28b6e.PNG)

## Switch to mumbai Tesnet
![before network switch](https://user-images.githubusercontent.com/41795852/225465557-16565430-3d1b-46e2-b827-644df601d040.PNG)

## Running Project Locally

1. Fork the repo
2. Clone the repo
3. After cloning the repo, go to [Quicknode][(https://www.quicknode.com/endpoints)](https://www.quicknode.com/endpoints) to make an account and generate your API endpoint key
4. Rename the `.env.example` file on the root of the project to `.env`, then paste your API endpont key in the `.env` file
5. Run `npm install` to install all the dependencies
6. Run `npm run dev` to start the project
7. Go to [http://localhost:3000](http://localhost:3000) to see the project running

## Contributing

If you want to contribute to this project, please read the [contributing guide](./CONTRIBUTING.md). If you have any ideas or suggestions, feel free to open an issue or a pull request. 

If you like this project, please give it a star ⭐️

## Acknowledgement

Built with 💗 by [samailamalima](https://github.com/samailamalima). Inspired by [BuiltSpace](https://buildspace.so/), powered by [Grandidah LLC](https://grandida.com/).
