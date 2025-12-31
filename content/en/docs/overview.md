---
title: Overview
linkTitle: Overview
weight: 1
description: >
  Understand what NDTwin is and its unique advantages using innovative digital twin technologies
---

{{% pageinfo %}}
**NDTwin (Network Digital Twin)** is an open source framework that employs innovative digital twin technologies to optimally operate and manage a network.
{{% /pageinfo %}}

## What is NDTwin?

NDTwin is a software system that functions as the digital twin of a network. It has the following features:

* **Real-time collection of network and flow states**: NDTwin continuously polls the SDN controller to update its real-time graph of switches and links. Besides, it uses the industry-standard sFlow mechanism, which is supported by switches of any brands, to continuously get the real-time states of all flows in the network.  
* **Simulation and AI/ML-assited Decision Making**: A built-in sFlow collector listens for telemetry data to calculate bandwidth utilization and identify traffic patterns (like Elephant Flows) with high precision.
* **Deployment Flexibility**: Whether you are running a simulation in **Mininet** or deploying on a physical **Testbed** with hardware switches, NDTwin adapts its monitoring strategy accordingly.

## Why Choose NDTwin?

If your team is developing advanced network applications such as dynamic routing, load balancing, or energy-aware traffic engineering, NDTwin offers distinct advantages over standard monitoring tools.

### Key Benefits

* **Native OpenFlow Support**: Fully compatible with OpenFlow 1.0/1.3 standards. It seamlessly integrates with standard SDN controllers like **Ryu** or ONOS.
* **Real-time Flow Visualization**: Eliminate manual CLI debugging. Our graphical interface displays active Flow Rules and packet match counters, mapped directly to the topology.
* **Precise Traffic Monitoring**: Unlike simple counters, our integrated sFlow technology performs **5-tuple sampling** (Src/Dst IP, Port, Protocol) to analyze real-time bandwidth usage and detect congestion bottlenecks.
* **Dynamic Topology Awareness**: The system automatically detects Link Failures or new switch connections, triggering alerts to help you verify if your rerouting algorithms react correctly.

## Use Cases

| Scenario | Description |
| :--- | :--- |
| **Algorithm Verification** | Validate if your new shortest-path or multipath routing algorithms work as expected under load. |
| **Network Education** | Help students visualize the abstract concept of the "Match-Action" mechanism in OpenFlow. |
| **Energy-Saving Research** | Simulate network behavior when specific switch ports are powered down to save energy, and verify connectivity is maintained. |

