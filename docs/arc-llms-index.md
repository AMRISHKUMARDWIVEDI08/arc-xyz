# Arc Documentation Index

Source: https://docs.arc.io/llms.txt

Arc is an open Layer-1 blockchain purpose-built for programmable money. The official documentation describes USDC as the native gas token, sub-second deterministic finality, EVM compatibility, opt-in privacy, and integration with Circle's platform.

## Canonical documentation map

### Network
- Network overview: https://docs.arc.io/arc-chain.md
- System overview: https://docs.arc.io/arc/concepts/system-overview.md
- Stable fee design: https://docs.arc.io/arc/concepts/stable-fee-design.md
- Deterministic finality: https://docs.arc.io/arc/concepts/deterministic-finality.md
- Opt-in privacy: https://docs.arc.io/arc/concepts/opt-in-privacy.md
- Post-quantum security: https://docs.arc.io/arc/concepts/post-quantum-security.md

### Integration and references
- Connect to Arc: https://docs.arc.io/arc/references/connect-to-arc.md
- Contract addresses: https://docs.arc.io/arc/references/contract-addresses.md
- EVM differences: https://docs.arc.io/arc/references/evm-differences.md
- Gas and fees: https://docs.arc.io/arc/references/gas-and-fees.md

### Build and contracts
- Build overview: https://docs.arc.io/build.md
- Sample applications: https://docs.arc.io/arc/references/sample-applications.md
- Deploy on Arc: https://docs.arc.io/arc/tutorials/deploy-on-arc.md
- Deploy via Circle Contracts: https://docs.arc.io/arc/tutorials/deploy-contracts.md
- Interact with contracts: https://docs.arc.io/arc/tutorials/interact-with-contracts.md
- Monitor contract events: https://docs.arc.io/arc/tutorials/monitor-contract-events.md

### App Kit
- App Kit overview: https://docs.arc.io/app-kit.md
- Installation: https://docs.arc.io/app-kit/tutorials/installation.md
- Adapter setups: https://docs.arc.io/app-kit/tutorials/adapter-setups.md
- Bridge: https://docs.arc.io/app-kit/bridge.md
- Bridge quickstart: https://docs.arc.io/app-kit/quickstarts/bridge-tokens-across-blockchains.md
- Bridge fees: https://docs.arc.io/app-kit/concepts/bridge-fees.md
- Bridge error recovery: https://docs.arc.io/app-kit/references/bridge-error-recovery.md
- Swap: https://docs.arc.io/app-kit/swap.md
- Same-chain swap: https://docs.arc.io/app-kit/quickstarts/swap-tokens-same-chain.md
- Cross-chain swap: https://docs.arc.io/app-kit/quickstarts/swap-tokens-crosschain.md
- Swap fees: https://docs.arc.io/app-kit/concepts/swap-fees.md
- Send: https://docs.arc.io/app-kit/send.md
- Send quickstart: https://docs.arc.io/app-kit/quickstarts/send-tokens-same-chain.md
- Unified Balance: https://docs.arc.io/app-kit/unified-balance.md
- Unified Balance quickstart: https://docs.arc.io/app-kit/quickstarts/unified-balance-deposit-and-spend.md
- Unified Balance fees: https://docs.arc.io/app-kit/concepts/unified-balance-fees.md
- SDK reference: https://docs.arc.io/app-kit/references/sdk-reference.md
- Supported blockchains: https://docs.arc.io/app-kit/references/supported-blockchains.md

### AI and agents
- Arc MCP Server: https://docs.arc.io/ai/mcp.md
- Agentic economy: https://docs.arc.io/build/agentic-economy.md
- Register an AI agent: https://docs.arc.io/arc/tutorials/register-your-first-ai-agent.md
- ERC-8183 job: https://docs.arc.io/arc/tutorials/create-your-first-erc-8183-job.md

### Infrastructure
- Integrate overview: https://docs.arc.io/integrate.md
- Running a node: https://docs.arc.io/arc/concepts/running-a-node.md
- Run an Arc node: https://docs.arc.io/arc/tutorials/run-an-arc-node.md
- Node providers: https://docs.arc.io/arc/tools/node-providers.md
- Data indexers: https://docs.arc.io/arc/tools/data-indexers.md
- Oracles: https://docs.arc.io/arc/tools/oracles.md
- Account abstraction: https://docs.arc.io/arc/tools/account-abstraction.md
- Compliance vendors: https://docs.arc.io/arc/tools/compliance-vendors.md

## Critical Arc-specific implementation notes

The official Arc index currently highlights these differences from standard Ethereum/EVM assumptions:

- USDC uses 18 decimals natively on Arc.
- A system emitter at `0xffffFFFfFFffffffffffffffFfFFFfffFFFfFFfE` logs USDC Transfer events.
- The mempool enforces a 20 Gwei `maxFeePerGas` floor.
- Blocklist reverts consume gas without a receipt.
- Sending to `address(0)` reverts rather than succeeding.

Treat the official EVM Differences page as canonical because these details can affect balances, event indexing, gas estimation, and transfer logic.

## Official tools

- Arc Testnet explorer: https://testnet.arcscan.app
- Circle faucet: https://faucet.circle.com
- Arc docs: https://docs.arc.io/
