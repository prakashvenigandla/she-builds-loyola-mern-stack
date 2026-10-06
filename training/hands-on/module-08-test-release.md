# Module 08 Lab | Test and Release Checklist

**Pair with:** PPT 08 slides 2–6 and Demo 08 | **Suggested time:** 2–3 hours within the 10-hour module

## Challenge

Add confidence checks to the team's event application, then prepare or perform a deployment using an approved course environment.

## Tasks

1. Write one API test for valid creation and one for invalid input; include status and response assertions.
2. Run the frontend production build and record the result. Fix only errors in the team's code.
3. List required environment variable names (never their values) and confirm the deployed services have them configured.
4. Deploy or follow the instructor simulation. Smoke-test event listing and registration in the production URL.
5. Record one sanitized error/log observation and a rollback or recovery action.

## Acceptance checks

- Tests fail if the key validation/status behavior regresses.
- Production build succeeds; no secret is in the repository or output.
- Live/simulated smoke test covers one successful and one rejected workflow.
- Deployment record includes URL, date, test result, and known limitation.

**Extension:** add a CI workflow that runs tests and build on a pull request. **Evidence:** test output and a completed release checklist.