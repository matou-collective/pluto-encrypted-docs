---
sidebar_position: 1
---

# Module leveldb

This is a RXDB LevelDB storage that supports encryption middleware. In order to use this in your pluto-encrypted database you must write the following code: Creating a LevelDB compatible storage is very simple.

```
import { createLevelDBStorage } from "@pluto-encrypted/leveldb";
import { Database } from "@pluto-encrypted/database";
//default password must be 32 bytes long
const defaultPassword = new Uint8Array(32).fill(1);
const database = db = await Database.createEncrypted({
         name: `my-db`,
         encryptionKey: defaultPassword,
         storage: createLevelDBStorage({
         dbName: "demo",
         dbPath: "/tmp/demo"
      })
});
```

_Defined in [packages/leveldb/src/index.ts:1](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/index.ts#L1)_

## Interfaces
- [LevelDBStorageInternals](/docs/leveldb/LevelDBStorageInternals.md)
- [TopLevelProperty](/docs/leveldb/TopLevelProperty.md)

## Type Aliases
- [CRDTSchemaOptions](/docs/leveldb/CRDTSchemaOptions.md)
- [CompressionMode](/docs/leveldb/CompressionMode.md)
- [FilledMangoQuery](/docs/leveldb/FilledMangoQuery.md)
- [IndexType](/docs/leveldb/IndexType.md)
- [LevelDBDataIndex](/docs/leveldb/LevelDBDataIndex.md)
- [LevelDBDataStructure](/docs/leveldb/LevelDBDataStructure.md)
- [LevelDBInternalConstructor](/docs/leveldb/LevelDBInternalConstructor.md)
- [LevelDBPreparedQuery](/docs/leveldb/LevelDBPreparedQuery.md)
- [LevelDBSettings](/docs/leveldb/LevelDBSettings.md)
- [LevelDBType](/docs/leveldb/LevelDBType.md)
- [MangoQuery](/docs/leveldb/MangoQuery.md)
- [MangoQueryNoLimit](/docs/leveldb/MangoQueryNoLimit.md)
- [MangoQuerySelectorAndIndex](/docs/leveldb/MangoQuerySelectorAndIndex.md)
- [MangoQuerySortDirection](/docs/leveldb/MangoQuerySortDirection.md)
- [MangoQuerySortPart](/docs/leveldb/MangoQuerySortPart.md)
- [PrimaryKey](/docs/leveldb/PrimaryKey.md)
- [RxJsonSchema](/docs/leveldb/RxJsonSchema.md)
- [RxQueryPlan](/docs/leveldb/RxQueryPlan.md)
- [RxQueryPlanKey](/docs/leveldb/RxQueryPlanKey.md)
- [RxStorageLevelDBType](/docs/leveldb/RxStorageLevelDBType.md)
- [StringKeys](/docs/leveldb/StringKeys.md)

## Properties
- [Level](/docs/leveldb/Level.md)

## Functions
- [createLevelDBStorage](/docs/leveldb/createLevelDBStorage.md)

## Properties
**Level**
```Level: any```