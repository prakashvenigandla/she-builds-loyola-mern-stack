# Module 07 PPT | Full Stack Integration and Authentication

**README duration:** 15 h | **Build thread:** register an attendee end to end | **Evidence:** React → API → MongoDB flow with protected action

## Slide sequence

1. **Trace one user journey** (5 min) — Form submit to response; name each layer and its responsibility.
2. **Connect without coupling** (15 min) — Frontend service calls API; JSON contract; loading, error, and success states.
3. **Complete CRUD across layers** (20 min) — Create a registration, read it back, update/cancel; inspect the network request.
4. **Authentication is identity** (20 min) — Register/login, hash passwords with a maintained library, issue/verify token; never store plaintext passwords.
5. **Authorization is permission** (15 min) — Student vs organizer; server checks role on every protected operation; UI hiding alone is not security.
6. **Config and safer files** (15 min) — Environment variables, validation, upload limits/type checks, safe error messages.
7. **Trace and test the flow** (10 min) — Run Demo 07, then Lab 07. Exit: where must the permission check happen?

## Instructor cues

Teach authentication as a flow and trust boundary, not a copy-paste token recipe. Use test accounts and fake data. Avoid inventing home-grown cryptography or showing real tokens in screenshots. Follow current framework/library guidance for token storage.