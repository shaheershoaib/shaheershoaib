<h1 align="center">Shaheer Shoaib</h1>

<p align="center">
  <em>Everyone is shipping gas. I build brakes.</em>
</p>

---

AI writes the code now. The interesting problem moved: it's no longer *can the agent
produce a change*, it's **can you trust the change it says it made**.

An agent that types "Fixed ✅" has given you a claim, not evidence. It ran the tests,
saw green, and closed the ticket — and the bug is still there, because the test
exercised the wrong thing, or the fix landed on the wrong surface, or it patched the
symptom instead of the cause.

Almost everything I build is some version of the referee for that: tooling that
re-proves an agent's work instead of taking its word, and that makes the invisible
parts of an agent setup visible.

## Projects

| | |
|---|---|
| **[receipts](https://github.com/shaheershoaib/receipts)** | A verification layer for AI-written code. The Gates — a standard a fix must clear — plus a Claude Code adapter, a CI enforcer, and verification memory. An agent can fake a screenshot; it can't fake the reported symptom still being there when `receipts` re-runs it. |
| **[system-explainer](https://github.com/shaheershoaib/system-explainer)** | Teaches how an unfamiliar system actually works, generates an interactive onboarding course from a repo, then *proves the course is true* — every snippet grounded against source, every claim adversarially checked, teaching measured with a simulated learner. |
| **[fanout](https://github.com/shaheershoaib/fanout)** | Decides what coding work can run in parallel, what has to serialize, and in what order — then runs it. Stdlib Python, zero dependencies, any agent runtime. |
| **[design-audit](https://github.com/shaheershoaib/design-audit)** | Extracts the design system a codebase *already has* and writes it down. Strictly observational: if `#dddcd5` is what ships, `#dddcd5` is what the audit shows. The fragmentation is the finding. |
| **[setup-audit](https://github.com/shaheershoaib/setup-audit)** | Agent setups fail open — a skill with a malformed frontmatter never loads, and nothing tells you. A dependency-free health check for `~/.claude`, with drift detection against a known-good snapshot. |

## The through-line

Three ideas show up in everything above:

**Absence is a finding.** A skill that didn't load, a pattern the repo doesn't
implement, a test that never ran — the negative result is information, and it should
be reported with the evidence that produced it, not silently omitted.

**Don't let the thing grade its own homework.** Verification has to be re-run by
something that isn't the agent, against the real build, or it isn't verification.

**Describe before you prescribe.** Most tools want to hand you a new system. You can't
choose what to change until someone has honestly written down what you have.

## Elsewhere

Most of my working hours go to full-stack product work — PHP on the server, JS on the
front, and the unglamorous integration layer where most real software actually lives.
The tools above came out of that, not the other way around.

<p align="center">
  <a href="mailto:shaheershoaib11@gmail.com">
    <img src="https://img.shields.io/badge/email-shaheershoaib11%40gmail.com-0b0b0b?style=flat-square&logo=gmail&logoColor=white" alt="Email">
  </a>
</p>
