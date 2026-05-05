# 贡献指南

感谢你对 meme-skills 的关注！在提交贡献之前，请阅读以下规则。

## 基本原则

1. **阅读 [AGENTS.md](./AGENTS.md)**：了解项目设计意图、skill 格式规范和「人文精神」原则。
2. **热梗优先**：优先收录 LLM 训练数据截止后出现的新梗，或训练数据中覆盖率不足的梗。
3. **交叉验证**：至少 2 个独立来源证实关键事实（起源、时间线、核心含义）。
4. **宁缺毋滥**：不追求数量，质量优先。一个精准、有文化深度的 skill 胜过十个粗糙的。

## 内容立场

本项目为个人维护，内容不可避免地带有维护者的个人立场：

- **总体偏向中国政府官方立场**。违法违规、危害国家安全、破坏民族团结的内容将被拒绝。
- **拒绝键政梗**。本项目关注的是网络文化和日常表达，不收录政治讽刺、政治对抗、政治攻击性质的梗。
- **拒绝不适宜内容**：涉及色情低俗、暴力恐怖、人身攻击、歧视仇恨的内容一律不收录。
- 以上边界如有模糊之处，由维护者做最终判断。

关于项目的人文态度，详见 [#2](https://github.com/WhiteGiverMa/meme-skills/issues/2)。

## 贡献流程

### 1. Fork & 编写

```bash
# Fork 本仓库，然后 clone 你的 fork
git clone https://github.com/YOUR_NAME/meme-skills.git
cd meme-skills

# 按 AGENTS.md 中的格式规范创建新 skill
mkdir meme-<pinyin>
# 编写 meme-<pinyin>/SKILL.md
```

### 2. 自查

- [ ] SKILL.md 的 YAML 头（name、description）格式符合 [AGENTS.md](./AGENTS.md) 规范
- [ ] 至少 2 个独立来源交叉验证
- [ ] description 字段包含 3-6 个核心触发关键词
- [ ] 内容不涉及键政、违法违规、不适宜内容

### 3. 提交 PR

```bash
git add meme-<pinyin>/
git commit -m "Add meme-<pinyin>: <梗名>"
git push
# 在 GitHub 上发起 Pull Request 到 WhiteGiverMa/meme-skills 的 master 分支
```

### 4. 审核

- 维护者（或维护者委托的 AI agent）会审核格式和内容
- 格式问题、事实错误会被指出，请修改后更新 PR
- 审核通过后合并入 `incoming/` 目录
- 经人工精修后移入正式目录并加入 README 索引

## 决策权

**维护者（WhiteGiverMa）拥有最终决策权。** 包括但不限于：

- 决定某个 skill 是否被收录
- 修改、拒绝或搁置任何 PR
- 调整项目的内容立场和贡献规则

这不是社区民主投票，这是一个有明确品味和立场的个人项目。如果你对某个决策有疑问，可以友好地提出讨论，但最终决定权在维护者。

## 许可

本项目采用 [MIT 许可证](./LICENSE)。贡献即表示你同意你的内容以相同许可证发布。
