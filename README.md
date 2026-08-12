# skillA · Claude Code Skill 合集

个人自创的 Claude Code skills 备份库。每个 skill 都是独立文件夹,复制到 `~/.claude/skills/` 即可安装使用。

## 已有 Skills

### ask-workdir — 创作前确认工作目录

**功能**:开始创作型任务(新项目、新文档、新代码等)前,先询问用户工作文件放在哪里:是使用不同盘的某个已有文件夹,还是新建一个文件夹存放。确认后才开始创作,避免文件乱放。

**安装方法**:

```bash
# Windows
cp -r skills/ask-workdir "$USERPROFILE/.claude/skills/"

# macOS / Linux
cp -r skills/ask-workdir ~/.claude/skills/
```

**使用方法**:
- 自动触发:重启 Claude Code 会话后,遇到创作类请求时会自动确认工作目录
- 手动触发:会话中直接输入 `/ask-workdir` 强制执行目录确认

## 目录结构

```
skillA/
├── README.md
└── skills/
    └── ask-workdir/
        └── SKILL.md
```

## 说明

- 每个 skill 采用官方格式:`SKILL.md` 包含 YAML frontmatter(name、description)与正文指令
- 本库中的 skill 基于个人使用习惯编写,欢迎借鉴
