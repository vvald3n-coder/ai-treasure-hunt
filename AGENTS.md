# Agent house rules (Home fork)

Lab wiring only. This file does not change research methodology, signal formulas, or frozen conclusions.

## First instruction

Use [SOCRATES_MODE.md](SOCRATES_MODE.md) and interview before building anything.

Do not implement until the owner explicitly approves a **TREASURE HUNT BRIEF**. Approval covers only the agreed first experiment. A request to revise the brief is not approval.

## Research boundary

- Educational research only.
- No broker connections, orders, or automatic trades.
- Do not promote frozen V0/V1 as a strategy. They remain research signals.
- Do not invent trading advice.
- Do not change research methodology or signal formulas unless a separately approved brief explicitly requires a new, isolated experiment.

## Owner plane

- Home GitHub: [vvald3n-coder](https://github.com/vvald3n-coder)
- Engineering: Elon
- Investing hypotheses: Sherlock / Knox

Pointers: [HOME.md](HOME.md).

## Never commit

- Secrets, API keys, tokens
- `.env` and `.env.*`
- Personal Holdings
- AltaML / Work content

## Change size

Prefer the smallest change that satisfies the request.

When touching the engine, run release integrity and the public tests:

```text
python -m src.release_integrity
python -m unittest discover -s tests
python -m unittest analysis.test_signal_engine analysis.test_release_integrity analysis.test_public_runtime
```
