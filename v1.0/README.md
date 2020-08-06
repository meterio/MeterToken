# Contracts
This is Meter/MeterGov ERC20 contracts can be uploaded to Meter and Ethereum. The ERC20 libraries are from openzeppelin.

The ERC20 contracts are upgrade-able by proxy.

Compile 
============
if smart contract is running on meter:
solc-static-linux-0.6.10 --optimize-runs 200 --overwrite --bin --abi --evm-version constantinople -o ./compiled WMTR.sol WMTRG.sol MeterERC20Proxy.sol

on ethereum:
solc-static-linux-0.6.10 --optimize-runs 200 --overwrite --bin --abi -o ./compiled WMTR.sol WMTRG.sol MeterERC20Proxy.sol

All outputs are located in directory compiled.

WMTR.sol is for Meter ERC2020
WMTRG.sol is for MeterGov ERC20
MeterERC20Proxy.sol is for proxy
