# Module 02 Demo | Interactive Event Card

**Time:** 15 minutes | **Paired lab:** [Lab 02](../hands-on/module-02-event-page.md)

## Prepare

Open a blank HTML file in a browser or use the cohort's existing starter. Explain that this minimal example demonstrates structure and behavior; students will style it in the lab.

```html
<form id="signup">
  <label for="email">College email</label>
  <input id="email" type="email" required>
  <button type="submit">Register</button>
</form>
<p id="message" role="status"></p>
<script>
  document.querySelector('#signup').addEventListener('submit', (event) => {
    event.preventDefault();
    document.querySelector('#message').textContent =
      'Registration details accepted for review.';
  });
</script>
```

## Run it

1. Submit empty; browser validation blocks submission.
2. Enter an invalid email; observe native validation.
3. Enter a valid-looking email; show the status message and explain `preventDefault`.
4. Resize the browser and tab through controls. Ask what is missing before this could store a registration.

**Expected:** no page reload, visible feedback, a label connected to its field. **Recovery:** if a local file blocks scripts, use the browser's developer tools or the course starter; explain the expected interaction with a sketch.