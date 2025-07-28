# MikroTik DMZ + Cisco L3 Secure Intranet Setup

## 🌐 Scenario Overview

This setup demonstrates a real-world network design where:
- MikroTik acts as edge firewall/router + DMZ host
- Cisco Layer 3 switch handles intranet VLAN routing
- Intranet can reach Internet, but not the DMZ
- DMZ is publicly accessible, but isolated from Intranet

## 🧱 IP Addressing Plan

| Zone           | Subnet          | Gateway                |
|----------------|-----------------|------------------------|
| DMZ            | 172.17.0.0/24   | 172.17.0.1             |
| Intranet (V1)  | 192.168.1.0/24  | 192.168.1.1            |
| Intranet (V2)  | 192.168.2.0/24  | 192.168.2.1            |
| Intranet (V3)  | 192.168.3.0/24  | 192.168.3.1            |
| Transit        | 10.0.0.0/30     | .1 MikroTik / .2 Cisco |

## 🔒 Security Policy

- ✅ Intranet → Internet: Allowed
- ✅ DMZ → Internet: Allowed
- ❌ Intranet → DMZ: Blocked (Firewall)
- ❌ Internet → Intranet: Blocked
- ✅ Internet → DMZ (80/443): Allowed
