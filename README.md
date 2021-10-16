In this project, instead of storing our password in database as it is, I will be using an encryption method
with an npm package "mongoose-encryption". This is a Level 2 security for storing password in database.

In cryptography, encryption is the process of encoding information. This process converts the original representation of the information, known as plaintext, into an alternative form known as ciphertext.

mongoose-encryption
===

Encryption is performed using AES-256-CBC with a random, unique initialization vector for each operation. Authentication is performed using HMAC-SHA-512.

We will not perform any authentication in this project.

Read mongoose-encryption documentation. There will be a part where it mentions about a secret string.

```
const secret = 'jsdhnicgvvtrbjjv';

userSchema.plugin(encrypt, {secret: secret});
```

Also read what plugins are in mongoose documentation.