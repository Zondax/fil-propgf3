# Filecoin Core Infrastructure & Integration Support

> Sustaining the Filecoin integration layer for wallets, exchanges, developers, and ecosystem services.

This project supports the parts of Filecoin that connect it to the outside world: the Ledger hardware-wallet stack for FIL, the Rosetta Filecoin implementation used by Coinbase, and the public node and archival infrastructure used by independent developers, exchanges, Beryx, and other ecosystem services.

## Scope

| Area | Included work |
| --- | --- |
| Ledger stack | FIL Ledger app, Ledger Live integration, and Rust, JavaScript, and Go libraries |
| Rosetta suite | Rosetta Filecoin libraries and proxy services used by exchange integrations |
| Public infrastructure | Public nodes, public RPC, archival nodes, and chain data services |
| Upgrade support | Compatibility work across Lotus, protocol, SDK, and network upgrades |

## Why It Matters

We operate these components as one shared platform because Filecoin protocol and SDK changes affect them together. A single Lotus upgrade can ripple through custody workflows, exchange integrations, public RPC access, and chain data services at the same time.

As one concrete example, our archival nodes hold complete chain history since genesis, which has allowed exchanges to backfill Filecoin data they could not reconstruct on their own.

## Grant Rationale

Running this as one shared fleet keeps the layer affordable. A single grant sustains infrastructure that would otherwise require several separate efforts while preserving operational continuity for the 2026 demand-side strategy.

The gap it fills is simple: Filecoin's demand-side growth depends on the network remaining reachable and transactable, and those outcomes fail when an upgrade quietly breaks the integration layer.

## Repositories

| Component | Repository |
| --- | --- |
| Ledger app | [Zondax/ledger-filecoin](https://github.com/Zondax/ledger-filecoin) |
| Ledger Rust library | [Zondax/ledger-filecoin-rs](https://github.com/Zondax/ledger-filecoin-rs) |
| Ledger JavaScript library | [Zondax/ledger-filecoin-js](https://github.com/Zondax/ledger-filecoin-js) |
| Ledger Go library | [Zondax/ledger-filecoin-go](https://github.com/Zondax/ledger-filecoin-go) |
| Rosetta Filecoin library | [Zondax/rosetta-filecoin-lib](https://github.com/Zondax/rosetta-filecoin-lib) |
| Rosetta Filecoin proxy | [Zondax/rosetta-filecoin-proxy](https://github.com/Zondax/rosetta-filecoin-proxy) |
| Indexing Rosetta proxy | [Zondax/filecoin-indexing-rosetta-proxy](https://github.com/Zondax/filecoin-indexing-rosetta-proxy) |
