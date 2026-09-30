# Bench results

No results are committed yet. The first results come from the sample run.

## Format

One CSV per motor, at `test/<variant>/<serial>.csv`, where `<variant>` is one of `1604-6S`, `1604-4S`, `2306-6S`, `2306-4S`.

| Column | Unit | Meaning |
|---|---|---|
| `test` | text | `kv`, `no_load_current`, `thrust`, `temperature` or `balance` |
| `setpoint` | text | Throttle percent or supply voltage, as the test defines it |
| `value` | number | The measured value |
| `unit` | text | `rpm_per_v`, `A`, `g`, `C` or `g_mm` |
| `date` | ISO 8601 | Date of the measurement |
| `setup` | text | Bench setup id from the testing repository |

A summary per variant goes in `test/<variant>/README.md` and states the number of motors it covers. Nothing in the README variants table is replaced by a measurement until that summary exists.
