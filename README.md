
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
______________________________________
2674$ truffle console
truffle(development)> todoList = await TodoList.deployed()
undefined
truffle(development)> 
________________________________

truffle(development)> todoList
TruffleContract {
  constructor:
   { [Function: TruffleContract]
     _constructorMethods:
      { configureNetwork: [Function: configureNetwork],
        setProvider: [Function: setProvider],
        new: [Function: new],
        at: [AsyncFunction: at],
        deployed: [AsyncFunction: deployed],
        defaults: [Function: defaults],
        hasNetwork: [Function: hasNetwork],
        isDeployed: [Function: isDeployed],
        detectNetwork: [AsyncFunction: detectNetwork],
        setNetwork: [Function: setNetwork],
        setNetworkType: [Function: setNetworkType],
        setWallet: [Function: setWallet],
        resetAddress: [Function: resetAddress],
        link: [Function: link],
        clone: [Function: clone],
        addProp: [Function: addProp],
        toJSON: [Function: toJSON],
        decodeLogs: [Function: decodeLogs] },
     _properties:
      { contract_name: [Object],
        contractName: [Object],
        gasMultiplier: [Object],
        timeoutBlocks: [Object],
        autoGas: [Object],
        numberFormat: [Object],
        abi: [Object],
        metadata: [Function: metadata],
        network: [Function: network],
        networks: [Function: networks],
        address: [Object],
        transactionHash: [Object],
        links: [Function: links],
        events: [Function: events],
        binary: [Function: binary],
        deployedBinary: [Function: deployedBinary],
        unlinked_binary: [Object],
        bytecode: [Object],
        deployedBytecode: [Object],
        sourceMap: [Object],
        deployedSourceMap: [Object],
        source: [Object],
        sourcePath: [Object],
        legacyAST: [Object],
        ast: [Object],
        compiler: [Object],
        schema_version: [Function: schema_version],
        schemaVersion: [Function: schemaVersion],
        updated_at: [Function: updated_at],
        updatedAt: [Function: updatedAt],
        userdoc: [Function: userdoc],
        devdoc: [Function: devdoc],
        networkType: [Object],
        immutableReferences: [Object] },
     _property_values: {},
     _json:
      { contractName: 'TodoList',
        abi: [Array],
        metadata:
         '{"compiler":{"version":"0.5.16+commit.9c3226ce"},"language":"Solidity","output":{"abi":[{"inputs":[],"payable":false,"stateMutability":"nonpayable","type":"constructor"},{"constant":true,"inputs":[],"name":"last_completed_migration","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[],"name":"owner","outputs":[{"internalType":"address","name":"","type":"address"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"internalType":"uint256","name":"completed","type":"uint256"}],"name":"setCompleted","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[],"name":"taskCount","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"}],"devdoc":{"methods":{}},"userdoc":{"methods":{}}},"settings":{"compilationTarget":{"/Users/fab/workspace/initethereumsoliditytodo/contracts/TodoList.sol":"TodoList"},"evmVersion":"istanbul","libraries":{},"optimizer":{"enabled":false,"runs":200},"remappings":[]},"sources":{"/Users/fab/workspace/initethereumsoliditytodo/contracts/TodoList.sol":{"keccak256":"0x20939c37a1cf54fab1061a99ddc2e4d8e9557944e5438256e2c9752cc820d00b","urls":["bzz-raw://f6450f50f0c1f296d2684a2eb7d9bb60d1f8e870bfec8ce62346d6a556e19939","dweb:/ipfs/QmeUa322Sf1j2PaRZn1wojYA2AqxAjG29QVDxsohebVEay"]}},"version":1}',
        bytecode:
         '0x6080604052600060025534801561001557600080fd5b50336000806101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055506101cb806100656000396000f3fe608060405234801561001057600080fd5b506004361061004c5760003560e01c8063445df0ac146100515780638da5cb5b1461006f578063b6cb58a5146100b9578063fdacd576146100d7575b600080fd5b610059610105565b6040518082815260200191505060405180910390f35b61007761010b565b604051808273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390f35b6100c1610130565b6040518082815260200191505060405180910390f35b610103600480360360208110156100ed57600080fd5b8101908080359060200190929190505050610136565b005b60015481565b6000809054906101000a900473ffffffffffffffffffffffffffffffffffffffff1681565b60025481565b6000809054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16141561019357806001819055505b5056fea265627a7a723158202fe769f6fb2d38c8c5c61c5c469f010edc221e0ea7265d70ddd47293e8fe867d64736f6c63430005100032',
        deployedBytecode:
         '0x608060405234801561001057600080fd5b506004361061004c5760003560e01c8063445df0ac146100515780638da5cb5b1461006f578063b6cb58a5146100b9578063fdacd576146100d7575b600080fd5b610059610105565b6040518082815260200191505060405180910390f35b61007761010b565b604051808273ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200191505060405180910390f35b6100c1610130565b6040518082815260200191505060405180910390f35b610103600480360360208110156100ed57600080fd5b8101908080359060200190929190505050610136565b005b60015481565b6000809054906101000a900473ffffffffffffffffffffffffffffffffffffffff1681565b60025481565b6000809054906101000a900473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff163373ffffffffffffffffffffffffffffffffffffffff16141561019357806001819055505b5056fea265627a7a723158202fe769f6fb2d38c8c5c61c5c469f010edc221e0ea7265d70ddd47293e8fe867d64736f6c63430005100032',
        immutableReferences: undefined,
        sourceMap:
         '66:377:1:-;;;188:1;161:28;;196:56;8:9:-1;5:2;;;30:1;27;20:12;5:2;196:56:1;235:10;227:5;;:18;;;;;;;;;;;;;;;;;;66:377;;;;;;',
        deployedSourceMap:
         '66:377:1:-;;;;8:9:-1;5:2;;;30:1;27;20:12;5:2;66:377:1;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;116:39;;;:::i;:::-;;;;;;;;;;;;;;;;;;;90:20;;;:::i;:::-;;;;;;;;;;;;;;;;;;;;;;;161:28;;;:::i;:::-;;;;;;;;;;;;;;;;;;;329:112;;;;;;13:2:-1;8:3;5:11;2:2;;;29:1;26;19:12;2:2;329:112:1;;;;;;;;;;;;;;;;;:::i;:::-;;116:39;;;;:::o;90:20::-;;;;;;;;;;;;;:::o;161:28::-;;;;:::o;329:112::-;308:5;;;;;;;;;;;294:19;;:10;:19;;;290:26;;;425:9;398:24;:36;;;;290:26;329:112;:::o',
        source:
         '// SPDX-License-Identifier: MIT\npragma solidity >=0.4.21 <0.7.0;\n\ncontract TodoList {\n    address public owner;\n    uint256 public last_completed_migration;\n    uint256 public taskCount = 0;\n\n    constructor() public {\n        owner = msg.sender;\n    }\n\n    modifier restricted() {\n        if (msg.sender == owner) _;\n    }\n\n    function setCompleted(uint256 completed) public restricted {\n        last_completed_migration = completed;\n    }\n}\n',
        sourcePath:
         '/Users/fab/workspace/initethereumsoliditytodo/contracts/TodoList.sol',
        ast: [Object],
        legacyAST: [Object],
        compiler: [Object],
        networks: [Object],
        schemaVersion: '3.2.2',
        updatedAt: '2020-07-17T00:07:15.310Z',
        networkType: 'ethereum',
        devdoc: [Object],
        userdoc: [Object] },
     configureNetwork: [Function: bound configureNetwork],
     setProvider: [Function: bound setProvider],
     new:
      { [Function: bound new] estimateGas: [Function: bound estimateDeployment] },
     at: [AsyncFunction: bound at],
     deployed: [AsyncFunction: bound deployed],
     defaults: [Function: bound defaults],
     hasNetwork: [Function: bound hasNetwork],
     isDeployed: [Function: bound isDeployed],
     detectNetwork: [AsyncFunction: bound detectNetwork],
     setNetwork: [Function: bound setNetwork],
     setNetworkType: [Function: bound setNetworkType],
     setWallet: [Function: bound setWallet],
     resetAddress: [Function: bound resetAddress],
     link: [Function: bound link],
     clone: [Function: bound clone],
     addProp: [Function: bound addProp],
     toJSON: [Function: bound toJSON],
     decodeLogs: [Function: bound decodeLogs],
     class_defaults:
      { from: '0xd45400ce8a4FAB401C1F5d8f264bBabB7E4fFB4f',
        gas: 6721975,
        gasPrice: 20000000000 },
     interfaceAdapter: Web3InterfaceAdapter { web3: [Web3Shim] },
     web3:
      Web3Shim {
        currentProvider: [Getter/Setter],
        _requestManager: [RequestManager],
        givenProvider: null,
        providers: [Object],
        _provider: [HttpProvider],
        setProvider: [Function],
        BatchRequest: [Function: bound Batch],
        extend: [Function],
        version: '1.2.1',
        utils: [Object],
        eth: [Eth],
        shh: [Shh],
        bzz: [Bzz],
        networkType: 'ethereum' },
     currentProvider:
      HttpProvider {
        host: 'http://127.0.0.1:7545',
        httpAgent: [Agent],
        timeout: 0,
        headers: undefined,
        connected: true,
        send: [Function],
        _alreadyWrapped: true },
     network_id: '5777',
     ens: { enabled: false, registryAddress: null } },
  methods:
   { 'last_completed_migration()':
      { [Function]
        call: [Function],
        sendTransaction: [Function],
        estimateGas: [Function],
        request: [Function] },
     'owner()':
      { [Function]
        call: [Function],
        sendTransaction: [Function],
        estimateGas: [Function],
        request: [Function] },
     'taskCount()':
      { [Function]
        call: [Function],
        sendTransaction: [Function],
        estimateGas: [Function],
        request: [Function] },
     'setCompleted(uint256)':
      { [Function]
        call: [Function],
        sendTransaction: [Function],
        estimateGas: [Function],
        request: [Function] } },
  abi:
   [ { inputs: [],
       payable: false,
       stateMutability: 'nonpayable',
       type: 'constructor',
       constant: undefined },
     { constant: true,
       inputs: [],
       name: 'last_completed_migration',
       outputs: [Array],
       payable: false,
       stateMutability: 'view',
       type: 'function',
       signature: '0x445df0ac' },
     { constant: true,
       inputs: [],
       name: 'owner',
       outputs: [Array],
       payable: false,
       stateMutability: 'view',
       type: 'function',
       signature: '0x8da5cb5b' },
     { constant: true,
       inputs: [],
       name: 'taskCount',
       outputs: [Array],
       payable: false,
       stateMutability: 'view',
       type: 'function',
       signature: '0xb6cb58a5' },
     { constant: false,
       inputs: [Array],
       name: 'setCompleted',
       outputs: [],
       payable: false,
       stateMutability: 'nonpayable',
       type: 'function',
       signature: '0xfdacd576' } ],
  address: '0x671Da68D4236Ec15f5Ebf688bA92574A7cEC2231',
  transactionHash: undefined,
  contract:
   Contract {
     currentProvider: [Getter/Setter],
     _requestManager:
      RequestManager {
        provider: [HttpProvider],
        providers: [Object],
        subscriptions: {} },
     givenProvider: null,
     providers:
      { WebsocketProvider: [Function: WebsocketProvider],
        HttpProvider: [Function: HttpProvider],
        IpcProvider: [Function: IpcProvider] },
     _provider:
      HttpProvider {
        host: 'http://127.0.0.1:7545',
        httpAgent: [Agent],
        timeout: 0,
        headers: undefined,
        connected: true,
        send: [Function],
        _alreadyWrapped: true },
     setProvider: [Function],
     BatchRequest: [Function: bound Batch],
     extend:
      { [Function: ex]
        formatters: [Object],
        utils: [Object],
        Method: [Function: Method] },
     clearSubscriptions: [Function],
     options: { address: [Getter/Setter], jsonInterface: [Getter/Setter] },
     defaultAccount: [Getter/Setter],
     defaultBlock: [Getter/Setter],
     methods:
      { last_completed_migration: [Function: bound _createTxObject],
        '0x445df0ac': [Function: bound _createTxObject],
        'last_completed_migration()': [Function: bound _createTxObject],
        owner: [Function: bound _createTxObject],
        '0x8da5cb5b': [Function: bound _createTxObject],
        'owner()': [Function: bound _createTxObject],
        taskCount: [Function: bound _createTxObject],
        '0xb6cb58a5': [Function: bound _createTxObject],
        'taskCount()': [Function: bound _createTxObject],
        setCompleted: [Function: bound _createTxObject],
        '0xfdacd576': [Function: bound _createTxObject],
        'setCompleted(uint256)': [Function: bound _createTxObject] },
     events: { allEvents: [Function: bound ] },
     _address: '0x671Da68D4236Ec15f5Ebf688bA92574A7cEC2231',
     _jsonInterface: [ [Object], [Object], [Object], [Object], [Object] ] },
  last_completed_migration:
   { [Function]
     call: [Function],
     sendTransaction: [Function],
     estimateGas: [Function],
     request: [Function] },
  owner:
   { [Function]
     call: [Function],
     sendTransaction: [Function],
     estimateGas: [Function],
     request: [Function] },
  taskCount:
   { [Function]
     call: [Function],
     sendTransaction: [Function],
     estimateGas: [Function],
     request: [Function] },
  setCompleted:
   { [Function]
     call: [Function],
     sendTransaction: [Function],
     estimateGas: [Function],
     request: [Function] },
  sendTransaction: [Function],
  send: [Function],
  allEvents: [Function],
  getPastEvents: [Function] }

____________________________________
truffle(development)> todoList.address
'0x671Da68D4236Ec15f5Ebf688bA92574A7cEC2231'
____________________________________

truffle(development)> todoList.address
'0x671Da68D4236Ec15f5Ebf688bA92574A7cEC2231'
truffle(development)> todoList.taskCount()
BN {
  negative: 0,
  words: [ 0, <1 empty item> ],
  length: 1,
  red: null }
truffle(development)>

____________________________________

truffle(development)> taskCount = await todoList.taskCount()
undefined
truffle(development)> taskCount.toNumber()
0
truffle(development)> 

________

2677$ truffle compile

Compiling your contracts...
===========================
> Compiling ./contracts/TodoList.sol
> Artifacts written to /Users/fab/workspace/initethereumsoliditytodo/build/contracts
> Compiled successfully using:
   - solc: 0.5.16+commit.9c3226ce.Emscripten.clang

2686$ 

________
