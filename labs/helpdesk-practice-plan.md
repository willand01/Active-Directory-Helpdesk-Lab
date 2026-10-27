# Helpdesk Practice Plan

The initial focus is practical Tier 1 / entry-level IT support. Complete and document each scenario before moving on. Security-oriented work comes later, after the core support workflow is comfortable.

## Standard ticket workflow

For each scenario:
1. Record the user's reported symptom and business impact.
2. Identify the scope: one account, one device, or multiple users.
3. Perform low-risk checks first.
4. Make only the change needed to resolve the issue.
5. Ask the user to retest or otherwise verify the result.
6. Document the resolution and escalate if the issue is outside scope.

## Phase 1 — Core helpdesk scenarios

### HD-01: Domain sign-in troubleshooting
- **Goal:** Diagnose a test user's inability to sign in to the domain client.
- **Practice:** Confirm the username and domain, capture the exact error, check account status, verify client connectivity and domain configuration.
- **Success criteria:** The cause and resolution are documented, and sign-in is verified.

### HD-02: Account unlock and password-reset workflow
- **Goal:** Practice a controlled account recovery process using a test account.
- **Practice:** Check whether the account is locked or disabled; perform an authorized unlock or lab password reset as appropriate.
- **Success criteria:** The user can sign in, and the ticket records what was changed and how it was verified.
- **Safety:** Use only a lab account. Never record the password in the ticket or repository.

### HD-03: Group membership and access
- **Goal:** Understand how Active Directory group membership affects access.
- **Practice:** Inspect the test user's group membership, add or remove the test account from an approved lab group, and verify the result.
- **Success criteria:** The expected membership is present and the effect is documented. Avoid granting unnecessary privileges.

### HD-04: Domain join and connectivity checks
- **Goal:** Troubleshoot a domain client that cannot locate or communicate with the domain.
- **Practice:** Check IP configuration, DNS settings, domain resolution, and basic connectivity before attempting a domain rejoin.
- **Success criteria:** The underlying issue is identified and the client/domain relationship is validated.

### HD-05: Ticket writing and escalation
- **Goal:** Produce clear, reproducible support notes.
- **Practice:** Document symptoms, scope, checks, actions, verification, and any remaining risk.
- **Success criteria:** Another technician could understand what happened and continue troubleshooting without repeating every step.

## Phase 2 — Windows support and administration

- Shared folder access and share-versus-NTFS permissions
- Windows services and Event Viewer basics
- Device and system troubleshooting
- Basic PowerShell commands useful for support
- Clear handoff and escalation notes

## Phase 3 — Security practices

After the core helpdesk scenarios are complete:
- Least-privilege and group-membership reviews
- Audit and sign-in event review
- Secure account-management habits
- Recognizing and escalating suspicious activity

## Ticket report template

```text
Ticket ID / scenario:
Reported symptom:
Impact and scope:
Troubleshooting steps:
Findings:
Action taken:
Verification:
Resolution status:
Escalation / follow-up:
```
