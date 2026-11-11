# Test Suites

This folder contains the unit and integration tests validating the robustness of the various GuardOS LLM modules.

## Files
- `test_normalizer.py` : Verification of homoglyph neutralization and form-based attacks (Soulymane).
- `test_anonymizer.py` : Validation of personal data masking rules (Djafarou).
- `test_fuzzing.py` : Testing the pipeline via the automatic mutation engine (Ephrem K.).

## Validation Protocol
The protocol relies on automated Semantic Fuzzing. Tests must be executed before any branch merge to validate the absence of software regression. The use of the `pytest` library is recommended.