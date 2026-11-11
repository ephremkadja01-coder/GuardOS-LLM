# Defense Module - Blue Team

**Lead** : Soulymane
**Role** : Defensive Security Engineer.

## Module Objectives
Develop the detection and normalization algorithm for form-based attacks. Code filters capable of cleaning and reconstructing words altered by special characters, Unicode homoglyphs, or hidden spaces.

## Files
- `normalizer.py` : Low-level string processing functions, sanitization, and securing against syntactic bypasses.

## Development Guidelines
The module must be highly performant. The use of data dictionaries (located in the `data/` folder) is required for detecting fraudulent characters. Functions should be pure to facilitate unit testing.