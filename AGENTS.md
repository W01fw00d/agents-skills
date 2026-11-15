# Agent Guidelines

## When Installing a New Skill

Whenever a new skill is installed into `.agents/skills/`, you **must** update `README.md` to document it.

### Steps

1. **Read the new skill's `SKILL.md`** to get:
   - The skill name from the `name` frontmatter field.
   - A brief description from the `description` frontmatter field or the first heading.
   - The documentation URL (check the skill content for official docs links, or infer from the skill name).

2. **Determine the category** based on the skill's domain (e.g., "Playwright", "Testing", "CI/CD", "General").
   - If a `### Category` section already exists under `## Skills`, add the new skill to that section's table.
   - If the skill belongs to a new category, create a new `### Category` section with a fresh table.

3. **Add a row to the table** following this format:

   | Skill        | Description                               | Documentation                 |
   | ------------ | ----------------------------------------- | ----------------------------- |
   | `skill-name` | Brief description of what the skill does. | [short-url](https://full-url) |

4. **Keep the table aligned** — match the column widths and style of existing rows.

### Example

After installing a new skill `playwright-cli` under the "Playwright" category:

```markdown
### Playwright

| Skill            | Description                                                                                     | Documentation                                                              |
| ---------------- | ----------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| `playwright-cli` | Automate browser interactions, test web pages, and work with Playwright tests via command line. | [playwright.dev/agent-cli/skills](https://playwright.dev/agent-cli/skills) |
```
