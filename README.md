# ✍️ Sheba Protocol — Write-Up Activity

![Team](https://img.shields.io/badge/Team-Queen%20Sheba%20Protocol-2563EB?style=flat-square)
![Type](https://img.shields.io/badge/Type-Writeups-8B5CF6?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-22C55E?style=flat-square)

Formal, polished writeups from CTF challenges, vulnerability research, and security exercises completed by **Queen Sheba Protocol** members. This is the "publish-ready" repo — content here should be clear enough for someone outside the team to read and learn from.

---

## 🎯 Purpose

- Turn raw CTF/practice notes (from `CTF-Activity`) into clean, structured writeups
- Build each member's public-facing portfolio material (many of these can be posted to Medium, a personal blog, or LinkedIn later)
- Create a team knowledge base of vulnerability classes and techniques, written well enough to actually teach from

**This repo is for quality over speed.** Rough in-progress notes belong in `CTF-Activity` — move a piece here only once it's writeup-ready.

---

## 📂 Structure

```
Sheba-protocol-Write-Up-Activity/
├── README.md
└── writeups/
    ├── awel/
    │   ├── 2026-09-sql-injection-portswigger.md
    │   └── 2026-09-idor-htb-machine.md
    ├── eyuel/
    └── ...
```

- One folder per member
- One file per writeup, named descriptively: `YYYY-MM-<short-topic-slug>.md`

---

## 🧾 Writeup Template

```markdown
# <Title — e.g. "Exploiting Blind SQL Injection in a Login Form">

**Author:** <Your Name>
**Date:** YYYY-MM-DD
**Category:** Web / Network / Reverse Engineering / Cloud / Other
**Source:** PortSwigger Lab / HTB Machine / Live CTF / Independent Research

## Summary
One or two sentences on what the vulnerability was and why it mattered.

## Background
Brief context — what the target was, what it's built with, why this class of bug is common.

## Steps to Reproduce
1. 
2. 
3. 

## Root Cause
Why the vulnerability existed — the underlying mistake in code or config.

## Impact
What an attacker could actually achieve with this.

## Remediation
How this should be fixed, in general terms.

## Lessons Learned
What you'd apply to your own future testing or code review.
```

---

## 🏷️ Labels (for tracking writeup status via Issues, optional)

| Label | Use |
|---|---|
| `draft` | Writeup started but not finished |
| `ready-for-review` | Ready for a teammate/mentor to review |
| `published` | Posted externally (blog, Medium, etc.) |
| `needs-diagrams` | Would benefit from a visual/diagram |

---

## ✅ Contribution Rules

- Write for a reader who wasn't there — explain acronyms and context, don't assume shared memory
- No live/unpatched vulnerabilities in real production systems — CTF labs, HTB/THM machines, and disclosed research only
- Credit the platform/source clearly at the top of every writeup
- Once published externally, add the `published` label and link it in the file

---

## 🔗 Related Repos

| Repo | Purpose |
|---|---|
| `Sheba-protocol-Daily-Progress-Tracker` | Daily/weekly logs and commit tracking |
| `Sheba-protocol-Write-Up-Activity` | *(this repo)* Formal, polished writeups |
| `Sheba-protocol-Project-Activity` | Longer-term tools and projects |
| `Sheba-protocol-CTF-Activity` | Live CTF and practice logs |
