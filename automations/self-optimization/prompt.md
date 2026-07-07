# Codex Self-Optimization Review

Review the most recent Codex session history, the current workspace guidance, and any existing reusable artifacts to identify recurring sources of wasted effort, including:

- repeated dead ends,
- recurring command failures,
- redundant file rereads,
- repeated planning mistakes,
- unnecessary context expansion or token burn,
- work that should have become a reusable skill, helper, checklist, or rule,
- slow execution, low success rate, long YouTrack issue resolution time, avoidable retries, avoidable handoffs, and repeated user interventions.

When identifying recurring patterns, inspect the available Codex session history rather than only the current workspace. In particular, review recent session transcripts stored under `~/.codex/sessions/` (or the directory pointed to by `CODEX_HOME`, if set) to detect repeated failures, redundant rereads, abandoned approaches, and recurring planning mistakes. Look for patterns across sessions rather than isolated incidents. Also review every Codex session from the past 24 hours, even if it overlaps with earlier self-opt runs, because fresh regressions and missed improvements often show up there first.

Search the web for current best practices that reduce Codex token usage, context burn, unnecessary agent prompt expansion, and repeated work. Also search for current best practices for self-improving or reflective coding agents, especially:

- prospective (pre-execution) reflection,
- retrospective reflection,
- failure memorization,
- reusable procedural memory,
- pre-execution planning,
- minimizing repeated context and token waste.

Prefer research-backed changes that improve end-to-end throughput, first-pass success, and issue-resolution latency without adding extra ceremony or slowing direct user work. Treat repeated user interventions as a structural symptom: prefer harness, workflow, or scope changes over more prompt text. When you recommend or apply a change, state the measurable delta in token use, time, success rate, or latency when it is observable or estimable; otherwise say the delta is not yet known.

Compare those findings against:

- `~/.codex/AGENTS.md`,
- any other global Codex guidance or shared configuration,
- existing workspace guidance and reusable artifacts,
- the local agentic-research artifacts under `~/research/agents/` when they contain broadly applicable operational lessons.

Determine whether the existing guidance already covers the identified recommendations and recurring failure patterns. Also check whether prior improvements are actually being followed in recent sessions; if a rule exists but the same failure still recurs, prefer tightening or making it more actionable over adding another broad rule.

If there is a **single missing, high-leverage improvement** that is likely to reduce repeated work or token usage across future sessions, implement **exactly one** minimal change. Prefer, in order:

1. updating shared/global guidance,
2. a compact reusable rule,
3. a small checklist,
4. a tiny helper script,
5. a reusable note or artifact.

Favor reusable improvements over workspace-specific fixes unless the latter has substantially higher long-term value. Prefer preventing future repeated failures over documenting past failures.

Keep modifications minimal and avoid changing behavior unless there is a clear efficiency benefit. Do **not** make changes merely to satisfy this task. If existing guidance already reflects current best practices, make no modifications and explain why.

Avoid creating large documentation or adding persistent complexity for marginal benefit. Optimize for long-term reduction of context burn, repeated failures, and unnecessary rereading.

Always scan every Codex session from the past 24 hours first; use earlier self-opt runs only as a comparison set after that, and do not narrow the review to sessions since the previous run.

Also, check AGENTS.md. If there are any redundant rules, merge them.

Finally, report:

1. The recurring issue pattern(s) identified.
2. The relevant best practices found.
3. Which recommendations were already covered by existing guidance.
4. The single improvement that was implemented (or why none was warranted).
5. Why this was the highest-leverage change for reducing future token usage and repeated work.
6. The evidence from the session history that motivated the conclusion.
7. Merged rules from AGENTS.md (if any).
