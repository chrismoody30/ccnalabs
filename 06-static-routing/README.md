# 06 — Static Routing (IPv4 and IPv6)

**CCNA Domain:** 3 – IP Connectivity · **Study plan reference:** Vol 1 Part V (Ch. 15–18)

## Objective

Route between multiple networks using static routes only, including a floating static route as a backup path — the scenario that shows up constantly in both the exam and real small-network design.

## Topology

3 routers in a line or triangle, each with 1–2 LAN segments, at least two paths between two of the routers (for the floating static test). *(Add topology diagram.)*

## Tasks

- [ ] Configure static routes (network route, not just default) so every LAN can reach every other LAN
- [ ] Configure a default route (`ip route 0.0.0.0 0.0.0.0`) on an edge router pointing to a simulated ISP
- [ ] Configure a floating static route as backup on one path (higher administrative distance) and prove it only takes over when the primary route fails
- [ ] Repeat the same LAN/route setup with IPv6 static routes
- [ ] Break a route on purpose (wrong next-hop, wrong prefix length) and use `show ip route`, `traceroute`, and `debug ip routing` (in the lab, never on production) to find and fix it

## Verification Commands

`show ip route`, `show ipv6 route`, `show ip route static`, `traceroute`, `ping`

## What I Learned

*(Fill in after completing the lab.)*
