# Capital Loss And Freeze Notes

This freeze preserves the April 14 baseline first.

That means the original high-edge posture is protected cleanly before any capital-protection add-on is described as an upgrade.

## Why

- the operator wanted the April 14 high-edge behavior protected forever
- later changes may help, but they are still changes
- a loss helper should not be silently baked into the baseline unless receipts prove it belongs there

## OANDA Note

The restored OANDA baseline here is the protected April 14 continuous posture.

A separate dev-only giveback guard was replay-tested after the restore work:

- arm after about `+$350`
- lock after about `-$175` from session peak

That candidate helped in replay, but it is not merged into this freeze reference.

## Coinbase Note

The Coinbase side is also frozen to its April 14 baseline family. This repo keeps the focused session-aware behavior anchored and does not pretend later live variants are automatically equivalent.

## Practical Meaning

- use this freeze for the protected April 14 baseline
- test later capital-loss add-ons separately before promotion
