# MyToken Contract

This contract implements a basic token system called "MyToken" in the Solidity programming language. The contract allows minting and burning of tokens, along with storing token details and balances for addresses.

## Requirements

1. The contract has the following public variables:
   - `token_name`: A string variable that represents the name of the token. In this case, the token name is "Ether".
   - `token_abbrv`: A string variable that represents the abbreviation of the token. In this case, the abbreviation is "ETH".
   - `token_total_supply`: An unsigned integer variable that represents the total supply of the token. The initial total supply is set to 10,000.

2. The contract uses a mapping to store balances of addresses. The mapping associates an address with its corresponding balance.

3. The contract provides a `mint` function that takes two parameters: an address and a value. This function increases the total supply of the token by the specified value and increases the balance of the provided address by that amount.

4. The contract provides a `burn` function that works the opposite of the `mint` function. It takes an address and a value as parameters and deducts the specified value from the total supply and the balance of the provided address.

5. The `burn` function includes conditionals to ensure that the balance of the sender address is greater than or equal to the amount that is supposed to be burned.

## Usage

1. Deploy the `MyToken` contract on the Ethereum network.
2. Access the public variables:
   - `token_name`: Retrieve the name of the token.
   - `token_abbrv`: Retrieve the abbreviation of the token.
   - `token_total_supply`: Retrieve the total supply of the token.
3. Use the `mint` function to create new tokens:
   - Provide an address and the amount of tokens to be minted.
   - The total supply and the balance of the provided address will be increased accordingly.
4. Use the `burn` function to destroy tokens:
   - Provide an address and the amount of tokens to be burned.
   - The total supply and the balance of the provided address will be reduced if the sender's balance is greater than or equal to the specified amount.

**Note:** It is essential to handle the deployment and interaction with the contract through a compatible Ethereum client or development framework.
