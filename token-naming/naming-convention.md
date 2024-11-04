# Naming Convention

## Past naming convention

iotube is currently supporting **28** assets from 5 different blockchains

* IoTeX
* Ethereum
* Binance Smart Chain
* Polygon
* Solana

Historically, assets from Ethereum bridged via iotube to IoTeX were named _`ioABC`_ (where _`ABC`_ is the symbol in the original blockchain). Assets from Binance Smart Chain were named _`ABC-bsc`_. Assets from Polygon were named _`ABC-matic`_. While this format is accurate, it is long and complex.&#x20;

## Current Naming convention

After a [governance proposal](https://gov.iotex.io/#/iotex.eth/proposal/QmbWqwVEmv4ArVgiki19oPBjYDZmZvLnjSpGieo3MtSQBD),  iotube and all IoTeX ecosystem projects will follow a new convention for cross-chain tokens naming and display symbols.

In short, the naming convention says to:

1.  Leave the token symbol **unchanged** for

    → any _native_ tokens bridged _from their origin blockchain_. For example, `ETH` from Ethereum, `BNB` from Binance Smart Chain, `MATIC` from Polygon.

    → any layer-2 tokens bridged from their origin blockchain. For example, most stable coins on the Ethereum blockchain like `USDT`, `USDC`, `UNI`, etc...
2. Add a **short suffix** to any tokens that come from a blockchain that _is not their origin network_. For example, `USDC` from Polygon becomes `USDC_m`, `USDT` from Binance Smart Chain becomes `USDT_b`.

## Examples&#x20;

### Bridged from Ethereum

| Symbol on Ethereum | Symbol on IoTeX (old) | Symbol on IoTeX (new) |
| ------------------ | --------------------- | --------------------- |
| `ETH/WETH`         | `ioETH`               | `ETH`                 |
| `USDT`             | `ioUSDT`              | `USDT`                |
| `USDC`             | `ioUSDC`              | `USDC`                |
| `DAI`              | `ioDAI`               | `DAI`                 |
| `UNI`              | `ioUNI`               | `UNI`                 |
| `WBTC`             | `ioWBTC`              | `WBTC`                |
| `PAXG`             | `ioPAXG`              | `PAXG`                |
| `MCN/CMCN`         | `MCN`                 | `MCN`                 |
| `CYC`              | `CYC`                 | `CYC`                 |

### Bridged from BSC

<table><thead><tr><th width="183.80672258908592">Symbol on BSC</th><th width="285.5917058897972">Symbol on IoTeX</th><th>Symbol on IoTeX (new)</th></tr></thead><tbody><tr><td><code>BNB/WBNB</code></td><td><code>BNB-bsc</code></td><td><code>BNB</code></td></tr><tr><td><code>BUSD</code></td><td><code>BUSD-bsc</code></td><td><code>BUSD_b</code></td></tr></tbody></table>

### Tokens bridged from Polygon

| Symbol on Polgyon | Symbol on IoTeX (old) | Symbol on IoTeX (new) |
| ----------------- | --------------------- | --------------------- |
| `Matic/WMatic`    | `WMatic`              | `Matic`               |
| `WETH`            | `WETH-matic`          | `WETH_m`              |
| `WBTC`            | `WBTC-matic`          | `WBTC_m`              |
| `DAI`             | `DAI-maitc`           | `DAI_m`               |
| `USDT`            | `USDT-matic`          | `USDT_m`              |
| `USDC`            | `USDC-matic`          | `USDC_m`              |
| `Sushi`           | `SUSHI-matic`         | `Sushi_m`             |
| `QUICK`           | `QUICK-matic`         | `QUICK_m`             |
| AAVE              | AAVE-matic            | AAVE\_m               |

_For the full list of all tokens supported by iotube, please visit_

[_https://iotube.org/assets_](https://iotube.org/assets)

## Developers

Developers can fetch this list to stay up-to-date with all cross-chain tokens supported by iotube and share the same naming convention across the IoTeX ecosystem.

#### &#x20;JSON file

[https://iotube.org/tokenlist/tube-iotex-tokens.json](https://iotube.org/tokenlist/tube-iotex-tokens.json)

#### &#x20;HTTP

[https://tokenlists.org/token-list?url=https%3A%2F%2Fiotube.org%2Ftokenlist%2Ftube-iotex-tokens.json](https://tokenlists.org/token-list?url=https%3A%2F%2Fiotube.org%2Ftokenlist%2Ftube-iotex-tokens.json)
