# Primitive Data Types  
Here we introduce some primitive data types available in Solidity.  
* `boolean`
* `uint`
* `int`
* `address`

```
// SPDX-License-Identifier: MIT
pragma solidity ^0.6.10;

contract Primitives {
	bool boo = true;

	/*
	uint stands for unsigned integer, meaning non negative integers
	different sizes are available
		uint8		ranges from 0 to 2 ** 8 - 1
		uint16	ranges from 0 to 2 ** 16 - 1
		...
		uint256 ranges from 0 to 2 ** 256 - 1
	*/
	uint8 u8 = 1;
	uint256 u256 = 456;
	uint u = 123; // uint is an alias for uint256

	/*
	Negative numbers are allowed for int types.
	Like uint, different ranges are available from int8 to int256
	*/
	int8 i8 = -1;
	int256 i256= 456;
	int i = -123; // int is same as int256

	address addr = 0xCA35b7d915458EF540aDe6068dFe2F44E8fa733c;

	// Default values
	// Unassigned variables have a default value
	bool defaultBool; // false
	uint defaultUint; // 0
	int defaultInt; // 0
	address defaultAddr; // 0x0000000000000000000000000000000000000000
}
```