# Testnet deployment

1. Generate and fund a deployer identity.
2. Build the contract with `stellar contract build`.
3. Deploy the Wasm using Stellar CLI.
4. Put the returned contract ID in frontend and backend environment files.
5. Build both TypeScript services and run smoke tests.

```bash
stellar keys generate blink-deployer --network testnet --fund
stellar contract deploy \
  --wasm target/wasm32v1-none/release/link_registry.wasm \
  --source blink-deployer \
  --network testnet
```

Mainnet requires a dedicated configuration review, RPC provider, monitoring, abuse response process, and contract audit.

