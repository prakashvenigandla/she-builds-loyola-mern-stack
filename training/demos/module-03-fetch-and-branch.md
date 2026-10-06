# Module 03 Demo | Fetch and Branch

**Time:** 18 minutes | **Paired lab:** [Lab 03](../hands-on/module-03-api-git.md)

## Prepare

Use a throwaway Git repository or the course starter. The API example uses JSONPlaceholder and is optional; prepare this local fallback: `[{"title":"Campus Robotics Meetup"}]`.

```js
async function loadEvents() {
  try {
    const response = await fetch('https://jsonplaceholder.typicode.com/posts/1');
    if (!response.ok) throw new Error(`HTTP ${response.status}`);
    const post = await response.json();
    console.log({ title: post.title, state: 'loaded' });
  } catch (error) {
    console.error('Could not load events:', error.message);
  }
}
loadEvents();
```

## Run it

1. Predict what `await` pauses and what it does not pause; run once.
2. Change the URL to an invalid path, inspect the response, then add/check `response.ok` before parsing.
3. Switch to the local fallback and identify the same data shape.
4. In Git, create `feature/event-feed`, make one small change, inspect `git diff`, commit it, and open a pull request if GitHub is available.

**Expected:** failure is handled and the diff is reviewable. **Recovery:** skip live GitHub if network/auth is unavailable; review the branch diff with a partner.