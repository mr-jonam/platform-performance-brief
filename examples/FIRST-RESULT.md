# First result: an explicit transaction-rate assumption

This is a fictional arithmetic example, not a captured measurement or performance-test result.

## Inputs

| Input | Assumption |
| --- | --- |
| Active people in the window | 120 |
| Business transactions per person in that window | 3 |
| Window length | 15 minutes |

## Expected arithmetic

- Total business transactions: 120 × 3 = 360.
- Window length: 15 × 60 = 900 seconds.
- Average business transaction rate: 360 ÷ 900 = **0.4 per second**.

## Try and inspect

1. Follow the [local preview instructions](../README.md#start-here).
2. Open the Mini tool page and enter 120 people, 3 transactions and 15 minutes.
3. Compare its arithmetic with the calculation above.
4. Change only the window to 30 minutes: the assumed total remains 360 and the average becomes 0.2 per second.

A useful next question is: **Which evidence would justify these demand assumptions?** No peak factor, HTTP request count, concurrency, capacity or pass/fail threshold can be inferred from this arithmetic.

Read the [decision guide](../GUIDE.md) and [source status](../SOURCES.md) before discussing an actual workload.
