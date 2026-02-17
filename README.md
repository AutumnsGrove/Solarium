# Solarium

*The celestial workshop. A room designed for light.*

---

Solarium is a private workbench for freelance security consulting. It sits at the edge of the grove, facing outward — toward client codebases, toward the work beyond.

This is where you gear up before an engagement. Where you debrief when you come back. The tools are within reach. The logbook is open. The Bestiary is on the desk in a shaft of afternoon sun.

---

## The Rooms

```
Solarium/
├── Antechamber/     The waiting room. New clients, initial inquiries,
│                    30-minute assessments. Engagements begin here.
│
├── Bench/           The workbench. Active client engagements.
│   └── [client]/    Each client gets their own space.
│
├── Dispatch/        The shipping room. Deliverables ready to go out —
│                    proposals, reports, final remediation packages.
│
├── Bodega/          The archive. Completed engagements. The records
│                    you can't afford to lose.
│
└── docs/            The documents. Templates, reference materials,
                     the Bestiary's marginalia. All at hand.
```

---

## The Pipeline

```
Antechamber → Bench → Dispatch → Bodega
  (intake)   (work)   (ship)   (archive)
```

The full engagement protocol lives in:
→ [`docs/freelance-engagement-runbook.md`](docs/freelance-engagement-runbook.md)

---

## The Documents

| Document | Purpose |
|----------|---------|
| [Engagement Runbook](docs/freelance-engagement-runbook.md) | 8-phase pipeline, start to finish |
| [Scope Cheat Sheet](docs/freelance-scope-cheatsheet.md) | 5-question gate, pricing rules, red flags |
| [Proposal Template](docs/freelance-proposal-template.md) | Client-facing proposal format |
| [Services Agreement](docs/freelance-services-agreement.md) | Contract template |
| [Portfolio Draft](docs/portfolio-page-draft.md) | Arbor hero + page body copy |
| [Naming Journey](docs/freelance-workbench-naming-journey.md) | How this workspace got its name |

---

## The Skills

The Bestiary lives in `.claude/skills/`. Key creatures for freelance work:

| Skill | When to Invoke |
|-------|---------------|
| `raven-investigate` | Full security audit — Phase 3 (audit) and Phase 7 (re-assess) |
| `osprey-appraise` | Turn the Raven's case file into a proposal — Phase 4 |
| `raccoon-audit` | Secret cleanup and rotation — Phase 6 |
| `turtle-harden` | Defense-in-depth hardening — Phase 6 |
| `spider-weave` | Auth system rebuilds — Phase 6 |
| `beaver-build` | Security regression tests — Phase 6 |
| `hawk-survey` | Deep dive when Raven finds a domain that needs more |

---

## Per-Engagement Structure

When a new engagement begins, create a client folder under `Bench/`:

```
Bench/
└── [client-name]-[YYYY-MM]/
    ├── case-file.md          Raven's security posture assessment
    ├── proposal.md           Filled Osprey proposal (from template)
    ├── agreement.md          Signed services agreement
    ├── notes.md              Working notes, client comms log
    └── before/               Snapshots before remediation
    └── after/                Snapshots after remediation
```

When the engagement closes, move the folder to `Bodega/`.

---

*`AutumnsGrove/Solarium` — a room designed for light.*
