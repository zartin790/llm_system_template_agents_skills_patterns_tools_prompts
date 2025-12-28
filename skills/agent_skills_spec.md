# Agent Skills Spec

A skill is a folder of instructions, scripts, and resources that agents can discover and load dynamically to perform better at specific tasks. A folder is recognized as a skill when it contains a `SKILL.md` file.

# Skill Folder Layout

A minimal skill folder looks like this:

```
my-skill/
  - SKILL.md
```

More complex skills can add additional directories and files as needed.

# The SKILL.md file

The skill's entrypoint is the `SKILL.md` file. It must start with a YAML frontmatter followed by regular Markdown.

## YAML Frontmatter

Required:
- `name` — hyphen-case name matching the directory name; lowercase alphanumeric + hyphen
- `description` — what the skill does and when to use it

Optional:
- `license` — short license name or bundled license filename
- `allowed-tools` — list of pre-approved tools
- `metadata` — map for additional custom properties

## Markdown Body

No restrictions. Use it for instructions, examples, and guidance the agent should follow when the skill is active.

# Additional Information

For a minimal example, see `skills/template-skill/SKILL.md`.

# Version History

- 1.0 (2025-10-16) Public Launch
