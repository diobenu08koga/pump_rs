# pump-rs

A collection of pump.fun related utilities, centered around sniping new launches.

## Journey

This project evolved from listening on pump.fun stream from the frontend API (avg ~5-10 slots), to using pumpportal API for data (avg 1-5 slots), to using a custom on-chain program with deadline control and deserializing raw shreds from Jito Shredstream (avg 0.5 slots over 100+ entries).

## Features

The profits of this bot stem from being faster than other snipers and dumping on them. There are some sniper bots that hold a token and sell later if it turns out to be a good one, but currently most launches fail to reach the bonding curve.

Strategy for the seller service is to wait for the confirmation of transaction to arrive through the PubSub client and sell straight-away.

## Usage

```bash
Usage: pump-rs <COMMAND>

Commands:
  wallets
  look-for-geyser
  bundle-status
  subscribe-tip
  get-tx
  slot-created
  subscribe-pump
  test-slot-program
  slot-subscribe
  is-on-curve
  subscribe
  seller
  bench-pump
  bench-portal
  snipe-portal
  snipe-pump
  analyze
  sanity
  close-token-accounts
  pump-service
  bump-pump
  sweep-pump
  buy-pump-token
  help
```

## Disclaimer

This is provided as-is and runs on mainnet. It can cause losses and is unlikely to be profitable for most users.

## Project Structure

- `src/` - Source code
- `runs/` - Run data and logs
- `docker-compose.yaml` - Docker configuration
- `Cargo.toml` - Rust dependencies
- `README.md` - Documentation
