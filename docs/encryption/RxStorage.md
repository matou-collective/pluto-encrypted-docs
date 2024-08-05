---
sidebar_position: 1
---

# RxStorage
## Interface RxStorage ```<Internals, InstanceCreationOptions>```

A RxStorage is a module that acts as a factory that can create multiple RxStorageInstance objects.

All data inputs and outputs of a StorageInstance must be plain json objects. Do not use Map, Set or anything else that cannot be JSON.stringify-ed. This will ensure that the storage can exchange data when it is a WebWorker or a WASM process or data is send via BroadcastChannel.


## Type Parameters
- Internals
- InstanceCreationOptions

## Hierarchy
- RxStorage

_Defined in node_modules/rxdb/dist/types/types/rx-storage.interface.d.ts:43_

INDEX

### Properties

**Readonly** name

```
name: string
```

name of the storage engine used to detect if plugins do not work so we can throw proper errors.

_Defined in node_modules/rxdb/dist/types/types/rx-storage.interface.d.ts:48_

**Readonly** rxdbVersion

```
rxdbVersion: string
```

RxDB version is part of the storage so we can have fallbacks and stuff when multiple storages with different version are in use like in the storage migration plugin.

_Defined in node_modules/rxdb/dist/types/types/rx-storage.interface.d.ts:56_


### Methods
**createStorageInstance**

```
createStorageInstance<RxDocType>(params): Promise<RxStorageInstance<RxDocType, Internals, InstanceCreationOptions, any>
```
Creates a storage instance that can contain the NoSQL documents of a collection.

**Type Parameters**
- RxDocType

**Parameters**
- **params:** ```RxStorageInstanceCreationParams<RxDocType, InstanceCreationOptions>```

**Returns** ```Promise<RxStorageInstance<RxDocType, Internals, InstanceCreationOptions, any>>```

_Defined in node_modules/rxdb/dist/types/types/rx-storage.interface.d.ts:62_

TODO: 
- [ ] Need to add:
    - [ ] Settings
        - [ ] Member Visibility
          - [ ] Protected
          - [ ] Private
          - [x] Inherited
          - [ ] External 