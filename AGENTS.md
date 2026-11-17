# AGENTS.md

Guidelines for AI coding agents and human contributors working in ha-c4 repositories.

## Commit messages

Keep commit messages concise and specific. The diff already shows *what* changed. The message should say *why*.

### Format

```
<Subject: imperative, 50 chars or fewer, no period>

<Optional body: why the change was needed, wrapped at 72 chars.>

<Optional trailers: Fixes #N, Co-authored-by: ...>
```

### Rules

- **Use the imperative mood**: "Add", "Fix", "Remove", not "Added" or "Fixes".
- **Keep the subject to 50 characters or fewer** (72 at most), capitalized, with no trailing period.
- **Make one logical change per commit.** If the subject needs "and", consider splitting the commit.
- **Add a body only when it says something new**, such as the reason, a trade-off, or a non-obvious side effect. Leave it out for self-explanatory changes.
- **Skip filler**: no "Update file.py", "Fix bug", "Misc changes", "WIP", lists of every file touched, or emoji.
- **Credit the source when porting from a fork.** Link the original commit in the body and add a `Co-authored-by:` trailer for its author. If you don't know their email, use their GitHub noreply address.
- **Don't add AI attribution trailers** such as `Co-Authored-By: Claude`. It's already known that AI agents work in ha-c4 repositories. Use `Co-authored-by:` only to credit the people whose work you port.

### Examples

Good:

```
Fix thermostat setpoint rounding in Fahrenheit
```

```
Port dimmer ramp-rate support from community fork

Adds variable ramp times for dimmers, adapted to the current
director API.

Ported from: https://github.com/<user>/pyControl4/commit/<sha>
Co-authored-by: Original Author <author@example.com>
```

Avoid:

```
Updated stuff
```

```
Fixed bugs in light.py, climate.py and director.py and also added tests and cleaned up formatting
```
