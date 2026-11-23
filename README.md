# droidtop-plugin-oldversions
droidtop source plugin: older versions of free software and freeware (OldVersion.com first, then GitHub/GitLab releases and other archives). mytop-project/tracker#647

## Branches

The owner, 2026-11-10: "Just like with the enginehost cores, the plugin-core branch is the wrapper code that makes
it a plugin, we have a branch for the actual core code, and releases are a blending of both."

- **`plugin-core`** (this branch, the default): the wrapper that makes it a droidtop plugin, and each line's pin in
  `plugin-line/lines/<line>/line.json`.
- **`creation`**: the core code, once there is any (this plugin is a design so far).
- **`plugin/<line>`**: `creation` at a pinned commit with `plugin-core` written over it, composed by
  mytop-project/droidtop-platforms `tools/plugin_line.py`. Releases are built from it; nothing is authored there.

Every change lands through a `ci/` branch. There is no `main`.
