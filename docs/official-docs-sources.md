# Official Arc + Circle Documentation Sources

This repository uses the following official documentation as canonical sources. These links should be checked for current details before implementation because documentation, APIs, contract addresses, supported chains, and SDK behavior can change.

## Arc

Official documentation: https://docs.arc.io/

LLM-optimized documentation index: https://docs.arc.io/llms.txt

Key areas:
- Arc network and architecture
- EVM differences
- Connect to Arc / RPC
- Contract addresses
- Gas and fees
- Deploy and interact with contracts
- App Kit: Bridge, Swap, Send, Unified Balance
- AI agents and ERC-8004 / ERC-8183
- Node operation
- Infrastructure, indexers, oracles, account abstraction and compliance

Important current implementation notes from the official index:
- USDC is the native gas token on Arc.
- Arc targets the Osaka EVM baseline; Arc-specific EVM differences must be checked before writing production code.
- Arc documentation currently describes Testnet availability.
- Arc transactions have sub-second deterministic finality.
- App Kit provides Bridge, Swap, Send and Unified Balance capabilities.
- Contract addresses should always be checked against the official Arc contract-address reference rather than hardcoded from memory.

## Circle

Official developer documentation: https://developers.circle.com/

LLM-optimized documentation index: https://developers.circle.com/llms.txt

Key areas:
- USDC and EURC
- Circle Wallets: developer-controlled, user-controlled and modular
- CCTP V2
- Bridge Kit
- Gateway / Unified Balance / Nanopayments / x402
- Agent Stack
- Smart Contract Platform
- Paymaster
- Circle Payments Network
- Circle Mint
- StableFX
- xReserve
- APIs, SDKs and OpenAPI specifications

Important current implementation notes from the official index:
- Use the correct Circle wallet model for the application.
- Use CCTP V2 for cross-chain transfers unless an explicitly documented exception applies.
- Use Bridge Kit for frontend bridging and CCTP directly for backend transfers where appropriate.
- Gas Station and Paymaster are different products: Gas Station sponsors gas for Circle Wallet transactions, while Paymaster enables gas payment in USDC.
- Gateway supports unified USDC balances and gasless nanopayments using x402.
- USDC contract addresses must be looked up per chain from Circle's official reference.
- Prefer official SDKs over raw API calls where the SDK supports the required operation.
- API authentication and testnet/mainnet configuration must follow the current official documentation.
- Use webhooks for asynchronous operations where available.

## Source policy

Do not treat this file as a substitute for the live documentation. For production implementation, verify current details against the official Arc and Circle documentation above, especially:
- chain IDs and RPC URLs
- contract addresses
- token decimals
- supported chains
- SDK/API versions
- authentication requirements
- fee models
- transaction lifecycle and webhook events
- security and compliance requirements

Last source verification: 2026-09-06
