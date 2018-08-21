# Lottery-smart-contract

A simple lottery smart contract with the follwing features :

- Any user on the Ethereum network can enter the lottery (as a player) who is able to fulfill the minimum requirement of sending more than 0.1 ether to the lottery pool. 
- Only the Manager ie. the person who deploys the contract can pick up the winner.
- The lottery gets reset after a winner is picked.
- Since Solidity doesn't have a random number generator library so a psuedo number generator has been defined which looks like this :
#random_number = uint(keccak256(abi.encodePacked(block.difficulty, now, players)))
(players is an array for storing addresses of all players participating in the lottery)
- Also the code for the React Web-app for the same lottery contract is available at: https://github.com/ppoply/Lottery-smart-contract-react-app

<strong> Note : This whole project is part of Udemy's "Ethereum and Solidity: The Complete Developer's Guide" course by Stephen Grider.</strong>
