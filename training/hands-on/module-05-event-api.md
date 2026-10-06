# Module 05 Lab | Event REST API

**Pair with:** PPT 05 slides 2–6 and Demo 05 | **Suggested time:** 3–5 hours within the 20-hour module

## Challenge

Extend the tiny Express API into an event resource API. Keep data in memory for this lab; persistence is Module 06.

## Tasks

1. Implement `GET /api/events` and `GET /api/events/:id`.
2. Implement `POST /api/events` with required title and date validation.
3. Implement `PUT` or `PATCH /api/events/:id` and `DELETE /api/events/:id`.
4. Add request logging and a final error handler. Do not send stack traces to clients.
5. Save or export an API-client collection, or document equivalent curl requests.

## Acceptance checks

- Create returns 201; invalid input returns 400; unknown IDs return 404.
- GET returns JSON with a consistent event shape; update and delete affect later reads.
- The server handles malformed/missing data without crashing.
- Tests include one success and one failure for each write operation.

**Extension:** add pagination with `limit` and `offset`. **Evidence:** API collection plus a short note that explains why memory storage is temporary.