# NEAR Protocol

NEAR Protocol provides blockchain infrastructure with JSON-RPC 2.0 and REST APIs for querying accounts, transactions, tokens, NFTs, and staking data on the NEAR network. Developers can interact with the NEAR blockchain through the official RPC endpoints, the FASTNEAR indexed REST API, and the NearBlocks explorer API.

## APIs

### NEAR RPC API

JSON-RPC 2.0 API for programmatic access to the NEAR blockchain. All requests are POST to a provider endpoint with the method name in the URL path.

- **Base URL (Mainnet):** `https://rpc.mainnet.near.org`
- **Docs:** https://docs.near.org/api/rpc/introduction
- **Auth:** None (public endpoint, rate-limited)

**Methods include:** `send_tx`, `tx`, `block`, `chunk`, `query` (view_account, view_code, view_state, call_function), `status`, `health`, `network_info`, `validators`, `gas_price`, `light_client_proof`

### FASTNEAR Indexed REST API

Low-latency indexed REST API for account-centric reads including fungible tokens, NFTs, and staking.

- **Base URL (Mainnet):** `https://api.fastnear.com`
- **Docs:** https://docs.fastnear.com/
- **Auth:** API key via `Authorization: Bearer {key}` or `?apiKey=`

**Endpoints include:** `/v1/account/{id}/full`, `/v1/account/{id}/ft`, `/v1/account/{id}/nft`, `/v1/account/{id}/staking`, `/v1/ft/{token_id}/top`

### NearBlocks Explorer API

REST API derived from the NearBlocks block explorer with tiered subscription plans.

- **Base URL:** `https://api.nearblocks.io`
- **Docs:** https://api.nearblocks.io/api-docs/
- **Auth:** API key (dashboard)
- **Plans:** Free ($0), Startup ($67.15/mo), Standard ($254.15/mo), Professional ($764.15/mo), Enterprise (custom)

## Links

- Website: https://near.org
- Developer Docs: https://docs.near.org
- GitHub: https://github.com/near
- NearBlocks: https://nearblocks.io
- FASTNEAR: https://fastnear.com
