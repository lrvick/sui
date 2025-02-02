---
title: Sui Bridging
---

Bridging is the process of moving tokens from one blockchain to another. When you use a bridge to move tokens between blockchains that are incompatible, the tokens are "wrapped" by the bridge, which means that they get converted to a derivative token for the target blockchain. You can transfer tokens in from other blockchains to SUI, or transfer SUI tokens out to other blockchains.

Sui supports bridging through [Wormhole Connect](#wormhole-connect) and [Wormhole Portal Bridge](#wormhole-portal-bridge).

## Wormhole Connect

Use to bridge tokens from any Wormhole supported chain into Sui and get dropped off with extra Sui to pay gas fees. Developers can also embed the Connect Token Bridge directly into their own websites and dApps.

### Wormhole Connect asset support

Initially, [Wormhole Connect](https://www.portalbridge.com/sui/) supports only lock-and-mint bridging for ETH, WETH, USDC, MATIC, WMATIC, BNB, WBNB, AVAX, WAVAX, FTM, WFTM, CELO, GLMR, WGLRM, AND SOL across Ethereum, Polygon, BSC, Avalanche, Celo, Moonbeam, Solana and Sui. This means that any native token bridged through Wormhole Connect and the underlying Wormhole Token Bridge are received as a Wormhole-minted token on the destination chain. In some cases, Wormhole-minted tokens are the canonical representation on the chain. See the [Wormhole token list](https://github.com/wormhole-foundation/wormhole-token-list) on GitHub. Some Wormhole-minted tokens support swapping on the destination chain's DEX(s) for whichever assets you need.

### Wormhole Connect automatic relay

On EVM-based chains and Sui, Wormhole Connect lets you bridge assets while having to pay gas only on the source chain. The automatic relaying feature pays gas on behalf of users on the destination chain.

### Wormhole Connect gas drop-off

The gas drop-off feature enables users to pay an additional fee on the source chain to request a small amount of native gas on the destination chain. For example, a user bridging USDC from Ethereum to Sui can pay a fee denominated in USDC from their sending wallet to receive some native SUI in their receiving wallet. This is in addition to the USDC they are bridging over. Gas drop-off is currently supported on EVM-based chains and Sui.

To learn more about Wormhole Connect, see their [FAQ](https://docs.wormhole.com/wormhole/faqs) page.

## Wormhole Portal Bridge

The Wormhole powered [Portal Bridge](https://www.portalbridge.com/sui) supports bridging any asset from any of the [22 supported Wormhole chains](https://www.wormhole.com/network).

## Token address list

The following table lists the address associated with each token type. You can confirm the legitimacy of tokens when you bridge them by confirming that the address used matches the address for the token type.

| Token   | Address                                                            |
| ------- | ------------------------------------------------------------------ |
| CELO    | 0xa198f3be41cda8c07b3bf3fee02263526e535d682499806979a111e88a5a8d0f |
| tBTC    | 0x079b5d71523f15724f71dd40b238063d5ee756672435ccb27328c0a8664c0d16 |
| USDC    | 0x5d4b302506645c37ff133b98c4b50a5ae14841659738d6d733d59d0d217a93bf |
| USDCarb | 0xe32d3ebafa42e6011b87ef1087bbc6053b499bf6f095807b9013aff5a6ecd7bb |
| USDCbnb | 0x909cba62ce96d54de25bec9502de5ca7b4f28901747bbf96b76c2e63ec5f1cba |
| USDCpol | 0xdb9ed08481f9dd565fd36b834eb3c2cda1ee5f388048154807cffcb0267ed3b2 |
| USDCsol | 0xb231fcda8bbddb31f2ef02e6161444aec64a514e2c89279584ac9806ce9cf037 |
| USDT    | 0xc060006111016b8a020ad5b33834984a437aaa7d3c74c18e09a95d48aceab08c |
| WAVAX   | 0x1e8b532cca6569cab9f9b9ebc73f8c13885012ade714729aa3b450e0339ac766 |
| WBNB    | 0xb848cce11ef3a8f62eccea6eb5b35a12c4c2b1ee1af7755d02d7bd6218e8226f |
| WBTC    | 0x027792d9fed7f9844eb4839566001bb6f6cb4804f66aa2da6fe1ee242d896881 |
| WETH    | 0xaf8cd5edc19c4512f4259f0bee101a40d41ebed738ade5874359610ef8eeced5 |
| WFTM    | 0x6081300950a4f1e2081580e919c210436a1bed49080502834950d31ee55a2396 |
| WGLMR   | 0x66f87084e49c38f76502d17f87d17f943f183bb94117561eb573e075fdc5ff75 |
| WMATIC  | 0xdbe380b13a6d0f5cdedd58de8f04625263f113b3f9db32b3e1983f49e2841676 |
| WSOL    | 0xb7844e289a8410e50fb3ca48d69eb9cf29e27d223ef90353fe1bd8e27ff8f3f8 |
