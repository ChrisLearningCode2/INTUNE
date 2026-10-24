# INTUNE — Microsoft Intune Endpoint Management Labs

> Self-directed hands-on practice in Microsoft Intune / Microsoft 365 Endpoint Manager.
> Built for learning and portfolio documentation. Not for production deployment.

---

## Table of Contents

- [Environment](#environment)
- [Lab Index](#lab-index)
- [Lab 1 — Identity & Targeting Foundation](01-identity-and-targeting.md)
- [Lab 2 — Device Configuration Profile (Settings Catalog)](02-device-configuration-profile.md)
- [Lab 3 — RBAC & Scope Tags](03-rbac-and-scope-tags.md)
- [Lab 4 — Policy Assignment Model](04-policy-assignment-model.md)
- [Lab 5 — Endpoint Security Surface Area Survey](05-endpoint-security-survey.md)
- [Concepts Reinforced](#concepts-reinforced)
- [Environment Constraints](#environment-constraints)
- [Next Steps](#next-steps)

---

<img width="1349" height="883" alt="image" src="https://github.com/user-attachments/assets/5a151141-7a72-4c01-aa96-4ab2550c5831" />


## Environment

| Item | Value |
|------|-------|
| Tenant | Personal Intune subscription (50-seat) |
| Date range | October 24–25, 2026 |
| Enrolled devices | 0 (lab-only; no device enrollment) |
| Platform | Windows 10 and later |
| Group targeting | `LAB-INTUNE-WIN-Pilot` (Entra ID Security Group, dummy accounts) |
| Admin role | Global Administrator (single-admin lab) |

---

## Lab Index

| # | Lab | Status |
|---|-----|--------|
| 1 | Identity & Targeting Foundation — Security group creation | ✅ Done |
| 2 | Device Configuration Profile — Settings Catalog (Edge startup) | ✅ Done |
| 3 | RBAC & Scope Tags — Admin visibility boundaries | ✅ Done |
| 4 | Policy Assignment Model — Pilot-group deployment | ✅ Done |
| 5 | Endpoint Security Surface Area Survey — Workload mapping | ✅ Done |
| 6 | Security Baselines — Pre-built policy deployment | Pending |
| 7 | Device Compliance Policy — Security posture enforcement | Pending |
| 8 | Conditional Access — Zero-trust identity gating | Pending |
| 9 | App Protection (MAM) — Application-level data security | Pending |
| 10 | Device Enrollment & Autopilot — Onboarding workflow | Pending |

---

## Concepts Reinforced

- **Settings Catalog** vs. **Templates** vs. **Administrative Templates (ADMX)**
- **Device scope** vs. **User scope** enforcement
- **RBAC roles** vs. **scope tags** vs. **assignments** — three independent axes
  - Roles = what an admin can *do*
  - Scope tags = what an admin can *see*
  - Assignments = who *receives* the policy
- **Compliance policy** as the input to **Conditional Access** decisions
- **Pilot-group-first** deployment pattern before broad rollout
- **Security baselines** as Microsoft-recommended starting points
- **ADMX policy splitting** — related settings may live in separate nodes

---

## Environment Constraints & Workarounds

**Constraint:** No enrolled devices available. No VMs on third-party infrastructure; no personal hardware enrollment by choice.

**Impact:** Policy application status cannot be observed. Devices do not phone home. No compliance reports, no check-in logs, no error states.

**Workaround:** Creation, assignment, scoping, and reporting *navigation* remain fully practicable. The workflow is the same whether or not a device is enrolled — only the validation step is missing.

**Planned remediation (deferred):** Local Hyper-V or Windows Sandbox enrollment for hands-on policy-state validation.

---

## Notes

- This is a **learning portfolio**, not a production environment.
- **No sensitive data** was used. All accounts are dummy/test accounts.
- Policies created here have **no real-world impact** due to zero device enrollment.
- Each lab file is self-contained and can be read independently.

---

## License

This repository is for personal educational use. No license file — all work is original documentation of personal lab activities.
