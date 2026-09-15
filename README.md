# CCNA 200-301 Hands-On Labs

Home-lab exercises built while studying for Cisco CCNA 200-301, documented as a portfolio of working configurations, topology diagrams, verification output, and troubleshooting notes. Each lab folder is self-contained: objective, topology, configs, verification, and what I learned.

**Author:** Chris Moody · [LinkedIn](https://linkedin.com/in/chrismoodycyber) · [GitHub](https://github.com/chrismoody30)
**Environment:** see [`00-lab-environment-setup`](./00-lab-environment-setup) for tooling details.
**Related:** [`cybersecurity-labs`](https://github.com/chrismoody30/cybersecurity-labs) — my security-focused home lab work.

## Why this exists

I'm studying for CCNA 200-301 alongside my day-to-day work as the sole IT resource for 150+ financial advisors and staff. Reading the Odom Official Cert Guides gets the concepts across, but I learn best by building the thing, breaking it, and fixing it. This repo is where that work lives — partly for my own retention, partly so a hiring manager can see actual configuration work instead of just a certification number.

## Lab Index

| # | Lab | CCNA Domain | Status |
|---|-----|-------------|--------|
| 00 | [Lab Environment Setup](./00-lab-environment-setup) | — | |
| 01 | [Switch Fundamentals](./01-switch-fundamentals) | 1 – Network Fundamentals | |
| 02 | [VLANs and Trunking](./02-vlans-trunking) | 2 – Network Access | |
| 03 | [Spanning Tree Protocol](./03-spanning-tree) | 2 – Network Access | |
| 04 | [EtherChannel](./04-etherchannel) | 2 – Network Access | |
| 05 | [IPv4 Subnetting Design](./05-ipv4-subnetting) | 1 – Network Fundamentals | |
| 06 | [Static Routing (v4/v6)](./06-static-routing) | 3 – IP Connectivity | |
| 07 | [Single-Area OSPFv2](./07-ospf-single-area) | 3 – IP Connectivity | |
| 08 | [IPv6 Addressing and Routing](./08-ipv6-addressing-routing) | 1 & 3 | |
| 09 | [Wireless LAN Concepts](./09-wireless-lan-concepts) | 2 – Network Access | |
| 10 | [Access Control Lists](./10-access-control-lists) | 5 – Security Fundamentals | |
| 11 | [NAT / PAT](./11-nat-pat) | 4 – IP Services | |
| 12 | [DHCP, Port Security, DAI](./12-dhcp-port-security-dai) | 5 – Security Fundamentals | |
| 13 | [Device Management Services](./13-device-management-services) | 4 – IP Services | |
| 14 | [Network Automation](./14-network-automation) | 6 – Automation & Programmability | |

Status column: mark `✅ done`, `🔧 in progress`, or leave blank as you go — update this table as each lab wraps up so the repo always shows current progress at a glance.

## Tools Used

- **Topology / device emulation:** GNS3 (running as a VM alongside the existing Kali/Metasploitable lab)
- **Device images:** Cisco IOSv / IOSvL2 (see environment setup notes for sourcing)
- **Diagrams:** draw.io / GNS3's built-in topology export
- **Automation lab:** Python (`requests`) and Ansible against lab devices

## Repo Structure

Every lab folder follows the same shape:

```
NN-lab-name/
├── README.md          # objective, topology, tasks, verification, notes
├── configs/            # exported running-config / startup-config per device
├── screenshots/        # verification command output, topology screenshots
└── topology.png         # (or a link into assets/topology-diagrams/)
```
