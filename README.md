# SimpleFirst

SimpleFirst 是一个面向多语言软件开发的 Codex Skill。它要求 coding agent 默认选择简单、清晰、易维护的方案，避免过度设计，同时保留必要的正确性、安全、注释和测试。

## 核心原则

- 优先复用仓库现有实现、标准库、平台能力和已有依赖。
- 不为推测性的未来需求增加抽象、配置或扩展点。
- 以最低认知成本为目标，不以代码行数最少为目标。
- Bug 修复定位共享根因，并检查相关调用方。
- 不为了简化而牺牲校验、安全、一致性和错误处理。
- 使用目标语言惯用的文档注释，并让测试范围与变更风险匹配。

## 安装

将仓库克隆到 Codex Skills 目录：

```bash
git clone https://github.com/sanwzzz/SimpleFirst.git ~/.codex/skills/simple-first
```

在任务中显式调用：

```text
$simple-first
```

Codex 也可以根据 `SKILL.md` 中的 description 在编码任务中自动选择该 Skill。

## License

[MIT](LICENSE)
