---
description: USDC on IoTeX Tutorial
---

# USDC

ioTube, the official bridge of IoTeX, introduced ioUSDC, a bridged token from Ethereum, on 9/14//2021. Since its launch, ioUSDC has been integrated with over 10 DeFi protocols and is held by over 5,000 wallet addresses. Recently, Circle proposed the [Bridged USDC Standard](https://github.com/circlefin/stablecoin-evm/blob/master/doc/bridged\_USDC\_standard.md), a specification and process for deploying a bridged form of USDC on EVM blockchains. This standard includes the optionality for Circle to seamlessly upgrade to native USDC issuance in the future. The Bridged USDC Standard provides a secure and standardized method for any EVM blockchain and rollup team to transfer ownership of a bridged USDC token contract to Circle, facilitating an upgrade to native USDC. The new naming convention for this Circle supported USDC is USDC.e

By implementing the proposed deployment and migration strategy, IoTeX will enhance its DeFi ecosystem's compatibility and ensure seamless token transactions for users. This initiative will leverage Circle's standard token format, positioning IoTeX for future integrations and improvements.

{% hint style="info" %}
Auto conversion of ioUSDC to USDC.e is going to be supported in the next release of ioTube in Nov 2024.
{% endhint %}

### Tutorial Below:

**Bridging USDC from Ethereum network to IoTeX network**

1. Connect your wallet, then select Ethereum network and find USDC in the list of tokens.

<figure><img src="../.gitbook/assets/Screenshot 2024-08-14 at 2.38.21 PM.png" alt=""><figcaption></figcaption></figure>

2. Enter the amount you wish to bridge and then press the bridge button. You will have to approve 2 different transactions in your wallet.

<figure><img src="../.gitbook/assets/Screenshot 2024-08-14 at 2.31.23 PM.png" alt=""><figcaption></figcaption></figure>

3. The bridged IoTeX will be available on IoTeX network as ioUSDC.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2024-08-14 at 2.42.27 PM.png" alt=""><figcaption></figcaption></figure>

**Converting ioUSDC to Circle supported token USDC.e**

1. Go to convert tab in navigation.

<figure><img src="../.gitbook/assets/Screenshot 2024-08-14 at 2.46.51 PM.png" alt=""><figcaption></figcaption></figure>

2. Find ioUSDC in list of tokens.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2024-08-14 at 2.47.10 PM.png" alt=""><figcaption></figcaption></figure>

3. Enter the amount you wish to convert and then press the convert button. You will have to approve 2 different transactions in your wallet.

<figure><img src="../.gitbook/assets/Screenshot 2024-08-14 at 2.47.04 PM.png" alt=""><figcaption></figcaption></figure>

4. You will then see USDC.e in your wallet.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2024-08-14 at 2.52.37 PM.png" alt=""><figcaption></figcaption></figure>

**Bridging from USDC.e on IoTeX Network to another network**

1. Follow the above method to convert from USDC.e back to ioUSDC.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2024-08-14 at 2.54.36 PM.png" alt=""><figcaption></figcaption></figure>

2. Go to the "Bridge" tab in the navigation. Select Withdraw instead of Deposit. Change the selected "From" network to IoTeX Network.

<figure><img src="../.gitbook/assets/Screenshot 2024-08-14 at 2.59.11 PM.png" alt=""><figcaption></figcaption></figure>

3. Select ioUSDC from the list of tokens. Enter the amount you wish to bridge to the other network. And finally hit the "Withdraw" button. You will have to approve 2 different transactions in your wallet.

<figure><img src="../.gitbook/assets/Screenshot 2024-08-14 at 3.00.48 PM.png" alt=""><figcaption></figcaption></figure>
