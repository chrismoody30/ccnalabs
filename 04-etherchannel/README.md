# 04 — EtherChannel

**CCNA Domain:** 2 – Network Access · **Study plan reference:** Vol 1 Ch. 10

## Objective

Bundle multiple physical links into one logical link using both negotiation protocols, and prove the bundle survives a single link failure without dropping the connection.

## Topology

2 switches connected by 2–3 parallel physical links. *(Add topology diagram.)*

## Tasks

- [ ] Configure a manual Layer 2 EtherChannel (`channel-group mode on`) and verify with `show etherchannel summary`
- [ ] Reconfigure the same bundle using LACP (`active`/`passive`) instead
- [ ] Reconfigure using PAgP (`desirable`/`auto`) and note the syntax/behavior differences from LACP
- [ ] Start a continuous ping across the bundle, shut down one member link, and confirm the ping keeps flowing
- [ ] Deliberately mismatch a port setting (e.g., speed) between bundle members and document how the switch reacts

## Verification Commands

`show etherchannel summary`, `show etherchannel port-channel`, `show interfaces port-channel 1`, `show spanning-tree`

## What I Learned

*(Fill in after completing the lab.)*
