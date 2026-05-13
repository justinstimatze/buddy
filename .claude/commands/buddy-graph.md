---
description: Generate and open an interactive visualization of Buddy guard-mode reasoning data using the Buddy CLI.
---

Run the Buddy graph CLI to visualize the reasoning graph.

If a session ID is provided in `$ARGUMENTS`, pass it through to the command.

```bash
if command -v buddy >/dev/null 2>&1; then
  buddy graph $ARGUMENTS --open
else
  node dist/cli/buddy.js graph $ARGUMENTS --open
fi
```

Execute the bash block above and then report the saved graph path and basic graph counts back to the user.
