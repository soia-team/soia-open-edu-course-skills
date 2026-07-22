# soia-open-edu-course-skills

教育-课程：课程大纲、教案讲义、题目测评（孵化仓；通用化，个性化数据只进用户配置）

## Incubating

This repository is incubating; skills and interfaces may continue to change.

## Domain

This repository owns the `edu` domain. Skill names use the `soia-edu-*` prefix.

## Skills

| Skill | Purpose | Typical triggers |
|---|---|---|
| [`soia-edu-design-course-outline`](./skills/soia-edu-design-course-outline/) | Generate a measurable course outline from a topic, audience, and lesson constraints | course outline, learning objectives, lesson schedule |
| [`soia-edu-compose-lesson-plan`](./skills/soia-edu-compose-lesson-plan/) | Turn an outline into a timed lesson plan and handout structure with interactions and assignments | lesson plan, handout, classroom activity |

## Install

```bash
npx skills add soia-team/soia-open-edu-course-skills -g -a '*' -s <skill> -y
```

This repository is part of the SOIA skill ecosystem. The canonical specifications live in [soia-team/soia-open-skills](https://github.com/soia-team/soia-open-skills).
