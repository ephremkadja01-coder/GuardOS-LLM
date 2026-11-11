# Safety Module - Governance and Compliance

**Lead** : Djafarou
**Role** : Governance and Compliance Expert (AI Safety).

## Module Objectives
Design the automatic anonymization module for information flows. Develop textual identification rules based on linguistic patterns to detect and mask sensitive personal data on the fly (emails, phone numbers adapted to Ivorian formats).

## Files
- `anonymizer.py` : Semantic masking, tokenization scripts, and toxicity verification for outgoing flows.

## Development Guidelines
The module operates after the normalization phase. Detection rules must rely on configurations from the `data/patterns_ci.json` file. Data modification must be irreversible to guarantee privacy protection.