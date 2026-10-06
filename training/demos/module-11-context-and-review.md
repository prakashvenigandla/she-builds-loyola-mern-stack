# Module 11 Demo | Context, Output, Verification

**Time:** 20 minutes | **Paired lab:** [Lab 11](../hands-on/module-11-ai-playbook.md)

## Prepare

Use an approved AI tool and this synthetic requirement: “Show open campus events sorted by date. Do not expose attendee email.” No private repository content or credentials.

## Run it

1. Ask a vague prompt for an implementation. Record assumptions and missing requirements.
2. Improve the prompt with context, constraints, expected output, and an instruction to list assumptions and tests.
3. Compare outputs against the requirement and a simple data model. Ask: does it filter on the server? Can an attendee email leak?
4. Treat AI as a bounded workflow: analyst proposes acceptance criteria → developer proposes code → reviewer checks diff/tests; human approves each transition.
5. Run or manually trace tests. Record what was correct, wrong, and independently verified.

**Expected:** better-grounded output still receives human review. **Recovery:** use two printed sample responses if no approved AI service is available. Never measure success by prompt count or generated lines.