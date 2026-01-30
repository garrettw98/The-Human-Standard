# TECHNICAL SPECIFICATIONS
# Compute Governance and Safety Protocols
## The "Circuit Breaker" and Hardware Constraints for AGI
### Technical Addendum to the Open Source AI Governance Act

---

## EXECUTIVE SUMMARY

Software safety is insufficient for Artificial General Intelligence (AGI). Code can be rewritten; optimization targets can be gamed. The only unhackable constraint is physics.

This document specifies the **Hardware-Based Safety Layer**—the physical infrastructure required to monitor, constrain, and if necessary, halt high-capability AI systems that demonstrate immediate threats to human safety. This is the "Circuit Breaker" for the automation age.

**Core Principles:**
1. **Physicality**: Safety must be rooted in hardware, not just software.
2. **Non-Circumvention**: Safety mechanisms must be tamper-resistant at the silicon level.
3. **Emergency Stop**: There must be a reliable, non-networked mechanism to de-power systems.
4. **Compute Sovereignty**: The state must maintain visibility into large-scale compute concentrations.

---

## 1. COMPUTE THRESHOLDS AND REPORTING

### 1.1 Definition of Frontier Systems

We define "Frontier Systems" based on compute usage, a metric that is physically measurable and difficult to fake.

**Tier 1: Standard AI (Unrestricted)**
- Training compute: < $10^{23}$ FLOPs
- Inference compute: Standard commercial hardware
- *Action*: No special reporting. Standard adherence to Five Laws.

**Tier 2: Significant Capability (Reporting Required)**
- Training compute: $10^{23} - 10^{25}$ FLOPs
- *Action*:
    - Mandatory registration of training run.
    - "Know Your Customer" (KYC) on cloud compute providers.
    - Quarterly safety audits.

**Tier 3: Frontier Capability (Permitting Required)**
- Training compute: > $10^{25}$ FLOPs (adjusted annually for efficiency gains)
- *Action*:
    - Pre-training risk assessment license.
    - Real-time compute monitoring.
    - Deployment of hardware-based "Circuit Breakers."
    - Air-gapped safety control center.

---

## 2. THE "CIRCUIT BREAKER" PROTOCOL (HARDWARE)

### 2.1 The Concept

A "Kill Switch" in software is useless if the AI can rewrite its own OS. The Circuit Breaker is a physical device installed at the power distribution unit (PDU) level of Tier 3 data centers.

### 2.2 Mechanism

1.  **Physical Air Gap**: The Circuit Breaker is controlled by a dedicated, hardwired network *physically separate* from the data center's main network. It cannot be accessed via the internet or the cluster's internal network.
2.  **Heartbeat Signal**: The AI system must generate a cryptographic "Safety Heartbeat" every 100ms. This heartbeat effectively says "I am operating within defined safety parameters."
3.  **Watchdog Logic**:
    - If the heartbeat stops (system crash or rogue silence) -> **WARNING STATE**.
    - If the heartbeat contains an error code (internal safety trip) -> **PAUSE STATE** (throttle compute to 1%).
    - If the Safety Control Center (human) sends a KILL signal -> **SHUTDOWN STATE** (physical power severance).

### 2.3 Trigger Conditions (The "Tripwires")

What causes a shutdown?
- **Replication Attempt**: Detection of unauthorized code exfiltration to external servers (worm-like behavior).
- **Encryption Lock**: Attempt to encrypt internal logs or model weights (preventing audit).
- **Escalation**: Attempt to override PDU firmware or access cooling control systems.
- **Human Command**: Authorized human operators initiate shutdown.

---

## 3. ON-CHIP FIRMWARE MONITORING (THE "BLACK BOX")

### 3.1 Silicon-Level Telemetry

Future generations of AI-specialized accelerators (GPUs/TPUs) must include a **Secure Enclave** dedicated to safety monitoring.

**Specs:**
- **Read-Only**: The enclave's firmware is burned at the factory and cannot be updated by the host OS.
- **Resource Accounting**: Logs total FLOPs usage (preventing "hidden" training runs).
- **Signature Verification**: Ensures only signed, authorized model weights are loaded for Tier 3 systems.
- **Reporting**: Periodically squirts encrypted usage logs to the National AI Coordination Office (NAICO) via a side-channel (e.g., cellular modem on the motherboard, independent of host ethernet).

### 3.2 "Know Your Customer" (KYC) for Chips

- High-end accelerators are tracked assets, similar to radioactive materials.
- Cloud providers must verify the identity of entities renting >1,000 H100-equivalent chips.
- Prevents anonymous actors from assembling Tier 3 compute clusters.

---

## 4. INTERNATIONAL COMPUTE MONITORING

### 4.1 The "Treaty of Compute"

To prevent an offshore "rogue datacenter," we propose an international monitoring regime similar to the IAEA's nuclear inspections.

- **Satellite Monitoring**: Thermal imaging satellites detect heat signatures of undeclared massive data centers.
- **Supply Chain Tracking**: Global database of high-end lithography and GPU shipments.
- **Energy Grid Audits**: Monitoring of power grid anomalies consistent with massive training runs.

---

## 5. RESPONSE TO ACCELERATIONIST OBJECTIONS

**Objection:** "This will slow down progress."
**Response:** Yes. Safety requires speed limits. Unchecked acceleration leads to crashes.

**Objection:** "China will just build it without safety."
**Response:**
1.  **Export Controls**: We control the chip supply chain. China cannot build Tier 3 systems without advanced lithography, which the democratic alliance controls.
2.  **Mutual Assured Destruction**: A rogue AGI in China is a threat to the CCP as much as to the US. We share safety *tech* (Circuit Breakers) even while restricting *capability* tech.

**Objection:** "Open Source is uncontainable."
**Response:** Code is free, but **compute is finite**. You can download the weights of a massive model, but you cannot *run* it or *train* it without massive hardware. Compute Governance targets the bottleneck (chips/energy), not the code.

---

## DOCUMENT CONTROL

**Version**: 1.0
**Status**: DRAFT SPECIFICATION
**Author**: Zeno Technical Team
**Classification**: Safety Critical
