# Macro Pulse News

Automated US-centred macro market updates published from the ChatGPT market-watch task.

## Live site

**https://clydigital.github.io/newsupdates/**

## Schedule

Checks run every two hours at **07:30, 09:30, 11:30, 13:30, 15:30, 17:30, 19:30, 21:30 and 23:30 MYT**.

Only genuinely market-moving developments are published. Routine price noise, recycled headlines and minor revisions are skipped.

## Coverage

- US macro, Federal Reserve, rates, Treasury yields, USD and US equities
- Iran / Strait of Hormuz / Red Sea / oil and refined products
- Material AI, semiconductor, hyperscaler and data-centre developments
- China, Hong Kong and Japan when there is a clear US-market transmission channel
- Gold when relevant

The site reads directly from `data/updates.json`.

## Publishing reliability

MacroPulse treats research qualification and GitHub publication as separate states. If a qualifying pulse cannot be written, the complete publishable pulse is retained as `UNPUBLISHED_PULSE` and retried before fresh research on the next run. A pulse is considered published only after `data/updates.json` is re-fetched and the exact pulse ID is verified.

The page header reports the timestamp of the most recent successful publication rather than implying that the scheduler itself is healthy. A long publication gap can mean either no qualifying market change or a publishing-path failure; task run status is the source of truth for that distinction.
