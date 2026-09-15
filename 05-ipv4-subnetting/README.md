# 05 — IPv4 Subnetting Design

**CCNA Domain:** 1 – Network Fundamentals · **Study plan reference:** Vol 1 Part IV (Ch. 11–14)

## Objective

This one is design-and-verify rather than pure CLI: take a single address block and subnet it to fit a realistic small-office requirement, then actually configure and verify it in the lab — closing the loop between the subnetting math and a working network.

## Scenario

Given `192.168.10.0/24`, design subnets for: Staff LAN (up to 50 hosts), Guest LAN (up to 20 hosts), a point-to-point WAN link between two routers, and a Management subnet (up to 10 hosts). Use VLSM to avoid wasting address space.

## Tasks

- [ ] Write out the full subnet plan on paper/markdown first: network address, mask (both dotted-decimal and CIDR), usable range, broadcast address, for each subnet
- [ ] Build the topology and assign the addresses accordingly
- [ ] Configure and verify reachability across all subnets via static or dynamic routing
- [ ] Deliberately compute one subnet wrong, configure it that way, and document the resulting symptom (e.g., hosts that can't reach their gateway) before fixing it

## Deliverable

`subnet-plan.md` in this folder with the full VLSM table, plus configs and verification output once built.

## What I Learned

*(Fill in after completing the lab.)*
