# Educators — QUICKWIT

**Project:** QUICKWIT  
**Category:** SEARCH_ENGINES  
**Upstream:** https://github.com/quickwit-oss/quickwit  
**Pinned commit:** `8f865ff98603db649a9f6338b9b40cf0bf3a64a3`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `dc720f20cf07a14d1a6d4a61dc90c2b0be80d8eaae638145bc2961978efafb8c`  
**Date:** October 2026

## Teaching with QUICKWIT

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `dc720f20cf07a14d1a6d4a61dc90c2b0be80d8eaae638145bc2961978efafb8c` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
