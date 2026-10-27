# Active Directory Helpdesk Lab

A practical Windows and Active Directory home lab focused first on entry-level IT support and helpdesk workflows. Security-focused exercises will be added after the core support skills are documented.

## Lab environment

- **Virtualization:** Oracle VirtualBox
- **Domain controller:** AD-DC01
- **Operating system:** Windows Server 2022 Evaluation (Desktop Experience)
- **Domain:** `adlab.local`
- **NetBIOS name:** `ADLAB`
- **Client:** AD-CLIENT01 (Windows 11)
- **Virtual network:** SOC Lab NAT Network (`10.0.2.0/24`)
- **Domain controller IP:** `10.0.2.5` (lab address)
- **Client IP:** `10.0.2.6` (lab address)

These are private lab addresses and may change if the virtual network is reconfigured.

## Completed foundation

- Installed and configured a Windows Server domain controller.
- Verified Active Directory Domain Services and domain-controller advertising.
- Configured and tested the `adlab.local` domain.
- Joined the Windows client to the domain.
- Created a lab user and the `GG_Helpdesk_Lab` security group.
- Added the lab user to the helpdesk lab group.
- Practiced troubleshooting a domain sign-in issue.

## Documentation

- [Lab journal](lab-journal.md) — setup notes and completed milestones.
- [Architecture](docs/architecture.md) — virtual machines, network, and domain layout.
- [Helpdesk practice plan](labs/helpdesk-practice-plan.md) — staged practice tickets and skills checklist.

## Roadmap

### Phase 1 — Core helpdesk skills
- User sign-in troubleshooting
- Account lockout and password-reset workflows
- Group membership and access troubleshooting
- Domain join and basic DNS/connectivity checks
- Clear ticket notes, validation, and escalation

### Phase 2 — Windows support and administration
- Workstation inventory and basic troubleshooting
- Shared folders and NTFS/share permissions
- Services, Event Viewer, and common Windows issues
- Basic PowerShell for support tasks

### Phase 3 — Security practices
- Least privilege and access reviews
- Audit logs and sign-in investigation
- Secure account-management procedures
- Documenting suspicious activity and escalation

## Safe lab practices

Use test accounts and non-production data only. Take VirtualBox snapshots before major configuration changes. Do not store real passwords, recovery codes, or other secrets in this repository.

This is a learning project; lab outcomes should be described accurately and not represented as production enterprise experience.
