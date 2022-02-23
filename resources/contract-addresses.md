---
description: Addresses and BscScan links for deployed CBX Protocol and CBX DAO contracts.
---

# Contract Addresses

## Candybox Protocol V1

### BNB Chain(BSC) Mainnet

TerminalDirectory: [`0xD4d698441EEC2A7f1408679811DfA85fC6B18546`](https://bscscan.com/address/0xD4d698441EEC2A7f1408679811DfA85fC6B18546)

TerminalV1: [`0xfA6Dc05a3944b215016Af3Cedf69a570D4e50ab1`](https://bscscan.com/address/0xfA6Dc05a3944b215016Af3Cedf69a570D4e50ab1)

Projects: [`0xE3672BADde62F4D3F5fef89A72a008fd1FC9cC10`](https://bscscan.com/address/0xE3672BADde62F4D3F5fef89A72a008fd1FC9cC10)\`\`

TicketBooth: [`0xFFFB3C2d3cFb43B61a04B5703692d21923f8558B`](https://bscscan.com/address/0xFFFB3C2d3cFb43B61a04B5703692d21923f8558B)

ModStore: [`0x53dc2F8568dfBC9a81468a2F20dB6B2ADd7e4ed3`](https://bscscan.com/address/0x53dc2F8568dfBC9a81468a2F20dB6B2ADd7e4ed3)

OperatorStore: [`0xb0bA3061dAF010BFD166FE2F0AA69C51e0364c56`](https://bscscan.com/address/0xb0bA3061dAF010BFD166FE2F0AA69C51e0364c56)

FundingCycles: [`0xbb84B712269386B3495dCEb1e81ee505da417e66`](https://bscscan.com/address/0xbb84B712269386B3495dCEb1e81ee505da417e66)

Active7DaysFundingCycleBallot: [`0xa0A2370Ad1D5AD31d30665E3B759be2Ba177211a`](https://bscscan.com/address/0xa0A2370Ad1D5AD31d30665E3B759be2Ba177211a)

Active3DaysFundingCycleBallot: [`0x05ED5FE62FDb5216b1105Ed7DE80A79b01D8642F`](https://bscscan.com/address/0x05ED5FE62FDb5216b1105Ed7DE80A79b01D8642F)

Active1DayFundingCycleBallot: N/A

Governance: [`0x2e4728687bb38151d1dF72A50DF9663f0738bbde`](https://bscscan.com/address/0x2e4728687bb38151d1dF72A50DF9663f0738bbde)

Prices: [`0xa7C434C234D17F833a906Bf0fE67D525F788E438`](https://bscscan.com/address/0xa7C434C234D17F833a906Bf0fE67D525F788E438)\`\`

### bscTestnet

[https://github.com/candyboxdao/candy-contracts/tree/main/deployments/bscTestnet](https://github.com/candyboxdao/candy-contracts/tree/main/deployments/bscTestnet)


## Candybox DAO

### $CBX

BNB Chain BEP-20 Token: [0x344289F69B46854356305dE561D3D8F2d5e1EBA8](https://bscscan.com/token/0x344289F69B46854356305dE561D3D8F2d5e1EBA8)

{% hint style="info" %}
To reduce gas fees, newly issued $CBX tokens are stored in the Candybox [TicketBooth](../protocol-v1/ticketbooth/) contract by default ("staked"). $CBX holders can call the `unstake` function on the TicketBooth contract to mint $CBX BEP-20 tokens to their wallets. In the frontend, this is called `Claim` and can be found under the `Manage` button.

The above BEP-20 contract reflects the total supply of minted BEP-20 $CBX tokens.

To ascertain the total supply of claimed (BEP-20) and unclaimed ("staked") $CBX tokens, call the `totalSupplyOf()` function on the TicketBooth contract above, passing project id `1` as the argument.
{% endhint %}

### Gnosis Multisig

ComingSoon
