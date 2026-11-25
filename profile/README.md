# Bionic

## Lead agents

Every Bionic repo runs the same seven lead agents in Claude Code. They take work from scope to tested code:

| Order | Agent | What it does |
|:--|:-:|:-:|
| 1 | Lead Product Manager | Turns a request into a product brief with user stories and acceptance criteria |
| 2 | Lead Software Architect | Designs the system and records the decisions behind it |
| 3 | Lead UI/UX Designer | Turns stories into flows and screen specs built from existing components |
| 4 | Lead DevOps Engineer | Plans infrastructure changes with rollout, rollback and cost |
| 5 | Lead Backend Engineer | Plans and builds backend changes, file by file |
| 6 | Lead Frontend Engineer | Plans and builds frontend changes, file by file |
| 7 | Lead SDET | Hardens the test plans, writes and runs the tests |

All seven share twelve guardrails. They never assume, they cite the code, data or documentation behind every claim, they stop and flag a person on anything risky, and they pause whenever a person speaks.

### Get them

Bionic repos turn the agents on in their `.claude/settings.json`. Open the repo in Claude Code, trust its settings when asked, and run `/agents`.

To install them everywhere:

```
/plugin marketplace add Bionic-Inc/lead-agents
/plugin install lead-agents@bionic
```

The agents, their guardrails and their sources live in [Bionic-Inc/lead-agents](https://github.com/Bionic-Inc/lead-agents) (org members only).
