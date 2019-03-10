### tendermint
---
https://github.com/tendermint/tendermint

```
```

```
go get github.com/tendermint/tendermint
cd $GOPATH/src/github.com/tendermint/tendermint
make get_tools
make get_vendor_deps
make install_abci

abci-cli kvstore

tendermint init
tendermint node

curl -s localhost:26657/status
curl -s 'localhost:26657/broadcast_tx_commit?tx="abcd"'
```

```
{
  "jsonrpc": "2.0",
  "id": "",
  "deliver_tx": {
    "tags": [
      {
        "key": "xxxxxx",
        "value": "amFl"
      },
      {
        "key": "xxxxxx",
        "value": "xxxxx"
      }
    ]
  },
  "hash": "xxxxxxxxxxxx",
  "height": 14
}
```


