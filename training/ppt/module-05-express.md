# Module 05 PPT | Node.js and Express APIs

**README duration:** 20 h | **Build thread:** event REST API | **Evidence:** CRUD endpoints tested with meaningful status codes

## Slide sequence

1. **Why move a rule to the server?** (5 min) — A browser can be changed; capacity and data rules need server enforcement.
2. **Node and the request lifecycle** (15 min) — Runtime, packages, Express route, request → middleware → handler → response.
3. **Design resource URLs** (20 min) — `/api/events`, `GET`, `POST`, `PATCH`, `DELETE`; choose status codes and JSON shape.
4. **CRUD without mystery** (20 min) — Read a tiny in-memory collection first; explain that it resets when the server restarts.
5. **Middleware and validation** (20 min) — Request logging, JSON parser, input checks, central error handling; order matters.
6. **Test the contract** (15 min) — Postman/curl: happy path, missing fields, unknown ID, unsupported method.
7. **Build and inspect** (10 min) — Run Demo 05, then Lab 05. Exit: why should invalid input not return 200?

## Instructor cues

Start in-memory to teach HTTP without database setup; label persistence as the next module. Keep authentication as a later module. Never expose stack traces or environment values in responses.