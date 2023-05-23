# Receiver-Tools 

This folder offers several tools that simplify the interaction with the Smart Contracts Lab oracle. 

## SCL_informed.sol

SCL_informed.sol should be imported into the Solidity code of your smart contract application. It is an *abstract contract* which means it is not a standalone contract but assists you in connecting to the oracle. By importing it into your contract, it allows you to call the following three functions:

- The *GetTransactionCosts* function calculates the value you need to send with the Order function. This value corresponds to the sum of the sender fee and the gas for the delivery transaction.

- The *Order* function is used to place an order as described in the corresponding commitment.

- The *CancelOrder* function allows you to cancel an unfilled order (for any reason). As a result, the sender fee will be reimbursed to the address from which the Order function was called .

## Minimal use case

The minimal use case is an example of a smart contract that interacts with the Smart Contracts Lab oracle. To learn how to order and receive data, this example might serve as a first point of reference.

## Additional Information

### Smart Contracts Lab Addresses

- Polygon Mainnet: 0x58e60cDC29099Aa54Df0EDCBF102896a819689Dc 
- Mumbai testnet: 0x58e60cDC29099Aa54Df0EDCBF102896a819689Dc 

### Smart Contracts Lab Commitments

- 1  Random Number Generator

