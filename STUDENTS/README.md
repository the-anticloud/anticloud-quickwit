# Students — QUICKWIT

**Project:** QUICKWIT  
**Category:** SEARCH_ENGINES  
**Upstream:** https://github.com/quickwit-oss/quickwit  
**Pinned commit:** `8f865ff98603db649a9f6338b9b40cf0bf3a64a3`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `dc720f20cf07a14d1a6d4a61dc90c2b0be80d8eaae638145bc2961978efafb8c`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `8f865ff98603db649a9f6338b9b40cf0bf3a64a3`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `dc720f20cf07a14d1a6d4a61dc90c2b0be80d8eaae638145bc2961978efafb8c`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
