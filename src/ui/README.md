# User Interface Module

**Lead** : Masso and Ephrem K.
**Role** : Supervision and Audit Interface.

## Module Objectives
Develop the test interface powered by a lightweight application server. Provide an audit space to simulate messages and immediately visualize security verdicts, as well as a dashboard presenting activity graphs.

## Files
- `dashboard.py` : Streamlit application for dynamic rendering of security statuses, syntax highlighting of modified text segments, and display of latency metrics.

## Development Guidelines
The interface must communicate exclusively via asynchronous HTTP requests with Masso's server. No business or security logic should be implemented directly within this interface.