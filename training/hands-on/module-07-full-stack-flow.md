# Module 07 Lab | End-to-End Event Registration

**Pair with:** PPT 07 slides 2–6 and Demo 07 | **Suggested time:** 3–4 hours within the 15-hour module

## Challenge

Connect the event UI to the API and database. Add a simple attendee/organizer distinction to a prepared authentication starter. Do not build cryptography yourself.

## Tasks

1. Submit registration from React through a frontend service to the API; show loading, success, and failure states.
2. Persist and read back the registration. Validate input on the server even if the form also validates it.
3. Use the course-approved password hashing and token libraries in the starter. Keep secrets in environment configuration.
4. Protect one organizer operation on the server and test both an authorized and unauthorized request.
5. Document the request flow and how to run the app without sharing credentials.

## Acceptance checks

- The created record survives a server restart and appears in the UI.
- Invalid input is rejected server-side; the UI gives a useful response.
- Passwords are not stored in plaintext; unauthorized role gets 403 from the server.
- Secrets are absent from code, commits, screenshots, and logs.

**Extension:** add a validated image-upload boundary using the provided course utility. **Evidence:** sanitized request trace and short security checklist.