# Module 08 Demo | Test Before Release

**Time:** 18 minutes | **Paired lab:** [Lab 08](../hands-on/module-08-test-release.md)

## Prepare

Use the module 05 API or instructor starter. In a terminal, prepare two requests: a valid event and a missing-title event. Use fake values only.

## Run it

1. Run the existing test command; read the assertion, not just the green output.
2. Send a valid create request and verify the status/body.
3. Send `{}` and confirm 400; demonstrate how this test catches a regression if validation is removed.
4. Show the production build command and identify which environment variable points to the API/database without revealing its value.
5. Walk the deploy checklist: build, configure, deploy, health check, smoke test, logs, rollback decision.

```text
Release gate: tests pass -> build succeeds -> config exists -> app responds -> key user flow works
```

**Expected:** a specific failing case is tested; students distinguish build success from feature verification. **Recovery:** use a pre-recorded deployment and ask learners to diagnose a deliberately missing environment variable from sanitized logs.