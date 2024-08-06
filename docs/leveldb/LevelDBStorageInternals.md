---
sidebar_position: 2
---

# LevelDBStorageInternals

## Interface ```LevelDBStorageInternals<RxDocType>```

Main storage interface for LevelDBStorage

### Type Parameters
- **RxDocType**

### Hierarchy
- **LevelDBStorageInternals**

_Defined in [packages/leveldb/src/leveldb/types.ts:38](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L38)_


### Properties INDEX
- [bulkGet](#bulkget)
- [bulkPut](#bulkput)
- [clear](#clear)
- [close](#close)
- [documents](#documents)
- [get](#get)
- [getDocuments](#getdocuments)
- [getIndex](#getindex)
- [refCount](#refcount)
- [removed](#removed)
- [schema](#schema)
- [set](#set)
- [setIndex](#setindex)
- [updateIndex](#updateindex)

### Properties

#### bulkGet
```
bulkGet: ((keys) => Promise<RxDocumentData<RxDocType>[]>)
```

**Type declaration**
- ```(keys): Promise<RxDocumentData<RxDocType>[]>```

  **Parameters**
    - keys: string[]
    **Returns** ```Promise<RxDocumentData<RxDocType>[]>```

_Defined in [packages/leveldb/src/leveldb/types.ts:52](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L52)_


#### bulkPut
```
bulkPut: ((items, collectionName, schema) => Promise<any>)
```

**Type declaration**
- ```(items, collectionName, schema): Promise<any>```

  **Parameters**
    - **items:** any
    - **collectionName:** string
    - **schema:** ```Readonly<RxJsonSchema<RxDocumentData<RxDocType>>>```
  **Returns** ```Promise<any>```

_Defined in [packages/leveldb/src/leveldb/types.ts:44](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L44)_


#### clear
```
clear: (() => Promise<void>)
```

**Type declaration**
- ```(): Promise<void>```
  **Returns** ```Promise<void>```

_Defined in [packages/leveldb/src/leveldb/types.ts:49](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L49)_


#### close
```
close: (() => Promise<void>)
```

**Type declaration**
- ```(): Promise<void>```
  **Returns** ```Promise<void>```

_Defined in [packages/leveldb/src/leveldb/types.ts:48](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L48)_

#### documents
```
documents: Map<string, RxDocumentData<RxDocType>>
```

_Defined in [packages/leveldb/src/leveldb/types.ts:40](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L40)_

#### get
```
get: ((key) => Promise<null | RxDocumentData<RxDocType>>)
```

**Type declaration**
- ```(key): Promise<null | RxDocumentData<RxDocType>>```

  **Parameters**
  - key: string
  **Returns** ```Promise<null | RxDocumentData<RxDocType>>```

_Defined in [packages/leveldb/src/leveldb/types.ts:50](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L50)_


#### getDocuments
```
getDocuments: ((query) => Promise<Map<string, RxDocumentData<RxDocType>>>)
```

**Type declaration**

- ```(query): Promise<Map<string, RxDocumentData<RxDocType>>>```
  **Parameters**
  - query: string[]
  **Returns** ```Promise<Map<string, RxDocumentData<RxDocType>>>```

_Defined in [packages/leveldb/src/leveldb/types.ts:39](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L39)_


#### getIndex
```
getIndex: ((key) => Promise<string[]>)
```

**Type declaration**
- ```(key): Promise<string[]>```
  **Parameters**
  - key: string
  **Returns** ```Promise<string[]>```

_Defined in [packages/leveldb/src/leveldb/types.ts:51](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L51)_


#### refCount
```
refCount: number
```

_Defined in [packages/leveldb/src/leveldb/types.ts:42](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L42)_


#### removed
```
removed: boolean
```

_Defined in [packages/leveldb/src/leveldb/types.ts:41](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L41)_


#### schema
```
schema: RxJsonSchema<RxDocumentData<RxDocType>>
```

_Defined in [packages/leveldb/src/leveldb/types.ts:43](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L43)_


#### set
````
set: ((key, data) => Promise<void>)
````

**Type declaration**
- ```(key, data): Promise<void>```

  **Parameters**
  - **key:** string
  - **data:** ```RxDocumentData<RxDocType>```
  **Returns** ```Promise<void>```

_Defined in [packages/leveldb/src/leveldb/types.ts:53](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L53)_


#### setIndex
```
setIndex: ((key, ids) => Promise<void>)
```

**Type declaration**
- ```(key, ids): Promise<void>```

  **Parameters**
  - key: string
  - ids: string[]
  **Returns** ```Promise<void>```

_Defined in [packages/leveldb/src/leveldb/types.ts:54](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L54)_


#### updateIndex
```
updateIndex: ((key, id) => Promise<void>)
```

**Type declaration**
- ```(key, id): Promise<void>```

  **Parameters**
  - key: string
  - id: string
  **Returns** ```Promise<void>```

_Defined in [packages/leveldb/src/leveldb/types.ts:55](https://github.com/atala-community-projects/pluto-encrypted/blob/48380434/packages/leveldb/src/leveldb/types.ts#L55)_