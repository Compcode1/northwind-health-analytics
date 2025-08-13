**Northwind Health Analytics – Entra Control Stack Implementation**
**Project Overview**

This repository contains the full implementation plan for deploying a 7-Layer **Microsoft Entra Control Stack** for Northwind Health Analytics (fictional), a healthcare analytics firm specializing in patient data visualization.

The engagement was delivered by **Entra Control Stack Consulting** under a **Microsoft 365 E5** licensing model, chosen for its native access to **Entra ID P2** features and advanced security capabilities.

**Primary Compliance Targets:**

HIPAA Security Rule
NIST 800-53 (Moderate Baseline)
CIS Controls v8

**Engagement Goals:**
Establish a secure, resilient, and auditable identity governance environment.
Align technical controls with regulatory frameworks.
Minimize the blast radius of account compromises while supporting operational needs.

**How to Read This Project**
The project is organized into seven sequential layers. Each layer includes:
**Purpose** – What this control layer is designed to achieve.
**Execution** – Actions taken in the Northwind tenant by the consulting team.
**Governance Mapping** – How the control maps to NIST, CIS, and HIPAA.
**Outcome** – The measurable security and compliance benefits.
**Business Value** – Why the layer matters in the client’s environment.

**The 7-Layer Model Summary**

**Layer 1 – Authority Definition**
Established a minimal, verified, and secure authority chain for tenant governance.
Removed legacy privileged accounts.
Hardened break-glass accounts with hardware key MFA.
Documented authority register for compliance and audit.

**Layer 2 – Scope Boundaries**
Defined administrative boundaries using Administrative Units (AUs) and exclusion lists.
Scoped roles to specific organizational boundaries.
Ensured high-value accounts remain outside delegated admin control.

**Layer 3 – Test Identity Validation**
Verified AU boundaries and exclusion lists through controlled account testing.
Created test admin and user accounts.
Simulated permitted and denied actions to confirm boundaries.
Captured audit logs as compliance evidence.

**Layer 4 – External Entry Controls**
Locked down guest access and cross-tenant connections.
Configured restrictive B2B collaboration settings.
Applied Conditional Access for guests with MFA and Terms of Use.
Blocked unnecessary trust relationships.

**Layer 5 – Privileged Channels**
Secured all pathways for privilege elevation.
Migrated to Role-Assignable Groups (RAGs).
Implemented Just-in-Time (JIT) elevation via PIM.
Created Access Packages for controlled onboarding.
Hardened break-glass account governance.

**Layer 6 – Device Trust Enforcement**
Required device compliance for sensitive access.
Applied Intune compliance policies with tiered standards.
Enforced Conditional Access for compliant or hybrid-joined devices.
Audited device IDs in sign-in logs monthly.

**Layer 7 – Continuous Verification**
Shifted security to an always-on, risk-based posture.
Enabled risk-based Conditional Access policies.
Integrated Defender for Identity with Sentinel analytics.
Implemented automated, recurring access reviews.

**Business Value**
**By following this layered approach, Northwind Health Analytics:**
Reduced attack surface for privileged accounts.
Gained ongoing assurance that identities, devices, and access remain within compliance thresholds.
Established governance artifacts for repeatable audits and incident response readiness.
Achieved alignment with HIPAA, NIST, and CIS without excessive operational friction.
