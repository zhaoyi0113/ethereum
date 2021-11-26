#


- Create nodes

```bash
mkdir node01 node02 node03
geth --datadir "/PATH_TO_NODE01/" account new
```

- Use puppeth to generate genesis config json file

After that, run the command to init each node.

```bash
geth --datadir "/PATH_TO_NODE/" init genesis.json
```

- Launch the node

```bash
geth --datadir node1 --http --dev --http.corsdomain "*" --http.api web3,eth,debug,personal,net
```

- Attach to the node

```bash
geth attach http://localhost:8545
```
