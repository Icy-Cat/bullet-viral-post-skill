# bullet-viral-post

> 作者（推文来源）：**软苏 Grace（@Graceruansu）**  
> X 账号：<https://x.com/Graceruansu>

面向中文 X/Twitter 的爆款推文生成 Skill。

## 效果预览

![前后效果对比（来源：软苏 Grace 推文）](./assets/before-after.jpg)

> 图源：<https://x.com/i/status/2031180628222423468>

---

## 一键安装（新手直接复制）

### macOS / Linux

```bash
git clone https://github.com/Icy-Cat/bullet-viral-post-skill.git /tmp/bullet-viral-post-skill && \
mkdir -p ~/.claude/skills/bullet-viral-post && \
cp -R /tmp/bullet-viral-post-skill/* ~/.claude/skills/bullet-viral-post/
```

### Windows PowerShell

```powershell
git clone https://github.com/Icy-Cat/bullet-viral-post-skill.git "$env:TEMP/bullet-viral-post-skill";
New-Item -ItemType Directory -Force "$HOME/.claude/skills/bullet-viral-post" | Out-Null;
Copy-Item -Recurse -Force "$env:TEMP/bullet-viral-post-skill/*" "$HOME/.claude/skills/bullet-viral-post/";
```

---

## 安装后怎么用

- 直接输入：`/bullet-viral-post`
- 或输入关键词：`推特爆款` / `爆款推文` / `/bullet`

## 快速检查

- 存在目录：`~/.claude/skills/bullet-viral-post/`
- 目录里有：`SKILL.md`、`step1-input-analysis.md`、`step9-auto-save.md`

## 路径配置（可选）

自动保存草稿路径支持变量：`{{DRAFT_BASE_PATH}}/YYYY-MM/`  
默认示例见 `step9-auto-save.md`。

## 版本

`0.1.2`
