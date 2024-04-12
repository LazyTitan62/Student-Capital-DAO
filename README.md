## DAO Workflow

### Applicants

1.  setup wallet
2.  Mint nft
3.  Submit application via Deform

### Backend

1. connect result csv to google form
2. pull results from Google form
3. import the applications to our website

### Committe:

1. review the applications on the website
2. vote on the committe portal

### Smart Contract

1. smart contract collects the result and determines the winner
2. informs the website about the winner
3. smart contract distributes the funds to the winner

## Website

Applications that recieved grants will be posted on the website.

## Deform

Applications will be submitted through Deform which is gated with NFT.

Submission guide: tbd

## Smart Contract

-   Solidity smart contract on arbitrum
-   right to vote: NFT gated or wallet address
-   Every application will be identified using the following information:

```
struct application {
    address walletAddress;
    uint256 number;
    uint8 votes;
    uint8 grantAmount;
    boolean receivedGrant;
}
```

-   An application will only be passed if over half of the committee members vote for it.
-   Once an application is passed, the contract will send grants to the given wallet address.

## Wallet

Phantom: https://phantom.app/

All applicants should set up a their own Phantom wallet in order to receive grants.

Tutorial: tbd
