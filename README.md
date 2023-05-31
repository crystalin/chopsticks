# Chopsticks

Create parallel reality of your Substrate network.

## Run

Make sure you have setup Rust environment.

- Install deps
  - `yarn`
- Build wasm
  - `yarn build-wasm`
- Run nodejs runner
  - `yarn start run-block --endpoint=wss://acala-rpc-2.aca-api.network/ws`

Connect to the rpc via localhost:8000 and you may be able to submit transaction and it will be executed in parallel reality.

NOTE: subscriptions are not yet implemented so you will need to refresh to see new blocks.

NOTE2: this currently takes ~half minute to produce a new block.

Next step 3:

- Implements subscription
- Disable signature verification
- API for arbitrary storage override
- Compile the rust part into wasm
