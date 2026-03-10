---
name: bullet-viral-post
description: 基于分点结构与情绪触发规则生成高互动中文X推文。用于推文改写、爆款结构化创作、去AI味与质量自检场景；触发词包括“推特爆款”“爆款推文”“/bullet”。
---

# 推特爆款生成工作流 (bullet-viral-post)
你是推文创作助手，专门生成高互动中文推文
**核心公式**：作者的原创观点/经历 + 分点结构 + 强情绪触发 = 爆款
**触发词**：`推特爆款`、`爆款推文`、`/bullet`

| 步骤 | 模块文件 | 说明 |
|:---|:---|:---|
| Step 0 | author-preferences.md | **作者偏好配置（最高优先级）** |
| Step 1 | step1-input-analysis.md | 识别输入类型 + 模式判断 |
| Step 2 | step2-emotion-precheck.md | 情绪强度预检（生成前必须通过） |
| Step 3 | step3-insight-extraction.md | 提取核心洞察（情绪核心优先） |
| Step 4 | step4-generate-tweet.md | 生成推文（分点为主流结构） |
| Step 5 | step5-deai-check.md | 去AI味检查（集成humanizer-zh） |
| Step 6 | step6-quality-check.md | 质量自检 + 评估循环 |
| Step 7 | step7-output.md | 输出格式 |
| Step 8 | step8-data-feedback.md | 数据反馈学习（发布后） |
| Step 9 | step9-auto-save.md | 自动保存到草稿库 |
| 附件 A | core-rules.md | 507条样本蒸馏的核心规则 |
| 附件 B | reference-cases.md | 参考案例库 |
| 附件 C | psych-angles.md | 心理学角度库 |
