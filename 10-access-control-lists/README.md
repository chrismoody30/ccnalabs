# 10 — Access Control Lists

**CCNA Domain:** 5 – Security Fundamentals · **Study plan reference:** Vol 2 Ch. 1–3 (+ the 13 bundled ACL labs in the Vol 2 Network Simulator Lite)

## Objective

Write standard and extended ACLs by hand until wildcard mask math is automatic, and understand exactly how placement (which interface, which direction) changes what gets filtered.

## Topology

3+ routers/subnets so there's a real routing path to filter traffic across, at least one subnet representing "servers" and one representing "clients." *(Add topology diagram.)*

## Tasks

- [ ] Write a standard ACL to block one specific host from reaching a subnet, apply it in the correct direction/location, and verify the block works — and that everything else still passes
- [ ] Write an extended ACL matching specific protocol + port (e.g., permit HTTP/HTTPS to a server subnet, deny everything else) and verify with `telnet`/`curl`/`ping` tests from a client
- [ ] Convert a numbered ACL to a named ACL and add a line mid-list using sequence numbers, without recreating the whole thing
- [ ] Apply an ACL to the wrong interface/direction on purpose, observe the (lack of) effect, then fix it and document the difference
- [ ] Use `show access-lists` match counters to prove which lines are actually being hit by traffic

## Verification Commands

`show access-lists`, `show ip interface <if>` (to confirm what's applied where), `ping`, `telnet`

## What I Learned

*(Fill in after completing the lab.)*
