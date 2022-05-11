# Special Need of Crosschained Token?

If you only need the bridged token to be a standard XRC20/BEP20/ERC20 token, you can stop here, your token should be good to go.

If you have special need for your bridged token, you will need to create your own Crosschained Token and add your customized code to the smart contract. Here are the steps

1. Fork this `CrossChainERC20.sol` from [https://github.com/iotubeproject/iotube-contracts/blob/master/contracts/CrosschainERC20.sol](https://github.com/iotubeproject/iotube-contracts/blob/master/contracts/CrosschainERC20.sol)
2. Add your customized code to the sol file.  (You can contact us for a code review)
3.  Deploy the smart contract with parameters&#x20;

    | \_coToken  | <p>The token address of your token</p><p><strong>0x00 address (if not on source chain)</strong></p>                                                                                                                            |
    | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
    | \_minter   | <p>IoTeX: 0x4799d57abf5f12ca4ef5375c9dadf8fe7fa5a454<br>BSC:<br>0xf72CFb704d49aC7BB7FFa420AE5f084C671A29be<br>ETH:<br>0x964f4f19bc823e72cc1f806021937cfc06f63b45<br>Polygon:<br>0x12af43ef94B05A0a3447A05eEE629C7D88A30a5f</p> |
    | \_name     | Token's name                                                                                                                                                                                                                   |
    | \_symbol   | Token's Symbol                                                                                                                                                                                                                 |
    | \_decimals | Token's decimals                                                                                                                                                                                                               |


4. Verify your code on blockchain explorer
5. Add your Crosschained Token to the token submission request (issue on github)

Please discuss with us if you have any questions.

&#x20;

