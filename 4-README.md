# basis-board

Every tokenized stock (B20) on Base, priced on-chain. Read-only, pinned-block, fail-closed. Base Stocks Maxxing - Programmable Stock Markets track.

- **Snapshot board (audited, hash-pinned):** https://dannytungadi5.github.io/basis-board/
- **LIVE companion (prices recomputed in your browser via dual-RPC eth_call):** https://dannytungadi5.github.io/basis-board/live.html

The live page queries two independent public Base RPCs at a pinned block and only shows values that match byte-for-byte. No wallet, no keys, no transactions.


375 pool records scanned; 82 verified and priced on-chain (snapshot coverage).

Two primary public Base RPC endpoints (mainnet.base.org and publicnode) are compared byte-for-byte. A third endpoint (BlastAPI) replaces one primary only after a transport failure; it is not a third vote. Two matching responses are required; a mismatch or only one usable response hides the value.
