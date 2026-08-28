# n8n Workflow Notes

Input: `RSS Feed Aggregator (1).json`

The workflow contains:

- Hourly trigger
- Hacker News RSS reader
- BBC News RSS reader
- One normalization node per source
- Merge node
- Sort and deduplicate function

The local dashboard mirrors the final normalized fields: `title`, `link`, `date`, and `source`. The browser dashboard adds a per-source six-item limit so the feed is balanced at 6 + 6.
