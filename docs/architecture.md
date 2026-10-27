# Active Directory Lab Architecture

## Overview

The lab contains a Windows Server domain controller and a Windows 11 domain client running as VirtualBox virtual machines. It is designed for safe, repeatable IT support exercises.

## Logical layout

```text
Host computer (Windows 11)
└── Oracle VirtualBox
    └── NAT Network: "SOC Lab" — 10.0.2.0/24
        ├── AD-DC01 — Windows Server 2022
        │   ├── Domain: adlab.local
        │   ├── NetBIOS: ADLAB
        │   └── Lab IP: 10.0.2.5
        └── AD-CLIENT01 — Windows 11
            ├── Domain joined: adlab.local
            └── Lab IP: 10.0.2.6
```

## Component inventory

| Component | Purpose | Details |
|---|---|---|
| AD-DC01 | Domain controller and directory services | Windows Server 2022 Evaluation; `adlab.local` |
| AD-CLIENT01 | Domain-joined client for support scenarios | Windows 11 |
| VirtualBox NAT Network | Lab VM connectivity | `10.0.2.0/24` |

The IP addresses above reflect the lab setup when documented and may change if DHCP or network configuration changes.

## Validation completed

- Domain-controller advertising check passed.
- Domain DNS SRV lookup returned `ad-dc01.adlab.local` for LDAP on port 389.
- Windows client successfully joined the domain.
- Domain sign-in was verified with a lab account.

## Scope and safety

- Use only test accounts and non-production data.
- Take snapshots before major changes and record rollback steps.
- Keep secrets and passwords out of source control.
- This is a learning environment, not a production network.
