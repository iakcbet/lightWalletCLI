# lightWalletCLI

A php based cli wallet for [Arionum][aro].

Requires php 7.2

## Usage

```bash
light-arionum-cli [command] [options]
```

## Commands

Command                                                                                     | Description
------------------------------------------------------------------------------------------- | ------------------
`balance`                                                                                   | Prints the balance
`export`                                                                                    | Prints the wallet data
`block`                                                                                     | Show data about the current block
`encrypt`                                                                                   | Encrypts the wallet
`decrypt`                                                                                   | Decrypts the wallet
`transactions`                                                                              | Show the latest transactions
`transaction [id]`                                                                          | Shows data about a specific transaction
`send [address] [value] [message]`                                                          | Sends a transaction (message optional)
`alias send [alias] [value] [message]`                                                      | Sends a transaction to an alis (message optional)
`alias set [alias]`                                                                         | Set your alias to the specified value
`masternode create [ip]`                                                                    | Send a masternode announcement transaction
`masternode pause`                                                                          | Pause the masternode
`masternode resume`                                                                         | Resume the masternode
`masternode release`                                                                        | Close the masternode and return the funds
`masternode voting-key`									    | Generates and sends to the blockchain the voting key
`masternode vote [voteid]`								    | Votes for a blockchain config change
`masternode change-ip [ip]`								    | Changes the masternode IP
`asset create [max_supply] [tradable] [price] [dividend only] [autodividend] [allow_bid]`   | Transforms this wallet into an asset
`asset send [asset id] [destination] [amount]`                                              | Sends asset units to another address
`asset market [asset id] [price] [units] [cancelable] [ask/bid]`                            | Submits an order on the blockchain asset market
`asset cancel-order [order-id]`                                                             | Cancels a blockchain asset market order
`asset dividends [amount]`                                                                  | Distributes amount as dividends to all asset holders
`asset inflate [amount]`                                                                    | Increases the max supply if the asset is inflatable
`asset balance`                                                                             | Shows all assets

To activate the testnet mode, create a file called .testnet in the same folder

## Development Fund

Coin | Address
---- | --------
[ARO]: | 5WuRMXGM7Pf8NqEArVz1NxgSBptkimSpvuSaYC79g1yo3RDQc8TjVtGH5chQWQV7CHbJEuq9DmW5fbmCEW4AghQr
[LTC]: | LWgqzbXGeucKaMmJEvwaAWPFrAgKiJ4Y4m
[BTC]: | 1LdoMmYitb4C3pXoGNLL1VRj7xk3smGXoU
[ETH]: | 0x4B904bDf071E9b98441d25316c824D7b7E447527
[BCH]: | qrtkqrl3mxzdzl66nchkgdv73uu3rf7jdy7el2vduw

If you'd like to support the Arionum development, you can donate to the addresses listed above.

[aro]: https://arionum.com
[ltc]: https://litecoin.org
[btc]: https://bitcoin.org
[eth]: https://ethereum.org
[bch]: https://www.bitcoincash.org
