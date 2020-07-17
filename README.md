
$ truffle version
Truffle v5.1.34 (core: 5.1.34)
Solidity v0.5.16 (solc-js)
Node v11.10.1
Web3.js v1.2.1

$ truffle init

Starting unbox...
=================

✔ Preparing to download box
✔ Downloading
✔ cleaning up temporary files
✔ Setting up box

Unbox successful, sweet!

Commands:

  Compile:        truffle compile
  Migrate:        truffle migrate
  Test contracts: truffle test


2672$ truffle compile

Compiling your contracts...
===========================
> Compiling ./contracts/Migrations.sol
> Compiling ./contracts/TodoList.sol
> Artifacts written to /Users/fab/workspace/initethereumsoliditytodo/build/contracts
> Compiled successfully using:
   - solc: 0.5.16+commit.9c3226ce.Emscripten.clang

2675$ trufgfle migrate
2_deploy_contracts.js
=====================

   Deploying 'TodoList'
   --------------------
   > transaction hash:    0x20c30196aee04cbb6dd2dc6904d26fb0a92822f2e5362d22a1ef0749b44fd17e
   > Blocks: 0            Seconds: 0
   > contract address:    0x671Da68D4236Ec15f5Ebf688bA92574A7cEC2231
   > block number:        9
   > block timestamp:     1594944435
   > account:             0xd45400ce8a4FAB401C1F5d8f264bBabB7E4fFB4f
   > balance:             99.96993128
   > gas used:            175225 (0x2ac79)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.0035045 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:           0.0035045 ETH


Summary
=======
> Total deployments:   2
> Final cost:          0.006788 ETH


Ganache :

address
0xd45400ce8a4FAB401C1F5d8f264bBabB7E4fFB4f
BALANCE
99.97 ETH

