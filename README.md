<img src="http://fcash.io/css/images/module-mnemonic.png" alt="fcash mnemonics" height="35">
BIP39 Mnemonics for fcash
=======

[![NPM Package](https://img.shields.io/npm/v/fcash-mnemonic.svg?style=flat-square)](https://www.npmjs.org/package/fcash-mnemonic)
[![Build Status](https://img.shields.io/travis/bitpay/fcash-mnemonic.svg?branch=master&style=flat-square)](https://travis-ci.org/bitpay/fcash-mnemonic)
[![Coverage Status](https://img.shields.io/coveralls/bitpay/fcash-mnemonic.svg?style=flat-square)](https://coveralls.io/r/bitpay/fcash-mnemonic)

A module for [fcash](https://github.com/bitpay/fcash) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install fcash-mnemonic
bower install fcash-mnemonic
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://fcash.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('fcash-mnemonic');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/bitpay/fcash/blob/master/CONTRIBUTING.md) on the main fcash repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/bitpay/fcash/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Fcash is a trademark maintained by BitPay, Inc.
