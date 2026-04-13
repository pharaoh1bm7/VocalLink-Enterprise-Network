# VocalLink-Enterprise-Network

<img width="1151" height="790" alt="Screenshot 2026-04-13 103621" src="https://github.com/user-attachments/assets/991ab29b-c526-4a0b-861a-d5225de0bd48" />

# VocalLink: OmniChannel Contact Center Infrastructure

## Overview
This project simulates a high-availability network for a large-scale Call Center (BPO). It is designed to handle massive VoIP traffic and data synchronization between 6 core departments using Cisco Packet Tracer.

## Technical Architecture
- **Routing Engine:** Single-Area OSPF (Area 0) for dynamic link failover and sub-second convergence between core routers.
- **Switching Logic:** Layer 3 Multilayer Switching (Cisco 3560) managing Inter-VLAN routing for isolated departmental traffic.
- **Scalability:** Designed to support 150+ concurrent agents across multiple VLANs.
- **Reliability:** Resolved complex OSPF routing loops and interface mismatches to ensure zero packet loss for voice traffic.

## Network Segments
- **Ops Floor:** High-density zone for customer service agents.
- **Data & Voice Core:** Centralized servers for CRM and VoIP SIP trunks.
- **Quality & Training:** Dedicated VLAN for call monitoring and agent onboarding.
- **Management & Admin:** Secure zones for executive and HR operations.

## Key Features
- Dynamic Routing (OSPF)
- VLAN Segmentation (VTP/802.1Q)
- Inter-VLAN Routing (SVI)
- Loop Prevention & Troubleshooting
