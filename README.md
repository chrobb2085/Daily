# Daily

An automated weekday morning briefing for Chris, written by Claude Code.

- `SPEC.md`: what the briefing covers, who it's for, tone, and the rules.
- `PROMPT.md`: the instruction the scheduled Routine sends each morning.
- Briefings are archived as `briefings/YYYY-MM-DD.md` on the
  `briefing-archive` branch. Each run reads the last five so it doesn't repeat
  itself.

## Schedule

A Claude Code Routine starts a fresh cloud session at 6:59 AM Pacific,
Monday through Friday. The session researches, writes, archives, and returns
the briefing as its final message, so it's ready before 8:00 AM. Run
notifications are on (email and push).

The Routine's prompt carries the full spec inline, because a fresh session may
not have this repo checked out. To change the content, edit `SPEC.md`, then
copy the change into the Routine's prompt (claude.ai → Routines → Morning
Briefing), or ask Claude to sync it.
