# Module 07 Demo | Trace a Registration Flow

**Time:** 20 minutes | **Paired lab:** [Lab 07](../hands-on/module-07-full-stack-flow.md)

## Prepare

Use the prior React/API/database exercises or a known-good instructor starter with fictional data. In the browser network panel, clear prior requests. No real account or secret is needed.

## Run it

1. Submit a valid-looking registration and trace: form state → `POST /api/events/:id/register` → server validation → database write → JSON response → UI update.
2. Submit missing required data; identify which layer rejects it and confirm the database remains unchanged.
3. Attempt organizer-only action as a student. Show the server's 403 even if the UI button is manually revealed.
4. Explain the password path: hash on registration, compare on login, issue short-lived signed token, verify identity and role on protected server route.
5. Point to configuration loaded from environment; never print its values.

**Expected:** students can name each boundary and see success/failure states. **Recovery:** if integration is broken, use an architecture sequence diagram and captured sanitized requests; do not live-debug unrelated setup for the whole class.