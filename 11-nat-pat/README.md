# 11 — NAT / PAT

**CCNA Domain:** 4 – IP Services · **Study plan reference:** Vol 2 Ch. 10

## Objective

Configure all three flavors of NAT covered on the exam and be able to explain, from `show ip nat translations` output, exactly which address is inside-local vs. inside-global vs. outside-local vs. outside-global.

## Topology

An "inside" LAN behind a router, an "outside" network simulating the internet, private addressing inside and public-style addressing outside. *(Add topology diagram.)*

## Tasks

- [ ] Configure static NAT for a single inside host and verify translation with `show ip nat translations`
- [ ] Configure dynamic NAT with a pool and exhaust the pool on purpose to see the failure behavior
- [ ] Configure NAT overload (PAT) for the whole inside network sharing one outside address, and verify multiple simultaneous sessions translate correctly
- [ ] Break translation on purpose (wrong ACL matching inside traffic, or NAT applied to the wrong interface direction) and use `debug ip nat` (lab only) to find and fix it

## Verification Commands

`show ip nat translations`, `show ip nat statistics`, `debug ip nat` (lab only)

## What I Learned

*(Fill in after completing the lab.)*
