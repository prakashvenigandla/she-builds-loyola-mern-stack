# Module 06 Lab | Persist and Query Events

**Pair with:** PPT 06 slides 2–6 and Demo 06 | **Suggested time:** 2–3 hours within the 10-hour module

## Challenge

Design a MongoDB collection for fictional campus events and answer practical questions from the event team. Use local MongoDB or a provided sandbox.

## Tasks

1. Propose fields and types for title, category, start time, venue, seats, and status. Mark required fields and one validation rule.
2. Insert at least five fictional events across two categories.
3. Query open events sorted by start time; update seats/status; handle an unknown event.
4. Aggregate event counts by category. Add an index only for a query you can name.
5. If using Mongoose, define a schema/model and keep database configuration outside source control.

## Acceptance checks

- A peer can explain the document shape and why it fits the lab's queries.
- Queries return the expected subset and sorting; update is verified with a follow-up read.
- Aggregation groups records correctly; invalid records are rejected by schema or explained.
- No credential or real personal data is committed.

**Extension:** add pagination or compare query plans before/after an index. **Evidence:** schema sketch, saved queries, and one example output.