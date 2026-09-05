# Arc XYZ — Arc + Circle Developer Knowledge Base

This repository is the reference hub for building with **Arc** and **Circle**.

## Official documentation

- Arc Docs: https://docs.arc.io/
- Arc documentation index: https://docs.arc.io/llms.txt
- Circle Developer Docs: https://developers.circle.com/
- Circle documentation index: https://developers.circle.com/llms.txt

## What is stored here

- Official documentation indexes captured from Arc and Circle.
- A structured map of the major Arc and Circle developer areas.
- Important implementation rules and Arc-specific EVM differences.
- Links to official canonical pages so future work can verify current details.

## Arc core rules to remember

1. USDC is Arc's native gas token.
2. Arc is EVM compatible but has Arc-specific runtime differences; read the EVM Differences reference before writing code involving USDC, transfers, gas, or transaction history.
3. Arc provides sub-second deterministic finality; applications generally do not need Ethereum-style multi-confirmation waiting.
4. Arc currently exposes Testnet documentation and a Circle faucet.
5. Always verify current contract addresses from the official Arc contract-address reference rather than hardcoding stale values.
6. Arc App Kit provides Bridge, Swap, Send and Unified Balance workflows.

## Circle core rules to remember

1. Select the correct Circle wallet model: Developer-Controlled, User-Controlled, or Modular.
2. Use CCTP V2 for cross-chain USDC/EURC transfers unless a documented chain-specific exception requires V1.
3. Use Bridge Kit/App Kit for frontend bridging; use CCTP directly when backend control is appropriate.
4. Gas Station and Paymaster solve different gas-payment problems; choose based on the wallet architecture.
5. Gateway supports unified USDC balances and nanopayments/x402 use cases.
6. Look up current USDC contract addresses per chain from Circle's official address reference.
7. Prefer official SDKs where available instead of manually rebuilding API behavior.
8. Use webhooks for asynchronous operation state changes when the product supports them.
9. Never store API keys, entity secrets, private keys, seed phrases, or other credentials in this repository.

## Repository policy

This repository is a **knowledge/reference repository**, not a mirror of the Arc or Circle websites. Official links are retained so the source can be checked whenever documentation changes.

Last documentation index capture: 2026-09-06.
