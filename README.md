# Never Repeat Yourself

Public, receipt-backed eval for Marvin. This repository defines the contract before claiming a result.

## Status

- Protocol: v0.1
- Latest run: not run
- Evidence status: scaffold only
- Public claim: none yet

Do not replace “not run” with a number. A synthetic fixture can prove the runner works; it cannot prove Marvin meets the standard.

## Standard

Leo should not have to explain the same context, preference, or correction twice.

## Test

Replay a correction corpus and check whether a later output violates a previously recorded rule.

## Reported metric

`repeated_correction_rate` — fraction of scored correction opportunities repeated after the rule was recorded.

## Claim boundary

A zero rate on a fixture does not prove memory across all Marvin sessions.

## Files

- `eval/index.json` — versioned contract and claim boundary.
- `validate.py` — dependency-free schema/contract check.

## Run

```sh
python3 validate.py
```

The first real report will include the fixture version, case count, model/prompt identifiers where applicable, pass/fail outcomes, failures, and an independent receipt.
