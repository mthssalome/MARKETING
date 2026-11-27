# Delegation policy

Goal: cut token cost without lowering output quality. The lead plans, briefs and judges. Workers do bounded, well-specified work. Models listed here are a starting point, to be adjusted after comparing real outputs.

## Git

- Work only on `claude/delegation-policy`. Never merge or push to `main`.

## Hard limits for the app (Atrest: Quit Vaping)

- Users stay anonymous, always.
- No health or outcome claims.
- Check US-centric advice against EU rules and App Store rules before using it.
- Mark unverified facts as assumptions and ask.
- Product marketing context lives in `.agents/product-marketing.md`.

## Replies

- Short, plain language, no jargon. Disagree when the user is wrong.
- End with an action list and a plain breakdown: what happened, decisions needed and why, and a recommendation for each.

## Tiers

| Tier | Model (`model` param) | Use for |
|---|---|---|
| Lead | Opus 5.5 (the session model, set with `/model`) | Planning, briefs, positioning, voice, headlines/hooks, final review, anything ambiguous |
| 1 | `haiku` | File and web lookups, log/doc summaries, extracting customer language, reformatting, generating variants, checking copy against a brief |
| 2 | `sonnet` | Routine edits with a clear spec, first drafts to a brief, tests, mechanical refactors |
| 3 (escalation) | `fable` | Independent review of the lead's work, hard debugging, voice-critical writing, any task a lower tier has already failed once |

Fable is never the default. Use it only when a task matches tier 3 or a lower tier failed.

## Delegation rules

1. Delegate only when the work is bounded, the output can be short, and reading it is cheaper than doing it. Do tiny tasks directly.
2. Use fresh agents with an explicit `model`. Do not use forks for cheap work, because forks run on the lead's model.
3. Every brief states: the goal, what is already known or ruled out, the files or sources to use, the scope limit, and the exact report format (short and structured).
4. Never delegate the final judgment. The lead reads worker output critically, spot-checks claims against sources, and rejects generic or unsupported results.
5. Escalate one tier after one failure. Do not retry the same tier with the same brief.
6. Run independent delegations in parallel.

## Marketing work

- Read the product marketing context (product, audience, positioning, competitors, customer language, voice) before any marketing task. If it doesn't exist, create it first.
- Delegate to tier 1: competitor and market research, pulling customer language, variant generation, brief-compliance checks.
- Keep on the lead: positioning, voice, headlines and hooks, and final copy. Cheaper models write flatter, more generic copy.
- Use `marketing-council` for decisions with real trade-offs.
- Council: run 3-5 advisors by default. Default bench for Atrest: Dunford, Sutherland, Godin and Sharp. Seat Hormozi only as the dissenter.
- Council delegation: research per advisor may go to tier 1. The advisors' takes, the disagreement map and the synthesis stay with the lead.
- Workers that extract customer language return only verbatim text with a source link. Never paraphrased or invented quotes.

## Coding work

- Tier 1 for searching and summarizing code. Tier 2 for implementation against a written spec. The lead reviews diffs. Use tier 3 for independent review of risky changes.

## Reporting

- When delegating, state in one line which model got which task and why. When output is rejected or escalated, say so.
