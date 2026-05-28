---
name: status
description: Show the user's recent Invoomen generations and credit balance.
---

The user wants a quick status of their Invoomen account.

1. Call `get_balance`. Print plan, total credits, renewal date.
2. Call `list_recent_generations` with `limit: 10`. Print a compact list:
   `<status> · <kind> · <model_id> · <when>`.
3. If the user mentioned a specific generation_id, call `get_generation` for
   it and show the URL or error.

Keep it terse — under 12 lines unless the user asks for detail.
