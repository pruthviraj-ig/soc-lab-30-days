# Lab 13 — Unified Kill Chain Framework Analysis & Threat Modelling

Platform: TryHackMe  
Room: Unified Kill Chain  
Role Simulation: SOC Analyst Level 1 — Threat Modelling & Attack Lifecycle Analysis

---

## Objective

Understand how the Unified Kill Chain framework expands traditional attack lifecycle analysis by combining cyber intrusion stages with adversary behaviour tracking. The lab focused on identifying attacker objectives, mapping malicious activities across attack phases, and improving SOC detection and response strategies.

---

## Technologies & Concepts Used

- Unified Kill Chain Framework
- Threat Modelling Concepts
- SOC Investigation Workflow
- Attack Lifecycle Analysis
- Privilege Escalation Detection
- Network Propagation Concepts

---

## Key Concepts Reviewed

### Kill Chain

A Kill Chain describes the structured phases attackers follow to achieve compromise objectives inside a target environment.

SOC analysts use kill chain models to:

- Identify attacker progression
- Detect intrusion stages early
- Implement defensive controls.

---

### Threat Modelling

Threat modelling focuses on understanding:

- Adversary objectives
- Attack pathways
- Vulnerable systems
- Defensive gaps.

Used by SOC analysts to predict attacker behaviour and improve detection logic.

---

## Unified Kill Chain Overview

The Unified Kill Chain expands traditional models into three major attacker goals:

- Goal In — Initial Foothold
- Goal Through — Network Propagation
- Goal Out — Actions on Objectives

This provides deeper visibility into lateral movement and persistence activities.

---

## Tasks Completed

---

### Task 1 — Introduction

- Reviewed purpose of kill chain frameworks.
- Learned benefits of identifying attacker progression.

---

### Task 2 — What is a Kill Chain

Studied:

- Military origin of kill chain concept.
- Cyber adaptation for intrusion detection.

Key Learning:

Attackers must complete multiple stages to achieve objectives.

---

### Task 3 — Threat Modelling

Reviewed how organisations analyse:

- Threat actors
- Attack paths
- Risk exposure.

SOC analysts apply threat modelling to strengthen detection strategies.

---

### Task 4 — Unified Kill Chain Introduction

Learned expansion beyond traditional Cyber Kill Chain.

Unified Kill Chain focuses on:

- Internal movement.
- Persistence mechanisms.
- Objective achievement.

---

### Task 5 — Goal In (Initial Foothold)

Activities studied:

- Phishing attacks
- Exploit public-facing applications
- Credential harvesting.

SOC Focus:

Detect initial compromise indicators early.

---

### Task 6 — Goal Through (Network Propagation)

Studied attacker movement inside networks.

Examples:

- Privilege escalation
- Lateral movement
- Credential dumping.

SOC Monitoring Includes:

- Abnormal authentication attempts.
- Administrator privilege misuse.

---

### Task 7 — Goal Out (Actions on Objectives)

Final attacker objectives include:

- Data exfiltration
- Ransomware deployment
- System sabotage.

SOC analysts prioritise containment and incident response.

---

### Task 8 — Practical Exercise

Completed Unified Kill Chain scenario investigation.

Mapped attacker actions including:

- Failed administrator login attempts.
- Privilege escalation activity.
- Persistence setup.
- Network pivoting.

Example Scenario:

Failed administrator login attempts indicated an attacker attempting privilege escalation.

Correct Phase:

Privilege Escalation (Goal Through).

---

## SOC Skills Practiced

- Threat lifecycle analysis
- Attack stage identification
- Privilege escalation detection
- Threat modelling fundamentals
- Incident investigation reasoning.

---

## SOC Tools Simulated

- SOC Investigation Workflow
- Threat Modelling Analysis
- Incident Classification Process.

---

## Key Learning

The Unified Kill Chain provides deeper visibility into attacker behaviour after initial compromise. SOC analysts can improve detection by focusing on attacker movement, persistence, and objective achievement phases.

---

## Evidence

Screenshots captured during:

- Practical scenario mapping.
- Phase identification exercises.
- Investigation workflow.

Location:

screenshots/
