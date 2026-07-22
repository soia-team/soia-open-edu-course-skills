# SOIA 教育课程技能库

教育-课程：课程大纲、教案讲义、题目测评（孵化仓；通用化，个性化数据只进用户配置）

## 孵化中

本仓处于孵化阶段，技能和接口可能继续调整。

## 域说明

本仓负责 `edu` 域，技能名称统一使用 `soia-edu-*` 前缀。

## 技能清单

| 技能 | 用途 | 典型触发 |
|---|---|---|
| [`soia-edu-design-course-outline`](./skills/soia-edu-design-course-outline/) | 从主题、受众与课时约束生成目标可测的课程大纲 | 课程大纲、教学目标、课时规划 |
| [`soia-edu-compose-lesson-plan`](./skills/soia-edu-compose-lesson-plan/) | 按大纲编写含时间、互动、作业的教案与讲义结构 | 教案、讲义、课堂活动 |

## 安装

```bash
npx skills add soia-team/soia-open-edu-course-skills -g -a '*' -s <skill> -y
```

本仓属于 SOIA 技能生态，规范真源见 [soia-team/soia-open-skills](https://github.com/soia-team/soia-open-skills)。
