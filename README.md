# marketplace

Joshua Light's plugins for Claude Code and Codex. The marketplace is named `joshua-light`.

## Plugins

| Plugin | What it does | Source |
| --- | --- | --- |
| `style` | A visual style for reports, explainers, dashboards, slides, and charts: dark gray panels, black borders, square corners, outlined headings. | [joshua-light/style](https://github.com/joshua-light/style) |

## Install

Add the marketplace once, then install a plugin by name.

Claude Code:

```sh
claude plugin marketplace add joshua-light/marketplace
claude plugin install style@joshua-light
```

Inside a session, the same two steps are `/plugin marketplace add joshua-light/marketplace` and `/plugin install style@joshua-light`.

Codex:

```sh
codex plugin marketplace add joshua-light/marketplace
codex plugin add style@joshua-light
```

## Layout

| Path | Purpose |
| --- | --- |
| `.claude-plugin/marketplace.json` | The catalog Claude Code reads. |
| `.agents/plugins/marketplace.json` | The catalog Codex reads. |

Each plugin lives in its own repository; this one only lists them. To add a plugin, add an entry with the same `name` to both files.

## License

MIT.
