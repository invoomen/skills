---
name: characters
description: List the user's saved characters and elements.
---

Call `list_characters` and `list_elements` in parallel.

- Characters: people / mascots / recurring subjects the user has saved at
  `/elements/character`.
- Elements: props, scenes, styles saved at `/elements/elements`.

Print each list as `@<name> — <short description>`. If either is empty, tell
the user where to create some.

Mention that any of these names can be used inside a prompt to a `generate_*`
tool with an `@` prefix.
