# SOIA Open Skills Catalog

> Generated from `skills/*/SKILL.md` and optional `agents/openai.yaml`.
> Do not edit by hand. Run `python3 scripts/generate_skill_catalog.py`.
> Discoverable by `npx skills add soia-team/soia-open-edu-course-skills -l`: 2 skills.

## Source Fields

- `SKILL.md` is the canonical cross-agent instruction file. Capabilities, dependencies, setup, workflow steps, logs, and completion summaries must live there.
- `agents/openai.yaml` is optional UI/catalog metadata for OpenAI/Codex-style surfaces and SOIA registry display: `display_name`, `short_description`, and `default_prompt`.
- Claude Code and generic skills.sh-compatible agents must be assumed to consume `SKILL.md`; do not put required workflow steps only in `agents/openai.yaml`.
- Legacy `metadata.json` files are not used to generate this catalog.

## Education

| Skill | Description | Default Prompt |
|---|---|---|
| [`soia-edu-compose-lesson-plan`](./soia-edu-compose-lesson-plan/) | 按课程大纲编写含时间、互动和作业的教案与讲义结构 | Use $soia-edu-compose-lesson-plan to turn my course outline into a timed lesson plan and handout structure. |
| [`soia-edu-design-course-outline`](./soia-edu-design-course-outline/) | 从主题、受众与课时约束生成目标可测的课程大纲 | Use $soia-edu-design-course-outline to design a measurable course outline from my topic, audience, and lesson constraints. |

## Registry Export

Generate v7 SOIA registry manifests from the same sources when needed:

```bash
python3 scripts/generate_skill_catalog.py --registry-out <soia-repo>/runtime/registry/skills
```
