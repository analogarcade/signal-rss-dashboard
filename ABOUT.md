# About Signal

Signal turns a simple RSS aggregation workflow into a quick local reading desk. Its design keeps the interface quiet and information-dense: source, title, time, and destination are visible in one symmetric row.

## Why it exists

The accompanying n8n workflow already performs the important data work—reading Hacker News and BBC News, normalizing fields, deduplicating links, and sorting stories. Signal makes that output easy to scan in a browser without requiring a hosted service or a database.

## Design principles

1. Show the newest information first.
2. Keep both sources equally represented.
3. Make the first screen useful without scrolling through cards.
4. Respect operating-system appearance preferences.
5. Keep the runtime small, inspectable, and easy to run locally.

## Scope

Signal is intentionally a local dashboard, not a replacement for n8n. It does not publish, edit, or redistribute source content; links open at their original publishers.
