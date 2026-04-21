# April 14 Restored Edge Freeze

This public repo is the freeze index for the restored April 14, 2026 high-edge baseline family across both bots.

- `oanda/` = the protected OANDA April 14 continuous baseline
- `coinbase/` = the protected Coinbase Advanced April 14 freeze baseline

This is a `baseline clone`, not a new experiment.

## What Each Bot Does

- `OANDA`: trades foreign exchange through the OANDA practice FX broker. The protected target here is the April 14 continuous posture that pushed the practice account into the `7k+` range before later giveback.
- `Coinbase Advanced`: trades crypto through Coinbase Advanced Trade. The protected target here is the April 14 focused live Coinbase freeze that uses a small curated crypto universe and session-aware strategy routing.

## Frozen Identities

- `OANDA`
  - snapshot: `OANDA_GREEN_DAY_LOCK_CONTINUOUS_20260414`
  - profile: `practice_green_day_lock_continuous`
  - runtime ID: `RBOTZILLA_OANDA_CLEAN__OANDA_GREEN_DAY_LOCK_CONTINUOUS_20260414__5446fd8bceea`
  - source root: `OAD_FREEZE`
- `Coinbase Advanced`
  - snapshot: `COINBASE_CLEAN_24H_COVERAGE_20260414`
  - profile: `live_focus4_session_truth_sol_overnight`
  - source root: `CBA_FREEZE`

## Included Here

- freeze manifest
- per-bot receipts
- plain-English restore guides
- capital-loss note about what was frozen versus what stayed experimental

## Not Included Here

- live broker credentials and private keys
- backup clutter and legacy exports
- the full private local runtime payload

## Restore Starting Point

Start with:

- `oanda/README.md`
- `coinbase/README.md`
- `docs/CAPITAL_LOSS_AND_FREEZE_NOTES.md`
- `FREEZE_MANIFEST.json`

## Version Control

- freeze name: `dual-bot-restored-edge-20260421`

If a later version proves better, it should become a new frozen version with a new identity. It should not silently replace this April 14 restore baseline.
