To run a full node on your system
To create a private blockchain
geth->will import new block headers
geth attach ipc://./pipe/geth.ipc
->
personal.newAccount()
passphrase abd repeat passphrase->1234
->account created address
eth.syncing

For Private Network:
geth --datadir test init ./genesis.json
geth --datadir .\test\ --nodiscover (for no peer discovery)

For mining:
in another window(side window):
geth attach ipc://./pipe/geth.ipc
eth.accounts

personal.newAccount()
passphrase abd repeat passphrase->1234

miner.setEtherbase(eth.accounts[0])
for CPU
miner.start(1)

For checking balance:
eth.getBalance(eth.accounts[0])

Reference: https://geth.ethereum.org/docs/interface/mining