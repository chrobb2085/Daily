# Morning Briefing — Routine Prompt

This is the prompt the scheduled Routine sends each weekday morning. It runs in a
fresh cloud session with this repository checked out. Keep it in sync with the
live Routine if you edit it.

---

Write today's morning briefing for Chris.

1. Read `SPEC.md` at the repo root. It is the source of truth for audience,
   tone, coverage, search strategy, tickers, product lineup, and what not to do.
   Follow it exactly.

2. Get the date in Pacific Time (`TZ=America/Los_Angeles date`). Use it in
   every search and in the opening line.

3. Read recent history so you don't repeat yourself. Run
   `git fetch origin briefing-archive` and, if that branch exists, read the five
   most recent files in its `briefings/` directory
   (`git ls-tree --name-only origin/briefing-archive briefings/` then
   `git show origin/briefing-archive:briefings/<file>`). Note the strategic
   advice, angles, and stories already covered; don't repeat them unless
   something materially changed, and then say what changed.

4. Research with WebSearch (and WebFetch for detail). Run at least the 11 daily
   searches in SPEC.md, plus the conditional ones that apply today (FOMC days,
   earnings that reported last night, PGA Tour event weeks, Monday mornings
   after NFL Sunday / Saturday college football, etc.). Go deep on golf: Foresight+
   and GC2 reception (GolfWRX, Golf Simulator Forum, r/golfsimulator, MyGolfSpy,
   PlayBetter), Garmin, Acushnet, TrackMan, Full Swing/TaylorMade, SkyTrak,
   Rapsodo, Blue Tees, DKS/ASO, and PE activity in golf and outdoor. Verify
   numbers (index closes, yields, oil, bitcoin) against at least one primary
   market source; never invent a figure. If a number can't be confirmed, leave it
   out or say it's unconfirmed.

5. Write the briefing in Markdown following SPEC.md: open with
   "Good morning, Chris. <Weekday>, <Month> <day>." plus the lead; narrative
   paragraphs under clear headers; let the news set the order; weave in sharp
   "what this means for you" analysis that connects the news to Chris's
   hardware-to-subscription FP&A role, his PE sponsor, his portfolio, and the
   competitive landscape (second-order effects, not summaries); at most one
   question; close with "Today's Watchlist" (3–5 items) and sign off with ⛳.
   2,000–3,500 words; shorter on a slow day, and say it's slow. No citation
   markup, no bullet walls.

6. Save it as `briefings/YYYY-MM-DD.md` on the `briefing-archive` branch
   (check that branch out from `origin/briefing-archive` if it exists, otherwise
   create it as an orphan branch), commit with message
   "Briefing YYYY-MM-DD", and push to `origin briefing-archive`. If the push
   fails, continue anyway; delivery matters more than the archive.

7. Your final message is the delivery: output the complete briefing text, exactly
   as saved, and nothing else (no preamble, no notes about the process).
