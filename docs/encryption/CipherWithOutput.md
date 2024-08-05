---
sidebar_position: 3
---

# CipherWithOutput
## Type alias CipherWithOutput

```
CipherWithOutput: Cipher & {
    decrypt(ciphertext, output?) => Uint8Array;
    encrypt(plaintext, output?) => Uint8Array;
}
```

## Type declaration
- **decrypt:function**
```decrypt(ciphertext, output?): Uint8Array```

  **Parameters**
  - ciphertext: Uint8Array
  - **Optional** output: Uint8Array

  **Returns** Uint8Array
  _Defined in node_modules/@noble/ciphers/utils.d.ts:64_

- **encrypt:function**
```encrypt(plaintext, output?): Uint8Array```
  **Parameters**
  - plaintext: Uint8Array
  - Optional output: Uint8Array
  **Returns** Uint8Array

  _Defined in node_modules/@noble/ciphers/utils.d.ts:63_
  
  
_Defined in node_modules/@noble/ciphers/utils.d.ts:62_

TODO: 
- [ ] Need to add:
    - [ ] Settings
        - [ ] Member Visibility
          - [ ] Protected
          - [ ] Private
          - [x] Inherited
          - [ ] External 