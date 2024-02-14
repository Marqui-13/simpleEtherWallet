# Simple Ether Wallet Smart Contract

The Simple Ether Wallet smart contract provides a basic implementation of a personal wallet on the Ethereum blockchain. It enables the owner to receive ether and withdraw ether from the wallet securely. The contract is designed with simplicity in mind, ensuring that even those new to Ethereum and Solidity can understand and interact with it.

## Features

- Receive Ether: Automatically receive ether sent to the contract's address.
- Withdraw Ether: The owner can withdraw ether to their address.
- Check Balance: View the current ether balance of the wallet.

## Technology Stack

- Solidity ^0.8.13: The contract is written in Solidity.
- Ethereum Blockchain: The contract is intended to be deployed on the Ethereum blockchain.

## Smart Contract Functions

- `receive() external payable`: Allows the contract to receive ether.
- `withdraw(uint _amount) external`: Enables the owner to withdraw ether from the contract.
- `getBalance() external view returns (uint)`: Returns the contract's current ether balance.

## Deployment

To deploy this contract, you will need:

1. An Ethereum wallet with some ether for gas fees.
2. Access to a Solidity development environment, such as Remix IDE, Truffle, or Hardhat.

### Steps

1. Compile the Contract: Ensure that you are using a Solidity compiler version of ^0.8.13 or newer.
2. Deploy the Contract: Deploy the contract to your desired network (mainnet or testnet) using your chosen development environment.
3. Interact with the Contract: After deployment, you can interact with the contract through your development environment or a web3 interface.

## Interacting with the Contract

- To Receive Ether: Send ether to the contract's address.
- To Withdraw Ether: Call the `withdraw` function with the desired ether amount to withdraw (only the owner can do this).
- To Check Balance: Call the `getBalance` function to view the ether balance of the wallet.

## Security Considerations

- The `withdraw` function includes a require statement to ensure that only the owner can withdraw ether, enhancing security.
- Regularly monitor transactions to ensure that only authorized operations are being executed.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE) file for details.

## Acknowledgments

- Ethereum and Solidity documentation for providing the foundational knowledge needed to build this project.