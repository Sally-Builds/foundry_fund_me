## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

- **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
- **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
- **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
- **Chisel**: Fast, utilitarian, and verbose solidity REPL.

### Test

```shell
$ forge test
$ forge test -vv #for console visibility
```

### Test file

```solidity
import {Test} from "forge-std/Test.sol";

contract FundMeTest is Test { //test must Inherit Test contract
    function setUp() external {} // this function runs first
}

```

### Types of Test
what can we do to work with addresses outside of our system or network?

1) Unit - Testing a specific part of our code
2) Integration - Testing how our code works with other parts of our code
3) Forked - Testing our code on a simulated real environment
4) Staging - Testing our code in a real environment that is not production


# Foundry Devops Tools