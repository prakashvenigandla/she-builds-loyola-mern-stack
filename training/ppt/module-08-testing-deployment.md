# Module 08 PPT | Testing, Deployment and DevOps

**README duration:** 10 h | **Build thread:** prove and publish the event app | **Evidence:** test run + documented deployment

## Slide sequence

1. **“Works on my machine” is not enough** (5 min) — What can differ in a deployed app? Build, environment, database, network.
2. **Test at useful boundaries** (15 min) — Unit, integration, functional/API checks; pick the smallest test that catches the risk.
3. **Test a contract and a failure** (20 min) — Request validation, status codes, UI feedback; test expected and rejected input.
4. **Build and configure** (15 min) — Development vs production, environment variables, build output, secrets hygiene.
5. **Deploy with a rollback mindset** (15 min) — Frontend, API, database, HTTPS, health check; verify each dependency.
6. **Automate the repeatable parts** (15 min) — CI pipeline: install, test, build; deploy only after checks pass.
7. **Verify the live experience** (10 min) — Run Demo 08, then Lab 08. Exit: what would you check first after a failed release?

## Instructor cues

Use an approved hosting account or prerecorded deployment for the live demo. Platforms and free tiers change; teach the checks and environment flow rather than a vendor-specific promise. Never expose `.env` values.