# Kronos Notary — Witness Ledger

A clean, append-only witness of sealed records.

Each commit advances the chain head. The chain proves *who said what, when, graded how* —
and that no record was altered after sealing, **even by the operator**.

We do not certify that any claim is TRUE. We certify that it was SAID, then, by them,
graded thus, and untouched since. Trust, not truth. The audit trail wins.

- `HEAD.json` — current chain head (seq + hash + seal time).
- `witness.log` — append-only line per seal: seq, record hash, head hash, time.

No personal data lives here — only hashes, sequence numbers, and seal metadata.
