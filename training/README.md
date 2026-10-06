# MERN Value-Added Course Trainer Pack

This pack turns the curriculum in the repository README into teachable, practice-first sessions. It is designed for engineering college students with little or no prior full-stack experience.

## Folders

- `ppt/`: slide-by-slide Markdown outlines plus editable PowerPoint decks (`module-01.pptx` through `module-11.pptx`). The decks explain each curriculum topic in plain language and pair it with a concrete example.
- `demos/`: facilitator runbooks for short, visible demonstrations. Each one names its setup, steps, expected result, and recovery path.
- `hands-on/`: student lab sheets aligned to the corresponding deck and demo, with checks and an extension.
- `tools/generate_decks.py`: source data and generator for the PowerPoint decks.

Every module uses the same number in all three folders. Recommended course thread: build a small **Campus Event Desk** from a problem sketch to a deployed application, while keeping each exercise independently approachable. Students may use fictional data only.

## Module Map

| Module | Curriculum focus | Duration | Student evidence |
| --- | --- | ---: | --- |
| 01 | Programming and web foundations | 5 h | Request map and expense summary logic |
| 02 | HTML, CSS, JavaScript | 10 h | Responsive event card and registration form |
| 03 | ES6+, APIs, Git and GitHub | 15 h | API-powered event feed and reviewed change |
| 04 | React | 25 h | Component-based event browser |
| 05 | Node.js and Express | 20 h | Tested event REST API |
| 06 | MongoDB and Mongoose | 10 h | Event collection, queries, and model |
| 07 | Full-stack integration and authentication | 15 h | Secure, end-to-end registration flow |
| 08 | Testing, deployment and DevOps | 10 h | Test evidence and deployment checklist |
| 09 | Capstone | 24 h | Team-built, demonstrated MERN solution |
| 10 | Interview and placement readiness | 6 h | Portfolio evidence and practiced answers |
| 11 | AI-assisted software engineering | 10 h | Reusable, reviewed AI workflow and playbook |

## How to Use the Pack

1. Start with the module's `ppt/module-NN-*.md` outline and adapt its examples to the cohort.
2. Rehearse the matching `demos/module-NN-*.md` runbook before class; demos are intentionally short and have a fallback.
3. Give students the corresponding `hands-on/module-NN-*.md` lab. Keep the acceptance checks visible while they work.
4. End with the exit ticket and ask students to save the named evidence in their course repository.

## Regenerate the PowerPoints

With Python 3 available, install the generator dependency and run:

```sh
python3 -m pip install --user python-pptx
python3 training/tools/generate_decks.py
```

The generated decks are saved in `training/ppt/`. Update the topic data in the generator when the README curriculum changes, then rerun the command.

The README remains the source of truth for curriculum breadth and durations. These artifacts simplify the concepts and add practical evidence; they do not replace the listed learning outcomes or milestone projects.