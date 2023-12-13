---
title: PacketRusher
version: "1.0"
description: PacketRusher is an open-source performance testing tool for 5G Core networks.
image: /img/platforms/packetrusher.png
width: large
priority: 7
active: false
tags:
  - packetrusher
---
PacketRusher is an open-source dedicated to the performance testing and automatic validation of 5G Core Networks using simulated UE (user equipment) and gNodeB (5G base station).

## Features
* Simulate multiple UEs and gNodeB from a single tool
  * We tested up to 10k UEs!
* Supports both N2 (NGAP) and N1 (NAS) interfaces for stress testing
* --pcap parameter to capture pcap of N1/N2 traffic
* Implements main control plane procedures:
  * Supports UE attach/detach (registration/authentifcation/security mode) procedures
  * Supports Create/Delete PDU Sessions,  up to 15 PDU Sessions per UE
  * Supports Xn handover: UE handover between simulated gNodeB (PathSwitchRequest)
* Implements high-performant N3 (GTP-U) interface
  * Generic tunnel supporting all kind of traffic (TCP, UDP, Video…)
    * We tested iperf3 traffic, and Youtube traffic through PacketRusher
    * We roughly reach 5 GB/s per UE, which is more than what a real UE can achieve.
* Integrated all-in-one mocked 5GC/AMF for PacketRusher's integration testing

## GitHub repositories

[PacketRusher on GitHub](https://github.com/HewlettPackard/PacketRusher): Main PacketRusher repository.

[Quickstart Guide](https://github.com/HewlettPackard/PacketRusher/blob/main/README.md): Learn how to install and use PacketRusher in chrono time.



[PacketRusher's Wiki on GitHub](https://github.com/HewlettPackard/PacketRusher/wiki): Get hints on how to use PacketRusher.