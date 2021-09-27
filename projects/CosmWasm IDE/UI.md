# UI Suggestions
## CONTRACT CREATION SECTION

### Left side (Categories)

On the left of the IDE have a browser tab on left where you can create files for your project. It be nice to have
it read the languages when you name the file `.js` `.rs` ect.

### Right side

- Compile: on your right hand side have a ' start to compile ' this compiles the code in to binary form which will be
  ready for deployment.  if no errors show then you move to the next step.
- Run: we use this tab to test deploy, remix IDE you have diff env to choose i.e JavaScript VM, Injected Web3 (use
  Keplr extension) and Web3 Provider for example. This can be a simple deploy button which triggers a script. (Orkun can add to the ideas of ENV here). After execution it shows a nice deployed contract in the ' deployed contracts tab ' here you will find all the get and set functions where you can get value of a variable ect.
- Settings: settings tab im not sure what you could add in here. But all n all could be something useful
- Analysis: Option to check history of deployed contracts ect. ( More to add)
- Debugger: Rust debugger possibly showing here.
- Support: Support from CW if things are getting confusing.

#### Deploy Smart Contract Section

So on this page we need something like the following

- From (connected wallets): So in order to deploy contract we need to have a page that has our injected web3 wallet.(Keprl) a drop down menu which has FROM that when user wallet is connected it shows our address and balance of wallet.

Two ways to deploy contract:
- Rust Contract Source Code Below 'from' drop down possibly have our Rust Source code showing of a particular smart contract code that we create in the previous page of our IDE.
- Contract Byte Code: Contract bite code to use to deploy also.

What ever you use it automatically compiles and give you another drop down menu of the type of Smart contracts you would like to deploy. (cw20 ... "my first token" .. mint NFT ect. )

<img width="731" alt="image 1" src="https://user-images.githubusercontent.com/68139321/133888149-39de91f1-fb23-4f96-adf5-2919f0960f53.png">

Another section I feel can be built solely for Deploy Function capabilities. This section is the next stage along of
the users Smart Contract creation. Here we can test the functionality of our code on a selected chain to test before deployment.

Here are some ideas of what can be in this section:
- Deploy function: Hit on the deploy function button and the tx is then completed.

<img width="731" alt="2" src="https://user-images.githubusercontent.com/68139321/133888205-581c4a81-c606-4391-9518-8bddd8a6fde5.png">

There is another way we can deploy by selecting Injective web3 on our environments tab and with that i should be able to read our address on this IDE which we can deploy contract using it also.

- Wallet: section showing the balance of a selected wallet.
- Contracts: a list of deployed contracts or created tokens on chain





