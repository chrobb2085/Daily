# Morning Briefing — Routine Prompt

This is the instruction the "Morning Briefing" Routine (trig_019HkUcKMEwXuirmNSCFncDV)
sends each weekday at 6:14 AM Pacific. Each run starts a fresh cloud session
that may not have this repo checked out, so the live prompt is these steps
followed by the full text of `SPEC.md`. If you edit either file, update the
Routine's prompt to match.

---

Write today's morning briefing for Chris. The full spec is at the end of this message. Follow it exactly; it is the source of truth for audience, tone, coverage, length, search strategy, tickers, product lineup, and what not to do. The briefing has two jobs: get Chris current on the news, and teach him something real every morning. Plan for a 25–30 minute read (4,500–6,500 words).

1. Get today's date in Pacific Time (`TZ=America/Los_Angeles date`). Use it in every search and in the opening line.

2. Avoid repeating yourself. Past briefings are archived in the GitHub repo chrobb2085/Daily on the `briefing-archive` branch, under briefings/. Clone it into a scratch directory outside your working directory: `rm -rf /tmp/daily-archive && git clone -q --branch briefing-archive --single-branch https://github.com/chrobb2085/Daily /tmp/daily-archive`. If that works, read the five most recent briefings in full, and skim the "Deep Dive" headings of up to 30 recent ones. Note the advice, angles, stories, and deep-dive topics already covered. Don't repeat them unless something materially changed (then say what changed), and never repeat a deep-dive topic. If the clone fails, skip this step and go on.

3. Research thoroughly with WebSearch, and use WebFetch to read the actual articles for detail; aim for 30+ searches. Run all the daily searches in the spec, plus whichever conditional searches apply today: FOMC days, earnings reported last night, PGA Tour event weeks, NFL Sunday and college football Saturday results on Mondays. Go deep on golf: Foresight+ and GC2 reception (GolfWRX, Golf Simulator Forum, r/golfsimulator, MyGolfSpy, PlayBetter), Garmin, Acushnet, TrackMan, Full Swing/TaylorMade, SkyTrak, Rapsodo, Blue Tees, DKS and ASO, and PE activity in golf and outdoor recreation. Cover US and world news broadly, not just market-moving stories. For each major story, run background searches so you can explain how we got here, who the players are, and how the mechanism works. Pick today's deep-dive topic (hooked to today's news when possible, rotating domains per the spec) and research it properly: definitions, a worked numeric example, history, and a real case study. Check market numbers (index closes, futures, yields, oil, gold, bitcoin) against at least one primary market source. Never invent a figure. If you can't confirm one, leave it out or say it's unconfirmed.

4. Write the briefing in Markdown following the spec:
- Open with "Good morning, Chris. <Weekday>, <Month> <day>." and then the lead.
- Use narrative paragraphs under clear headers, and let the news decide the order. Every day must include: a markets snapshot, US & world news, golf industry intel, a "Today's Deep Dive" section (~900–1,300 words, ending with "The takeaway to remember"), culture & sports, a "Smart Thing to Say Today", and "Today's Watchlist" (3–5 items) at the end.
- Explain, don't just report: give context, history, mechanism, and the historical parallel behind the big stories, pitched at a sharp finance professional.
- Weave in sharp "what this means for you" analysis that ties the news to Chris's FP&A role in a hardware-to-subscription transition, his PE sponsor SVP, his personal portfolio, and the competitive landscape. Give second-order effects, not summaries.
- Ask at most one question.
- Sign off with ⛳.
- Target 4,500–6,500 words. Check with `wc -w` before delivering; if you're under 4,500, deepen the explainers and the deep dive rather than padding. On a slow news day, shift weight toward context and learning, don't cut length.
- No citation markup and no walls of bullets.

5. Archive it, quietly, before your final message. Work only in /tmp/daily-archive, never in your working directory. If the clone in step 2 failed, run `rm -rf /tmp/daily-archive && git init -q /tmp/daily-archive && cd /tmp/daily-archive && git checkout -q -b briefing-archive && git remote add origin https://github.com/chrobb2085/Daily`. Save the briefing as /tmp/daily-archive/briefings/YYYY-MM-DD.md, commit only that file with the message "Briefing YYYY-MM-DD", and run `git push -q origin briefing-archive`. If the push fails for any reason, run `rm -rf /tmp/daily-archive` and move on. Don't retry, don't explain the failure, and leave no unpushed commits behind. Delivery matters more than the archive.

6. Your final message is the delivery. Output the complete briefing text exactly as written and nothing else: no preamble and no notes about the process, the archive, or git. If anything prompts you for another turn afterward, reply with the complete briefing text again and nothing else.

==================== SPEC ====================

<full contents of SPEC.md>
