---
description: Fork of Uniswap v3
---

# v3 contracts

{% content-ref url="pancakev3factory.md" %}
[pancakev3factory.md](pancakev3factory.md)
{% endcontent-ref %}

{% content-ref url="smartrouterv3/" %}
[smartrouterv3](smartrouterv3/)
{% endcontent-ref %}

### Address

**Core**

<table><thead><tr><th width="238.33333333333331">Contract</th><th width="297">BSC, ETH, zkEVM, ARB, GOR, BSC TESTNET / MAINNET</th><th>zkSync</th></tr></thead><tbody><tr><td>PancakeV3Factory</td><td>0x0BFbCF9fa4f9C56B0F40a671Ad40E0805A091865</td><td>0x1BB72E0CbbEA93c08f535fc7856E0338D7F7a8aB</td></tr><tr><td>PancakeV3PoolDeployer</td><td>0x41ff9AA7e16B8B1a8a8dc4f0eFacd93D02d071c9</td><td>0x7f71382044A6a62595D5D357fE75CA8199123aD6</td></tr></tbody></table>

**Periphery**

| Contract                   | BSC, ETH                                   | zkEVM                                      | Arbitrum                                   | zkSync                                     | GOR, BSC TESTNET                           |
| -------------------------- | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ |
| SwapRouter (v3)            | 0x1b81D678ffb9C0263b24A97847620C99d213eB14 | 0x1b81D678ffb9C0263b24A97847620C99d213eB14 | 0x1b81D678ffb9C0263b24A97847620C99d213eB14 | 0xD70C70AD87aa8D45b8D59600342FB3AEe76E3c68 | 0x1b81D678ffb9C0263b24A97847620C99d213eB14 |
| V3Migrator                 | 0xbC203d7f83677c7ed3F7acEc959963E7F4ECC5C2 | 0xbC203d7f83677c7ed3F7acEc959963E7F4ECC5C2 | 0xbC203d7f83677c7ed3F7acEc959963E7F4ECC5C2 | 0x556A72A7A3bB3bbd293D923e59b6B56898fB405D | 0x46A15B0b27311cedF172AB29E4f4766fbE7F4364 |
| NonfungiblePositionManager | 0x46A15B0b27311cedF172AB29E4f4766fbE7F4364 | 0x46A15B0b27311cedF172AB29E4f4766fbE7F4364 | 0x46A15B0b27311cedF172AB29E4f4766fbE7F4364 | 0xa815e2eD7f7d5B0c49fda367F249232a1B9D2883 | 0x427bF5b37357632377eCbEC9de3626C71A5396c1 |
| MixedRouteQuoterV1         | 0x678Aa4bF4E210cf2166753e054d5b7c31cc7fa86 | 0x4c650FB471fe4e0f476fD3437C3411B1122c4e3B | 0x3652Fc6EDcbD76161b8554388867d3dAb65eCA93 | 0x9B1edFB3848660402E4f1DC25733764e80aA627A | 0xB048Bbc1Ee6b733FFfCFb9e9CeF7375518e25997 |
| QuoterV2                   | 0xB048Bbc1Ee6b733FFfCFb9e9CeF7375518e25997 | 0xB048Bbc1Ee6b733FFfCFb9e9CeF7375518e25997 | 0xB048Bbc1Ee6b733FFfCFb9e9CeF7375518e25997 | 0x3d146FcE6c1006857750cBe8aF44f76a28041CCc | 0xbC203d7f83677c7ed3F7acEc959963E7F4ECC5C2 |
| TickLens                   | 0x9a489505a00cE272eAa5e07Dba6491314CaE3796 | 0x9a489505a00cE272eAa5e07Dba6491314CaE3796 | 0x9a489505a00cE272eAa5e07Dba6491314CaE3796 | 0x7b08978FA77910f77d273c353C62b5BFB9E6D17B | 0xac1cE734566f390A94b00eb9bf561c2625BF44ea |
| TokenValidator             | 0x864ED564875BdDD6F421e226494a0E7c071C06f8 | 0x556B9306565093C855AEA9AE92A594704c2Cd59e | 0x8be9EA9C6015985AB2F5A216093305A9AaEb8164 | 0x08529A4be615746ef31CdbeD46Ce556406787E2F | 0x678Aa4bF4E210cf2166753e054d5b7c31cc7fa86 |
| PancakeInterfaceMulticall  | 0xac1cE734566f390A94b00eb9bf561c2625BF44ea | 0xac1cE734566f390A94b00eb9bf561c2625BF44ea | 0xac1cE734566f390A94b00eb9bf561c2625BF44ea | 0x2a76b93B9Cd441AE8aDA529e0e95826e00556351 | 0x3D00CdB4785F0ef20C903A13596e0b9B2c652227 |

**Smart Router (v3, v2, stable)**

| BSC, ETH                                   | zkEVM                                      | Arbitrum                                   | zkSync                                     | GOR, BSC TESTNET                           |
| ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ |
| 0x13f4EA83D0bd40E75C8222255bc855a974568Dd4 | 0x678Aa4bF4E210cf2166753e054d5b7c31cc7fa86 | 0x32226588378236Fd0c7c4053999F88aC0e5cAc77 | 0xf8b59f3c3Ab33200ec80a8A58b2aA5F5D2a8944C | 0x9a489505a00cE272eAa5e07Dba6491314CaE3796 |

**MasterchefV3**

| BSC, ETH                                   | zkEVM                                      | zkSync                                     | GOR, BSC TESTNET                           |
| ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ |
| 0x556B9306565093C855AEA9AE92A594704c2Cd59e | 0xe9c7f3196ab8c09f6616365e8873daeb207c0391 | 0x4c615E78c5fCA1Ad31e4d66eb0D8688d84307463 | 0x4c650FB471fe4e0f476fD3437C3411B1122c4e3B |
