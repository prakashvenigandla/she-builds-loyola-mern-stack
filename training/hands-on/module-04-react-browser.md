# Module 04 Lab | Searchable Event Browser

**Pair with:** PPT 04 slides 2–6 and Demo 04 | **Suggested time:** 4–6 hours within the 25-hour module

## Challenge

Build a responsive event browser using the course React starter. Begin with local fictional data; API integration and routing can be added as separate checkpoints.

## Tasks

1. Make reusable `EventCard` and `EventList` components. Pass event data with props.
2. Add controlled search and a no-results state. Avoid storing values that can be derived from existing state.
3. Add a registration form with field labels, validation feedback, and a success state.
4. Add an event-detail route if the class has covered React Router. Keep route setup separate from list rendering.
5. Add loading/error states only when connecting to an API; do not fake a successful response.

## Acceptance checks

- Search updates as the user types and a missing result is handled.
- Repeated cards are rendered from data with stable keys.
- Components have a clear purpose; form state is controlled and feedback is readable.
- Layout works at a narrow width and controls have labels.

**Extension:** add a category filter or event-detail route. **Evidence:** working local page and a 60-second explanation of one state decision.