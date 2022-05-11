# Architecture

### Overview

[ioTube](https://iotube.org) utilizes multiple smart contracts on both the origin/destination blockchain to enable cross-blockchain token transfers.&#x20;

It starts when a user deposits assets into the _Cashier contract_ on _Chain A_, which is an event that is _observed_ by multiple _Witness nodes_. These witnesses verify this event and send a signature to the _Relayer network_, which aggregates all signatures and instructs the _Validator contract_ on Chain B to mint the same amount of _Proxy_ _tokens_ that were deposited on Chain A.

![](https://iotex.io/blog/content/images/2021/07/Witnees-Chain-AtoB.jpg)

### Architecture

The ioTube v5 architecture is composed of the following contracts:

* _**WitnessList**_: stores the list of active witnesses
* _**TokenList**_: stores the list of whitelisted tokens
* _**TokenSafe**_: stores the tokens deposited into the _Token_ cashier, that are used to transfer to recipients by the _Transfer validator_ contract
* _**MinterPool**_: holds the minter authority of all mintable tokens
* _**TokenCashier**_: accepts token/coin deposits and emits a receipt for each deposit
* _**TransferValidator**_: validates witness signatures and then withdraws tokens from _Token safe_ to recipients.

#### Deposits

For depositing assets, the _**TokenCashier**_ contract validates the following:

1. Checks if the asset is listed and active
2. Checks if the amount is within the maximum limits
3. Checks if the asset is a _Proxy token_ (e.g., `ioETH` on IoTeX is a proxy token)
4. If a proxy, burns it and creates a receipt; if not a proxy, deposits it into the _**TokenSafe**_.

![Depositing Flowchart](https://iotex.io/blog/content/images/2021/07/Depositing-Flow-1.jpg)

Once _Witnesses_ detect a deposit, they will sign an _Attestation_ and send it to the _Relayers network_, which collects attestations from witnesses and submits them to _**TransferValidator**_.

![](https://iotex.io/blog/content/images/2021/07/Transfer-Validator.jpg)

### Minting

For minting (i.e., issuing _Proxy_ assets), the _**TokenValidator**_ contract ensures:

1. The asset being converted is whitelisted and active via _**TokenList**_
2. The transfer has attestations from at least two-thirds of all witnesses
3. If so, the contract mints _Proxy tokens_ and transfers them to the given recipient.

![Relaying Flowchart](https://iotex.io/blog/content/images/2021/07/Relaying-Flow-1.jpg)

That’s it!&#x20;

After tokens are _bridged_ to IoTeX, Ethereum, BSC, or Polygon they may be traded on the respective decentralized exchanges, including [mimo](http://mimo.exchange) (on IoTeX), [Quickswap](overview-and-architecture.md#overview) (on Polygon), [Uniswap](https://uniswap.org) (on Ethereum), and [PancakeSwap](https://pancakeswap.finance) (on Binance Smart Chain).&#x20;

Stay tuned for even more cross-chain integrations to leading blockchain networks in the near future! Check out the ioTube open-source code [here](https://github.com/iotexproject/ioTube):

{% embed url="https://github.com/iotexproject/ioTube" %}
