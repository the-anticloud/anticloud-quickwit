# Academic Use — QUICKWIT

**Project:** QUICKWIT  
**Category:** SEARCH_ENGINES  
**Upstream:** https://github.com/quickwit-oss/quickwit  
**Pinned commit:** `8f865ff98603db649a9f6338b9b40cf0bf3a64a3`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `dc720f20cf07a14d1a6d4a61dc90c2b0be80d8eaae638145bc2961978efafb8c`  
**Date:** October 2026

## Scope

QUICKWIT is available for academic research under the Apache 2.0 terms of the
Anticommons 0.1.0 dual licence. Citation details are in `23_HOW_TO_CITE`.

## What is available to researchers

- The full upstream source, pinned at `8f865ff98603db649a9f6338b9b40cf0bf3a64a3`
- The 16-check assurance register with per-check evidence and hashes
- The AIOSS ledger attesting the project artifacts
- Benchmark output in `BENCH.json`

## Reproducing the result

```
python tools/run_bench.py --out BENCH.json
```

Then recompute any row's SHA3-256 from `ISOLATED_LAB_RESULTS/04_Evidence/`.

## Contact

lois@0-1.gg · 0-1.gg
