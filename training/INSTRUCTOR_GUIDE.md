# Instructor Guide

## Teaching stance

Assume students are new to the tool, not incapable of the problem. Explain one idea, show it in a small working example, let students change it, then ask them to explain the result. Prefer familiar campus workflows and fictional data over abstract examples. Do not turn setup friction into a test of student ability.

## Repeatable session rhythm

- **Connect:** start with a campus scenario and ask what a user needs to accomplish.
- **Model:** teach one concept in a short slide sequence; narrate decisions and likely mistakes.
- **Show:** run the paired demo, including one intentional failure and how to inspect it.
- **Build:** students complete the paired lab in small increments and verify each acceptance check.
- **Share:** invite a few students to demonstrate a working behavior and describe one trade-off.
- **Reflect:** collect the exit ticket and note who needs a setup or concept follow-up.

Use this rhythm repeatedly within the curriculum's stated hours; a module's slide outline is a teaching spine, not a claim that a long module can be delivered in one lecture.

## Setup and inclusion

- Check editor, browser, Node.js/npm, Git, and the module-specific database or testing tools before class. Offer a prepared Codespace or paired workstation where possible.
- Provide a known-good starter and a screenshot/recording of the expected result. Pair students intentionally and rotate driver/navigator roles.
- Keep API keys, passwords, personal information, and real student records out of demos, screenshots, prompts, and Git history.
- For network-dependent demos, use the runbook's local/fallback path. Do not make course progress depend on a public API staying available.
- Assess observable behavior and reasoning, not typing speed or visual polish.

## AI use across the course

AI is an assistant, not an authority. Students should state the task and constraints, inspect generated code, run checks, and disclose meaningful AI assistance. Never paste secrets, private records, or unlicensed material into a model. For security-related output, require a human review and a test; a confident explanation is not evidence of correctness.

## Feedback rubric

Use a lightweight 0-2 scale: **0** not yet demonstrated; **1** partly working or explained with prompts; **2** works and the student can explain the key decision. Apply it to the lab's acceptance checks, then give one next step. Avoid grading students against production-scale expectations during a beginner module.