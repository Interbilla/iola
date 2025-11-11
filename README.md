# IOLA (Interbella)

- **Token ID:** `0xd1aae85c...e5dcea::IolaCoin::IOLACOIN`
- **Decimals:** 6
- **Network:** IOTA Rebased Testnet
- **Issuer:** `0x7ced4d4e...bc46611`

This repo serves as the canonical on-chain/off-chain registry for IOLA.

# iola
IOLA Coin proof-of-record and token registry

# clone
git clone https://github.com/Interbilla/iola.git
cd iola

# verify tag signature
git verify-tag iola-1.0.0

# show tokenId from the tagged version
git show iola-1.0.0:registry/iola-registry.json | jq -r '.tokenId'

# verify checksum matches the file contents at that tag
git show iola-1.0.0:registry/checksums.txt
git show iola-1.0.0:registry/iola-registry.json | sha256sum

