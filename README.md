# 🪂 Foundry Merkle Airdrop CU

> A simple and gas-optimized Merkle tree–based airdrop contract built using Foundry.  
> Users can claim tokens if they are in a predefined Merkle tree and provide a valid EIP-712 signature.

---

## 📦 Features

- ✅ Airdrop protected by a Merkle root (only whitelisted addresses can claim)
- ✅ EIP-712 signature verification (ensures the claim is authorized)
- ✅ Single-claim enforcement (no double-spending)
- ✅ Uses OpenZeppelin libraries for security
- ✅ Built and tested using [Foundry](https://book.getfoundry.sh/)

---

## 🧱 Contract Summary

- The contract uses:
  - `MerkleProof` for validating whitelist
  - `EIP712` & `ECDSA` for verifying claims via off-chain signatures
  - `SafeERC20` for safe token transfers
- A user must:
  1. Have a valid Merkle proof
  2. Provide a valid EIP-712 signature
  3. Have not claimed before

---

## 🧪 How to Test It

### 1. Clone & Install

## Documentation

https://book.getfoundry.sh/

## Usage

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Format

```shell
$ forge fmt
```

### Gas Snapshots

```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

### Deploy

```shell
$ forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
$ cast <subcommand>
```

### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```
