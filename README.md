# bullet-viral-post

> 作者（推文来源）：**软苏 Grace（@Graceruansu）**  
> X 账号：<https://x.com/Graceruansu>

面向中文 X/Twitter 的爆款推文生成 Skill。  
目标：把高互动写法流程化，稳定产出可复盘内容。

## 效果示意（原推文对比图）

![前后效果对比（来源：软苏 Grace 推文）](./assets/before-after.jpg)

> 图源：<https://x.com/i/status/2031180628222423468>

---

## 功能概览

- 输入识别：互动型 / 曝光型
- 情绪预检：不达标先换素材
- 洞察提取：优先“扎心场景”
- 分点生成：3-5 点，冲突递进
- 去 AI 味：词汇/句式过滤
- 质量自检：不通过自动重写（最多 2 轮）
- 结构化输出：正文 + 元数据
- 数据反馈：发布后持续优化

---

## 目录结构

- `SKILL.md`（入口）
- `_meta.json`（元信息）
- `author-preferences.md`
- `core-rules.md`
- `reference-cases.md`
- `psych-angles.md`
- `step1-input-analysis.md` ~ `step9-auto-save.md`

---

## 安装（Claude Code）

### 个人级安装（推荐）

**macOS / Linux（仓库根目录执行）**

```bash
mkdir -p ~/.claude/skills/bullet-viral-post
cp -R ./skills/bullet-viral-post/* ~/.claude/skills/bullet-viral-post/
```

**Windows PowerShell（仓库根目录执行）**

```powershell
New-Item -ItemType Directory -Force "$HOME/.claude/skills/bullet-viral-post" | Out-Null
Copy-Item -Recurse -Force "./skills/bullet-viral-post/*" "$HOME/.claude/skills/bullet-viral-post/"
```

### 项目级安装（仅当前项目生效）

**macOS / Linux**

```bash
mkdir -p ./.claude/skills/bullet-viral-post
cp -R ./skills/bullet-viral-post/* ./.claude/skills/bullet-viral-post/
```

**Windows PowerShell**

```powershell
New-Item -ItemType Directory -Force "./.claude/skills/bullet-viral-post" | Out-Null
Copy-Item -Recurse -Force "./skills/bullet-viral-post/*" "./.claude/skills/bullet-viral-post/"
```

---

## GitHub 一键安装片段

把 `https://github.com/Icy-Cat/bullet-viral-post-skill.git` 换成你的仓库地址。

**macOS / Linux**

```bash
git clone https://github.com/Icy-Cat/bullet-viral-post-skill.git /tmp/bullet-viral-post
mkdir -p ~/.claude/skills/bullet-viral-post
cp -R /tmp/bullet-viral-post/skills/bullet-viral-post/* ~/.claude/skills/bullet-viral-post/
```

**Windows PowerShell**

```powershell
git clone https://github.com/Icy-Cat/bullet-viral-post-skill.git "$env:TEMP/bullet-viral-post"
New-Item -ItemType Directory -Force "$HOME/.claude/skills/bullet-viral-post" | Out-Null
Copy-Item -Recurse -Force "$env:TEMP/bullet-viral-post/skills/bullet-viral-post/*" "$HOME/.claude/skills/bullet-viral-post/"
```

---

## 调用方式

- 直接调用：`/bullet-viral-post`
- 语义触发：`推特爆款` / `爆款推文` / `/bullet`

---

## 校验清单

- 目录存在：`~/.claude/skills/bullet-viral-post/` 或 `./.claude/skills/bullet-viral-post/`
- 入口文件存在：`SKILL.md`
- 关键规则文件存在：`author-preferences.md`、`core-rules.md`、`step1~step9`
- 自动保存路径可配置：`step9-auto-save.md` 中使用 `{{DRAFT_BASE_PATH}}/YYYY-MM/`

---

## 路径配置

在执行自动保存前，先设置你的草稿根目录变量：

- 变量名：`DRAFT_BASE_PATH`
- 示例值：`AI_Author/01-内容生产/推文管理系统/01-草稿库`

---

## 版本

`0.1.2`
