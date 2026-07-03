# My Dev Plugins (Fork of claude-plugins-official)

A curated subset of development tool plugins, forked from [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official).

Renamed to `my-dev-plugins` to avoid the reserved `claude-plugins-official` identifier.

## What's included

49 development-focused plugins selected from the 255+ in the official marketplace:

| Category | Count | Examples |
|----------|-------|---------|
| Development workflow | 33 | feature-dev, code-modernization, playground |
| Productivity (dev-oriented) | 12 | commit-commands, code-review, github, gitlab |
| Security / code quality | 3 | security-guidance, semgrep, sonarqube |
| Testing | 1 | playwright |

Includes 12 language servers (TypeScript, Python, Go, Rust, Java, C#, Kotlin, C/C++, PHP, Ruby, Lua, Swift).

## Installation

### Step 1: Add this marketplace

In Claude Code or Claude Desktop:

```
/plugin marketplace add YOUR_GITHUB_USERNAME/claude-plugins-official
```

Or via Claude Desktop Settings > Plugins & skills > Plugin marketplaces > + Add marketplace > GitHub repo > `YOUR_GITHUB_USERNAME/claude-plugins-official`

### Step 2: Install plugins

```
/plugin install commit-commands@my-dev-plugins
/plugin install code-review@my-dev-plugins
/plugin install feature-dev@my-dev-plugins
```

Browse all: `/plugin > Discover` (select `my-dev-plugins` marketplace)

### Step 3: Reload

```
/reload-plugins
```

## Syncing with upstream

```bash
git remote add upstream https://github.com/anthropics/claude-plugins-official.git
git fetch upstream
git merge upstream/main
# Resolve conflicts (keep your name changes, merge new plugins)
git push origin main
```

## License

See each plugin's LICENSE file. Original code is licensed under Apache 2.0 by Anthropic.
