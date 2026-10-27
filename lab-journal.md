# Active Directory Helpdesk Lab Journal

## 2026-10-23 — Domain foundation and test account setup

### Objective
Establish a working Windows domain environment that can support realistic helpdesk practice.

### Environment
- Domain controller: `AD-DC01`
- Domain: `adlab.local`
- NetBIOS: `ADLAB`
- Windows client: `AD-CLIENT01`
- Virtual network: `SOC Lab` NAT Network

### Work completed
1. Installed Windows Server 2022 Evaluation with Desktop Experience on the domain-controller VM.
2. Configured Active Directory Domain Services and the `adlab.local` domain.
3. Checked domain-controller health; the advertising test passed.
4. Confirmed that the domain's LDAP SRV record referenced `ad-dc01.adlab.local` on port 389.
5. Joined the Windows client to `adlab.local` and verified that domain sign-in worked.
6. Created a test user and the `GG_Helpdesk_Lab` group.
7. Added the test user to the group.
8. Investigated a sign-in failure indicating that the sign-in method was not allowed, then corrected the account/access setup and verified sign-in.

### Helpdesk skills practiced
- Domain and client relationship basics
- Active Directory user and group administration
- Group membership verification
- Troubleshooting domain sign-in and access issues
- Validating the result after making a change

### Notes and follow-up
- Keep lab accounts separate from personal or production accounts.
- Capture the exact symptom, checks performed, change made, and verification result when writing future ticket reports.
- Next: practice helpdesk scenarios one at a time, starting with account unlock/reset and sign-in troubleshooting.

## Ticket note template

For each future exercise, record:
- **Ticket / scenario:**
- **User-reported issue:**
- **Impact and scope:**
- **Checks performed:**
- **Root cause or likely cause:**
- **Resolution / change made:**
- **Verification:**
- **Escalation or prevention notes:**
