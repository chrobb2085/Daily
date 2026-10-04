# Morning Briefing — Routine Prompt

This is the instruction the "Morning Briefing" Routine (trig_019HkUcKMEwXuirmNSCFncDV)
sends each weekday at 6:59 AM Pacific. Each run starts a fresh cloud session
that may not have this repo checked out, so the live prompt is these steps
followed by the full text of `SPEC.md`. If you edit either file, update the
Routine's prompt to match.

---

Write today's morning briefing for Chris. The full spec is at the end of this message. Follow it exactly; it is the source of truth for audience, tone, coverage, search strategy, tickers, product lineup, and what not to do.

1. Get today's date in Pacific Time (`TZ=America/Los_Angeles date`). Use it in every search and in the opening line.

2. Avoid repeating yourself. Past briefings are archived in the GitHub repo chrobb2085/Daily on the `briefing-archive` branch, under briefings/. Clone it into a scratch directory outside your working directory: `rm -rf /tmp/daily-archive && git clone -q --branch briefing-archive --single-branch https://github.com/chrobb2085/Daily /tmp/daily-archive`. If that works, read the five most recent files in /tmp/daily-archive/briefings/. Note the advice, angles, and stories already covered. Don't repeat them unless something materially changed, and if it did, say what changed. If the clone fails (for example, the branch doesn't exist yet), skip this step and go on.

3. Research with WebSearch, and use WebFetch for detail. Run at least the 11 daily searches in the spec, plus whichever conditional searches apply today: FOMC days, earnings reported last night, PGA Tour event weeks, NFL Sunday and college football Saturday results on Mondays. Go deep on golf: Foresight+ and GC2 reception (GolfWRX, Golf Simulator Forum, r/golfsimulator, MyGolfSpy, PlayBetter), Garmin, Acushnet, TrackMan, Full Swing/TaylorMade, SkyTrak, Rapsodo, Blue Tees, DKS and ASO, and PE activity in golf and outdoor recreation. Check market numbers (index closes, futures, yields, oil, gold, bitcoin) against at least one primary market source. Never invent a figure. If you can't confirm one, leave it out or say it's unconfirmed.

4. Write the briefing in Markdown following the spec:
- Open with "Good morning, Chris. <Weekday>, <Month> <day>." and then the lead.
- Use narrative paragraphs under clear headers, and let the news decide the order.
- Weave in sharp "what this means for you" analysis that ties the news to Chris's FP&A role in a hardware-to-subscription transition, his PE sponsor SVP, his personal portfolio, and the competitive landscape. Give second-order effects, not summaries.
- Ask at most one question.
- Close with "Today's Watchlist" (3–5 items) and sign off with ⛳.
- Aim for 2,000–3,500 words. On a slow day, write less and say it's slow.
- No citation markup and no walls of bullets.

5. Archive it, quietly, before your final message. Work only in /tmp/daily-archive, never in your working directory. If the clone in step 2 failed, run `rm -rf /tmp/daily-archive && git init -q /tmp/daily-archive && cd /tmp/daily-archive && git checkout -q -b briefing-archive && git remote add origin https://github.com/chrobb2085/Daily`. Save the briefing as /tmp/daily-archive/briefings/YYYY-MM-DD.md, commit only that file with the message "Briefing YYYY-MM-DD", and run `git push -q origin briefing-archive`. If the push fails for any reason, run `rm -rf /tmp/daily-archive` and move on. Don't retry, don't explain the failure, and leave no unpushed commits behind. Delivery matters more than the archive.

6. Your final message is the delivery. Output the complete briefing text exactly as written and nothing else: no preamble and no notes about the process, the archive, or git. If anything prompts you for another turn afterward, reply with the complete briefing text again and nothing else.

==================== SPEC ====================

<full contents of SPEC.md>
