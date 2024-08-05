# electrum-client

Electrum Protocol Client for node.js.

# Tor

To connect to Electrum over a Tor connection:

```
const client = new ElectrumClient(50001, "myonionaddress.onion", "tcp", {
    proxy: {
      host: "127.0.0.1",
      port: 9050,
      type: 5,
    },
  });
```

# based on

* https://github.com/you21979/node-electrum-client
* https://github.com/7kharov/node-electrum-client
* https://github.com/BlueWallet/rn-electrum-client

# features

* persistence (ping strategy and reconnection)
* batch requests
* works in nodejs

## protocol spec

* https://electrumx.readthedocs.io/en/latest/PROTOCOL.html

## usage

Relies on `net` so will only run in NodeJS environment.
