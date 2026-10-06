# Module 05 Demo | Tiny Event API

**Time:** 20 minutes | **Paired lab:** [Lab 05](../hands-on/module-05-event-api.md)

## Prepare

In a disposable folder run `npm init -y` and `npm install express`; save this as `server.js`. This uses in-memory data for teaching, not production.

```js
const express = require('express');
const app = express();
app.use(express.json());
const events = [{ id: 1, title: 'Robotics Meetup' }];

app.get('/api/events', (_req, res) => res.json(events));
app.post('/api/events', (req, res) => {
  if (!req.body.title?.trim()) return res.status(400).json({ error: 'title is required' });
  const event = { id: Date.now(), title: req.body.title.trim() };
  events.push(event);
  res.status(201).json(event);
});
app.listen(3000, () => console.log('API listening on port 3000'));
```

## Run it

1. Start with `node server.js`; GET `/api/events` in a browser or API client.
2. POST `{}` and inspect the 400 response.
3. POST `{"title":"Design Jam"}` with JSON content type; inspect 201 and the returned record.
4. Restart the server; point out why the new record disappears.

**Expected:** JSON list, useful 400, created record with 201. **Recovery:** if the port is occupied, use another port and update the URL; if setup fails, trace the routes on the board.