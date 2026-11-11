# Dictionaries and Static Data

This folder contains the flat configuration files and dictionaries used by the application's analysis engines.

## Files
- `homoglyphes.json` : Mapping table for visually similar Unicode characters (used by Soulymane's defense module).
- `patterns_ci.json` : Regular expressions and identification structures for West African personal data (used by Djafarou's compliance module).

## Maintenance
These files are dynamically loaded at application startup or during requests. They must be kept up to date to ensure the effectiveness of security filters.