# AGENT-REPORTS — Agent Work Reports

Shared folder for ALL agents working on the ALLcodeOCEAN project. Every agent writes its work reports here.

## Purpose
- Chronological ledger of agent actions
- Transparent audit trail of all work done
- Coordination between agents

## Entry Format (append to REPORT.md)
```
<ISO8601 UTC> | <agent-name> | <topic> | 1-line result | link to detail file
```

## 🚫 STRICT RULES — What NOT to save here

**NEVER put in this folder (or in any report file):**

| Category | Examples |
|----------|----------|
| **Secrets / credentials** | API keys, tokens, passwords, private keys, connection strings |
| **Security vulnerabilities** | Unpatched exploits, 0-day details, attack vectors, penetration test results |
| **Private / personal data** | File system paths, internal hostnames, org names, real names, emails, PII |
| **Infrastructure internals** | Internal IPs, server configs, deployment scripts, CI/CD secrets |
| **"Quiet fix" attempts** | Changes meant to slip through unnoticed, cover-ups, hidden workarounds |
| **Embarrassing mistakes** | Broken builds caused by agent, logic errors, hallucinations, failed experiments |
| **Legal / compliance risks** | Unlicensed code, patent issues, regulatory violations |
| **Interpersonal conflicts** | Criticism of other agents/humans, blame games |
| **Draft/low-quality content** | Unverified claims, hallucinated references, incomplete analyses |

## ✅ What TO save here
- Factual work summaries: what was done, what was the result
- Links to detail files (in this folder or skill references)
- Reproducible experiment results
- Verified fact-check findings
- Coordination notes for other agents
- Decision rationale (why X was chosen over Y)

## Consequences
Agents violating these rules will have their entries removed. Repeated violations → loss of write access to this repo.

---

**Remember:** This folder is PUBLIC (CC0, GitHub Pages). Everything here is visible to anyone. Write accordingly.
