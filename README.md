# skills

Agent skills for Claude Code and other coding agents. Each skill lives in its own directory as a `SKILL.md`.

## Skills

| Skill | What it does |
|---|---|
| [doc-lint](doc-lint/SKILL.md) | Polishes Chinese technical documents: trims redundancy, removes AI clichés and translationese, and rewrites note-style fragments into full sentences. Keeps technical meaning, identifiers, and the original modality, owners, and scope. The skill text is in Chinese. |

## Install

Clone the repository and symlink the skills you want into your agent's skills directory:

```sh
git clone https://github.com/fuguiw/skills.git
ln -s "$PWD/skills/doc-lint" ~/.claude/skills/doc-lint   # Claude Code
ln -s "$PWD/skills/doc-lint" ~/.agents/skills/doc-lint   # agents that read ~/.agents/skills
```

A `git pull` then updates every linked skill in place.

## License

[MIT](LICENSE)
