# CryptoJS

Port of CryptoJS for using with CommonJS.

Original project: https://code.google.com/p/crypto-js/

### Usage with Browserify

```javascript
window.CryptoJS = require('./path/to/crypto-js');
require('./path/to/crypto-js/components/enc-base64');
require('./path/to/crypto-js/components/md5');
require('./path/to/crypto-js/components/evpkdf');
require('./path/to/crypto-js/components/cipher-core');
require('./path/to/crypto-js/components/aes');
```

### Encryption/Decryption

```javascript
var passphrase = 'MyKeyHere';
var encrypted = CryptoJS.AES.encrypt('ssshhhhh!', passphrase); // .toString() for just string
var decrypted = CryptoJS.AES.decrypt(encrypted, passphrase); // .toString(CryptoJS.enc.Utf8) for getting back `ssshhhhh!`
```