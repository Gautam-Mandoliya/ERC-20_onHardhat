# Project: ERC20 TOKEN

## Description
The token smart contract is a basic implementation of an ERC-20 token using Solidity. It allows for the creation of a custom token with functionalities for minting, burning, and transferring tokens.

The key features of the smart contract are as follows:

`Token Creation:` The contract allows the owner to create a custom token by providing a name, symbol, and initial supply of tokens. The total supply of tokens is initialized with the provided initial supply, and the owner is assigned the entire supply.

`Minting:` The owner of the contract can mint additional tokens to a specified address. This function increases the total supply and updates the balance of the recipient accordingly.

`Burning:` Any address can burn their own tokens by calling the burn function. This function deducts the specified amount of tokens from the caller's balance and reduces the total supply accordingly.

`Transferring:` The transfer function allows any address to transfer tokens to another address. It deducts the specified amount of tokens from the sender's balance and adds them to the receiver's balance.

# Installation

First Ensure that you have Hardhat installed locally in your Gitpod workspace. 
If you haven't installed it yet, you can run the following command to install it: ` npm install hardhat `

1. In your terminal, navigate to the root directory of your Hardhat project.
Start the local Hardhat network by running the following command:` npx hardhat node `
(This command will start a local Ethereum network with a set of accounts and private keys, along with the associated blockchain.)
2.Once the local network is running, you will see a list of accounts along with their private keys in the terminal. Make note of the private keys for the accounts you want to use for interacting with the contract.

3.Open Remix (https://remix.ethereum.org/) in your web browser.

4.Create a new file and copy the updated contract code into it.

5.Compile the contract by selecting the appropriate compiler version (0.8.0 in this case) from the "Compiler" tab and clicking on "Compile MyToken.sol".

6.Deploy the contract by selecting the "Deploy & Run Transactions" plugin from the sidebar.

7.Choose "Injected Provider-Metamask" as the environment to connect Remix to your local Hardhat network.

8.In the "Deploy" section, enter the desired values for the name, symbol, and initialSupply parameters.

9.Click on the "Deploy" button.

10.Remix will prompt you to connect to a Metamask. Click on the "Connect" button and select "Custom" from the dropdown.

11.In the "Custom provider" section, enter the following details:

Network name: Any name you prefer (e.g., "Hardhat Local")
RPC URL: http://localhost:8545(or you can find it in 'port' option, copy address from there)
Chain ID: 31337 (or the chain ID of your local network)
Click on the "Connect" button.

12. Remix is now connected to your local Hardhat network. You can interact with the deployed contract by calling its functions, just like you would with a live network.

13. To execute transactions, click on the "transact" button next to the desired function in the "Deployed Contracts" section. Confirm the transaction in the Metamask popup using the private key of the desired account from your local Hardhat network.

14. Remix will display the transaction details, and you can see the emitted events and any changes in the contract state.

By following these steps, you can interact with the smart contract deployed on your local Hardhat network using Remix as the interface. Make sure to have both the local Hardhat network and Remix running simultaneously for seamless interaction.

# Author
Gautam Mandoliya

## License
This project is licensed under the MIT License - see the LICENSE.md file for details
