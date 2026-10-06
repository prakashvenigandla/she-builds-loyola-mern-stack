# Module 03 Lab | Event Feed and Reviewed Change

**Pair with:** PPT 03 slides 2–6 and Demo 03 | **Suggested time:** 3–4 hours within the 15-hour module

## Challenge

Load event-shaped data into the page, show a useful state while loading, and submit the change for review. Use a no-key public API only if available; otherwise use the supplied local JSON fixture.

## Tasks

1. Create a feature branch before editing. Keep the main branch unchanged.
2. Write an `async` function that loads data, checks the response, parses JSON, and handles failure.
3. Render at least three event rows with a loading message, empty state, and error state.
4. Commit a focused change. Include a pull request description with purpose, behavior tested, and known limitation.

## Acceptance checks

- Network/API failure is visible and does not crash the whole page.
- Loading and empty states differ from a successful list.
- Data is rendered from the returned object, not copied into each DOM row by hand.
- The branch diff is focused; a peer can explain what the commit changes.

**Extension:** add a filter by event title. **Evidence:** pull request link or saved diff, plus one failure case and its observed message.