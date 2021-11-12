# cht
**cht** is a blockchain built using Cosmos SDK and Tendermint Core.

## Get started

To get started clone this repository.
```
cd cht
starport chain serve
```

`serve` command installs dependencies, builds, initializes, and starts your blockchain in development.

Using the `starport chain serve` command is great for getting the chain started, but for running a node for long periods of time we will need to create a systemd process. This can be found in the developer documentation.

### Configure
In the Developer Docs there will be clear instructions on how to configure your full node to the live network.

### Launch

To launch your blockchain live on multiple nodes, use `starport network` commands. Learn more about [Starport Network](https://github.com/tendermint/spn).

### Web Frontend

Starport has scaffolded a Vue.js-based web app in the `vue` directory. Run the following commands to install dependencies and start the app:
This allows a web socket for developers to connect to the blockchain

```
cd vue
npm install
npm run serve
```

The frontend app is built using the `@starport/vue` and `@starport/vuex` packages. For details, see the [monorepo for Starport front-end development](https://github.com/tendermint/vue).

## Release
To release a new version of your blockchain, create and push a new tag with `v` prefix. A new draft release with the configured targets will be created.

```
git tag v0.1
git push origin v0.1
```

After a draft release is created, make your final changes from the release page and publish it.

### Install
To install the latest version of your blockchain node's binary, execute the following command on your machine:

```
curl https://get.starport.network/ChronicToken/cht@latest! | sudo bash
```
