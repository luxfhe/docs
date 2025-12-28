# 👷 luxfhe Hardhat Plugin 

luxfhe Hardhat Plugin is designed to extend your Hardhat environment with additional capabilities focused on luxfhe. It integrates seamlessly with your Hardhat projects to provide a local luxfhe environment, including customized network configuration and utilities for managing funds and permits within your blockchain applications.

## Features

- **Local luxfhe Environment:** Automatically sets up a local luxfhe network configuration within Hardhat, allowing for easy deployment and interaction with luxfhe contracts.
- **Faucet Integration:** Enables developers to easily obtain funds for testing purposes through a simple API call to a local faucet.
- **Permit Management:** Simplifies the process of creating and storing permit signatures required for transactions, reducing the complexity of interacting with contracts that require permissions.

If you want to see a full example in action, check out our [Hardhat Example Template](https://github.com/luxfheProtocol/luxfhe-hardhat-example)!

## Installation

To use luxfheJS in your Hardhat project, first install the plugin via npm (or your favorite package manager):

```sh
pnpm install luxfhe-hardhat-plugin
```

If you wish to run your own local dev environment, please install the [luxfhe-hardhat-docker](https://www.npmjs.com/package/luxfhe-hardhat-docker) plugin as well.

```sh
pnpm install luxfhe-hardhat-docker
```

## Setup

After installation, import the plugin in your Hardhat configuration file (e.g., `hardhat.config.js`):

```javascript
require("luxfhe-hardhat-plugin");
// if using the docker plugin
require("luxfhe-hardhat-docker");
```

or if you are using TypeScript, in your `hardhat.config.ts`:

```typescript
import "luxfhe-hardhat-plugin";
// if using the docker plugin
import "luxfhe-hardhat-docker";
```

## Configuration

### Network Configuration

The plugin automatically adds a `localluxfhe` network configuration to your Hardhat project. This configuration is designed for local development and includes settings such as gas estimates, accounts, and the local network URL.

This network is chosen as the default once the plugin is imported. 
If you want to use a different network, simply add `--network <custom_network>` to your hardhat commands, or set it as the default.

If you want to use luxfhe Helium Testnet (or a custom luxfhe network), you can add a new network configuration to your `hardhat.config.js` file:

```typescript
const config: HardhatUserConfig = {
    networks: {
        luxfheHelium: {
            url: "https://api.helium.luxfhe.zone",
            chainId: 8008135,
            accounts: mnemonic,
        },
    },
};

export default config;
```

### Using luxfheJS from Hardhat Runtime Environment

After importing `luxfhe-hardhat-plugin` hardhat will automatically extend the Hardhat Runtime Environment (HRE) with a `luxfhejs` object, providing access to luxfhe-specific functionality:

- Use the `luxfhejs` object directly to encrypt, unseal or manage permits.
- **`getFunds(address: string)`**: Request funds from the local faucet for the specified address.
- **`createPermit(contractAddress: string, provider?: SupportedProvider)`**: Create and store a permit for interacting with a contract.

## Usage

### Local Dev Environment

To set up a localluxfhe instance, simply import `luxfhe-hardhat-docker`. This will add two new hardhat tasks:

- **`localluxfhe:start`** To start a local dev environment using docker. By default, the instance will listen for rpc connections on port `42069`
- **`localluxfhe:stop`** Stops the docker container

To start the container:

```sh
pnpm hardhat localluxfhe:start
```

If starting the instance was successful, you should see the message: `Started Localluxfhe successfully at 127.0.0.1:42069`.

To stop the running container:

```sh
pnpm hardhat localluxfhe:stop
```

Which will result in `Successfully shut down Localluxfhe`

### Requesting Funds

To request funds from the local faucet for an address, use the `getFunds` method:

```javascript
await hre.luxfhejs.getFunds("your_wallet_address");
```

### Encryption

```javascript
const encyrptedAmount = await luxfhejs.encrypt_uint32(15);
```

### Creating a Permit

To create a permit for a contract, use the `createPermit` method:

```javascript
const permit = await hre.luxfhejs.createPermit("contract_address");
```

## Support

For issues, suggestions, or contributions, please open an issue or pull request in the [Hardhat luxfhe Plugin GitHub repository](https://github.com/luxfhe/luxfhe-hardhat-plugin).
