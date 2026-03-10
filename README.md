# bullet-viral-post

> 对应推文文章：<https://x.com/i/status/2031180628222423468>  
> 作者（推文来源）：**软苏 Grace（@Graceruansu）**  
> X 账号：<https://x.com/Graceruansu>

面向中文 X/Twitter 的爆款推文生成 Skill。

## 效果预览

![前后效果对比（来源：软苏 Grace 推文）](./assets/before-after.jpg)

> 图源：<https://x.com/i/status/2031180628222423468>

---

## 一键安装（推荐直接发给AI）

```text
请参照这个 README 的说明，为我安装 skill：
https://github.com/Icy-Cat/bullet-viral-post-skill/blob/main/README.md
```

## 手动安装（终端）

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

## 使用

```text
请用 bullet-viral-post 这个 skill，
基于“年轻人不结婚”这个话题写 1 条中文 X 推文。
```

- 也可直接输入：`/bullet-viral-post`
- 或关键词触发：`推特爆款` / `爆款推文` / `/bullet`

## 快速检查

- 存在目录：`~/.claude/skills/bullet-viral-post/`
- 目录里有：`SKILL.md`、`step1-input-analysis.md`、`step9-auto-save.md`

## 可选配置

自动保存草稿路径变量：`{{DRAFT_BASE_PATH}}/YYYY-MM/`（见 `step9-auto-save.md`）

## 版本

`0.1.2`
