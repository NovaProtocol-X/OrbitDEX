OrbitDEX

High-efficiency Concentrated Liquidity AMM on the Stellar Network

---

## Overview

OrbitDEX is a high-efficiency Automated Market Maker (AMM) deployed on the Stellar Network. It implements Concentrated Liquidity logic within Soroban smart contracts, giving Liquidity Providers (LPs) precise control over capital deployment by enabling them to allocate liquidity within custom price ranges.

This design maximizes capital efficiency and minimizes slippage for traders, all through the Stellar Asset Contract (SAC) interface.

---

## Features

- **Concentrated Liquidity** — LPs choose custom price ranges for targeted capital deployment
- **Capital Efficiency** — More liquidity where it's needed, less waste at unused price points
- **Low Slippage** — Optimized AMM curve for a better trader experience
- **SAC Integration** — Built natively on Stellar's Asset Contract interface
- **Soroban-Powered** — Fully on-chain logic via Soroban smart contracts

---

## Getting Started

### Prerequisites

- [Rust](https://www.rust-lang.org/tools/install)
- [Soroban CLI](https://soroban.stellar.org/docs/getting-started/setup)
- [Node.js](https://nodejs.org/) (for the web interface)
- `make`

### Installation

**1. Build the smart contracts:**
```bash
make build
```

**2. Run the test suite:**
```bash
cargo test
```

**3. Deploy to Testnet:**
```bash
make deploy
```

**4. Launch the web interface:**
```bash
cd web && npm run dev
```

---

## Project Structure

```
orbitdex/
├── contracts/          # Soroban smart contract source files
├── web/                # Frontend interface
├── tests/              # Integration and unit tests
├── Makefile            # Build and deploy commands
└── CONTRIBUTING.md     # Contribution guidelines
```

---

## Contributing

OrbitDEX follows the **Wave Program** sprint cycle for issue management. Before submitting a PR, review the currently scoped issues and open tasks in [CONTRIBUTING.md](./CONTRIBUTING.md).

---

## License

This project is licensed under the [MIT License](./LICENSE).
