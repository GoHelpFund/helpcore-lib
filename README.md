# Helpcore Library

[![Build Status](https://img.shields.io/travis/gohelpfund/helpcore-lib.svg?branch=master)](https://travis-ci.org/gohelpfund/helpcore-lib)
[![NPM Package](https://img.shields.io/npm/v/@gohelpfund/helpcore-lib.svg)](https://www.npmjs.org/package/@gohelpfund/helpcore-lib)

> A pure and powerful JavaScript Help library.

Help is a powerful new peer-to-peer platform for the next generation of financial technology. The decentralized nature of the Help network allows for highly resilient Help infrastructure, and the developer community needs reliable, open-source tools to implement Help apps and services.

## Table of Contents
- [Install](#install)
- [Usage](#usage)
- [Documentation](#documentation)
- [Contributing](#contributing)
- [License](#license)

## Install

### NodeJS

```
npm install @gohelpfund/helpcore-lib
```

### Browser

See the section below to generate your own bundle, or download the pre-generated [minified file](dist/helpcore-lib.min.js)

#### Building the Browser Bundle

To build a helpcore-lib full bundle for the browser:

```sh
npm run build
```

This will generate files named `helpcore-lib.js` and `helpcore-lib.min.js` in the `dist/` folder.

## Usage

### Browser

```
<script src='./dist/helpcore-lib.min.js' type="text/javascript"></script>
<script>
  const PrivateKey = helpcore.PrivateKey;
  const privateKey = new PrivateKey();
  const address = privateKey.toAddress().toString();
</script>
```

### Modules

Some functionality is implemented as a module that can be installed separately:

* [Payment Protocol Support](https://github.com/gohelpfund/helpcore-payment-protocol)
* [Peer to Peer Networking](https://github.com/gohelpfund/helpcore-p2p)
* [Help Core JSON-RPC](https://github.com/gohelpfund/helpd-rpc)
* [Payment Channels](https://github.com/gohelpfund/helpcore-channel)
* [Mnemonics](https://github.com/gohelpfund/helpcore-mnemonic)
* [Elliptical Curve Integrated Encryption Scheme](https://github.com/gohelpfund/bitcore-ecies-help)
* [Signed Messages](https://github.com/gohelpfund/bitcore-message-help)

### Development & Tests

```sh
git clone https://github.com/gohelpfund/helpcore-lib
cd helpcore-lib
npm install
```

Run all the tests:

```sh
npm test
```

You can also run just the Node.js tests with `npm run test:node`, just the browser tests with `npm run test:browser` or run a test coverage report with `npm run coverage`.

## Documentation

* [Addresses](docs/address.md)
* [Block](docs/block.md)
* [Crypto](docs/crypto.md)
* [Encoding](docs/encoding.md)
* [Hierarchically-derived Private and Public Keys](docs/hierarchical.md)
* [Mnemonic](docs/mnemonic.md)
* [Networks](docs/networks.md)
* [PrivateKey](docs/privatekey.md)
* [PublicKey](docs/publickey.md)
* [Script](docs/script.md)
* [Transaction](docs/transaction.md)
* [Using Different Units](docs/unit.md)
* [Unspent Output](docs/unspentoutput.md)
* [URI](docs/uri.md)
* [Governance Object / Proposal](docs/govobject/govobject.md)

### Examples

Some examples can be found [here](docs/examples.md), below is a list of direct links for some of them.

* [Generate a random address](docs/examples.md#generate-a-random-address)
* [Generate an address from a SHA256 hash](docs/examples.md#generate-a-address-from-a-sha256-hash)
* [Import an address via WIF](docs/examples.md#import-an-address-via-wif)
* [Create a Transaction](docs/examples.md#create-a-transaction)
* [Sign a Help message](docs/examples.md#sign-a-bitcoin-message)
* [Verify a Help message](docs/examples.md#verify-a-bitcoin-message)
* [Create an OP RETURN transaction](docs/examples.md#create-an-op-return-transaction)
* [Create a 2-of-3 multisig P2SH address](docs/examples.md#create-a-2-of-3-multisig-p2sh-address)
* [Spend from a 2-of-2 multisig P2SH address](docs/examples.md#spend-from-a-2-of-2-multisig-p2sh-address)

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/gohelpfund/helpcore-lib/blob/master/CONTRIBUTING.md) file.

## License

Code released under [the MIT license](LICENSE).

Copyright 2013-2017 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.  
Copyright 2016-2017 The Dash Foundation, Inc.
Copyright 2017-2018 Dash Core Group, Inc.
