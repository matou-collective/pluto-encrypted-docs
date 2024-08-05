---
sidebar_position: 1
---

# Module encryption

This package is an rxdb encryption layer, a replacement for the vulnerable crypto-js dependency provided by the free version of rxDB. The package can be used outside or Pluto as its fully compatible with RXDB.

### Examples
In order to use this package in any RXDB environment type the following code. Install the package with npm

```npm i @pluto-encrypted/encryption --save```

or with yarn

```npm i @pluto-encrypted/encryption --save```

Integrate in your existing RXDB storage.

```
import { wrappedKeyEncryptionStorage } from "@pluto-encrypted/encryption";
import { RxStorage } from "rxdb";
const storage: RxStorage<any, any> = wrappedKeyEncryptionStorage({
    storage: [[ADD your RXDB instance here]],
})
export default storage;
```

_Defined in [packages/encryption/src/index.ts:1](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/encryption/src/index.ts#L1)_

## Index

### Interfaces
- [RxStorage](/docs/encryption/RxStorage.md)

### Type Aliases
- [CipherWithOutput](/docs/encryption/CipherWithOutput.md)
- [InternalStorePasswordDocType](/docs/encryption/InternalStorePasswordDocType.md)

### Functions

- [decryptString](/docs/encryption/decryptString.md)
- [encryptString](/docs/encryption/encryptString.md)
- [wrappedKeyEncryptionStorage](/docs/encryption/wrappedKeyEncryptionStorage.md)