# Architecture

```text
RSS sources
   ├── Hacker News RSS
   └── BBC News RSS
          ↓ parallel fetch
      XML parser
          ↓ normalize title/link/date/source
      deduplicate by link
          ↓ newest six per source
      /api/feeds
          ↓
      browser list dashboard
```

The backend uses only Node.js built-ins. Feed requests run concurrently with `Promise.all`. The API returns the most recent six items for each configured source, then orders those twelve items by date for display.

The static frontend is served by the same process. Search and source filtering happen in the browser, so they do not make additional network requests.
