# PyKV

A Redis-compatible in-memory key-value store, built from scratch in Python.

Works with the real `redis-cli` and `redis-py` — no client changes needed.

## Status
🚧 Work in progress

- [ ] Phase 1: TCP server, RESP protocol, basic commands
- [ ] Phase 2: TTL, expiration, LRU eviction
- [ ] Phase 3: AOF persistence, fsync policy benchmarks
- [ ] Phase 4: Performance optimization, uvloop comparison

## Why
Building this from scratch to explore epoll-based event loops,
TCP stream framing, and the durability/throughput tradeoff in
write-ahead logging.

## Quick start
```bash
python -m pykv --port 6380
redis-cli -p 6380 ping
```

## Benchmarks
_TBD_

## Design decisions
_TBD_
