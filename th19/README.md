# TH19 Upgrade Planner data

`upgrades.json` is the upgrade list the TH19 Upgrade Planner app downloads when it opens (or when you press "Check for new data").
Edit this file and push to `main` — every copy of the app picks up the change; no reinstall needed.

Each entry:

| Field | Meaning |
| --- | --- |
| `id` | Unique key (name-level). Done ticks and copy counts in the app are saved against it, so don't rename existing ids. |
| `name`, `level` | What gets upgraded, and to which level |
| `copies` | Default number of that building (the app lets you override it) |
| `resource` | `Gold`, `Elixir`, `Dark Elixir`, or `null` if unknown |
| `cost`, `days` | Base cost and time before the Gold Pass; `null` = not known yet |
| `boost` | `Builder`, `Research` or `None` — which Gold Pass boost applies |
| `category` | One of the names in `categories` |
| `note` | Source or extra info shown under the name |

Costs/times so far come from Judo Sloth's TH19 Sneak Peek 1 and 2 videos (dev build).
