# UniversalToken (ERC-1400) fork

This project is a fork of [UniveralToken](https://github.com/Consensys/UniversalToken) (ERC-1400) by Consensys.

Its main purpose is to update the libraries to facilitate the compilation of smart contracts with [Hardhat](https://hardhat.org).

We do not guarantee the security or proper functioning of original smart contracts. No modification compared to the original project has been made on these.

Library:

- Solidity version: 0.8.7 (same version as the original project)

- OpenZeppelin version: [4.7.3](https://github.com/OpenZeppelin/openzeppelin-contracts/releases/tag/v4.7.3)

It is not possible to install and use a version > 4.7.3 (e.g 4.8.0) because the smart contracts are not compatible.

## Tools

To install the required node modules required:

```bash
npm install
```

Compile the contracts:

```bash
npx hardhat compile
```

## Contracts

In [compilation](./compilation):

- [ERC1400.json](compilation/ERC1400.json) is the resulting input JSON for the contract [ERC1400.sol](contracts/ERC1400.sol)
- [EtherscanVerification.sol](EtherscanVerification.sol) is the flattening file for [ERC1400.sol](contracts/ERC1400.sol) to verify it on Etherscan

See [Hardhat - Flattening your contracts](https://hardhat.org/hardhat-runner/docs/advanced/flattening)
