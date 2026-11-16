# Token-Burn Checklist — cap habits that keep a runaway agent from running up your bill

Every time your agent thinks, calls a tool, or retries a step, it spends tokens — and tokens are money. An agent with no caps will eventually loop: same failed step, retried all night, billed by the hour. These habits are the manual circuit breaker. Ten minutes to set up, two minutes a day to keep.

This checklist is the manual version of the caps our own agent runs under every day.

## Set your three numbers (once)

- [ ] **Daily cap.** Pick the most you are willing to spend in one day, in tokens or dollars, and set it where your provider or agent lets you set a hard limit. A cap you cannot set is not a cap — find the setting or use a tool that enforces it.
- [ ] **Per-hour cap.** A daily cap alone still lets an agent burn the whole day in one bad hour. Add an hourly ceiling so a loop trips fast, while you are awake to see it.
- [ ] **Loop limit.** Decide the most times the agent may retry the same step before it must stop and ask you. Three is a good start. "Keep trying until it works" is how bills happen.
- [ ] **Write the numbers down** in one place you will actually look — the top of your agent's notes file works.

## Make a tripwire (once)

- [ ] When a cap is hit, the agent **stops making new calls** — it does not finish "one more thing."
- [ ] The agent **logs why it stopped**: time, cap hit, what it was doing, how many retries it used.
- [ ] The agent **leaves the note where you will see it** — a plain alert file or a message to you, not buried in a debug log.

## Before you trust it (once per new setup)

- [ ] **Test with fake calls first.** Run the agent in test mode, or on a throwaway task, and watch it hit the cap on purpose. A breaker you have never seen trip is a hope, not a breaker.
- [ ] **Start tight.** Set the first week's caps lower than you think you need. Loosening a cap on purpose is a decision; raising one in a panic is not.

## Every day (two minutes)

- [ ] Glance at yesterday's usage. One number, no deep dive.
- [ ] If a cap tripped, read the log line before you reset anything.

## When a cap hits (do not skip steps)

- [ ] **Do not just raise the cap.** That teaches the loop nothing and pays for it twice.
- [ ] Read the log: what step looped, and why did the agent think retrying would help?
- [ ] Fix the cause — a clearer instruction, a missing permission, a smaller task — then reset the cap.
- [ ] If the same step trips twice in a week, lower its loop limit to 1 and make the agent ask you instead.

## Every week (five minutes)

- [ ] Look at the week's total next to last week's. Surprises are the thing you are hunting.
- [ ] If nothing tripped all week, tighten one number a little. Caps that never trip are set too high to protect you.
- [ ] Loosen a cap only on purpose, in writing, for a named job — never "just for now."

---

*Free sample from the Solopreneur Hardened Starter Vault — a pack of hardened skill files, guides, and adapter sheets for personal AI agent owners. The habits above work on their own; the Vault adds the per-skill limits, never-do lists, and stop-and-ask triggers that keep the work itself inside fences, not just the bill.*
