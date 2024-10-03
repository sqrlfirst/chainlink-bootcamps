# RWA Bootcamp

## Cross-chain real Estate

### Deploy RealEstateToken.sol to Avalanche Fuji

**Make sure to turn the Solidity compiler optimizer on to 200 runs and set EVM version to "Paris".**

To deploy the `RealEstateToken.sol` token to Avalanche Fuji we will need to provide the following information to constructor

- **uri_:** "" (this is the base ERC-1155 token URI, we will leave it empty)
- **ccipRouterAddress:** `0xF694E193200268f9a4868e4Aa017A0118C9a8177`
- **linkTokenAddress:** `0x0b9d5D9136855f6FEc3c0993feE6E9CE8a297846`
- **currentChainSelector:** `14767482510784806043`
- **functionsRouterAddress:** `0xA9d587a00A31A52Ed70D6026794a8FC5E2F5dCb0`

### Deploy Issuer.sol to Avalanche Fuji

To deploy the Issuer.sol token to Avalanche Fuji we will need to provide the following information to constructor

- **realEstateToken:** The address of the RealEstateToken.sol contract we previously deployed
- **functionsRouterAddress:** 0xA9d587a00A31A52Ed70D6026794a8FC5E2F5dCb0 