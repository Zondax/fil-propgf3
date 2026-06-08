# Filecoin Core Infrastructure & Integration Support

This project sustains the parts of Filecoin that connect it to the outside world: the Ledger hardware-wallet stack for FIL, including the device app and Rust, JavaScript, and Go libraries; the Rosetta Filecoin implementation used by Coinbase to integrate Filecoin; and the public node and archival infrastructure used by independent developers, exchanges, Beryx, and other ecosystem services.

We operate these components as one shared platform because Filecoin protocol and SDK changes affect them together. A single Lotus upgrade can impact custody workflows, exchange integrations, public RPC access, and chain data services at the same time, so we support exchanges and providers through every network upgrade. As one concrete example, our archival nodes keep complete chain history since genesis, allowing exchanges to backfill Filecoin data they could not reconstruct on their own.

Running this as one shared fleet keeps the layer affordable. A single grant sustains infrastructure that would otherwise require several separate efforts: public nodes, archival nodes, public RPC, the Rosetta suite, network-upgrade support, the Ledger app, and Ledger Live integration. The grant fills an operational continuity gap: the 2026 demand-side strategy depends on Filecoin remaining reachable and transactable, and those outcomes fail when an upgrade quietly breaks the integration layer.

## Links

- [ledger-filecoin](https://github.com/Zondax/ledger-filecoin)
- [ledger-filecoin-rs](https://github.com/Zondax/ledger-filecoin-rs)
- [ledger-filecoin-js](https://github.com/Zondax/ledger-filecoin-js)
- [ledger-filecoin-go](https://github.com/Zondax/ledger-filecoin-go)
- [rosetta-filecoin-lib](https://github.com/Zondax/rosetta-filecoin-lib)
- [rosetta-filecoin-proxy](https://github.com/Zondax/rosetta-filecoin-proxy)
- [filecoin-indexing-rosetta-proxy](https://github.com/Zondax/filecoin-indexing-rosetta-proxy)
