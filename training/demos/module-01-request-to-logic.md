# Module 01 Demo | Request to Logic

**Time:** 12 minutes | **Paired lab:** [Lab 01](../hands-on/module-01-web-foundations.md)

## Prepare

No installs. Put the words **browser**, **server**, and **database** on the board. Pick a fictional event with a capacity of 3.

## Run it

1. Ask a student acting as browser to request registration for `event-42`.
2. Server asks the database for remaining seats. Database replies `1`; server returns “Registration confirmed”. Repeat with `0`; return “Event full”.
3. Translate the decision together:

```text
FUNCTION register(remainingSeats)
  IF remainingSeats > 0
    RETURN "confirmed"
  ELSE
    RETURN "event full"
```

4. Show why a function helps: call it with `1`, `0`, and `-1`; ask what rule should reject the negative value.

## Check and recover

Ask students to identify who stores the seat count and who decides the response. If the role-play gets stuck, model one request end-to-end, then replay it with a changed input. Keep the scenario fictional; no student names or real registrations.