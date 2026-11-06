# x402-defi-data — installable agent skill

A drop-in agent skill that gives a DeFi/trading agent **decision-tagged** market
data it can pay for inline with x402 (USDC on Base):

- **`/defi/yields`** — pool yields, each row tagged `SUSTAINABLE | DECAYING | OUTLIER | AVOID` + `risk_score`
- **`/crypto/funding`** — cross-venue perp funding with an **OI-weighted** carry/arb verdict
- **`/crypto/prices`** — spot prices with a `confidence` and an auditable provenance trajectory

Keyless free previews and a 3-calls/day full-output trial need no wallet; the
paid call settles per-request in USDC on Base with no API key or account.

## Install

```bash
npx skills add rezearcher/x402-defi-data
```

Then the skill (`SKILL.md`) is available to the agent. See [`SKILL.md`](./SKILL.md)
for the full instructions, live endpoints, and the `pip install greyridge-x402-tools`
path for Python agents.

Provided by Grey Ridge Signals Group. Data is a decision aid, not investment advice.
