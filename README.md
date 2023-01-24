# IBAX Blockchain System Platform

[![Go Reference](https://pkg.go.dev/badge/github.com/arashdm2020/IBAX-Blockchain.svg)](https://pkg.go.dev/github.com/arashdm2020/IBAX-Blockchain)
[![Go Report Card](https://goreportcard.com/badge/github.com/arashdm2020/IBAX-Blockchain)](https://goreportcard.com/report/github.com/arashdm2020/IBAX-Blockchain)

## The Most Powerful Infrastructure for Applications on Decentralized/Centralized Ecosystems

A powerful blockchain system platform with a new system framework and a simplified programming language, it is including
smart contract, database table and interface.
## Support the project

I develop and maintain this package on my own for free in my spare time, any support is greatly appreciated.
## You can contact me on Telegram
<https://t.me/Blackspid3r9>


### Donate
Make a one time donation in a crypto currency of your choice. If you prefer to donate a currency not listed here please contact me.

**Eth**:  0x4eC35Dd891621109e6AC608d6B066e21156E8f80  

### Build from Source

#### Install Go

The build process for go-ibax requires Go 1.17 or higher. If you don't have it: [Download Go 1.17+](https://go.dev).

You'll need to add Go's bin directories to your `$PATH` environment variable e.g., by adding these lines to
your `/etc/profile` (for a system-wide installation) or `$HOME/.profile`:

```
export PATH=$PATH:/usr/local/go/bin
export PATH=$PATH:$GOPATH/bin
```

(If you run into trouble, see the [Go install instructions](https://go.dev/dl/)).

#### Compile

```
$ export GOPROXY=https://athens.azurefd.net
$ GO111MODULE=on go mod tidy -v

$ go build
```

### Run

1. Create the node configuration file:

```bash
$    go-ibax config
```

2. Generate node keys:

```bash
$    go-ibax generateKeys
```

3. Generate the first block. If you are creating your own blockchain network. You must use the `--test=true` option.
   Otherwise you will not be able to create new accounts.

```bash
$    go-ibax generateFirstBlock --test=true
```

4. Initialize the database.

```bash
$    go-ibax initDatabase
```

5.Starting go-ibax.

```bash
$    go-ibax start
```



