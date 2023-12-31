---

# AITU_Shadyman Token

## Overview

AITU_Shadyman is an ERC-20 token built on the Ethereum blockchain. It is implemented using the OpenZeppelin library, which provides standard implementations of the ERC-20 interface.

## Features

- **Token Name:** AITU_Shadyman
- **Symbol:** ATS
- **Total Supply:** 2000 ATS
- **Owner:** None.

## Getting Started

To deploy and use AITU_Shadyman token, follow these steps:

1. **Install Dependencies:**
   - Ensure you have Node.js and npm installed.
   - Install the necessary dependencies using `npm install`.

2. **Compile Smart Contract:**
   - Run `npx hardhat compile` to compile the Solidity smart contract.

3. **Deploy Smart Contract:**
   - Deploy the contract to the Ethereum blockchain using `npx hardhat run scripts/deploy.js`.

4. **Interact with the Contract:**
   - Use a tool like Remix or deploy a frontend to interact with the contract.
   - Alternatively, use the available functions in the contract, such as `getLastTransactionTimestamp`, `getTransactionSender`, and `getTransactionReceiver`.

## Smart Contract Details

- **getLastTransactionTimestamp:**
  - Returns the timestamp of the latest transaction in string format.

- **getTransactionSender:**
  - Returns the address of the sender of the current transaction.

- **getTransactionReceiver:**
  - Returns the address of the contract itself.

## Example Usage

```
function getLastTransactionTimestamp() external view returns (string memory) {
        return Strings.toString(block.timestamp);
  }
```

```
function getTransactionSender() external view returns (address) {
        return _msgSender();
    }
```

```
function getTransactionReceiver() external view returns (address) {
        return address(this);
    }
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [OpenZeppelin](https://openzeppelin.com/) for providing the ERC-20 implementation.

## Contact

For any inquiries, please contact [SHADYMAN] at [m.m.shdmn@gmail.com].

---
