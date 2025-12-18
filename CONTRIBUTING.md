# Contributing to Agent Skills

We welcome contributions to the universal skill repository.

## Adding a Skill

### Requirements

1. Your skill must follow the [Agent Skills specification](https://agentskills.io/specification)
2. The `SKILL.md` file must include valid YAML frontmatter with `name` and `description`
3. The skill name must be lowercase with hyphens only (e.g., `my-skill`)
4. The skill must actually work and provide value

### Process

1. Fork this repository
2. Create your skill folder: `skills/<skill-name>/`
3. Add your `SKILL.md` file with proper frontmatter:

```yaml
---
name: my-skill
description: What this skill does and when to use it.
license: MIT
---

# My Skill

Instructions for the agent...
```

4. Add an entry to `skills.json`:

```json
{
  "name": "my-skill",
  "description": "What this skill does and when to use it.",
  "category": "development",
  "author": "your-username",
  "source": "your-username/your-repo",
  "license": "MIT",
  "path": "skills/my-skill",
  "stars": 0,
  "downloads": 0,
  "featured": false,
  "verified": false
}
```

5. Submit a pull request

### Categories

Use one of these categories:

- `development` - Coding, debugging, testing, tooling
- `document` - PDF, Word, Excel, presentations
- `creative` - Art, design, visuals
- `business` - Communication, research, productivity
- `data` - Analytics, visualization, databases
- `content` - Writing, research, media
- `lifestyle` - Personal productivity

### Review Process

We review all submissions for:

- **Spec compliance**: Valid SKILL.md format
- **Quality**: Clear instructions, actually useful
- **Safety**: No malicious or harmful content
- **Uniqueness**: Not duplicating existing skills

## Updating Existing Skills

If you find a bug or want to improve an existing skill:

1. Fork the repo
2. Make your changes
3. Test that the skill still works
4. Submit a PR with a clear description of the change

## Questions?

Open an issue or visit [skillcreator.ai](https://skillcreator.ai).
