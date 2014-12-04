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