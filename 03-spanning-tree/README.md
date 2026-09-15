# 03 — Spanning Tree Protocol

**CCNA Domain:** 2 – Network Access · **Study plan reference:** Vol 1 Part III (Ch. 9–10)

## Objective

Build a deliberately looped topology, watch Rapid PVST+ prevent the loop, then manipulate root bridge election and observe convergence — the STP behavior you can't fully internalize just by reading about it.

## Topology

3 switches in a triangle (a physical loop), Rapid PVST+ enabled. *(Add topology diagram.)*

## Tasks

- [ ] Cable the triangle and confirm one link goes into blocking/discarding state
- [ ] Identify the root bridge with `show spanning-tree` and explain why it won the election (lowest priority, then lowest MAC)
- [ ] Force a different switch to become root by lowering its priority, and document the convergence
- [ ] Enable PortFast + BPDU Guard on an access port and confirm the port shuts down if it receives a BPDU
- [ ] Configure a Layer 2 EtherChannel between two of the switches (this doubles as prep for Lab 04) and observe how STP treats the bundle as one logical link

## Verification Commands

`show spanning-tree`, `show spanning-tree summary`, `show spanning-tree interface <if> detail`, `show interfaces status`

## What I Learned

*(Fill in after completing the lab — especially anything about convergence timing that differed from the textbook numbers.)*
