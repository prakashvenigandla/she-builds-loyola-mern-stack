# Module 04 Demo | React Event Browser

**Time:** 20 minutes | **Paired lab:** [Lab 04](../hands-on/module-04-react-browser.md)

## Prepare

Use the cohort's React/Vite starter. Add one local event object; no API key or backend is needed for this demo.

```jsx
function EventCard({ event }) {
  return <article><h2>{event.title}</h2><p>{event.venue}</p></article>;
}

function EventList() {
  const [query, setQuery] = React.useState('');
  const events = [{ id: 1, title: 'Robotics Meetup', venue: 'Lab 2' }];
  const visibleEvents = events.filter((event) =>
    event.title.toLowerCase().includes(query.toLowerCase())
  );
  return <main>
    <label>Search events <input value={query}
      onChange={(event) => setQuery(event.target.value)} /></label>
    {visibleEvents.length
      ? visibleEvents.map((event) => <EventCard key={event.id} event={event} />)
      : <p>No matching events.</p>}
  </main>;
}
```

## Run it

1. Render one card; add a second object and explain why `key` is needed.
2. Type a partial title; point to state, event handler, and derived filtered data.
3. Search for a missing title; inspect the empty state.
4. Change a card's venue and verify both cards still use the same component.

**Expected:** reusable card, controlled search, stable keys. **Recovery:** if the starter uses a different import setup, adapt only the `React` import; the component behavior is framework-version independent.