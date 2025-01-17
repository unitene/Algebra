

# IPoolInitializer


Creates and initializes Algebra Pools

Provides a method for creating and initializing a pool, if necessary, for bundling with other methods that
require the pool to exist.

*Developer note: Credit to Uniswap Labs under GPL-2.0-or-later license:
https://github.com/Uniswap/v3-periphery*




## Functions
### createAndInitializePoolIfNecessary


`function createAndInitializePoolIfNecessary(address token0, address token1, uint160 sqrtPriceX96) external payable returns (address pool)` payable external

Creates a new pool if it does not exist, then initializes if not initialized
*Developer note: This method can be bundled with others via IMulticall for the first action (e.g. mint) performed against a pool*



| Name | Type | Description |
| ---- | ---- | ----------- |
| token0 | address | The contract address of token0 of the pool |
| token1 | address | The contract address of token1 of the pool |
| sqrtPriceX96 | uint160 | The initial square root price of the pool as a Q64.96 value |

**Returns:**

| Name | Type | Description |
| ---- | ---- | ----------- |
| pool | address | Returns the pool address based on the pair of tokens and fee, will return the newly created pool address if necessary |




