# SOIA Education & Course Skills

[中文](README.md) · English

From a topic to a lesson plan you can teach from — outline, sessions, activities, handouts, in one line.

## What this is

`soia-open-edu-course-skills` splits course design into two steps, where the first feeds directly into the second:

```text
Topic + audience + session constraints
    ↓
Course outline (learning objectives, modules, session allocation)
    ↓
Lesson plans and handouts (activities, timing, teaching points)
```

Both skills are pure methodology — no network, no private data, no credentials. They work the moment they are installed.

### When to use it

- "Design an 8-session outline for 'Intro to Python' for absolute beginners."
- "Write the lesson plan for session 3 from this outline."
- "What classroom activities does this session need?"

### What it does not do

- Does not generate slide decks. For presentations use `soia-pkm-transform-article-ppt` in [soia-open-pkm-vault-skills](https://github.com/soia-team/soia-open-pkm-vault-skills).
- No question banks or exam systems.
- No subject-matter content library. Domain knowledge comes from you or the model; this repo supplies the instructional-design structure only.

## Where to start

Use the two skills in order:

| Your task | Use | Done when |
|---|---|---|
| Design a course outline | `soia-edu-design-course-outline` | Objectives, modules, and session allocation complete |
| Write a specific lesson plan | `soia-edu-compose-lesson-plan` | Activities, timing, and teaching points are ready to run |

Neither skill needs credentials or external tooling — both work right after install.

## Skill catalog

> **Ready to use**: ✅ works right after install · 🟡 needs an API key or a third-party login first

| Skill | Responsibility | Ready to use |
|---|---|---|
| `soia-edu-compose-lesson-plan` | Turn a course outline into an executable lesson plan and handout structure with timing, interactions, and assignments. | ✅ |
| `soia-edu-design-course-outline` | Design a measurable course outline from a topic, audience, and lesson constraints. | ✅ |

## Install

Installing the whole domain plugin is recommended — it brings every skill in this repo:

```bash
claude plugin marketplace add soia-team/soia-open-skills
```

```bash
claude plugin install soia-edu-course@soia
```

For Codex:

```bash
codex plugin marketplace add soia-team/soia-open-skills
codex plugin add soia-edu-course@soia
```

For a single skill you can use the npx route. Note the skill lands in the shared
source `~/.agents/skills`; if the plugin is installed too, the same skill shows up
twice and the two copies drift apart — pick one:

```bash
npx skills add soia-team/soia-open-edu-course-skills -g -a '*' -s <skill-name> -y
```

## Ecosystem

Specifications, the full ecosystem catalog, and install guides live in [soia-team/soia-open-skills](https://github.com/soia-team/soia-open-skills).
The full maintenance workflow is in [CONTRIBUTING.md](https://github.com/soia-team/soia-open-skills/blob/main/CONTRIBUTING.md).

## License

MIT License — see [LICENSE](./LICENSE).
