# Module 06 PPT | MongoDB and Data Modeling

**README duration:** 10 h | **Build thread:** persist events safely | **Evidence:** event schema, CRUD queries, and one useful report

## Slide sequence

1. **Data outlives a process** (5 min) — Revisit Module 05 restart; where should an event record live?
2. **Documents fit related facts** (15 min) — Database, collection, document, BSON; show one event JSON document.
3. **Model for questions** (20 min) — Identify required fields, ownership, and likely queries before choosing embedded/referenced data.
4. **CRUD and query filters** (20 min) — Insert, find, update, delete, sort, limit; use fictional dates and event status.
5. **Mongoose adds an application contract** (15 min) — Schema, model, validation, connection string in environment; distinguish ODM from database.
6. **Indexes and aggregation** (15 min) — Index fields used for search; group counts by category; discuss the cost of an unnecessary index.
7. **Design, query, explain** (10 min) — Run Demo 06, then Lab 06. Exit: which query should the chosen index accelerate?

## Instructor cues

Use local MongoDB or a prepared sandbox; never put a connection string in Git or slides. Keep one-to-many relationships concrete. Explain that aggregation is a pipeline of transformations, not magic reporting.