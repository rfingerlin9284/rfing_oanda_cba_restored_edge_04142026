# OANDA Freeze

This folder documents the restored April 14, 2026 OANDA high-edge baseline.

## Broker

- OANDA Practice FX

## What This Bot Does

- scans a focused forex basket
- routes entries by session and signal type
- sizes positions with the protected OANDA ladder behavior
- manages trades with OCO brackets, transcript-aware routing, and profit-harvest logic

## Protected Identity

- snapshot: `OANDA_GREEN_DAY_LOCK_CONTINUOUS_20260414`
- profile: `practice_green_day_lock_continuous`
- canonical runtime ID: `RBOTZILLA_OANDA_CLEAN__OANDA_GREEN_DAY_LOCK_CONTINUOUS_20260414__5446fd8bceea`

## Restore Notes

- source root: `OAD_FREEZE`
- this freeze follows the April 14 continuous baseline family, not the later April 20 hybrid relabels
- add your own OANDA credentials locally before running
