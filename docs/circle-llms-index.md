# Circle Developer Documentation Index

Source: https://developers.circle.com/llms.txt

Circle's developer platform provides infrastructure for digital dollars, including USDC/EURC, wallets, cross-chain transfers, payments, smart contracts, AI-agent financial infrastructure, and APIs.

## Core developer guidance

- Read the product overview before quickstarts.
- Choose the correct wallet model: Developer-Controlled, User-Controlled, or Modular.
- Prefer CCTP V2 for cross-chain transfers; V1 is legacy except for documented chain-specific requirements.
- Use Bridge Kit for frontend bridging and direct CCTP where backend-level control is appropriate.
- Gas Station sponsors gas for Circle Wallet transactions; Paymaster allows users to pay gas in USDC.
- Gateway supports unified USDC balances and nanopayments using x402.
- Never hardcode USDC addresses; use Circle's official address reference for the target chain.
- Prefer official SDKs when available.
- Circle APIs require authentication; keep keys and secrets outside source control.
- Use webhooks for asynchronous state changes when supported.

## USDC / EURC

- USDC overview: https://developers.circle.com/stablecoins/what-is-usdc.md
- EURC overview: https://developers.circle.com/stablecoins/what-is-eurc.md
- USDC contract addresses: https://developers.circle.com/stablecoins/usdc-contract-addresses.md
- EURC contract addresses: https://developers.circle.com/stablecoins/eurc-contract-addresses.md
- EVM USDC transfer quickstart: https://developers.circle.com/stablecoins/quickstarts/transfer-usdc-evm.md

## Wallets

- Wallet overview: https://developers.circle.com/wallets.md
- Wallet model selection: https://developers.circle.com/wallets/infrastructure-models.md
- Developer-Controlled Wallets: https://developers.circle.com/wallets/dev-controlled.md
- User-Controlled Wallets: https://developers.circle.com/wallets/user-controlled.md
- Modular Wallets: https://developers.circle.com/wallets/modular.md
- Account types: https://developers.circle.com/wallets/account-types.md
- Gas Station: https://developers.circle.com/wallets/gas-station.md
- Supported blockchains: https://developers.circle.com/wallets/supported-blockchains.md

## CCTP

- CCTP overview: https://developers.circle.com/cctp.md
- Supported chains/domains: https://developers.circle.com/cctp/concepts/supported-chains-and-domains.md
- Fees: https://developers.circle.com/cctp/concepts/fees.md
- Fast Transfer allowance: https://developers.circle.com/cctp/concepts/fast-transfer-allowance.md
- Forwarding service: https://developers.circle.com/cctp/concepts/forwarding-service.md
- Upfront fees: https://developers.circle.com/cctp/concepts/upfront-fees.md
- Ethereum → Arc: https://developers.circle.com/cctp/quickstarts/transfer-usdc-ethereum-to-arc.md
- Solana → Arc: https://developers.circle.com/cctp/quickstarts/transfer-usdc-solana-to-arc.md
- V1 → V2 migration: https://developers.circle.com/cctp/migration-from-v1-to-v2.md
- CCTP contracts: https://developers.circle.com/cctp/references/contract-addresses.md
- Technical guide: https://developers.circle.com/cctp/references/technical-guide.md

## Bridge Kit / App Kit

- Bridge Kit: https://developers.circle.com/bridge-kit.md
- Arc App Kit: https://docs.arc.io/app-kit.md

## Gateway / x402

- Gateway overview: https://developers.circle.com/gateway.md
- Unified Balance: https://developers.circle.com/gateway/quickstarts/unified-balance-evm.md
- Nanopayments: https://developers.circle.com/gateway/nanopayments.md
- x402: https://developers.circle.com/gateway/nanopayments/concepts/x402.md
- Gateway supported blockchains: https://developers.circle.com/gateway/references/supported-blockchains.md
- Gateway fees: https://developers.circle.com/gateway/references/fees.md

## Agent Stack

- Agent Stack overview: https://developers.circle.com/agent-stack.md
- Circle CLI: https://developers.circle.com/agent-stack/circle-cli.md
- Agent wallets: https://developers.circle.com/agent-stack/agent-wallets.md
- Agent nanopayments: https://developers.circle.com/agent-stack/agent-nanopayments.md
- Agent marketplace: https://developers.circle.com/agent-stack/agent-marketplace.md
- Discovery API: https://developers.circle.com/agent-stack/agent-marketplace/discovery-api.md

## Smart Contracts

- Contracts overview: https://developers.circle.com/contracts.md
- Deploy bytecode: https://developers.circle.com/contracts/scp-deploy-smart-contract.md
- Deploy templates: https://developers.circle.com/contracts/deploy-smart-contract-template.md
- Interact: https://developers.circle.com/contracts/scp-interact-smart-contract.md
- Templates: https://developers.circle.com/contracts/scp-templates-overview.md
- Event monitoring: https://developers.circle.com/contracts/scp-event-monitoring.md

## Paymaster

- Overview: https://developers.circle.com/paymaster.md
- Pay gas in USDC: https://developers.circle.com/paymaster/pay-gas-fees-usdc.md
- Addresses/events: https://developers.circle.com/paymaster/addresses-and-events.md

## Circle Payments Network

- CPN overview: https://developers.circle.com/cpn.md
- Payments: https://developers.circle.com/cpn/concepts/payments/payments.md
- Quotes: https://developers.circle.com/cpn/concepts/quotes.md
- Supported blockchains: https://developers.circle.com/cpn/references/blockchains/supported-blockchains.md
- Supported countries: https://developers.circle.com/cpn/references/compliance/supported-countries.md

## Circle Mint / StableFX / xReserve

- Circle Mint: https://developers.circle.com/circle-mint/introducing-circle-mint.md
- StableFX: https://developers.circle.com/stablefx.md
- xReserve: https://developers.circle.com/xreserve.md

## Developer resources

- API reference: https://developers.circle.com/api-reference.md
- API keys: https://developers.circle.com/api-reference/keys.md
- SDKs: https://developers.circle.com/sdks.md
- Sample projects: https://developers.circle.com/sample-projects.md
- Testnet faucets: https://developers.circle.com/wallets/developer-console-faucet.md
- OpenAPI specifications: https://developers.circle.com/openapi/

## AI-agent resources

- Circle MCP: https://developers.circle.com/ai/mcp.md
- Circle Skills: https://github.com/circlefin/skills
