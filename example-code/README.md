Example Code for INF-3200, Assignment 2
=====================================================

This repository contains example code and test utilities for Assignment 2.

- `dummy_node.py` ---
    A skeleton node that superficially implements the required API, but has no
    actual functionality.

- `api_check.py` ---
    A set of superficial API tests to check that they respond with the correct formats.
    The dummy node passes these tests.

Example usage
--------------------------------------------------

From the bash command line:

```bash
# Start nodes in background
./dummy_node.py --port 50001 &
./dummy_node.py --port 50002 &

# Run API check
./api_check.py $HOSTNAME:50001 $HOSTNAME:5002

# Kill nodes
pkill -f dummy_node.py
```
