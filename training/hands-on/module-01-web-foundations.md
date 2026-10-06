# Module 01 Lab | Map a Campus Request

**Pair with:** PPT 01 slides 2–6 and Demo 01 | **Suggested time:** 60–90 minutes within the 5-hour module

## Challenge

Design the logic for a fictional campus event registration and a small expense summary. Work in pairs; one person explains the steps while the other records them, then swap.

## Tasks

1. Draw the path for a student viewing an event and registering. Label frontend, backend, database, request, and response.
2. Write pseudocode for `register(remainingSeats)` with outcomes for available, full, and invalid capacity.
3. Write pseudocode that totals `[120, 80, 50]` and reports whether the spend is within a budget of `300`.
4. Make a three-row test table with input, expected result, and reason. Include a boundary case.

## Acceptance checks

- The diagram sends a request to a server and returns a response to the browser.
- The registration logic handles zero seats and rejects a negative seat count.
- The expense total is `250`; the budget decision is explained, not guessed.
- A partner can trace the pseudocode using the test table.

**Extension:** Add an event object with `title`, `capacity`, and `remainingSeats`. **Exit ticket:** Which rule belongs in the browser, and which must the server enforce too?