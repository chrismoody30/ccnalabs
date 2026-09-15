# 08 — IPv6 Addressing and Routing

**CCNA Domain:** 1 & 3 · **Study plan reference:** Vol 1 Part VII (Ch. 22–25)

## Objective

Get comfortable reading and writing IPv6 addresses without mentally translating everything back to IPv4, and see SLAAC/DHCPv6 behavior firsthand.

## Topology

Reuse the Lab 06 or 07 topology and re-address it in IPv6 (dual-stack is fine — keep IPv4 running alongside).

## Tasks

- [ ] Assign global unicast addresses manually on router interfaces, and confirm link-local addresses are auto-generated
- [ ] Enable SLAAC on a LAN segment and confirm a client auto-configures via `show ipv6 interface` on the client-facing side
- [ ] Configure a router as a stateless DHCPv6 relay/server for a segment that needs DNS info alongside SLAAC
- [ ] Configure IPv6 static routes and/or OSPFv3 between routers
- [ ] Use EUI-64 to generate an interface ID on one interface and verify the resulting address matches expectations

## Verification Commands

`show ipv6 interface brief`, `show ipv6 route`, `show ipv6 ospf neighbor` (if using OSPFv3), `ping ipv6`

## What I Learned

*(Fill in after completing the lab.)*
