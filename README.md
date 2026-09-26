# Dental Policy Monitor

A Claude skill that produces a one-page weekly brief on CMS, Medicare, Congress and state Medicaid dental policy changes. It links every item to a primary source and flags items relevant to Overjet (AI claims review, imaging, interoperability, prior auth, FWA, quality measures).

This skill is the **Delegate** part of the Lead / Team / Delegate framework: Claude gathers and summarizes, and Natalia reviews before anything is used.

## Files
- `SKILL.md`: the skill instructions (steps, sources, format, rules)
- `examples/`: a sample brief from the Sept 26, 2026 test run

## How it runs
- **On demand:** ask Claude for "the policy brief" or "what changed in dental policy since <date>".
- **Weekly:** a Claude scheduled task runs it every Monday at 7:45 am ET and covers the previous Monday through Sunday.

## Install in Claude
Upload the `dental-policy-monitor` folder as a skill in Claude (Settings → Capabilities → Skills), or ask Claude to propose it from `SKILL.md`.

Author: Natalia Chalmers, DDS, PhD
