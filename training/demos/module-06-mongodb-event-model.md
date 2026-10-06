# Module 06 Demo | Event Document and Query

**Time:** 18 minutes | **Paired lab:** [Lab 06](../hands-on/module-06-mongo-data.md)

## Prepare

Use a local MongoDB shell or a classroom sandbox with fictional records. Do not display credentials. If MongoDB is unavailable, run the same queries as a paper exercise.

```javascript
use campus_events
db.events.insertMany([
  { title: 'Robotics Meetup', category: 'technology', seats: 30, status: 'open' },
  { title: 'Design Jam', category: 'design', seats: 0, status: 'closed' }
])
db.events.find({ status: 'open' }).sort({ title: 1 })
db.events.updateOne({ title: 'Robotics Meetup' }, { $inc: { seats: -1 } })
db.events.aggregate([
  { $group: { _id: '$category', eventCount: { $sum: 1 } } }
])
```

## Run it

1. Insert and inspect one document; ask how it differs from a relational row.
2. Find open events, then decrement seats and verify the change.
3. Run the aggregation and explain each stage's input/output.
4. Ask what prevents `seats` from becoming negative; note that the query alone does not enforce every business rule.

**Expected:** find, update, and grouped counts work. **Recovery:** use screenshots or a printed result set if the classroom database is offline.