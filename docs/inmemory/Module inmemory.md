---
sidebar_position: 1
---

# Module inmemory

This is a RXDB InMemory storage that supports encryption middleware. In order to use this in your pluto-encrypted database you must write the following code: Creating a InMemory compatible storage is very simple.

```
import InMemory from "@pluto-encrypted/inmemory";
import { Database } from "@pluto-encrypted/database";
//default password must be 32 bytes long
const defaultPassword = new Uint8Array(32).fill(1);
const database = db = await Database.createEncrypted({
         name: `my-db`,
         encryptionKey: defaultPassword,
         storage: InMemory,
});
```

_Defined in [packages/inmemory/src/index.ts:1](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/inmemory/src/index.ts#L1)_

## Index

### Variables
- [storage](/docs/inmemory/storage.md)