# Uptick DID JS SDK

SDK to work with Uptick DID using JavaScript and TypeScript languages.

## Disclaimer

Uptick DID JS SDK is in public now. It may still contain bugs or missing functionality, that it will be added in next versions.

## Usage

Installation:

```bash
npm install @uptsmart/js-sdk
```

See [tests](/tests) for examples on how to use SDK.

## Tests

Run unit tests:

```bash
npm run test
```

Note: mtp / sig / auth / rhs files contain integration tests!

To run them, please set following variables:

```bash
export WALLET_KEY="...key in hex format"
export RPC_URL="...url to uptick network rpc node"
export RHS_URL="..reverse hash service url"
export IPFS_URL="url for ipfs"

```

And place actual circuits to `test/proofs/testdata`

## Documentation

### Generate documentation

1. Define path where documentation repository is located, for example:

    ```typescript
        const DOCS_DIR = '../js-sdk-tutorials/docs/api';
    ```

2. ```bash
        npm run tsc:declaration:watch
    ```

3. ```bash
        npm run doc:watch:website
    ```

Documentation can be found [here](https://uptickDID.github.io/js-sdk-tutorials/)
