# 07 — Single-Area OSPFv2

**CCNA Domain:** 3 – IP Connectivity · **Study plan reference:** Vol 1 Part VI (Ch. 19–21)

## Objective

Get OSPF neighbor adjacencies to actually form, then deliberately break the conditions for adjacency one at a time to see exactly which mismatch causes which failure — this is the single most common CCNA lab weak spot.

## Topology

3–4 routers in area 0, mix of point-to-point (serial/PPP) and broadcast (Ethernet) network types, at least one segment with a DR/BDR election happening. *(Add topology diagram.)*

## Tasks

- [ ] Enable OSPF and get full adjacencies between all routers, verify with `show ip ospf neighbor`
- [ ] Identify the DR and BDR on the multi-access segment and explain why those routers won
- [ ] Break adjacency by mismatching the area number on one side — document the log message and fix it
- [ ] Break adjacency by mismatching the hello/dead timers — document the symptom
- [ ] Break adjacency with a subnet mask mismatch on a shared segment — document the symptom
- [ ] Set OSPF priority to manipulate the DR election on purpose
- [ ] Adjust cost on one link to force traffic over a specific path, verify with `show ip route` and `show ip ospf interface`

## Verification Commands

`show ip ospf neighbor`, `show ip ospf interface`, `show ip protocols`, `show ip route ospf`, `debug ip ospf adj` (lab only)

## What I Learned

*(Fill in after completing the lab — this is worth writing up in detail, since OSPF neighbor troubleshooting comes up constantly in real jobs too.)*
