# Bila UiTM Cuti — Grok Bot

![Bila UiTM Cuti by Shahrul](https://x.ai/bot/NdfYE7nsqkzFLbgVmWx1U/opengraph-image-bntnog?ff10f2afb2aeb68b)

A UiTM academic calendar assistant built on [Grok Bot](https://x.ai/bot), giving students live answers about lectures, cuti (semester breaks), exams, registration periods, and Malaysia public holidays — right inside Grok.

**Add it here:** https://x.ai/bot/NdfYE7nsqkzFLbgVmWx1U

## What it does

- Answers questions about UiTM academic dates: lecture weeks, cuti, exam periods, registration windows, and public holidays.
- On first use, asks whether you're in **Group A** or **Group B**. Group A has only one program, so the bot resolves it automatically without asking further.
- Defaults to the **current academic session**, but you can ask about upcoming or past sessions anytime.
- Talks in casual **Bahasa Malaysia / English**, the way students actually text.
- Never guesses — every date is pulled live from a custom remote data source (see below), not from the model's memory.

## How it works

This bot is a **Grok Bot template** connected to a custom **remote MCP server**:

```
https://mcp.bilauitmcuti.com/mcp
```

Grok Bot calls this MCP endpoint on every relevant question to fetch live, up-to-date academic calendar data instead of relying on the model's own (potentially outdated) knowledge. The MCP server is backed by the same data powering [bilauitmcuti.com](https://bilauitmcuti.com).

## What is Grok Bot?

Grok Bot is xAI's platform for AI "teammates" — persistent, named agents you give real work to, not just a chat window you type into.

Each Bot runs on its own persistent cloud computer with a browser, filesystem, and terminal, so it can use connectors/MCP servers or operate apps and websites directly, and actually finish tasks in real tools rather than just handing back chat drafts. Bots keep memory, files, browser sessions, and preferences across turns, so context builds up over time instead of resetting on every task. Multiple Bots can also coordinate with each other, sharing context and handing off work, and can learn a multi-step workflow just by being shown it once, then re-run it later as a routine.

For this project, the Bila UiTM Cuti Bot is a narrower case: a single-purpose Bot wired to one remote MCP server so it always answers academic calendar questions from live data instead of guessing.

Bots on the platform are built by third-party creators, not by xAI/SpaceXAI itself — this one was created independently by Shahrul as part of the Bila UiTM Cuti project.

## Related

- **Calendar:** [bilauitmcuti.com](https://bilauitmcuti.com)

## Disclaimer

This is an unofficial, student-built tool and is not affiliated with UiTM. Always double-check critical dates (exam registration, etc.) against official UiTM sources.
