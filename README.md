# SOIA 教育课程技能库

[English](README.en.md) · 中文

从一个主题到能直接上讲台的教案——大纲、课时、活动、讲义，一条线走完。

## 这是什么

`soia-open-edu-course-skills` 把课程设计拆成两步，前一步的产出直接喂给后一步：

```text
主题 + 受众 + 课时约束
    ↓
课程大纲（教学目标、模块划分、课时分配）
    ↓
教案与讲义（课堂活动、时间安排、讲授要点）
```

两个技能都是纯方法论——不联网、不读私有数据、不需要任何凭据，装完直接能用。

### 适合什么场景

- 「给『Python 入门』设计一个 8 课时的大纲，学员是零基础。」
- 「按这份大纲写第 3 课的教案。」
- 「这堂课需要什么课堂活动？」

### 不负责什么

- 不生成课件 PPT。要做演示文稿，用 [soia-open-pkm-vault-skills](https://github.com/soia-team/soia-open-pkm-vault-skills) 的 `soia-pkm-transform-article-ppt`。
- 不做题库与考试系统。
- 不含任何学科内容库。学科知识由你提供或由模型自身能力承担，本仓只负责教学设计的结构。

## 从哪里开始

两个技能按顺序用即可：

| 你要做的 | 用这个 | 完成标准 |
|---|---|---|
| 设计课程大纲 | `soia-edu-design-course-outline` | 教学目标、模块划分、课时分配齐全 |
| 写具体教案 | `soia-edu-compose-lesson-plan` | 课堂活动、时间安排、讲授要点可直接执行 |

本仓两个技能都不需要凭据或外部工具，装完即可使用。

## 技能清单

> **开箱可用**：✅ 装完即可使用 · 🟡 还需申请 API key 或完成第三方登录

| 技能 | 一句话职责 | 开箱可用 |
|---|---|---|
| `soia-edu-compose-lesson-plan` | 按课程大纲编写可执行教案与讲义结构。 | ✅ |
| `soia-edu-design-course-outline` | 从主题、受众和课时约束设计课程大纲。 | ✅ |

## 安装

推荐装整个领域插件，一次装好本仓全部技能：

```bash
claude plugin marketplace add soia-team/soia-open-skills
```

```bash
claude plugin install soia-edu-course@soia
```

Codex 用户：

```bash
codex plugin marketplace add soia-team/soia-open-skills
codex plugin add soia-edu-course@soia
```

只要单个技能时可用 npx 路线。注意技能会落进共享真源 `~/.agents/skills`；
若同时装了插件，同一技能会出现两份索引且各自漂移，建议二选一：

```bash
npx skills add soia-team/soia-open-edu-course-skills -g -a '*' -s <技能名> -y
```

## 验证与贡献

改动技能后，提交前跑：

```bash
python3 -m unittest discover -s tests -p 'test_*.py'
python3 scripts/generate_skill_catalog.py --check
python3 scripts/audit_skills.py --strict
```

贡献流程、技能契约与发布步骤见元仓
[CONTRIBUTING.md](https://github.com/soia-team/soia-open-skills/blob/main/CONTRIBUTING.md)。

## 生态导航

规范真源、全生态技能目录与安装指南见 [soia-team/soia-open-skills](https://github.com/soia-team/soia-open-skills)。
维护本仓技能的完整流程见 [CONTRIBUTING.md](https://github.com/soia-team/soia-open-skills/blob/main/CONTRIBUTING.md)。

## License

MIT License — see [LICENSE](./LICENSE).
