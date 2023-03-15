## [M2 Domain Project Documentation](https://domain-serviceon-polygon.vercel.app/)

## Overview 
The Domains contract is an ERC721 token that allows users to register and manage domain names. Each token represents a unique domain name and is owned by the user who registered it. The contract stores the name, record, and owner address of each domain.

Contract Structure
The Domains contract inherits from ERC721URIStorage, which is an OpenZeppelin library contract that implements the ERC721 interface for non-fungible tokens with a URI-based metadata extension.

## State Variables
### The contract has several state variables:

`owner`: the address of the contract owner, who has the ability to withdraw funds from the contract.
`_tokenIds`: a Counters.Counter object that is used to keep track of the current token ID when minting new tokens.
`names`: a mapping of token IDs to domain names.
`records`: a mapping of domain names to records.
`domains`: a mapping of domain names to owner addresses.
`tld`: a string representing the top-level domain for all registered domains.
`SVG_PART_ONE`: a string containing SVG data for a graphical representation of the domain name.
## Functions
### The contract has several functions:

`constructor`: sets the contract owner and top-level domain.

`register`: allows a user to register a domain name by minting a new token with the given name.

`setRecord`: allows the owner of a domain to set the record associated with the domain.

`getRecord`: allows anyone to retrieve the record associated with a domain.

`transfer`: allows the owner of a domain to transfer ownership of the domain to another Ethereum address

`getDomainOwner`: allows anyone to retrieve the owner address associated with a domain.

`tokenURI`: overrides the tokenURI function from the ERC721URIStorage contract to return metadata for a given token ID.
## Modifiers
### The contract has two modifiers:
In addition, the contract includes several modifiers for access control:

`onlyOwner`: restricts access to functions that can only be called by the contract owner (specified in the owner variable)

`isAuthorized`: restricts access to functions that can only be called by the owner of a particular domain

`unregistered`: can be applied to functions that require a domain name that has not already been registered.
## Libraries
### The contract imports two external libraries:

`Base64`: contains functions for encoding and decoding base64 strings.

`StringUtils`: contains string manipulation functions.
## Conclusion
That's an overview of what the Domains contract does and how it's structured. With this documentation, other developers should be able to understand the purpose and functionality of the contract.

Finally, the contract includes several error functions for handling common error cases, such as unauthorized access or already registered domains.
