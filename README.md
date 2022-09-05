# BlockshipDAO

## Insipiration:
Inspiration behind this project came from NounsDAO. NounsDAO bootstraps identities and provides a tressury which is controlled by governance. 

We’ll discuss different components of BlockshipDAO in this document and also discuss the vision of this project.

## Idea:
Idea behind BlockshipDAO is that to provide treasury for community good projects which includes:
- DAO Tooling
- ZKPs
- Infrastructure / Blockchain
- DeFi helper tools
- Funding research proposals

Tressury will be build using NounsDAO model where each day a random textual NFT will be generated.

## Functionalities:
### NFT Buying:
Every day at 00:00 UTC a random textual NFT (BLOCKs) will be generated and people can bid on it. Whoever has the highest bid at the end of the day will receive that BLOCK.
### Proposal Creation:
People can create proposals. For proposal creation people need to have 2 BLOCKs.
### Voting:
People can vote on proposals. For voting 1 BLOCK = 1 VOTE

## Front-end:
Front-end will have three pages. 
### BID PAGE:

[Bid Area](https://nouns.wtf/)

It will look like NounsDAO page. The only difference will be the textual NFT. 

### VOTE/SUBMIT:
[Governance Page](https://nouns.wtf/vote) the UI/UX will resemble like this. 

## Technical Architecture:
### Random BLOCK generator:
We will need to build a class where we have a list of words in dictionary and daily a random 7 words NFT is generated like LootBox.
### NFT Transfer:
Whenever the day is completed, backend server will be responsible for the minting of the NFT to the highest bidder on the Polygon Blockchain.
### Bid Collector:
Backend server will be responsible for the storage of bids and addresses off-chain. No smart contract work is needed in this component. 
### Smart Contract:
ERC721 contract will be made. More like LootBox where the randomness can be predicted by putting the NFT id. 

## Open discussions:
- Where to host backend?
- UI/UX Design.
- Front-end tech stack.
- Backend tech-stack.
- Incentivization model for people to build reputation only if the proposal is in the above category defined and for voters as well. Kind a like soul bound tokens. 
