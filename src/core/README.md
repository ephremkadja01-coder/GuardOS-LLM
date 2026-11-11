# Core Module - Red Team

**Lead** : Ephrem K.
**Role** : Offensive Security Analyst and Initial Architecture Designer.

## Module Objectives
Design the complete attack simulation framework. Develop a Fuzzing engine capable of automatically generating mutations of forbidden textual requests by altering their logico-semantic structure.

## Files
- `fuzzing_engine.py` : Core payload generation engine (Base64, Hexadecimal encoding, character substitution).
- `console.py` : Standalone visual interface for managing and launching offensive test campaigns.

## Development Guidelines
All functionalities must be tested against the server developed by the infrastructure team. The code must remain strictly isolated and must not import modules from the `defense/` or `safety/` folders.