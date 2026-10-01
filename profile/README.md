# Ownbound

### Truly Owned. Freely Shared.

**True ownership for digital books.** Buy a book and you genuinely own it: read it
anywhere, lend it to a friend one reader at a time, get it back, or sell it on -
just like a paperback. Ownership is recorded on a public ledger, so your library
outlives any single store, including ours.

## How it works

- **Own** - buy a book once and keep it; ownership lives on-chain, not in a vendor database.
- **Lend** - send it to a friend, one reader at a time, with a due date; it returns to you automatically.
- **Resell** - pass a finished book on, and the author earns a royalty every time it changes hands.
- **Read anywhere** - open it in any browser; sign in with email, no crypto knowledge needed.

## For authors and publishers

Keep the majority of every first sale and earn a perpetual royalty on every resale,
with a transparent, on-chain record of how your books move.
See [what Ownbound means for authors](https://ownbound.net/for-authors).

## Under the hood

Ownbound enforces single-holder access with a smart contract and holder-gated decryption:

- **Smart contract** (Solidity) records `owner` / `currentHolder` per copy and enforces one reader at a time.
- **Content** is AES-256-GCM encrypted; decryption keys never appear in any public file.
- **Reading is gated live:** the holder's wallet signs a one-time nonce, a key server re-checks
  on-chain holder status, and the book is decrypted in the browser - the plaintext never leaves the device.
- **Open and auditable:** the live contract runs on a public network.
  [View it on the explorer](https://sepolia.etherscan.io/address/0x712f6c5679C6A47a51B93077E19b6CA5FCcCA6E7).

Currently in **early access** on the Ethereum Sepolia testnet. Repositories are private
during the pilot; selected components may be opened as the project matures.

## Links

- Website: https://ownbound.net
- Library (app): https://app.ownbound.net
- LinkedIn: https://www.linkedin.com/company/ownboundbooks
- X: https://x.com/ownboundbooks
- Contact: hello@ownbound.net

---

_Built in Sydney, Australia._
